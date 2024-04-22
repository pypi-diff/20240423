# Comparing `tmp/mdxcanvas-0.0.8.tar.gz` & `tmp/mdxcanvas-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxcanvas-0.0.8.tar", max compression
+gzip compressed data, was "mdxcanvas-0.1.0.tar", max compression
```

## Comparing `mdxcanvas-0.0.8.tar` & `mdxcanvas-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-08-18 21:11:52.811761 mdxcanvas-0.0.8/LICENSE
--rw-r--r--   0        0        0       86 2023-09-02 15:54:56.741590 mdxcanvas-0.0.8/mdxcanvas/.env
--rw-r--r--   0        0        0      156 2024-02-22 01:16:53.597390 mdxcanvas-0.0.8/mdxcanvas/__init__.py
--rw-r--r--   0        0        0    20076 2024-02-23 22:32:22.256825 mdxcanvas-0.0.8/mdxcanvas/canvas_creator.py
--rw-r--r--   0        0        0      908 2024-02-23 21:51:03.183019 mdxcanvas-0.0.8/mdxcanvas/deploy.py
--rw-r--r--   0        0        0      873 2024-03-03 02:14:30.291845 mdxcanvas-0.0.8/mdxcanvas/extensions.py
--rw-r--r--   0        0        0    26912 2024-03-21 15:41:21.126179 mdxcanvas-0.0.8/mdxcanvas/parser.py
--rw-r--r--   0        0        0      628 2024-03-21 15:41:21.126433 mdxcanvas-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 mdxcanvas-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-31 20:08:12.653583 mdxcanvas-0.1.0/LICENSE
+-rw-r--r--   0        0        0      156 2024-02-23 19:51:14.711484 mdxcanvas-0.1.0/mdxcanvas/__init__.py
+-rw-r--r--   0        0        0    20889 2024-04-22 22:07:08.576608 mdxcanvas-0.1.0/mdxcanvas/canvas_creator.py
+-rw-r--r--   0        0        0      908 2024-02-23 20:06:54.416736 mdxcanvas-0.1.0/mdxcanvas/deploy.py
+-rw-r--r--   0        0        0     3392 2024-04-22 22:07:08.576705 mdxcanvas-0.1.0/mdxcanvas/document_schema.py
+-rw-r--r--   0        0        0      873 2024-02-26 20:43:38.531257 mdxcanvas-0.1.0/mdxcanvas/extensions.py
+-rw-r--r--   0        0        0     2689 2024-04-22 22:07:08.576782 mdxcanvas-0.1.0/mdxcanvas/jinja_parser.py
+-rw-r--r--   0        0        0    25486 2024-04-22 22:07:08.577304 mdxcanvas-0.1.0/mdxcanvas/parser.py
+-rw-r--r--   0        0        0      559 2024-04-22 22:07:08.577386 mdxcanvas-0.1.0/mdxcanvas/question_schema.py
+-rw-r--r--   0        0        0     1878 2024-04-22 22:07:08.577697 mdxcanvas-0.1.0/mdxcanvas/templating.py
+-rw-r--r--   0        0        0    15308 2024-04-22 22:07:08.577804 mdxcanvas-0.1.0/mdxcanvas/yaml_parser.py
+-rw-r--r--   0        0        0      651 2024-04-22 22:08:25.240353 mdxcanvas-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 mdxcanvas-0.1.0/PKG-INFO
```

### Comparing `mdxcanvas-0.0.8/LICENSE` & `mdxcanvas-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.0.8/mdxcanvas/canvas_creator.py` & `mdxcanvas-0.1.0/mdxcanvas/canvas_creator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import random
 import re
 from datetime import datetime
 import json
 import os
 import textwrap
-
 import uuid
+
+import pygments
+
 import argparse
 from xml.etree import ElementTree as etree
 
 import pytz
 from canvasapi import Canvas
 from canvasapi.assignment import Assignment
 
@@ -18,16 +21,19 @@
 
 import markdown as md
 from markdown.extensions.codehilite import makeExtension as makeCodehiliteExtension
 
 from pathlib import Path
 from bs4 import BeautifulSoup
 
+from jinja_parser import process_jinja
+
 from .extensions import BlackInlineCodeExtension
 from .parser import DocumentParser, make_iso
