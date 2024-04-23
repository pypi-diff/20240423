# Comparing `tmp/biblelib-0.3.3.tar.gz` & `tmp/biblelib-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblelib-0.3.3.tar", max compression
+gzip compressed data, was "biblelib-0.3.4.tar", max compression
```

## Comparing `biblelib-0.3.3.tar` & `biblelib-0.3.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.3/LICENSE.md
--rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.3/LICENSE.md~
--rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.3/README.md
--rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.3/biblelib/__init__.py
--rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.3/biblelib/book/ReadMe.md
--rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.3/biblelib/book/__init__.py
--rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.3/biblelib/book/book.py
--rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.3/biblelib/book/books.tsv
--rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.3/biblelib/sources.py
--rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.3/biblelib/unit/__init__.py
--rw-r--r--   0        0        0     5834 2024-02-02 00:49:16.545913 biblelib-0.3.3/biblelib/unit/book.py
--rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.3/biblelib/unit/bookchapters.tsv
--rw-r--r--   0        0        0     7217 2024-02-02 00:50:41.685079 biblelib-0.3.3/biblelib/unit/chapter.py
--rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.3/biblelib/unit/chapters.tsv
--rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.3/biblelib/unit/chapterverses.tsv
--rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.3/biblelib/unit/pericope.py
--rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.3/biblelib/unit/tempchapter.py
--rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.3/biblelib/unit/unit.py
--rw-r--r--   0        0        0     5945 2024-04-19 20:18:36.271104 biblelib-0.3.3/biblelib/unit/unitrange.py
--rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.3/biblelib/unit/verse.py
--rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.3/biblelib/versification/Enumerator.py
--rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.3/biblelib/versification/Mapper.py
--rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.3/biblelib/versification/ReadMe.md
--rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.3/biblelib/versification/VrefReader.py
--rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.3/biblelib/versification/__init__.py
--rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.3/biblelib/versification/eng-nt-vref.txt
--rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.3/biblelib/versification/eng-ot-vref.txt
--rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.3/biblelib/versification/eng-protestant-vref.txt
--rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.3/biblelib/versification/org-nt-vref.txt
--rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.3/biblelib/versification/org-ot-vref.txt
--rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.3/biblelib/versification/org-protestant-vref.txt
--rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.3/biblelib/versification/rso-nt-vref.txt
--rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.3/biblelib/versification/rso-ot-vref.txt
--rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.3/biblelib/versification/rso-protestant-vref.txt
--rw-r--r--   0        0        0      959 2024-03-14 17:56:36.859595 biblelib-0.3.3/biblelib/word/__init__.py
--rw-r--r--   0        0        0    22893 2024-04-18 23:52:17.261353 biblelib-0.3.3/biblelib/word/bcvwpid.py
--rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.3.3/biblelib/word/mappings.py
--rw-r--r--   0        0        0     1324 2024-04-19 20:25:13.001522 biblelib-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.3.4/LICENSE.md
+-rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.3.4/LICENSE.md~
+-rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.3.4/README.md
+-rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.3.4/biblelib/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.3.4/biblelib/book/ReadMe.md
+-rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.3.4/biblelib/book/__init__.py
+-rw-r--r--   0        0        0    15533 2024-03-24 20:04:43.564328 biblelib-0.3.4/biblelib/book/book.py
+-rw-r--r--   0        0        0     5178 2024-04-18 23:10:23.491912 biblelib-0.3.4/biblelib/book/books.tsv
+-rw-r--r--   0        0        0     2114 2024-03-11 18:59:03.207673 biblelib-0.3.4/biblelib/sources.py
+-rw-r--r--   0        0        0      807 2024-02-02 00:29:34.781053 biblelib-0.3.4/biblelib/unit/__init__.py
+-rw-r--r--   0        0        0     5936 2024-04-23 02:01:59.233109 biblelib-0.3.4/biblelib/unit/book.py
+-rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.3.4/biblelib/unit/bookchapters.tsv
+-rw-r--r--   0        0        0     7217 2024-04-23 02:09:13.463233 biblelib-0.3.4/biblelib/unit/chapter.py
+-rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.3.4/biblelib/unit/chapters.tsv
+-rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.3.4/biblelib/unit/chapterverses.tsv
+-rw-r--r--   0        0        0     7558 2023-09-08 17:09:37.206917 biblelib-0.3.4/biblelib/unit/pericope.py
+-rw-r--r--   0        0        0    29962 2023-09-01 16:52:21.204686 biblelib-0.3.4/biblelib/unit/tempchapter.py
+-rw-r--r--   0        0        0     3564 2024-02-02 00:50:46.449409 biblelib-0.3.4/biblelib/unit/unit.py
+-rw-r--r--   0        0        0     6339 2024-04-23 02:09:29.760805 biblelib-0.3.4/biblelib/unit/unitrange.py
+-rw-r--r--   0        0        0     1534 2023-11-15 21:26:03.558678 biblelib-0.3.4/biblelib/unit/verse.py
+-rw-r--r--   0        0        0     5010 2024-03-11 18:59:15.691582 biblelib-0.3.4/biblelib/versification/Enumerator.py
+-rw-r--r--   0        0        0     2108 2024-03-19 16:38:12.467449 biblelib-0.3.4/biblelib/versification/Mapper.py
+-rw-r--r--   0        0        0     2992 2024-02-21 01:50:54.075772 biblelib-0.3.4/biblelib/versification/ReadMe.md
+-rw-r--r--   0        0        0     1871 2024-03-15 00:46:57.917308 biblelib-0.3.4/biblelib/versification/VrefReader.py
+-rw-r--r--   0        0        0      355 2024-03-11 19:15:48.838121 biblelib-0.3.4/biblelib/versification/__init__.py
+-rw-r--r--   0        0        0    73057 2024-02-21 01:58:50.596799 biblelib-0.3.4/biblelib/versification/eng-nt-vref.txt
+-rw-r--r--   0        0        0   217072 2024-02-21 01:58:57.893444 biblelib-0.3.4/biblelib/versification/eng-ot-vref.txt
+-rw-r--r--   0        0        0   290129 2024-02-21 01:59:00.692427 biblelib-0.3.4/biblelib/versification/eng-protestant-vref.txt
+-rw-r--r--   0        0        0    73037 2024-02-21 01:59:10.108486 biblelib-0.3.4/biblelib/versification/org-nt-vref.txt
+-rw-r--r--   0        0        0   217742 2024-02-21 01:59:11.043178 biblelib-0.3.4/biblelib/versification/org-ot-vref.txt
+-rw-r--r--   0        0        0   290779 2024-02-21 01:59:12.401051 biblelib-0.3.4/biblelib/versification/org-protestant-vref.txt
+-rw-r--r--   0        0        0    73017 2024-02-21 02:01:54.453211 biblelib-0.3.4/biblelib/versification/rso-nt-vref.txt
+-rw-r--r--   0        0        0   219552 2024-02-21 02:03:39.027636 biblelib-0.3.4/biblelib/versification/rso-ot-vref.txt
+-rw-r--r--   0        0        0   292569 2024-02-21 02:01:57.600383 biblelib-0.3.4/biblelib/versification/rso-protestant-vref.txt
+-rw-r--r--   0        0        0      993 2024-04-23 02:10:18.899048 biblelib-0.3.4/biblelib/word/__init__.py
+-rw-r--r--   0        0        0    25849 2024-04-23 02:10:27.855441 biblelib-0.3.4/biblelib/word/bcvwpid.py
+-rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.3.4/biblelib/word/mappings.py
+-rw-r--r--   0        0        0     1324 2024-04-23 02:14:02.953441 biblelib-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 biblelib-0.3.4/PKG-INFO
```

### Comparing `biblelib-0.3.3/LICENSE.md` & `biblelib-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/LICENSE.md~` & `biblelib-0.3.4/LICENSE.md~`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/README.md` & `biblelib-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/book/ReadMe.md` & `biblelib-0.3.4/biblelib/book/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/book/book.py` & `biblelib-0.3.4/biblelib/book/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/book/books.tsv` & `biblelib-0.3.4/biblelib/book/books.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/sources.py` & `biblelib-0.3.4/biblelib/sources.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/unit/__init__.py` & `biblelib-0.3.4/biblelib/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/unit/book.py` & `biblelib-0.3.4/biblelib/unit/book.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """Define Book class.
 
 Some duplication here with book.book that should be resolved, probably
 by migrating that code here.
 
 >>> from biblelib.unit import book
+# normally initialized by AllBookChapters
+>>> mrk = book.BookChapters("41", "41016", start_ID="410001")
+>>> mrk.bookname
+'MRK'
+
 >>> b
 Book(identifier='BID('41')')
 >>> b.identifier.book_ID
 '41'
 >>> b.lastchapter
 16
 >>> b.data
@@ -23,16 +28,14 @@
 from dataclasses import dataclass
 from typing import Optional
 
 # from collections import UserDict
 # from csv import DictReader
 from pathlib import Path
 
-# from typing import Any
-
 from biblelib.word import BID, BCID
 from biblelib import book
 from .unit import Unit, Versification, pad
 from .chapter import Chapter, Chapters
 
 UNITPATH = Path(__file__).parent
```

