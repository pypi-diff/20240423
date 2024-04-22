# Comparing `tmp/almirah-0.2.0.tar.gz` & `tmp/almirah-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almirah-0.2.0.tar", max compression
+gzip compressed data, was "almirah-0.3.0.tar", max compression
```

## Comparing `almirah-0.2.0.tar` & `almirah-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
--rw-r--r--   0        0        0     1072 2024-04-03 06:23:38.217076 almirah-0.2.0/LICENSE
--rw-r--r--   0        0        0      963 2024-04-03 06:23:38.217076 almirah-0.2.0/README.md
--rw-r--r--   0        0        0      225 2024-04-03 06:23:38.217076 almirah-0.2.0/almirah/__init__.py
--rw-r--r--   0        0        0      281 2024-04-03 06:23:38.217076 almirah-0.2.0/almirah/data/__init__.py
--rw-r--r--   0        0        0     5268 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/configs/bids.yaml
--rw-r--r--   0        0        0     8102 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/convert.py
--rw-r--r--   0        0        0     4646 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/dataset.py
--rw-r--r--   0        0        0     3784 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/indexer.py
--rw-r--r--   0        0        0     6854 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/layout.py
--rw-r--r--   0        0        0     1448 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/report.py
--rw-r--r--   0        0        0    12226 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/specification.py
--rw-r--r--   0        0        0    18868 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/db.py
--rw-r--r--   0        0        0     3830 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/utils.py
--rw-r--r--   0        0        0     1120 2024-04-03 06:23:38.225076 almirah-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 almirah-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-22 22:37:55.424893 almirah-0.3.0/LICENSE
+-rw-r--r--   0        0        0      963 2024-04-22 22:37:55.424893 almirah-0.3.0/README.md
+-rw-r--r--   0        0        0      335 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/__init__.py
+-rw-r--r--   0        0        0     5268 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/configs/bids.yaml
+-rw-r--r--   0        0        0      119 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/core/__init__.py
+-rw-r--r--   0        0        0     1829 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/core/base.py
+-rw-r--r--   0        0        0     1079 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/core/db.py
+-rw-r--r--   0        0        0     3213 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/core/uniquify.py
+-rw-r--r--   0        0        0    18179 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/database.py
+-rw-r--r--   0        0        0     3557 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/dataset.py
+-rw-r--r--   0        0        0     2479 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/indexer.py
+-rw-r--r--   0        0        0     8541 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/layout.py
+-rw-r--r--   0        0        0    12416 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/specification.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/__init__.py
+-rw-r--r--   0        0        0     8117 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/convert.py
+-rw-r--r--   0        0        0     2363 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/df.py
+-rw-r--r--   0        0        0     3611 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/gen.py
+-rw-r--r--   0        0        0     1766 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/lib.py
+-rw-r--r--   0        0        0     1648 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/logging.py
+-rw-r--r--   0        0        0     1471 2024-04-22 22:37:55.424893 almirah-0.3.0/almirah/utils/sqlalchemy.py
+-rw-r--r--   0        0        0     1086 2024-04-22 22:37:55.428892 almirah-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1694 1970-01-01 00:00:00.000000 almirah-0.3.0/PKG-INFO
```

### Comparing `almirah-0.2.0/LICENSE` & `almirah-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `almirah-0.2.0/README.md` & `almirah-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `almirah-0.2.0/almirah/data/configs/bids.yaml` & `almirah-0.3.0/almirah/configs/bids.yaml`

 * *Files identical despite different names*

### Comparing `almirah-0.2.0/almirah/data/convert.py` & `almirah-0.3.0/almirah/utils/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-"""Collection of file format converters."""
+"""File format conversion utility functions."""
 
 import os
 import mne
 import shlex
 import logging
 import mne_bids
 import mne_nirs
 
-from ..utils import run_shell
+from .gen import run_shell
 
 
 def dcm2nii(files, out, dst, **kwargs):
-    """Convert DICOM files to NIfTI and write to disk.
+    """
+    Convert DICOM files to NIfTI and write to disk.
 
     Parameters
     ----------
     files : List of Files
         List of File objects that represent the files to be converted.
-
     out : str
         Output format desired.
-
     dst: str
         Destination directory where converted files will be stored.
-
     config: str
         Path to config file. Should be compatible with dcm2bids
         version installed.
 
     Returns
     -------
     None
@@ -117,15 +115,15 @@
         os.makedirs(os.path.dirname(new_path), exist_ok=True)
         cmd = tmp.format(**args)
         run_shell(cmd)
         logging.info(f"Converted {file.path} and stored to {new_path}")
     logging.info("Conversion to asc complete")
 
 
-def nirs_conv(files, out, dst, **kwargs):
+def nirx2snirf(files, out, dst, **kwargs):
     """Convert NIRS data format and write to disk."""
 
     for file in files:
         raw = mne.io.read_raw_nirx(file.path)
         raw.anonymize(**kwargs.get("anonymize", {}))
         new_path = os.path.join(
             dst,
@@ -136,15 +134,15 @@
         )
         os.makedirs(os.path.dirname(new_path), exist_ok=True)
         mne_nirs.io.write_raw_snirf(raw, new_path)
         logging.info(f"Converted {file.path} and stored to {new_path}")
     logging.info("Conversion to snirf complete")
 
 