+from .yaml_parser import DocumentWalker, parse_yaml
 
 
 def readfile(filepath: Path):
     with open(filepath) as file:
         return file.read()
 
 
@@ -80,20 +86,27 @@
 
     if not any(fl.name == quiz_title for fl in course_folders):
         print(f"Created {quiz_title} folder")
         course.create_folder(name=quiz_title, parent_folder_path=generated_folder_name,
                              hidden=True)
 
 
+def generate_id(string: str) -> str:
+    """
+    Deterministic id generator for a given string.
+    """
+    return str(uuid.UUID(int=random.Random(string).getrandbits(128), version=4))
+
+
 def get_img_html(image_name, alt_text, style, course, image_folder: Path):
     """
     Returns the html for an image, and the path to the resource, so it can later be uploaded to Canvas.
     After uploading, the correct resource id must be substituted for the fake id using a text replace.
     """
-    fake_object_id = str(uuid.uuid4())
+    fake_object_id = generate_id(f"{image_name}{alt_text}{style}")
     style_text = f'style="{style}"' if style else ""
     html_text = f'<p><img id="{image_name}" src="/courses/{course.id}/files/{fake_object_id}/preview" alt="{alt_text}" {style_text}/></p>'
     resource = (fake_object_id, str(image_folder / image_name))
     return html_text, resource
 
 
 def process_images(html, course: Course, image_folder):
@@ -241,33 +254,32 @@
         course.create_assignment(assignment=element["settings"])
     print("Done")
     return canvas_assignment
 
 
 def modify_quiz(course: Course, element, delete: bool):
     name = element["name"]
-    settings: dict = element["settings"]
     print("Getting quiz from canvas")
     if canvas_quiz := get_quiz(course, name, delete):
         canvas_quiz: Quiz
         print(f"Editing canvas quiz {name} ...  ", end="")
-        canvas_quiz.edit(quiz=element["settings"])
+        canvas_quiz.edit(quiz=element)
     else:
-        canvas_quiz = create_quiz(course, element, name, settings)
+        canvas_quiz = create_quiz(course, element, name, element)
 
     replace_questions(canvas_quiz, element["questions"])
     canvas_quiz.edit()
     print("Done")
     return canvas_quiz
 
 
 def create_quiz(course, element, name, settings):
     print(f"Creating canvas quiz {name} ...  ", end="")
     try:
-        canvas_quiz = course.create_quiz(quiz=element["settings"])
+        canvas_quiz = course.create_quiz(quiz=element)
     except Exception as ex:
         print(ex)
         print()
         # Perhaps the quiz was partially created, and then the program crashed
         if canvas_quiz := get_quiz(course, name):
             canvas_quiz: Quiz
             print_red("Attempting to edit partially created quiz ...")