### Comparing `biblelib-0.3.3/biblelib/unit/bookchapters.tsv` & `biblelib-0.3.4/biblelib/unit/bookchapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/unit/chapter.py` & `biblelib-0.3.4/biblelib/unit/chapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,8 +165,8 @@
         """
         if not arg1:
             # arg0 is the stopping point
             verserange = range(arg0)
         else:
             assert arg0 > 0, "0 is not a valid value for arg0"
             verserange = range(arg0 - 1, arg1)
-        return [Verse(inst=(BCVID(self.inst.ID + pad(index + 1, count=3)))) for index in verserange]
+        return [Verse(inst=(BCVID(self.inst.ID + str(index + 1).zfill(3)))) for index in verserange]
```

### Comparing `biblelib-0.3.3/biblelib/unit/chapters.tsv` & `biblelib-0.3.4/biblelib/unit/chapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/unit/chapterverses.tsv` & `biblelib-0.3.4/biblelib/unit/chapterverses.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/unit/pericope.py` & `biblelib-0.3.4/biblelib/unit/pericope.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/unit/tempchapter.py` & `biblelib-0.3.4/biblelib/unit/tempchapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/unit/unit.py` & `biblelib-0.3.4/biblelib/unit/unit.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/unit/unitrange.py` & `biblelib-0.3.4/biblelib/unit/unitrange.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 >>> onechap.enumerate()
 [Verse(identifier='BCVID('41001040')'), Verse(identifier='BCVID('41001041')'), ... Verse(identifier='BCVID('41002002')')]
 
 
 """
 
 from dataclasses import dataclass, field