-def eeg_conv(files, out, dst, **kwargs):
+def eeg_converter(files, out, dst, **kwargs):
     """Convert EEG data format and write to disk."""
 
     # Set conversion logging level
     verbose = kwargs.get("logging", "INFO")
 
     # Set power line frequency to default if not provided
     line_freq = kwargs.get("line_freq", 50)
@@ -255,19 +253,19 @@
             ".gdf",
             ".mat",
             ".mff",
             ".nxe",
             ".set",
             ".vhdr",
         ),
-        "using": eeg_conv,
+        "using": eeg_converter,
     },
     ("ASCII",): {"from": (".edf",), "using": edf2asc},
     ("NIfTI",): {"from": (".dcm",), "using": dcm2nii},
-    ("SNIRF",): {"from": (".nirx",), "using": nirs_conv},
+    ("SNIRF",): {"from": (".nirx",), "using": nirx2snirf},
 }
 _DCM2NII_VALID_FLAGS = {"--forceDcm2niix", "--clobber"}
 _EDF2ASC_VALID_FLAGS = {
     "-t",
     "-c",
     "-z",
     "-v",
```

### Comparing `almirah-0.2.0/almirah/data/specification.py` & `almirah-0.3.0/almirah/specification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,131 +1,108 @@
-"""Define the standard for the data set."""
+"""Define the specification for the dataset."""
 
 import re
 import os
 import logging
-import warnings
-
 import pandas as pd
-from string import Formatter
 
-from .. import utils
+from string import Formatter
 
+from sqlalchemy.orm import Mapped
+from sqlalchemy.orm import mapped_column
 
-_TAG_PATTERN = re.compile(r"({([\w\d]*?)(?:<([^>]+)>)?(?:\|((?:\.?[\w])+))?\})")
+from sqlalchemy_json import NestedMutableJson
 
-__all__ = ["Specification"]
+from .core import Base
+from .core import uniquify
+from .indexer import index
 
+from .utils.gen import copy
+from .utils.gen import filename
+from .utils.gen import read_yaml
+from .utils.gen import get_dir_contents
 
-class Specification:
-    """Representation of the specification used.
 
-    Attributes
-    ----------
-    name : str
-        The name of the specification.
+_TAG_PATTERN_TEMPLATE = re.compile(
+    r"({([\w\d]*?)(?:<([^>]+)>)?(?:\|((?:\.?[\w])+))?\})"
+)
 
-    Parameters
-    ----------
-    spec : dict or str
-        The dict-converted YAML specification file or its path.
 
-    Notes
-    -----
-    The YAML file that describes the specification can be split into two parts.
-       - tag definitions
-       - path definitions
+@uniquify(index)
+class Specification(Base):
+    """Generic specification representation."""
 
-    More information on these will follow.
-    """
+    __tablename__ = "specifications"
+    __identifier_attrs__ = {"name"}
 
-    def __init__(self, details=None, name=None):
-        self.spec, self.name = get_spec(details, name)
+    name: Mapped[str] = mapped_column(primary_key=True, nullable=False)
+    details: Mapped[list[str]] = mapped_column(NestedMutableJson, nullable=False)
 
-    def get_valid_tags(self):
-        """Returns valid tag names."""
-        return [t.get("name") for t in self.spec.get("tags")]
+    def __init__(self, *, name, details):
+        self.name = name
+        self.details = details
 
-    def extract_tags(self, path):
-        """Returns tag:value pairs for file."""
-        tags = {}
-        for tag in self.spec.get("tags"):
-            val = re.findall(tag.get("pattern"), path)
-            if val:
-                tags[tag.get("name")] = val[0]
-        return tags
-
-    def validate(self, path):
-        """Returns True if path is valid."""
-        tags = self.extract_tags(path)
-        if self.build_path(tags) == path:
-            return True
-        return False
-
-    def build_path(self, tags, strict=False):
-        """Construct path provided a set of tags.
+    def build_path(self, tags, strict=True):
+        """
+        Construct path given a set of tags.
 
         Parameters
         ----------
         tags : dict
-            A dictionary with tag name, value pairs.
+            Dictionary of name:value tag pairs.
 
         strict : bool
             If True, the tags provided should exactly match the
             requirements. If False, extra tags are ignored and the
             first matching path is built.
 
         Returns
         -------
         path : str
             The constructed path if successful, else `None`.
-
         """
-
-        path_patterns = self.spec.get("path_patterns")
+        path_patterns = self.details.get("path_patterns")
         logging.debug(f"Building path with tags : {tags}")
 
         # Remove none values
         tags = {k: v for k, v in tags.items() if v or v == 0}
 
         # Work with extension with or without .
         if "extension" in tags:
             ext = tags.get("extension")
             tags["extension"] = ext if ext.startswith(".") else "." + ext
 
         # Attempt to match pattern with tags and return first match
         for pattern in path_patterns:
             path = pattern
-            matches = _TAG_PATTERN.findall(pattern)
+            matches = _TAG_PATTERN_TEMPLATE.findall(pattern)
 
             # Do not tamper with tags provided so that
             # it can be used for other patterns
             tags_copy = tags.copy()
 
             # Skip if strict set and all tags not matched
             if strict and set(tags_copy.keys()) - set([t[1] for t in matches]):
                 continue
 
-            # Validate and fill in missing tags with default
-            for subpattern, name, valid_vals, default in matches:
+            # Validate and fill in missing tags with default value
+            for subpat, name, valid_vals, default in matches:
                 valid = [v for v in valid_vals.split("|")]
 
                 if valid and name in tags_copy and tags_copy[name] not in valid:
                     continue
 
                 if name not in tags_copy and default:
                     tags_copy[name] = default
 
                 if valid and default and default not in valid:
-                    warnings.warn(
-                        f"Pattern {subpattern} is inconsistent as it defines an invalid default value"
-                    )
+                    raise ValueError(f"Inconsistent default in pattern {subpat}")
 
                 # Simplify path
-                path = path.replace(subpattern, "{%s}" % name)
+                path = path.replace(subpat, "{%s}" % name)
 
             # Keep or remove optional tags
             optional_patterns = re.findall(r"(\[.*?\])", path)
             for op in optional_patterns:
                 optional_tag = re.findall(r"\{(.*?)\}", op)[0]
                 path = (
                     path.replace(op, op[1:-1])
@@ -143,59 +120,81 @@
             # Fill in the fields
             path = path.format_map(tags_copy)
 
             return path
 
         return None
 
+    @staticmethod
+    def create_from_file(path):
+        """Create Specification from yaml file."""
+        n, d = filename(path), read_yaml(path)
+        spec = Specification(name=n, details=d)
+        index.add(spec)
+        return spec
+
+    def extract_tags(self, path):
+        """Return tag:value pairs based on file path."""
+        t = {}
+        for tag in self.details.get("tags"):
+            val = re.findall(tag["pattern"], path)
+            if val:
+                t[tag["name"]] = val[0]
+        return t
+
+    @classmethod
+    def get(cls, **identifiers):
+        d = identifiers.pop("details", None)
+        obj = index.get(cls, **identifiers)
+
+        if obj and d and obj.details != d:
+            return None
+
+        return obj
+
     def organize(self, rules):
-        """Create a organized copy of a source directory based on rules.
+        """
+        Create organized copy of source directories based on defined rules.
 
         Parameters
         ----------
         rules : dict
-            A dictionary describing the instructions for organizing.
-
-        Returns
-        -------
-        None
+            Dictionary describing instructions for organizing.
         """
 
         # Check for required keys
         for mandatory_key in [
             "source",
             "destination",
             "pattern",
             "tag_rules",
         ]:
             if mandatory_key not in rules:
                 raise KeyError(f"Expected '{mandatory_key}' key in rule.")
 
-        source = rules.get("source")
-        destination = rules.get("destination")
-        logging.info(f"Initiating organization of {source} -> {destination}")
+        src = rules.get("source")
+        dst = rules.get("destination")
+        logging.info(f"Organizing {src} based on {self.name} -> {dst}")
 
         overwrite = rules.get("overwrite", False)
         if overwrite:
-            logging.warning("Overwrite set: Existing files may be overwritten")
+            logging.warning("Overwrite set: Existing files will be overwritten")
 
         add = rules.get("add", None)
         for a in add or []:
             logging.info(f"File {a['path']} will be added as {a['position']}.")
 
         logging.debug(f"Matching contents with pattern {rules.get('pattern')}")
 
-        # Organize matched files as per rules
-        matches = utils.get_dir_contents(
-            source, rules.get("pattern"), rules.get("skip", None)
-        )
+        # Organize files matching pattern using rules
+        matches = get_dir_contents(src, rules["pattern"], rules.get("skip", None))
         for file in matches or []:
             logging.info(f"Found match with file {file}")
 
-            # Extract tags
+            # Extract tags for file
             tags = {}
             for rule in rules.get("tag_rules"):
                 tag_name = rule.get("name")
                 logging.debug(f"Foraging for {tag_name} tag")
 
                 if "value" in rule:
                     val = rule.get("value")
@@ -271,17 +270,17 @@
 
             # Warning, clunky code ahead. To be made better
             rel_path = self.build_path(tags)
             if not rel_path:
                 logging.error("Unable to build destination path for file")
                 continue
 
-            new_path = os.path.join(rules.get("destination"), rel_path)
+            new_path = os.path.join(dst, rel_path)
             logging.info(f"Target destination path is {new_path}")
-            utils.copy(file, new_path, overwrite)
+            copy(file, new_path, overwrite)
             logging.info("Moved file to target")
 
             if add:
                 for addition in add:
                     if addition["position"] == "content":
                         addition_path = os.path.join(
                             new_path, os.path.basename(addition["path"])
@@ -290,15 +289,15 @@
                         addition_path = os.path.join(
                             os.path.dirname(new_path), addition["path"]
                         )
                     else:
                         raise ValueError(
                             "Expected position to be either content or fellow"
                         )
-                    utils.copy(addition["path"], addition_path, overwrite)
+                    copy(addition["path"], addition_path, overwrite)
                     logging.info(f"Added addition at {addition_path}")
 
             if not rules.get("copy_fellows", False):
                 continue
 
             # Find fellows
             logging.info("Initiating copying of fellow files")
@@ -321,23 +320,25 @@
                         logging.info(f"File marked with suffix:{tag_val} tag")
 
                 # Copy fellow files
                 rel_path = self.build_path(tags_copy)
                 if not rel_path:
                     logging.error(f"Unable to build destination path for file {file}")
                     continue
-                new_path = os.path.join(rules.get("destination"), rel_path)
+                new_path = os.path.join(dst, rel_path)
                 logging.info(f"Target destination path is {new_path}")
-                utils.copy(fellow, new_path, overwrite)
-
-    def __repr__(self):
-        return f"<Specification name={self.name}>"
+                copy(fellow, new_path, overwrite)
 
+    @property
+    def tags(self):
+        """Return list of tags defined in the specification."""
+        return [t.get("name") for t in self.details.get("tags")]
 
-def get_spec(path=None, name=None):
-    if not path:
-        path = os.path.join(os.path.dirname(__file__), "configs", "bids.yaml")
-
-    spec = utils.read_yaml(path)
-    name = name if name else os.path.splitext(os.path.basename(path))[0]
+    def validate_path(self, path):
+        """Return True if path is valid according to specification."""
+        tags = self.extract_tags(path)
+        if self.build_path(tags) == path:
+            return True
+        return False
 
-    return spec, name
+    def __repr__(self):
+        return f"<Specification name: '{self.name}'>"
```

### Comparing `almirah-0.2.0/almirah/db.py` & `almirah-0.3.0/almirah/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,113 +1,133 @@
-"""Database and DataFrame functionality for data access and manipulation."""
+"""Database functionality for data write and access."""
 
-import os
 import logging
+import numpy as np
 import pandas as pd
 
+from sqlalchemy import URL
 from sqlalchemy import Table
 from sqlalchemy import Column
-from sqlalchemy import MetaData
 from sqlalchemy import ForeignKey
+from sqlalchemy import UniqueConstraint
 from sqlalchemy import ForeignKeyConstraint
 
-from sqlalchemy.types import Boolean
-from sqlalchemy.types import Float
-from sqlalchemy.types import Integer
-from sqlalchemy.types import String
-from sqlalchemy.types import DateTime
+from sqlalchemy.orm import Mapped
+from sqlalchemy.orm import mapped_column
 
-from sqlalchemy import create_engine
-from sqlalchemy.orm import sessionmaker
-
-from .utils import get_dtype, log_df, log_col
-
-__all__ = ["DBManager", "common_records", "migrate", "transform", "validate"]
-
-
-class DBManager:
-    """Interface to connect with db and perform operations."""
-
-    def __init__(self, db_path=None):
-        self.engine = get_db(db_path)
-        self.meta = self._init_metadata()
-        self._sessionmaker = sessionmaker(self.engine)
-        self._session = None
-
-    def _init_metadata(self):
-        meta = MetaData()
-        meta.reflect(bind=self.engine)
-        return meta
+from .core import uniquify
+from .core import DBManager
+from .indexer import index
+from .dataset import Component
+
+from .utils.df import common_rows
+from .utils.df import convert_column_type
+from .utils.logging import log_df
+from .utils.logging import log_col
+from .utils.sqlalchemy import get_sql_type
+
+
+@uniquify(index)
+class Database(Component):
+    """Generic database representation."""
+
+    __tablename__ = "databases"
+    __identifier_attrs__ = {"name", "host", "backend"}
+
+    id: Mapped[int] = mapped_column(ForeignKey("components.id"), primary_key=True)
+    name: Mapped[str] = mapped_column(nullable=False)
+    host: Mapped[str] = mapped_column(nullable=False)
+    backend: Mapped[str] = mapped_column(nullable=True)
+
+    __table_args__ = (UniqueConstraint("name", "host", "backend"),)
+    __mapper_args__ = {"polymorphic_identity": "database"}
+
+    def __init__(self, *, name, host, backend):
+        self.name = name
+        self.host = host
+        self.backend = backend
 
     @property
-    def session(self):
-        if self._session is None:
-            self._session = self._sessionmaker()
-        return self._session
+    def connection(self):
+        if not self.db:
+            raise TypeError(f"Connection to {self} not established")
+        return self.db.connection
 
     @property
-    def connection(self):
-        return self.engine.connect()
+    def meta(self):
+        if not self.db:
+            raise TypeError(f"Connection to {self} not established")
+        return self.db.metadata
 
     def build_column(self, name, dtype, **kwargs):
         """Build SQLalchemy Column object given column description."""
         primary = kwargs.get("primary", False)
         fk = [ForeignKey(f)] if (f := kwargs.get("refs")) else []
-        return Column(name, self.get_type(dtype), *fk, primary_key=primary)
+        return Column(name, get_sql_type(dtype), *fk, primary_key=primary)
 
     def build_constraint(self, cols, links):
         """Build SQLalchmy constraint objects given links."""
         return ForeignKeyConstraint(cols, links)
 
     def create_table(self, table, cols, refs=[]):
-        """Create or extend table in db given the description."""
+        """
+        Create or extend table within database given the description.
+
+        Parameters
+        ----------
+        table_name : str
+            Name of the table to create or extend.
+        columns : list of dict
+            List of columns specifications to add to the table.
+        constraints : list of dict, optional
+            List of table constraints.
+        """
         cls = [self.build_column(**c) for c in cols]
         cns = [self.build_constraint(**r) for r in refs]
         table = Table(table, self.meta, *cls, *cns, extend_existing=True)
-        table.create(bind=self.engine, checkfirst=True)
-
-    def get_primary(self, table):
-        """Returns priamry keys for table."""
-        return [c.name for c in self.meta.tables[table].primary_key]
+        table.create(bind=self.connection, checkfirst=True)
 
-    def get_type(self, dtype, default_length=250):
+    def connect(self, username, password):
         """
-        Return supported SQLalchemy type equivalent of provided dtype string.
+        Establish a connection to the database.
 
         Parameters
         ----------
-        dtype: str
-            Supported dtype string representation.
+        username : str
+            The database username.
+        password : str
+            The database password.
 
-        default_length: int, optional
-            Default length of string. Used if required by db backend.
+        Raises
+        ------
+        SQLAlchemyError
+            If the connection cannot be established.
         """
+        url = URL.create(
+            self.backend,
+            username=username,
+            password=password,
+            host=self.host,
+            database=self.name,
+        )
 
-        SQL_TYPE_EQUIVALENT = {
-            "boolean": Boolean,
-            "datetime": DateTime,
-            "float": Float,
-            "integer": Integer,
-            "str": String,
-        }
+        self.db = DBManager(url)
 
-        dtype, length = get_dtype(dtype, default_length)
-        stype = SQL_TYPE_EQUIVALENT[dtype]
+    def get_primary(self, table):
+        """Return priamry keys for table."""
 
-        return stype(length) if length else stype()
+        return [c.name for c in self.meta.tables[table].primary_key]
 
-    def get_table(self, table, cols=None):
-        """
-        Retrieve table records in db as a DataFrame.
+    def get_records(self, table, cols=None):
+        """Retrieve records from table in database as a DataFrame.
 
         Parameters
         ----------
         table : str
             Table in database from which to retrieve records.
-
         cols : list of str
             Column names to select from table.
         """
         return pd.read_sql_table(table, self.connection, columns=cols)
 
     def to_table(
         self,
@@ -121,105 +141,85 @@
         drop_na=None,
         threshold=None,
         if_exists="append",
         index=False,
         insert_method=None,
         **kwargs,
     ):
-        """Write records in DataFrame to a table.
+        """
+        Write records in DataFrame to a table.
 
         Parameters
         ----------
         df : pandas.DataFrame
             DataFrame containing records.
-
         table : str
             Table in database into which the records will be inserted.
-
         check_dups : bool, default True
             Check for duplicates in records.
-
         resolve_dups : [False, 'first', 'last'], default False
             Resolution method for duplicates if found.
-
         check_fks : bool, default False
             Check if foreign keys present in parent.
-
         resolve_fks : bool, default False
             Attempt to resolve missing foreign keys by inserting to parent.
-
         insert_ignore : bool, default Flase
             Ignore insertion of records already present in table.
-
         drop_na : list of df column names, default None
             If provided, records with na in all given columns are dropped.
-
         threshold : int, None
             If non-NA values < threshold, then record dropped.
-
         if_exists : ['append', 'replace', 'fail'], default 'append'
             Insert behavior in case table exists.
-
             - 'append' : Insert new values to the existing table.
             - 'replace' : Drop the table before inserting new values.
             - 'fail' : Raise a ValueError if table exists.
-
         index : bool, default False
             Write DataFrame index as a column. Uses index_label as the
             column name in the table.
-
         insert_method : {None, 'multi', callable}, optional
             Controls the SQL insertion clause used.
-
             - None : Uses standard SQL INSERT clause (one per row).
             - ‘multi’: Pass multiple values in a single INSERT clause.
             - callable with signature ``(pd_table, conn, keys, data_iter)``.
-
             Details and a sample callable implementation can be found
-            in the pandas section `insert method
-            <https://pandas.pydata.org/docs/user_guide/io.html#io-sql-method>`_.
-
+            on Insertion method section of :ref:`pandas:io.sql.method`.
         kwargs : key, value mappings Other keyword arguments are
-            passed down to `pandas.DataFrame.to_sql()
-            <https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.to_sql.html>`_
+            passed down to :doc:`pandas:reference/api/pandas.DataFrame.to_sql`.
 
         Returns
         -------
         rows : None or int
             Number of rows affected by to_sql. None is returned if the
             callable passed into `insert_method` does not return an
             integer number of rows.
 
         Raises
         ------
         ValueError
             - When values provided are not sufficient for insert operation.
             - When the table already exists and `if_exists` is 'fail'.
-
         OperationalError
             - Most likely there are duplicates records in the
               DataFrame. Other reasons are related to the database
-              operation and are detailed in sqlalchemy section
-              `OperationalError
-              <https://docs.sqlalchemy.org/en/20/errors.html#operationalerror>`_.
-
+              operation and are detailed on :ref:`sqlalchemy:error_e3q8`.
         """
 
         if drop_na or threshold:
             logging.info("Dropping records with missing information")
             df = df.dropna(subset=drop_na, thresh=threshold)
 
         if check_dups:
             df = df[self.resolve_dups(df, table, resolve_dups)]
 
         if check_fks:
             df = df[self.resolve_fks(df, table, resolve_fks)]
 
         if insert_ignore:
-            mask = common_records(df, self.get_table(table).astype(df.dtypes))
+            mask = common_rows(df, self.get_records(table).astype(df.dtypes))
             logging.info(f"Ignoring insert of {mask.sum()} common records")
             df = df[~mask]
 
         logging.info(f"Inserting {len(df.index)} records")
 
         df.to_sql(
             table,
@@ -228,47 +228,47 @@
             index=index,
             method=insert_method,
             **kwargs,
         )
 
     def resolve_dups(self, df, table, resolve=False):
         """
-        Resolve duplicate primary keys in DataFrame.
+        Resolve duplicate primary keys.
 
         Parameters
         ----------
         df : pandas.DataFrame
             DataFrame to check for duplicate records.
         table : str
             Table the records will be inserted into.
         resolve : [False, 'first', 'last'], default False
             Determines resolution method.
-
             * False : Mark all duplicates as False.
             * 'first' : Mark duplicates as False except for first occurence.
             * 'last' : Mark duplicates as False except for last occurence.
 
         Returns
         -------
         mask : pandas.Series
             Series of booleans showing whether each record in the
             Dataframe is not a duplicate.
 
         Raises
         ------
         ValueError
             When primary key duplicates are found and `resolve` is True.
-
         """
+
         dups = df.duplicated(self.get_primary(table), resolve)
         log_df(df[dups], "Found duplicate records")
         return ~dups
 
     def resolve_fks(self, df, table, resolve=False):
-        """
+        """Resolve missing foreign keys.
+
         Parameters
         ----------
         df : pandas.DataFrame
             Non-duplicated records to be checked.
         table : str
             Table the records will be inserted into.
         resolve : bool, optional
@@ -282,22 +282,21 @@
 
         Warnings
         --------
         Resolution fails with a ValueError when a foreign key
         constraint on a table does not reference all the columns that
         provide the required values to insert records into the parent
         table.
-
         """
         mask = pd.Series(True, index=df.index)
 
         for fkc in self.meta.tables[table].foreign_key_constraints:
             p_cols = [fk.column.name for fk in fkc.elements]
-            p_df = self.get_table(fkc.referred_table.name, p_cols)
-            p_mask = common_records(df, p_df, fkc.column_keys, p_cols)
+            p_df = self.get_records(fkc.referred_table.name, p_cols)
+            p_mask = common_rows(df, p_df, fkc.column_keys, p_cols)
 
             log_df(df[~p_mask], "Missing parent records")
 
             if not p_mask.all() and resolve:
                 logging.info("Resolving missing records by insert to parent")
                 self.to_table(
                     df[~p_mask][fkc.column_keys].set_axis(p_cols, axis=1),
@@ -308,167 +307,104 @@
                     resolve_fks=True,
                 )
                 p_mask[~p_mask] = True
 
             mask &= p_mask
         return mask
 
-    def __repr__(self):
-        return f"<DBManager '{self.engine.url}'>"
-
+    def report(self):
+        """Generate report for database."""
+        print(f"{self}:")
+
+        for table in self.meta.tables:
+            rows = len(self.get_records(table))
+            print("{:<60} : {:>60} records".format(table, rows))
+
+    def query(self, returns=None, **filters):
+        """Return table records that fit filter criteria."""
+        table = filters.pop("table", None)
+        if not table:
+            return None
+
+        df = self.get_records(table, returns)
+        df = df[np.logical_and.reduce([df[k] == v for k, v in filters.items()])]
+        return df
 
-def get_db(db_path):
-    """Returns SQLalchemy engine for provided URL."""
-    if not db_path:
-        db_path = "sqlite:///{}".format(
-            os.path.join(os.path.expanduser("~"), "index.sqlite")
-        )
-    return create_engine(db_path)
-
-
-def common_records(child, parent, child_on=None, parent_on=None):
-    """Check whether each record in a DataFrame is contained in another."""
-
-    return (
-        pd.merge(
-            child.reset_index(),
-            parent,
-            how="left",
-            left_on=child_on,
-            right_on=parent_on,
-            indicator="exists",
-        )
-        .replace({"both": True, "left_only": False, "right_only": False})
-        .set_index("index")["exists"]
-        .astype("bool")
-    )
+    def __repr__(self):
+        return f"<Database url: '{self.backend}:{self.name}@{self.host}'>"
 
 
 def check_for_key(key, mapping):
     """Return columns in table mapping which contain the key provided."""
 
     return [c["name"] for c in mapping["cols"] if key in c.keys()]
 
 
 def migrate(
     src,
-    target,
+    dst,
     mapping,
     dry_run=False,
     na_vals=[],
     dtype_kws=None,
     **kwargs,
 ):
     """
-    Transforms and migrates records from one db to another.
+    Transform and migrate records from one database to another.
 
     Parameters
     ----------
     src: str
-        SQLAlchemy database URL of database from which data is
-        transferred.
-
-    target: str
-        SQLAlchemy database URL of database to which data is
-        transferred.
-
+        Connection established source Database instance from which data is to
+        be transferred.
+    dst: str
+        Connection established destination Database instance to which data is
+        to be transferred.
     mapping: dict
         Dictionary providing information on column mappings, type,
         transformations, and validation checks.
-
     dry_run: bool
         If dry run, no records are inserted into target and tables are
         not created, but errors and invalid records are logged.
-
     na_vals: list, optional
         List of values to be considered as record not available. By
         default, the values '', 'None', 'NONE', 'NA', and 'Not Applicable'
         are considered.
-
     dtype_kws : dict, optional
         Key, value pairs that will be passed to
-        :meth:`napi.db.set_dtype()`.
-
+        :func:`almirah.utils.df.convert_column_type` kwargs.
     kwargs : key, value mappings
         Other keyword arguments are passed down to
-        :meth:`napi.db.to_table`.
+        `almirah.Database.to_table`.
     """
-
-    s = DBManager(src)
-    t = DBManager(target)
-
     na = ["", "None", "NONE", "NA", "N/A", "<NA>", "Not applicable"] + na_vals
 
     for m in mapping:
         logging.info(f"Transferring table {m['maps']} -> {m['table']}")
 
         # Extract source records
-        records = s.get_table(m["maps"]).replace(na, pd.NA)
+        records = src.get_records(m["maps"]).replace(na, pd.NA)
 
         # Transform and validate
         records = transform(records, dtype_kws, m)
         mask = validate(records, m)
 
         # Reshape data records
         df = reshape(records[mask], m.get("reshape", dict()))
 
         if dry_run:
             continue
 
         # Load records into target
-        t.create_table(m["table"], m["cols"] + m.get("attach", []), m.get("refs", []))
-        t.to_table(df, m["table"], threshold=m.get("threshold"), **kwargs)
-
-
-def set_dtype(series, dtype, **kwargs):
-    """
-    Set dtype of series.
-
-    Parameters
-    ----------
-    series: pandas.Series
-        Series for which the dtype has to set.
-
-    dtype: str
-        Supported dtype to which the series will be converted.
-
-    kwargs: key, value mappings
-        Other keyword arguments are passed down to `pandas.to_datetime()`_
-        if the dtype is 'datetime'.
-    """
-
-    dtype, _ = get_dtype(dtype)
-
-    if dtype == str:
-        series = series.astype(dtype)
-
-    elif dtype == "datetime":
-        series = pd.to_datetime(series, errors="coerce", **kwargs)
-
-    elif dtype in {"float", "integer"}:
-        series = pd.to_numeric(series, errors="coerce", downcast=dtype)
-
-    elif dtype == "boolean":
-        series = series.replace(
-            {
-                "1": True,
-                "0": False,
-                "True": True,
-                "False": False,
-                "Yes": True,
-                "No": False,
-            }
-        )
-        series = series.astype(dtype)
-
-    return series.convert_dtypes()
+        dst.create_table(m["table"], m["cols"] + m.get("attach", []), m.get("refs", []))
+        dst.to_table(df, m["table"], threshold=m.get("threshold"), **kwargs)
 
 
 def reshape(records, steps):
-    """Reshape table records into appropriate shape."""
+    """Reshape records into appropriate shape."""
 
     for procedure in steps:
         [(p, k)] = procedure.items()
 
         if p == "add":
             records[k["name"]] = k["value"]
 
@@ -480,68 +416,72 @@
 
         if p == "pivot":
             records = records.pivot_table(**k).reset_index()
 
     return records
 
 
-def transform(records, dtype_kws, mapping):
-    """Transform table records into appropriate format."""
+def replace_value(value, column, mapping, file):
+    """Return unique replacement for given value based on mapping in file."""
 
-    df = pd.DataFrame(index=records.index)
-    to_hide = check_for_key("hide", mapping)
-    error = pd.Series(False, index=records.index)
-
-    for col in mapping["cols"] + mapping.get("detach", []):
-        name, maps = col["name"], col["maps"]
-        logging.debug(f"Transforming column {name}")
-        df[name], col_error = transform_column(records[maps], dtype_kws, **col)
-        error |= col_error
-
-    log_df(records[error], "Error transforming records", hide=to_hide)
-    return df[~error]
-
-
-def replace_value(value, field, using, file):
-    # Get mapping
-    mapping = pd.read_csv(file, dtype=str)
+    # Load file into dataframe
+    df = pd.read_csv(file, dtype=str)
 
     # Find value to replace
-    result = mapping.query("`%s` == @value" % field)
+    result = df.query("`%s` == @value" % column)
 
     if len(result) == 0:
-        logging.error(f"Value '{value}' not found in field '{field}' of file '{file}'.")
+        logging.error(f"Value '{value}' not found in column '{column}' of '{file}'.")
         return
 
     if len(result) > 1:
-        logging.error(f"Non-unique mappings for value '{value}' in file {file}")
+        logging.error(f"Non-unique mappings for value '{value}' in {file}")
         return
 
-    return result.at[0, using]
+    return result.at[0, mapping]
+
 
+def replace_column(series, column, mapping, file, strict=True):
+    """Replace values in series based on mapping in file."""
 
-def replace_column(series, field, using, file, strict=True):
-    # Load mapping from file
-    mapping = pd.read_csv(file, dtype=str)
-    logging.info(f"Replacing values in '{field}' with '{using}' from {file}")
+    # Load file into dataframe
+    df = pd.read_csv(file, dtype=str)
+    logging.info(f"Replacing values in '{column}' with '{mapping}' from {file}")
 
     # Stop if non-unique mappings
-    if mapping.duplicated([field]).any():
+    if df.duplicated([column]).any():
         raise ValueError(f"Non-unique mappings found in file {file}")
 
-    mapping = pd.Series(mapping[using], index=mapping[field])
-    replaced = series.map(mapping)
+    df = pd.Series(df[mapping], index=df[column])
+    replaced = series.map(df)
 
     # Retain original value if replacement not strict
     if not strict:
         replaced.fillna(series, inplace=True)
 
     return replaced
 
 
+def transform(records, dtype_kws, mapping):
+    """Transform table into appropriate format."""
+
+    df = pd.DataFrame(index=records.index)
+    to_hide = check_for_key("hide", mapping)
+    error = pd.Series(False, index=records.index)
+
+    for col in mapping["cols"] + mapping.get("detach", []):
+        name, maps = col["name"], col["maps"]
+        logging.debug(f"Transforming column {name}")
+        df[name], col_error = transform_column(records[maps], dtype_kws, **col)
+        error |= col_error
+
+    log_df(records[error], "Error transforming records", hide=to_hide)
+    return df[~error]
+
+
 def transform_column(series, dtype_kws=dict(), **kwargs):
     """Transform column to appropriate datatype."""
 
     hide = kwargs.get("hide", False)
     s, error = series.copy(deep=True), series.isna()
 
     if pat := kwargs.get("extract"):
@@ -556,23 +496,23 @@
             s = s.replace({k["value"]: k["with"] for k in rep})
             logging.info("Replacing values with given in config")
 
     if ca := kwargs.get("case"):
         s = s.str.upper() if ca == "upper" else s.str.lower()
         logging.info(f"Changing case to {ca}")
 
-    s = set_dtype(s, kwargs["dtype"], **dtype_kws)
+    s = convert_column_type(s, kwargs["dtype"], **dtype_kws)
     error = series.notna() & s.isna()
     log_col(series[error], f"Error transforming values to {kwargs['dtype']}", hide=hide)
 
     return s, error
 
 
 def validate(records, mapping):
-    """Validate table records and return mask where True means valid."""
+    """Validate table and return mask where True means valid."""
 
     to_hide = check_for_key("hide", mapping)
     mask = pd.Series(True, index=records.index)
 
     for col in mapping["cols"] + mapping.get("detach", []):
         logging.debug(f"Validating column {col['name']}")
         mask &= validate_column(records[col["name"]], **col)
```

### Comparing `almirah-0.2.0/pyproject.toml` & `almirah-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "almirah"
-version = "0.2.0"
+version = "0.3.0"
 description = "a wardrobe for datasets"
 authors = ["girish <girishmm@ncbs.res.in>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.1.4"
 pyyaml = "^6.0.1"
 datalad = "^0.19.3"
 sqlalchemy = "^2.0.19"
+sqlalchemy-json = "^0.7.0"
 
 [tool.poetry.group.mri.dependencies]
 nibabel = "^5.2.0"
 dcm2bids = "^3.1.1"
 pydeface = "^2.0.2"
 
 [tool.poetry.group.eeg.dependencies]
@@ -28,19 +29,16 @@
 mne = "^1.6.0"
 mne-nirs = "^0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 furo = "^2023.9.10"
 towncrier = "^23.6.0"
-sphinx-copybutton = "^0.5.2"
 sphinx-autobuild = "^2021.3.14"
-
-[tool.poetry.group.mariadb.dependencies]
-pymysql = "^1.1.0"
+sphinx-copybutton = "^0.5.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.towncrier]
 package = "almirah"
```

### Comparing `almirah-0.2.0/PKG-INFO` & `almirah-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almirah
-Version: 0.2.0
+Version: 0.3.0
 Summary: a wardrobe for datasets
 License: MIT
 Author: girish
 Author-email: girishmm@ncbs.res.in
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datalad (>=0.19.3,<0.20.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
+Requires-Dist: sqlalchemy-json (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 <div id="top"></div>
 
 <br />
 <div align="center">
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: almirah Version: 0.2.0 Summary: a wardrobe for
+Metadata-Version: 2.1 Name: almirah Version: 0.3.0 Summary: a wardrobe for
 datasets License: MIT Author: girish Author-email: girishmm@ncbs.res.in
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: datalad (>=0.19.3,<0.20.0) Requires-
 Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
-Dist: sqlalchemy (>=2.0.19,<3.0.0) Description-Content-Type: text/markdown
+Dist: sqlalchemy (>=2.0.19,<3.0.0) Requires-Dist: sqlalchemy-json
+(>=0.7.0,<0.8.0) Description-Content-Type: text/markdown
 
                                ******** aallmmiirraahh ********
                            a wardrobe for datasets
                              _EE_xx_pp_ll_oo_rr_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _?Â_?»
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 ## About The Project Clothes can be organized, maintained, and easily accessed
```