@@ -482,30 +494,43 @@
     :param course: The canvas course to post to, obtained from the canvas api
     :param time_zone: The time zone of the course (e.g. "America/Denver")
     :param file_path: The path to the markdown file
     :param delete: If true, deletes all elements in the Canvas course with the same name as the elements in the file
     """
 
     print(f"Parsing file ({file_path.name}) ...  ", end="")
-    if "mdx" not in file_path.name:
-        print_red("Error: File must be a mdx file")
-        return
 
     assignment_groups = list(course.get_assignment_groups())
     names_to_ids = {g.name: g.id for g in assignment_groups}
 
-    # Provide processing functions, so that the parser needs no access to a canvas course
-    parser = DocumentParser(
-        path_to_resources=file_path.parent,
-        path_to_canvas_files=file_path.parent,
-        markdown_processor=lambda text: process_markdown(text, course, file_path.parent),
-        time_zone=time_zone,
-        group_identifier=lambda group_name: get_group_id(course, group_name, names_to_ids),
-    )
-    document_object = parser.parse(file_path.read_text())
+    if "jinja" in file_path.name:
+        content = process_jinja(file_path)
+    else:
+        content = file_path.read_text()
+
+    if "yaml" in file_path.name:
+        walker = DocumentWalker(
+            path_to_resources=file_path.parent,
+            path_to_canvas_files=file_path.parent,
+            markdown_processor=lambda text: process_markdown(text, course, file_path.parent),
+            time_zone=time_zone,
+            group_identifier=lambda group_name: get_group_id(course, group_name, names_to_ids)
+        )
+        document = parse_yaml(content)
+        document_object = walker.walk(document)
+    else:
+        # Provide processing functions, so that the parser needs no access to a canvas course
+        parser = DocumentParser(
+            path_to_resources=file_path.parent,
+            path_to_canvas_files=file_path.parent,
+            markdown_processor=lambda text: process_markdown(text, course, file_path.parent),
+            time_zone=time_zone,
+            group_identifier=lambda group_name: get_group_id(course, group_name, names_to_ids),
+        )
+        document_object = parser.parse(content)
 
     course_folders = list(course.get_folders())
 
     # Create multiple quizzes or assignments from the document object
     for element in document_object:
         if "resources" in element:
             element = upload_and_link_files(element, course, element["resources"], course_folders)
```

### Comparing `mdxcanvas-0.0.8/mdxcanvas/deploy.py` & `mdxcanvas-0.1.0/mdxcanvas/deploy.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.0.8/mdxcanvas/extensions.py` & `mdxcanvas-0.1.0/mdxcanvas/extensions.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.0.8/mdxcanvas/parser.py` & `mdxcanvas-0.1.0/mdxcanvas/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,32 @@
 from typing import Callable, Union
 
 import pytz
 from bs4 import BeautifulSoup
 from bs4.element import Tag, NavigableString
 from datetime import datetime
 from typing import Protocol, TypeAlias
-from collections import defaultdict
+from collections import defaultdict, OrderedDict
+from mdxcanvas.templating import Templater
 
 from jinja2 import Environment
 
 ResourceExtractor: TypeAlias = Callable[[str], tuple[str, list]]
 
 
+def order_elements(element: dict) -> OrderedDict:
+    new_list = []
+    for key, value in element.items():
+        if isinstance(value, dict):
+            new_list.append((key, order_elements(value)))
+        else:
+            new_list.append((key, value))
+    return OrderedDict(sorted(element.items(), key=lambda x: x[0]))
+
+
 def get_corrects_and_incorrects(question_tag):
     corrects = question_tag.css.filter('correct')
     incorrects = question_tag.css.filter('incorrect')
     return corrects, incorrects
 
 
 def get_correct_comments(question_tag):
@@ -93,15 +104,16 @@
 def get_text_contents(tag, children_tag_names: list[str] = ()):
     """
     Typically, the body of a tag is found at contents[0], and sub-tags (like answers) are found later.
     However, images sometimes separate the text into multiple parts.
     This function joins the text and images together.
     """
     return "".join(
-        [str(c) for c in tag.contents if isinstance(c, NavigableString) or (isinstance(c, Tag) and c.name not in children_tag_names)])
+        [str(c) for c in tag.contents if
+         isinstance(c, NavigableString) or (isinstance(c, Tag) and c.name not in children_tag_names)])
 
 
 question_types = [
     'calculated_question',
     'essay_question',
     'file_upload_question',
     'fill_in_multiple_blanks_question',
@@ -116,15 +128,16 @@
 ]
 
 
 class TFConverter:
     @staticmethod
     def process(correct_incorrect_tag, markdown_processor: ResourceExtractor):
         is_true = correct_incorrect_tag.name == "correct"
-        question_text, resources = markdown_processor(get_text_contents(correct_incorrect_tag, ["correct-comments", "incorrect-comments"]))
+        question_text, resources = markdown_processor(
+            get_text_contents(correct_incorrect_tag, ["correct-comments", "incorrect-comments"]))
         question = {
             "question_text": question_text,
             "question_type": 'true_false_question',
             "points_possible": get_points(correct_incorrect_tag),
             "correct_comments": get_correct_comments(correct_incorrect_tag),
             "incorrect_comments": get_incorrect_comments(correct_incorrect_tag),
             "answers": [
@@ -149,23 +162,26 @@
 
     @staticmethod
     def process(question_tag, markdown_processor: ResourceExtractor) -> Union[
         tuple[list[dict], list], tuple[dict, list]]: ...
 
 
 class AttributeAdder:
-    def __init__(self, settings: dict, settings_tag: Tag):
+    def __init__(self, settings: dict, settings_tag: Tag, parser):
         self.settings = settings
         self.settings_tag = settings_tag
+        self.parser = parser
 
-    def __call__(self, attribute, default=None, new_name=None, formatter=None):
+    def __call__(self, attribute, default=None, new_name=None, formatter=None, typ=None):
         if attribute in self.settings_tag.attrs or default is not None:
             value = self.settings_tag.get(attribute, default)
             if formatter:
                 value = formatter(value)
+            if typ:
+                value = self.parser.parse(value, typ)
             self.settings[new_name if new_name else attribute] = value
 
 
 def process(processor: Processor, question_tag, markdown_processor: ResourceExtractor):
     question, resources = processor.process(question_tag, markdown_processor)
     return question, resources
 
@@ -210,15 +226,16 @@
     question_type: str
     num_correct: Union[int, None]
 
     def process(self, question_tag, markdown_processor: ResourceExtractor):
         corrects, incorrects = get_corrects_and_incorrects(question_tag)
         check_correct_size(corrects, self.num_correct, self.question_type)
 
-        question_text, resources = markdown_processor(get_text_contents(question_tag, ["correct", "incorrect", "correct-comments", "incorrect-comments"]))
+        question_text, resources = markdown_processor(
+            get_text_contents(question_tag, ["correct", "incorrect", "correct-comments", "incorrect-comments"]))
         answers = []
         for answer in corrects + incorrects:
             answer_html, res = markdown_processor(get_text_contents(answer))
             answers.append((True if answer in corrects else False, answer_html))
             resources.extend(res)
 
         question = {
@@ -260,15 +277,16 @@
         matches = []
         for pair in pairs:
             answer_left, answer_right = pair.css.filter('left')[0], pair.css.filter('right')[0]
             matches.append((answer_left.string.strip(), answer_right.string.strip()))
 
         distractors = question_tag.css.filter('distractors')
         distractor_text = get_text_contents(distractors[0]).strip() if len(distractors) > 0 else None
-        question_text, resources = markdown_processor(get_text_contents(question_tag, ["pair", "correct-comments", "incorrect-comments"]))
+        question_text, resources = markdown_processor(
+            get_text_contents(question_tag, ["pair", "correct-comments", "incorrect-comments"]))
         question = {
             "question_text": question_text,
             "question_type": 'matching_question',
             "points_possible": get_points(question_tag),
             "correct_comments": get_correct_comments(question_tag),
             "incorrect_comments": get_incorrect_comments(question_tag),
             "answers": [
@@ -291,38 +309,53 @@
             "question_text": question_text,
             "question_type": 'text_only_question',
         }
         return question, resources
 
 
 class Parser:
-    @staticmethod
-    def get_list(string):
+    def __init__(self):
+        pass
+
+    def parse(self, string, typ):
+        if typ == str:
+            return string
+        elif typ == int:
+            return self.get_int(string)
+        elif typ == bool:
+            return self.get_bool(string)
+        elif typ == list:
+            return self.get_list(string)
+        elif typ == dict:
+            return self.get_dict(string)
+
+    def get_list(self, string):
         items = string.strip().split(',')
         return [cell.strip() for cell in items if cell.strip()]
 
-    @staticmethod
-    def get_bool(string):
+    def get_bool(self, string):
         # Forgiving boolean parser
         if isinstance(string, bool):
             return string
 
         if string.lower() == "true":
             return True
         elif string.lower() == "false":
             return False
         else:
             raise ValueError(f"Invalid boolean value: {string}")
 
-    @staticmethod
-    def get_dict(string):
+    def get_dict(self, string):
         # Assumes the string is a comma-separated list of key-value pairs
         # Example: "key1=value1, key2=value2 "
         return dict(cell.strip().split('=') for cell in string.split(',') if cell.strip())
 
+    def get_int(self, string):
+        return int(string)
+
 
 class OverrideParser:
     def __init__(self, date_formatter, templater, parser):
         self.date_formatter = date_formatter
         self.template = templater
         self.parser = parser
 
@@ -345,15 +378,15 @@
                 override["replacements"] = self.template(tag)
         return override
 
     def parse_assignment_tag(self, tag):
         settings = {
             "title": tag["title"],
         }
-        adder = AttributeAdder(settings, tag)
+        adder = AttributeAdder(settings, tag, self.parser)
         adder("available_from", new_name="unlock_at", formatter=self.date_formatter)
         adder("due_at", formatter=self.date_formatter)
         adder("available_to", new_name="lock_at", formatter=self.date_formatter)
         return settings
 
 
 class ModuleParser:
@@ -361,15 +394,15 @@
         self.parser = parser
 
     def parse_module_settings(self, module_tag):
         settings = {
             "name": module_tag["title"],
             "position": module_tag["position"],
         }
-        AttributeAdder(settings, module_tag)("published", False, formatter=self.parser.get_bool)
+        AttributeAdder(settings, module_tag, self.parser)("published", False, bool)
         return settings
 
     def parse(self, module_tag: Tag):
         module = {
             "type": "module",
             "name": module_tag["title"],
             "settings": self.parse_module_settings(module_tag),
@@ -392,23 +425,23 @@
 
     def parse_module_item(self, tag: Tag):
         item = {
             "title": tag["title"],
             "type": self.casing[tag.name],
         }
 
-        adder = AttributeAdder(item, tag)
-        adder("position")
-        adder("indent")
+        adder = AttributeAdder(item, tag, self.parser)
+        adder("position", int)
+        adder("indent", int)
         adder("page_url")
         adder("external_url")
-        adder("new_tab", True, formatter=self.parser.get_bool)
+        adder("new_tab", True, bool)
         adder("completion_requirement")
         adder("iframe")
-        adder("published", False, formatter=self.parser.get_bool)
+        adder("published", False, bool)
         return item
 
 
 class QuizParser:
     question_processors = {
         "multiple-choice": MultipleChoiceProcessor(),
         "multiple-answers": MultipleAnswersProcessor(),
@@ -424,64 +457,59 @@
         self.date_formatter = date_formatter
         self.template = templater
         self.parser = parser
 
     def parse(self, quiz_tag: Tag):
         quiz = {
             "type": "quiz",
+            "name": quiz_tag["title"],
             "questions": [],
-            "resources": [],
-            "replacements": [],
-            "settings": {}
+            "resources": []
         }
+        quiz.update(self.parse_quiz_settings(quiz_tag))
+
         for tag in quiz_tag.find_all():
-            if tag.name == "settings":
-                quiz["settings"] = self.parse_quiz_settings(tag)
-                quiz["name"] = quiz["settings"]["title"]
-            elif tag.name == "template-arguments":
-                quiz["replacements"] = self.template(tag)
-            elif tag.name == "question":
+            if tag.name == "question":
                 question, res = self.parse_question(tag)
                 quiz["resources"].extend(res)
                 # if question is a  list of questions, add them all
                 if isinstance(question, list):
                     quiz["questions"].extend(question)
                 else:
                     quiz["questions"].append(question)
             elif tag.name == "description":
                 description, res = self.markdown_processor(get_text_contents(tag))
                 quiz["resources"].extend(res)
-                quiz["settings"]["description"] = description
+                quiz["description"] = description
         return quiz
 
     def parse_quiz_settings(self, settings_tag):
         settings = {"title": settings_tag["title"]}
 
-        adder = AttributeAdder(settings, settings_tag)
+        adder = AttributeAdder(settings, settings_tag, self.parser)
 
         adder("quiz_type", "assignment")
         adder("assignment_group", None, "assignment_group_id", formatter=self.group_indexer)
-        adder("time_limit")
-        adder("points_possible")
-        adder("shuffle_answers", False, formatter=self.parser.get_bool)
-        adder("hide_results", formatter=self.parser.get_bool)
-        adder("show_correct_answers", True, formatter=self.parser.get_bool)
-        adder("show_correct_answers_last_attempt", False, formatter=self.parser.get_bool)
+        adder("time_limit", None, typ=int)
+        adder("shuffle_answers", False, typ=bool)
+        adder("hide_results", typ=str)
+        adder("show_correct_answers", True, typ=bool)
+        adder("show_correct_answers_last_attempt", False, typ=bool)
         adder("show_correct_answers_at", None, formatter=self.date_formatter)
         adder("hide_correct_answers_at", None, formatter=self.date_formatter)
-        adder("allowed_attempts")
+        adder("allowed_attempts", -1, typ=int)
         adder("scoring_policy", "keep_highest")
-        adder("one_question_at_a_time", False, formatter=self.parser.get_bool)
-        adder("cant_go_back", False, formatter=self.parser.get_bool)
+        adder("one_question_at_a_time", False, typ=bool)
+        adder("cant_go_back", False, typ=bool)
         adder("available_from", None, "unlock_at", formatter=self.date_formatter)
         adder("due_at", None, formatter=self.date_formatter)
         adder("available_to", None, "lock_at", formatter=self.date_formatter)
         adder("access_code")
-        adder("published", False, formatter=self.parser.get_bool)
-        adder("one_time_results", False, formatter=self.parser.get_bool)
+        adder("published", False, typ=bool)
+        adder("one_time_results", False, typ=bool)
 
         return settings
 
     def parse_question(self, question_tag: Tag):
         processor = self.question_processors[question_tag["type"]]
         return processor.process(question_tag, self.markdown_processor)
 
@@ -492,74 +520,68 @@
         self.group_indexer = group_indexer
         self.date_formatter = date_formatter
         self.template = templater
         self.parser = parser
 
     def parse(self, assignment_tag):
         assignment = {
-            "name": "",
             "type": "assignment",
+            "name": assignment_tag["title"],
             "resources": [],
-            "replacements": [],
-            "settings": {}
+            "settings": self.parse_assignment_settings(assignment_tag)
         }
+
         for tag in assignment_tag.find_all():
-            if tag.name == "settings":
-                settings = self.parse_assignment_settings(tag)
-                assignment["settings"].update(settings)
-            elif tag.name == "template-arguments":
-                assignment["replacements"] = self.template(tag)
-            elif tag.name == "description":
+            if tag.name == "description":
                 contents = get_text_contents(tag)
                 description, res = self.markdown_processor(contents)
                 assignment["settings"]["description"] = description
                 assignment["resources"].extend(res)
 
-        assignment["name"] = assignment["settings"]["name"]
+        assignment["name"] = assignment["name"]
         return assignment
 
     def parse_assignment_settings(self, settings_tag):
         settings = {"name": settings_tag["title"]}
 
-        adder = AttributeAdder(settings, settings_tag)
-        adder("position")
-        adder("submission_types", "none", formatter=self.parser.get_list)
-        adder("allowed_extensions", "", formatter=self.parser.get_list)
-        adder("turnitin_enabled", False, formatter=self.parser.get_bool)
-        adder("vericite_enabled", False, formatter=self.parser.get_bool)
-        adder("turnitin_settings")
-        adder("integration_data")
-        adder("peer_reviews", False, formatter=self.parser.get_bool)
-        adder("automatic_peer_reviews", False, formatter=self.parser.get_bool)
-        adder("notify_of_update", False, formatter=self.parser.get_bool)
-        adder("group_category", new_name="group_category_id")
-        adder("grade_group_students_individually", False, formatter=self.parser.get_bool)
-        adder("external_tool_tag_attributes", "", formatter=self.parser.get_dict)
-        adder("points_possible")
-        adder("grading_type", "points")
-        adder("available_from", new_name="unlock_at", formatter=self.date_formatter)
-        adder("due_at", formatter=self.date_formatter)
-        adder("available_to", new_name="lock_at", formatter=self.date_formatter)
-        adder("assignment_group", new_name="assignment_group_id", formatter=self.group_indexer)
-        adder("assignment_overrides")
-        adder("only_visible_to_overrides", False, formatter=self.parser.get_bool)
-        adder("published", False, formatter=self.parser.get_bool)
-        adder("grading_standard_id")
-        adder("omit_from_final_grade", False, formatter=self.parser.get_bool)
-        adder("hide_in_gradebook", False, formatter=self.parser.get_bool)
-        adder("quiz_lti")
-        adder("moderated_grading", False, formatter=self.parser.get_bool)
-        adder("grader_count")
-        adder("final_grader_id")
-        adder("grader_comments_visible_to_graders", False, formatter=self.parser.get_bool)
-        adder("graders_anonymous_to_graders", False, formatter=self.parser.get_bool)
-        adder("grader_names_visible_to_final_grader", False, formatter=self.parser.get_bool)
-        adder("anonymous_grading", False, formatter=self.parser.get_bool)
-        adder("allowed_attempts", formatter=lambda x: -1 if x == "not_graded" else x)
-        adder("annotatable_attachment_id")
+        adder = AttributeAdder(settings, settings_tag, self.parser)
+        adder("allowed_attempts", formatter=lambda x: -1 if x == "not_graded" else x),
+        adder("allowed_extensions", "", typ=list),
+        adder("annotatable_attachment_id"),
+        adder("assignment_group", new_name="assignment_group_id", formatter=self.group_indexer),
+        adder("assignment_overrides"),
+        adder("automatic_peer_reviews", False, typ=bool),
+        adder("available_from", new_name="unlock_at", formatter=self.date_formatter),
+        adder("available_to", new_name="lock_at", formatter=self.date_formatter),
+        adder("due_at", formatter=self.date_formatter),
+        adder("external_tool_tag_attributes", "", typ=dict),
+        adder("final_grader_id"),
+        adder("grade_group_students_individually", False, typ=bool),
+        adder("grading_standard_id"),
+        adder("grading_type", "points"),
+        adder("grader_comments_visible_to_graders", False, typ=bool),
+        adder("grader_count"),
+        adder("grader_names_visible_to_final_grader", False, typ=bool),
+        adder("graders_anonymous_to_graders", False, typ=bool),
+        adder("group_category", new_name="group_category_id"),
+        adder("hide_in_gradebook", False, typ=bool),
+        adder("integration_data"),
+        adder("moderated_grading", False, typ=bool),
+        adder("notify_of_update", False, typ=bool),
+        adder("omit_from_final_grade", False, typ=bool),
+        adder("only_visible_to_overrides", False, typ=bool),
+        adder("peer_reviews", False, typ=bool),
+        adder("points_possible"),
+        adder("position"),
+        adder("published", False, typ=bool),
+        adder("quiz_lti"),
+        adder("submission_types", "none", typ=list),
+        adder("turnitin_enabled", False, typ=bool),
+        adder("turnitin_settings"),
+        adder("vericite_enabled", False, typ=bool)
 
         return settings
 
 
 class PageParser:
     def __init__(self, markdown_processor: ResourceExtractor, date_formatter, parser):
         self.markdown_processor = markdown_processor
@@ -568,19 +590,19 @@
 
     def parse_page_settings(self, page_tag):
         settings = {
             "type": "page",
             "name": page_tag["title"],
             "body": "",
         }
-        adder = AttributeAdder(settings, page_tag)
+        adder = AttributeAdder(settings, page_tag, self.parser)
         adder("editing_roles", "teachers")
-        adder("notify_of_update", False, formatter=self.parser.get_bool)
-        adder("published", False, formatter=self.parser.get_bool)
-        adder("front_page", False, formatter=self.parser.get_bool)
+        adder("notify_of_update", False, typ=bool)
+        adder("published", False, typ=bool)
+        adder("front_page", False, typ=bool)
         adder("publish_at", formatter=self.date_formatter)
         return settings
 
     def parse(self, page_tag):
         page = {
             "type": "page",
             "name": page_tag["title"],
@@ -605,65 +627,43 @@
 
         self.jinja_env = Environment()
         # This enables us to use the zip function in template documents
 
         self.jinja_env.globals.update(zip=zip, split_list=lambda sl: [s.strip() for s in sl.split(';')])
 
         parser = Parser()
+        self.templater = Templater(self.jinja_env, self.path_to_files)
 
         self.element_processors = {
             "quiz": QuizParser(self.markdown_processor, group_identifier, self.date_formatter,
-                               self.parse_template_data, parser),
+                               self.parse_mdx_template_data, parser),
             "assignment": AssignmentParser(self.markdown_processor, group_identifier, self.date_formatter,
-                                           self.parse_template_data, parser),
+                                           self.parse_mdx_template_data, parser),
             "page": PageParser(self.markdown_processor, self.date_formatter, parser),
             "module": ModuleParser(parser),
-            "override": OverrideParser(self.date_formatter, self.parse_template_data, parser)
+            "override": OverrideParser(self.date_formatter, self.parse_mdx_template_data, parser)
         }
 
     def parse(self, text):
         soup = BeautifulSoup(text, "html.parser")
         document = []
         tag: Tag
         for tag in soup.children:
             parser = self.element_processors.get(tag.name, None)
             if parser:
-                elements = parser.parse(tag)
-                if not isinstance(elements, list):
-                    elements = [elements]
-                for element in elements:
-                    new_elements = self.create_elements_from_template(element)
+                templates = parser.parse(tag)
+                if not isinstance(templates, list):
+                    templates = [templates]
+                templates = [order_elements(template) for template in templates]
+                for template in templates:
+                    new_elements = self.templater.create_elements_from_template(template)
                     document.extend(new_elements)
         return document
 
-    def create_elements_from_template(self, element_template):
-        if not (all_replacements := element_template.get("replacements", None)):
-            return [element_template]
-
-        # Element template is an object, turn it into text
-        template_text = json.dumps(element_template, indent=4)
-
-        # Use the text to create a jinja template
-        template = self.jinja_env.from_string(template_text)
-
-        elements = []
-        for context in all_replacements:
-            for key, value in context.items():
-                context[key] = value.replace('"', '\\"')
-            # For each replacement, create an object from the template
-            rendered = template.render(context)
-            element = json.loads(rendered)
-            elements.append(element)
-
-        # Replacements become unnecessary after creating the elements
-        for element in elements:
-            del element["replacements"]
-        return elements
-
-    def parse_template_data(self, template_tag):
+    def parse_mdx_template_data(self, template_tag):
         """
         Parses a template tag into a list of dictionaries
         Each dictionary will become a canvas object
         Converts the following:
         | header1 | header2    |
         |---------|------------|
         | first   | quiz       |