-import re
+from typing import Optional
 
 from biblelib.book import Books
 from biblelib.word import BID, BCID, BCVID, simplify
 from .chapter import Chapter
 from .verse import Verse
 from .unit import pad
 
@@ -63,14 +63,16 @@
     """Manage a range of verses."""
 
     startid: BCVID
     endid: BCVID
     # these are computed from startid and endid
     ID: str = field(init=False)
     book: BID = field(init=False)
+    # initialized from startid, so could be misleading for
+    # cross-chapter ranges
     chapter: BCID = field(init=False)
 
     def __post_init__(self) -> None:
         """Check initialization values."""
         # enforce typs: a little hacky to change init values like this.
         # It would be less hacky to have a factory method that does this.
         if self.startid.__class__.__name__ != "BCVID":
@@ -83,14 +85,18 @@
         assert self.book == BID(
             self.endid.to_bid
         ), f"Startid {self.startid} and endid {self.endid} must be in the same book."
         # note this allows a vacuous range with the same start and
         # end: does that make sense?
         assert self.startid <= self.endid, f"Startid {self.startid} must precede endid {self.endid}."
 
+    def __repr__(self) -> str:
+        """Return a printed representation."""
+        return "<VerseRange: {self.ID}>"
+
     def enumerate(self) -> list[Verse]:
         """Return a list of Verse instances enumerating the verses in the range.
 
         Enumerations include the ending Verse value (unlike range).
         """
 
         def get_verses(bcid: BCID, startindex: int, endindex: int) -> list[Verse]:
@@ -119,30 +125,34 @@
                 firstverses = get_verses(firstbcid, startid_verse_index, firstchap.lastverse)
                 # may be empty
                 midbcids: list[Chapter] = chapenum[1:-1]
                 # get all verses for any middle chapters
                 # WRONG use of get_verses here now that this is a list of Chapters
                 midverses = [v for chap in midbcids for v in chap.enumerate(1, chap.lastverse)]
                 lastbcid = chapenum[-1].identifier
-                lastchap = Chapter(inst=lastbcid)
+                # lastchap = Chapter(inst=lastbcid)
                 lastverses = get_verses(lastbcid, 1, endid_verse_index)
                 return [v for v in (firstverses + midverses + lastverses)]
 
+    def enumerate_ids(self) -> list[BCVID | None]:
+        """Return a list of BCVID instances for the range."""
+        return [v.inst for v in self.enumerate()]
+
 
 # I also need WordRange for a sequence of word IDs
-def detect_name_range(ref: str):
+def detect_name_range(ref: str) -> str:
     """Return a range instance for a reference.
 
     Assumes it's called on a reference with a hyphen. Heuristic.
 
     """
     ref1, ref2 = ref.split("-")
     assert not ("," in ref1 or "," in ref2), f"Can't handle complex range: {ref}"
     namematch = BOOKS.nameregexp.match(ref1)
     assert namematch, f"Invalid name reference: {ref1}"
-    bookname, rest = ref1[: namematch.end()], ref1[(namematch.end() + 1) :]
+    bookname, _ = ref1[: namematch.end()], ref1[(namematch.end() + 1) :]
     usfmbook = BOOKS.fromname(bookname).usfmnumber
     if ":" in ref1:
         return f"{usfmbook}, verserange"
     else:
         # match digits
         return f"{usfmbook}, chapterrange"
```

### Comparing `biblelib-0.3.3/biblelib/unit/verse.py` & `biblelib-0.3.4/biblelib/unit/verse.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/Enumerator.py` & `biblelib-0.3.4/biblelib/versification/Enumerator.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/Mapper.py` & `biblelib-0.3.4/biblelib/versification/Mapper.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/ReadMe.md` & `biblelib-0.3.4/biblelib/versification/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/VrefReader.py` & `biblelib-0.3.4/biblelib/versification/VrefReader.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/eng-nt-vref.txt` & `biblelib-0.3.4/biblelib/versification/eng-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/eng-ot-vref.txt` & `biblelib-0.3.4/biblelib/versification/eng-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/eng-protestant-vref.txt` & `biblelib-0.3.4/biblelib/versification/eng-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/org-nt-vref.txt` & `biblelib-0.3.4/biblelib/versification/org-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/org-ot-vref.txt` & `biblelib-0.3.4/biblelib/versification/org-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/org-protestant-vref.txt` & `biblelib-0.3.4/biblelib/versification/org-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/rso-nt-vref.txt` & `biblelib-0.3.4/biblelib/versification/rso-nt-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/rso-ot-vref.txt` & `biblelib-0.3.4/biblelib/versification/rso-ot-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/versification/rso-protestant-vref.txt` & `biblelib-0.3.4/biblelib/versification/rso-protestant-vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/biblelib/word/__init__.py` & `biblelib-0.3.4/biblelib/word/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 
 from .mappings import Mapping, Mappings
 from .bcvwpid import (
     BID,
     BCID,
     BCVID,
+    BCVIDRange,
     BCVWPID,
     fromlogos,
     fromname,
     fromosis,
     fromusfm,
     fromubs,
     reftypes,
@@ -29,14 +30,15 @@
 )
 
 __all__ = [
     # bcvwpid
     "BID",
     "BCID",
     "BCVID",
+    "BCVIDRange",
     "BCVWPID",
     "fromlogos",
     "fromname",
     "fromosis",
     "fromusfm",
     "fromubs",
     "reftypes",
```

### Comparing `biblelib-0.3.3/biblelib/word/bcvwpid.py` & `biblelib-0.3.4/biblelib/word/bcvwpid.py`

 * *Files 8% similar despite different names*

```diff
@@ -271,14 +271,87 @@
 
     def to_usfm(self) -> str:
         """Return a USFM representation."""
         usfmbook = BOOKS.fromusfmnumber(self.book_ID).usfmname
         return f"{usfmbook} {int(self.chapter_ID)}:{int(self.verse_ID)}"
 
 
+def from_bcid_verse(bcid: BCID, verse: int) -> BCVID:
+    """Return a BCVID instance from a BCID and verse number."""
+    return BCVID(f"{bcid.ID}{pad3(str(verse))}")
+
+
+@dataclass
+class BCVIDRange:
+    """Represents a range of BCVID instances.
+
+    This can represent a range across chapter boundaries,
+    though such ranges cannot yet be enumerated.
+
+    It is an error if the start and end books are not the same.
+    """
+
+    startid: BCVID
+    endid: BCVID
+    # these are computed from startid and endid
+    ID: str = field(init=False)
+    book: BID = field(init=False)
+    # initialized from startid, so could be misleading for
+    # cross-chapter ranges
+    chapter: BCID = field(init=False)
+    end_chapter: BCID = field(init=False)
+
+    def __post_init__(self) -> None:
+        """Check initialization values."""
+        # enforce typs: a little hacky to change init values like this.
+        # It would be less hacky to have a factory method that does this.
+        if self.startid.__class__.__name__ != "BCVID":
+            self.startid = BCVID(self.startid.to_bcvid)
+        if self.endid.__class__.__name__ != "BCVID":
+            self.endid = BCVID(self.endid.to_bcvid)
+        self.ID = self.startid.ID + "-" + self.endid.ID
+        self.book: BID = BID(self.startid.to_bid)
+        self.chapter: BCID = BCID(self.startid.to_bcid)
+        self.end_chapter: BCID = BCID(self.endid.to_bcid)
+        assert self.book == BID(
+            self.endid.to_bid
+        ), f"Startid {self.startid} and endid {self.endid} must be in the same book."
+        # note this allows a vacuous range with the same start and
+        # end: does that make sense?
+        assert self.startid <= self.endid, f"Startid {self.startid} must precede endid {self.endid}."
+
+    def __repr__(self) -> str:
+        """Return a printed representation."""
+        return f"{type(self).__name__}('{self.ID}')"
+
+    def enumerate(self) -> list[BCVID]:
+        """Return a list of BCVID instances enumerating the verses in the range.
+
+        Enumerations include the ending BCVID value (unlike range).
+
+        Only implemented for ranges within the same chapter.  This
+        also assumes verse numbers are sequential, without gaps: that
+        won't be true for some Bible editions.
+
+        """
+        if self.startid == self.endid:
+            # vacuous range
+            return [self.startid]
+        elif self.chapter != self.end_chapter:
+            # this needs knowledge about how many Verses in a Chapter,
+            # which lives in unit.unitrange. Not sure how to integrate these two:
+            # maybe a special enumerate method for cross-chapter ranges?
+            raise NotImplementedError("Enumerating over chapter boundaries is not yet implemented.")
+        else:
+            return [
+                from_bcid_verse(self.chapter, n)
+                for n in range(int(self.startid.verse_ID), int(self.endid.verse_ID) + 1)
+            ]
+
+
 @dataclass(repr=False, unsafe_hash=True)
 class BCVWPID(BCVID):
     """Identifies words from Bible texts by book, chapter, verse, word, and word part.
 
     The core schema is BBCCCVVVWWWP, where
     - BB identifies a book
     - CCC identifies a chapter number
@@ -434,15 +507,15 @@
 
     Simpler here means less specified.
     For a BCID, the only simpler form is BID.
     For BCVID, BCID or BID.
     For BCVWID, BCID, BID, or BCVID.
     For BCVWPID, any of the other types.
     """
-    assert refinst.__class__ in get_args(reftypes), "Must be a reference instance"
+    assert refinst.__class__ in get_args(reftypes), f"{refinst} must be a reference instance"
     validtypes = {
         "BCID": ["BID"],
         "BCVID": ["BID", "BCID"],
         # no BCVWID yet
         "BCVWPID": ["BID", "BCID", "BCVID"],
     }
     assert refinst.__class__.__name__ in validtypes, f"{newclass} is not a valid simpler type."
```

### Comparing `biblelib-0.3.3/biblelib/word/mappings.py` & `biblelib-0.3.4/biblelib/word/mappings.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.3.3/pyproject.toml` & `biblelib-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biblelib"
-version = "0.3.3"
+version = "0.3.4"
 description = "Utilities for working with metadata for Bible books, references, pericopes, and other units."
 authors = ["Sean Boisen <sean.boisen@gmail.com>"]
 repository = "https://github.com/Clear-Bible/Biblelib/"
 # documentation = "https://sboisen.github.io/Biblelib/"
 readme = "README.md"
 # apparently text files are also shipped?
 # include = [
```

### Comparing `biblelib-0.3.3/PKG-INFO` & `biblelib-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblelib
-Version: 0.3.3
+Version: 0.3.4
 Summary: Utilities for working with metadata for Bible books, references, pericopes, and other units.
 Home-page: https://github.com/Clear-Bible/Biblelib/
 Author: Sean Boisen
 Author-email: sean.boisen@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