@@ -677,25 +677,15 @@
             {
                 "header1": "second",
                 "header2": "assignment"
             }
         ]
         """
         if template_tag.get("filename"):
-            csv = (self.path_to_files / template_tag.get("filename")).read_text()
-            headers, *lines = csv.split('\n')
+            psv = (self.path_to_files / template_tag.get("filename")).read_text()
+            headers, *lines = psv.split('\n')
         else:
             headers, separator, *lines = get_text_contents(template_tag).strip().split('\n')
-            # Remove whitespace and empty headers
-            headers = [h.strip() for h in headers.split('|') if h.strip()]
-            lines = [line for left_bar, *line, right_bar in [line.split('|') for line in lines]]
-
-        data = []
-        for line in lines:
-            line = [phrase.strip() for phrase in line]
-
-            replacements = defaultdict(dict)
-            for header, value in zip(headers, line):
-                replacements[header] = value
 
-            data.append(replacements)
-        return data
+        return self.templater.parse_psv(headers, lines)
+
+
```

### Comparing `mdxcanvas-0.0.8/pyproject.toml` & `mdxcanvas-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "mdxcanvas"
-version = "0.0.8"
+version = "0.1.0"
 description = "A Canvas LMS API wrapper for maintaining content in markdown"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Preston Raab <phr23@byu.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Jinja2 = "^3.1.2"
 Markdown = "^3.1.1"
 MarkupSafe = "^2.0.1"
 CanvasAPI = "^3.2.0"
 pytz = "^2024.1 "
 beautifulsoup4 = "^4.12.0"
 Pygments = "^2.17.2"
+strictyaml = "^1.7.3"
+
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 
 [tool.poetry.scripts]
 mdxcanvas = "mdxcanvas.deploy:entry"
```

### Comparing `mdxcanvas-0.0.8/PKG-INFO` & `mdxcanvas-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mdxcanvas
-Version: 0.0.8
+Version: 0.1.0
 Summary: A Canvas LMS API wrapper for maintaining content in markdown
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: CanvasAPI (>=3.2.0,<4.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: Markdown (>=3.1.1,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.0.1,<3.0.0)
 Requires-Dist: Pygments (>=2.17.2,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.0,<5.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
+Requires-Dist: strictyaml (>=1.7.3,<2.0.0)
```

