# Comparing `tmp/wingechr-datatools-0.8.0.tar.gz` & `tmp/wingechr-datatools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wingechr-datatools-0.8.0.tar", last modified: Wed Dec 20 08:04:00 2023, max compression
+gzip compressed data, was "wingechr-datatools-0.9.0.tar", last modified: Mon Jan 22 12:25:39 2024, max compression
```

## Comparing `wingechr-datatools-0.8.0.tar` & `wingechr-datatools-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-12-20 08:04:00.332734 wingechr-datatools-0.8.0/
--rw-rw-rw-   0        0        0      115 2023-12-11 15:27:57.000000 wingechr-datatools-0.8.0/.bumpversion.cfg
-drwxrwxrwx   0        0        0        0 2023-12-20 08:03:59.858601 wingechr-datatools-0.8.0/.github/
-drwxrwxrwx   0        0        0        0 2023-12-20 08:03:59.980736 wingechr-datatools-0.8.0/.github/workflows/
--rw-rw-rw-   0        0        0      897 2023-08-22 06:17:46.000000 wingechr-datatools-0.8.0/.github/workflows/test.yml
--rw-rw-rw-   0        0        0      122 2023-11-16 16:12:41.000000 wingechr-datatools-0.8.0/.gitignore
--rw-rw-rw-   0        0        0     1215 2023-08-22 06:17:46.000000 wingechr-datatools-0.8.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      489 2023-12-20 08:04:00.330248 wingechr-datatools-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-08-25 09:18:35.000000 wingechr-datatools-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-12-20 08:04:00.156851 wingechr-datatools-0.8.0/datatools/
--rw-rw-rw-   0        0        0      277 2023-12-11 15:28:06.000000 wingechr-datatools-0.8.0/datatools/__init__.py
--rw-rw-rw-   0        0        0     3311 2023-11-16 16:12:41.000000 wingechr-datatools-0.8.0/datatools/__main__.py
--rw-rw-rw-   0        0        0      758 2023-11-16 16:12:41.000000 wingechr-datatools-0.8.0/datatools/constants.py
--rw-rw-rw-   0        0        0      499 2023-12-11 15:09:25.000000 wingechr-datatools-0.8.0/datatools/exceptions.py
--rw-rw-rw-   0        0        0      543 2023-11-16 16:12:41.000000 wingechr-datatools-0.8.0/datatools/identify.py
--rw-rw-rw-   0        0        0    15578 2023-12-08 10:17:03.000000 wingechr-datatools-0.8.0/datatools/loader.py
--rw-rw-rw-   0        0        0     3861 2023-12-11 15:42:44.000000 wingechr-datatools-0.8.0/datatools/schema.py
--rw-rw-rw-   0        0        0    14631 2023-12-08 10:16:55.000000 wingechr-datatools-0.8.0/datatools/storage.py
--rw-rw-rw-   0        0        0    15450 2023-12-11 15:38:04.000000 wingechr-datatools-0.8.0/datatools/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-20 08:04:00.195473 wingechr-datatools-0.8.0/docs/
--rw-rw-rw-   0        0        0      132 2023-11-16 16:12:41.000000 wingechr-datatools-0.8.0/docs/index.md
--rw-rw-rw-   0        0        0       47 2023-11-16 16:12:41.000000 wingechr-datatools-0.8.0/docs/requirements-docs.txt
--rw-rw-rw-   0        0        0      727 2023-11-16 16:12:41.000000 wingechr-datatools-0.8.0/mkdocs.yml
--rw-rw-rw-   0        0        0      167 2023-11-16 16:12:41.000000 wingechr-datatools-0.8.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-12-20 08:04:00.333218 wingechr-datatools-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1794 2023-12-11 15:28:01.000000 wingechr-datatools-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-20 08:04:00.307613 wingechr-datatools-0.8.0/tests/
--rw-rw-rw-   0        0        0      421 2023-08-22 06:17:46.000000 wingechr-datatools-0.8.0/tests/__init__.py
--rw-rw-rw-   0        0        0     8019 2023-12-11 15:11:07.000000 wingechr-datatools-0.8.0/tests/test_frictionless.py
--rw-rw-rw-   0        0        0     5563 2023-12-11 15:32:06.000000 wingechr-datatools-0.8.0/tests/test_jsonschema.py
--rw-rw-rw-   0        0        0     1628 2023-12-11 15:27:15.000000 wingechr-datatools-0.8.0/tests/test_schema.py
--rw-rw-rw-   0        0        0     6660 2023-12-08 10:16:43.000000 wingechr-datatools-0.8.0/tests/test_storage.py
--rw-rw-rw-   0        0        0     7756 2023-12-11 15:38:04.000000 wingechr-datatools-0.8.0/tests/test_utils.py
--rw-rw-rw-   0        0        0      117 2023-08-22 06:17:46.000000 wingechr-datatools-0.8.0/tox.ini
-drwxrwxrwx   0        0        0        0 2023-12-20 08:04:00.327471 wingechr-datatools-0.8.0/wingechr_datatools.egg-info/
--rw-rw-rw-   0        0        0      489 2023-12-20 08:03:58.000000 wingechr-datatools-0.8.0/wingechr_datatools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      754 2023-12-20 08:03:59.000000 wingechr-datatools-0.8.0/wingechr_datatools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-20 08:03:58.000000 wingechr-datatools-0.8.0/wingechr_datatools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-12-20 08:03:58.000000 wingechr-datatools-0.8.0/wingechr_datatools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2023-12-20 08:03:58.000000 wingechr-datatools-0.8.0/wingechr_datatools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-12-20 08:03:58.000000 wingechr-datatools-0.8.0/wingechr_datatools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:25:39.081192 wingechr-datatools-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-22 12:25:39.081192 wingechr-datatools-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:25:39.081192 wingechr-datatools-0.9.0/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/identify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15071 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20906 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/datatools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 12:25:39.081192 wingechr-datatools-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:25:39.081192 wingechr-datatools-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/tests/test_frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/tests/test_jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7522 2024-01-22 12:25:03.000000 wingechr-datatools-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 12:25:39.081192 wingechr-datatools-0.9.0/wingechr_datatools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-01-22 12:25:39.000000 wingechr-datatools-0.9.0/wingechr_datatools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-01-22 12:25:39.000000 wingechr-datatools-0.9.0/wingechr_datatools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 12:25:39.000000 wingechr-datatools-0.9.0/wingechr_datatools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-22 12:25:39.000000 wingechr-datatools-0.9.0/wingechr_datatools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-22 12:25:39.000000 wingechr-datatools-0.9.0/wingechr_datatools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-22 12:25:39.000000 wingechr-datatools-0.9.0/wingechr_datatools.egg-info/top_level.txt
```

### Comparing `wingechr-datatools-0.8.0/datatools/utils.py` & `wingechr-datatools-0.9.0/datatools/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,594 +1,605 @@
-import atexit
-import csv
-import datetime
-import inspect
-import io
-import json
-import logging
-import os
-import pickle
-import re
-import socket
-import sys
-import time
-from contextlib import ExitStack as _ExitStack
-from io import BufferedReader
-from pathlib import Path
-from typing import Iterable, Union
-from urllib.parse import quote, unquote, unquote_plus, urlsplit
-
-import chardet
-import numpy as np
-import pandas as pd
-import requests
-import sqlparse
-import tzlocal
-import unidecode
-
-from .constants import (
-    ANONYMOUS_USER,
-    DATE_FMT,
-    DATETIMETZ_FMT,
-    DEFAULT_BUFFER_SIZE,
-    FILEMOD_WRITE,
-    LOCALHOST,
-    PARAM_SQL_QUERY,
-    TIME_FMT,
-)
-
-
-class ExitStack(_ExitStack):
-    __singleton_instance = None
-
-    def __new__(cls, *args, **kwargs):
-        if not cls.__singleton_instance:
-            cls.__singleton_instance = super().__new__(cls, *args, **kwargs)
-
-            print("register exit stack")
-
-            # register __exit__ on normal exit
-            atexit.register(cls.__singleton_instance.__exit__, None, None, None)
-
-            # register on unhandled Exception exit
-            sys.excepthook = cls.__singleton_instance.__exit__
-
-        return cls.__singleton_instance
-
-    def __exit__(self, exc_cls, exc_inst, exc_trace):
-        # do regular cleanup
-        super().__exit__(exc_cls, exc_inst, exc_trace)
-        if exc_inst:
-            raise exc_inst
-
-
-def normalize_sql_query(query: str) -> str:
-    """
-    Prettify an SQL query.
-
-    Args:
-        query (str): The SQL query to be prettified.
-
-    Returns:
-        str: The prettified SQL query.
-    """
-    query = sqlparse.format(
-        query,
-        reindent=False,
-        keyword_case="upper",
-        strip_comments=True,
-        strip_whitespace=True,
-    )
-    return query
-
-
-def get_free_port() -> int:
-    """Get a free port by binding to port 0 and releasing it.
-
-    Returns:
-        int: free port
-    """
-    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    sock.bind((LOCALHOST, 0))
-    _, port = sock.getsockname()
-    sock.close()
-    return port
-
-
-def wait_for_server(url, timeout_s=30) -> None:
-    """Wait for server to be responsive"""
-    wait_s = 0.5
-
-    time_start = time.time()
-    while True:
-        try:
-            requests.head(url)
-            logging.debug(f"Server is online: {url}")
-            return True
-        except requests.exceptions.ConnectionError:
-            pass
-
-        time_waited = time.time() - time_start
-        logging.debug(f"checking server ({time_waited}): {url}")
-        if timeout_s is not None and time_waited >= timeout_s:
-            break
-        time.sleep(wait_s)
-    raise Exception("Timeout")
-
-
-def uri_to_data_path(uri: str) -> str:
-    url_parts = urlsplit(uri)
-
-    # start with netloc
-    path = url_parts.netloc or ""
-    if path:
-        path = remove_port_from_url_netloc(path)
-        path = remove_auth_from_url_netloc(path)
-
-    # add actual path
-    path = path + (url_parts.path or "")
-
-    # add fragment
-    path = path + (url_parts.fragment or "")
-
-    path = unquote_plus(path)
-
-    return path
-
-
-def get_resource_path_name(path: str) -> str:
-    """should be all lowercase ascii
-    * uri: remove query
-
-    """
-    _path = path
-
-    path = path.lower()
-    for cin, cout in [
-        ("ä", "ae"),
-        ("ö", "oe"),
-        ("ü", "ue"),
-        ("ß", "ss"),
-    ]:
-        path = path.replace(cin, cout)
-    path = unidecode.unidecode(path)
-    path = re.sub(r":", "", path)
-    path = re.sub(r"[^a-z0-9/_.\-]+", " ", path)
-    path = path.strip()
-    path = re.sub(r"\s+", "_", path)
-    path = re.sub(r"_+", "_", path)
-    path = re.sub(r"/+", "/", path)
-    path = path.strip("/")
-
-    if not path:
-        raise ValueError(_path)
-
-    return path
-
-
-def get_query_arg(kwargs: dict, key: str, default=None) -> str:
-    """query args only come as lists, we want single value"""
-    values = kwargs.get(key)
-    if not values:
-        return default
-    if len(values) > 1:
-        logging.warning("multiple values defined")
-    value = values[0]
-    return unquote_plus(value)
-
-
-def get_hostname() -> str:
-    return socket.gethostname()
-
-
-def get_fqhostname() -> str:
-    """fully qualified hostname (with domain)"""
-    return socket.getfqdn()
-
-
-def get_username() -> str:
-    # getpass.getuser() does not always work
-    return os.environ.get("USERNAME") or os.environ.get("USER") or ANONYMOUS_USER
-
-
-def get_user_w_host() -> str:
-    return f"{get_username()}@{get_fqhostname()}"
-
-
-def get_now() -> datetime.datetime:
-    # my local timezone, e.g.  DstTzInfo 'Europe/Berlin' LMT+0:53:00 STD
-    tz_local = tzlocal.get_localzone()
-    # timezone as current utc offset (does not know about dst),
-    # e.g. datetime.timezone(datetime.timedelta(seconds=3600))
-    now = datetime.datetime.now()
-    # convert unaware datetime to proper timezone...
-    now_tz = now.replace(tzinfo=tz_local)
-    return now_tz
-
-
-def get_now_str() -> str:
-    now = get_now()
-    now_str = now.strftime(DATETIMETZ_FMT)
-    # add ":" in offset
-    now_str = re.sub("([+-][0-9]{2})([0-9]{2})$", r"\1:\2", now_str)
-    return now_str
-
-
-def platform_is_windows() -> bool:
-    # os.name: 'posix', 'nt', 'java'
-    return os.name == "nt"
-
-
-def platform_is_unix() -> bool:
-    return not platform_is_windows()
-
-
-def make_file_readonly(file_path: str) -> None:
-    """Note: in WIndows, this also prevents delete
-    but not in Linux
-    """
-    current_permissions = os.stat(file_path).st_mode
-    readonly_permissions = current_permissions & ~FILEMOD_WRITE
-    os.chmod(file_path, readonly_permissions)
-
-
-def is_file_readonly(file_path: str) -> None:
-    current_permissions = os.stat(file_path).st_mode
-    return not (current_permissions & FILEMOD_WRITE)
-
-
-def make_file_writable(file_path: str) -> None:
-    current_permissions = os.stat(file_path).st_mode
-    readonly_permissions = current_permissions | FILEMOD_WRITE
-    os.chmod(file_path, readonly_permissions)
-
-
-def is_uri(source: str):
-    return bool(re.match(".+://", source))
-
-
-def as_uri(source: str) -> str:
-    if not is_uri(source):
-        # assume local path
-        # uri must be absolute path
-        filepath_abs = Path(source).absolute()
-        uri = filepath_abs_to_uri(filepath_abs=filepath_abs)
-        logging.debug(f"Translate {source} => {uri}")
-    else:
-        uri = source
-    return uri
-
-
-def filepath_abs_to_uri(filepath_abs: Path) -> str:
-    """
-    Args:
-        abspath(Path): must be already absolute path!
-    """
-    uri = filepath_abs.as_uri()
-    url_parts = urlsplit(uri)
-
-    if not url_parts.netloc:
-        url_parts = url_parts._replace(netloc=get_hostname())
-
-    uri = url_parts.geturl()  # unsplit
-
-    # we dont want it quoted
-    uri = unquote(uri)
-
-    return uri
-
-
-def uri_to_filepath_abs(uri: str) -> str:
-    url = urlsplit(uri)
-
-    # if url.scheme != "file":
-    #    raise Exception(f"Not a file path: {uri}")
-
-    is_local = url.netloc == get_hostname()
-    is_win = re.match("/[a-zA-Z]:/", url.path) or (not is_local)
-
-    filepath_abs = url.path
-    if is_win:
-        if is_local:
-            # remove starting /
-            filepath_abs = filepath_abs.lstrip("/")
-
-        else:  # unc share
-            filepath_abs = f"//{url.netloc}{filepath_abs}"
-        filepath_abs = filepath_abs.replace("/", "\\")
-    else:  # posix
-        if not is_local:
-            raise NotImplementedError(f"unc share in posix: {uri}")
-        pass
-
-    return filepath_abs
-
-
-def remove_auth_from_uri_or_path(uri_or_path):
-    """remove username:password@ from uri"""
-    if not is_uri(uri_or_path):
-        return uri_or_path
-    url_parts = urlsplit(uri_or_path)
-    if url_parts.netloc:
-        url_parts = url_parts._replace(
-            netloc=remove_auth_from_url_netloc(url_parts.netloc)
-        )
-    if not url_parts.netloc:
-        # usually, netloc is empty, and so geturl() drops the "//"" at the beginning
-        url_parts = url_parts._replace(path="//" + url_parts.path)
-    return url_parts.geturl()
-
-
-def remove_auth_from_url_netloc(url_netloc: str) -> str:
-    """
-
-    url_path(str): path part of url
-    """
-    return re.sub("[^/@]+@", "", url_netloc)
-
-
-def remove_port_from_url_netloc(url_netloc: str) -> str:
-    """
-
-    url_path(str): path part of url
-    """
-    return re.sub(":[0-9]+$", "", url_netloc)
-
-
-def parse_cli_metadata(metadata_key_vals):
-    """cli: list of key=value"""
-    metadata = {}
-    for key_value in metadata_key_vals:
-        parts = key_value.split("=")
-        key = parts[0]
-        value = "=".join(parts[1:])
-        key = key.strip()
-        value = value.strip()
-        try:
-            value = json.loads(value)
-        except Exception:
-            pass
-        metadata[key] = value
-    return metadata
-
-
-def parse_content_type(ctype: str) -> dict:
-    result = {}
-    parts = [x.strip() for x in ctype.split(";")]
-    result["mediatype"] = parts[0]
-    for key_value in parts[1:]:
-        try:
-            key, value = key_value.split("=")
-            key = key.strip()
-            key = {"charset": "encoding"}.get(key, key)
-            value = value.strip()
-            result[key] = value
-        except Exception:
-            logging.warning(f"cannot parse {key_value}")
-
-    return result
-
-
-def json_serialize(x):
-    if isinstance(x, datetime.datetime):
-        return x.strftime(DATETIMETZ_FMT)
-    elif isinstance(x, datetime.date):
-        return x.strftime(DATE_FMT)
-    elif isinstance(x, datetime.time):
-        return x.strftime(TIME_FMT)
-    elif isinstance(x, np.bool_):
-        return bool(x)
-    elif inspect.isclass(x):
-        # classname
-        return x.__name__
-    else:
-        raise NotImplementedError(f"{x.__class__}: {x}")
-
-
-def as_byte_iterator(data: Union[bytes, Iterable, BufferedReader]) -> Iterable[bytes]:
-    if isinstance(data, bytes):
-        yield data
-    elif isinstance(data, BufferedReader):
-        while True:
-            chunk = data.read(DEFAULT_BUFFER_SIZE)
-            logging.debug(f"read {len(chunk)} bytes")
-            if not chunk:
-                break
-            yield chunk
-        try:
-            data.close()
-        except Exception as exc:
-            logging.warning(f"could not close BufferedReader: {exc}")
-    elif isinstance(data, Iterable):
-        yield from data
-    else:
-        raise NotImplementedError(type(data))
-
-
-def detect_encoding(sample_data: bytes) -> str:
-    result = chardet.detect(sample_data)
-    if result["confidence"] < 1:
-        logging.warning(f"Chardet encoding detection < 100%: {result}")
-    return result["encoding"]
-
-
-def detect_csv_dialect(sample_data: str) -> dict:
-    dialect = csv.Sniffer().sniff(sample_data)
-    dialect_dict = dict(
-        (k, v)
-        for k, v in dialect.__dict__.items()
-        if k
-        in [
-            "lineterminator",
-            "quoting",
-            "doublequote",
-            "delimiter",
-            "quotechar",
-            "skipinitialspace",
-        ]
-    )
-    return dialect_dict
-
-
-def get_sql_table_schema(cursor):
-    fields = [
-        {"name": name, "data_type": data_type, "is_nullable": is_nullable}
-        for (
-            name,
-            data_type,
-            _display_size,
-            _internal_size,
-            _precision,
-            _scale,
-            is_nullable,
-        ) in cursor.description
-    ]
-    return {"fields": fields}
-
-
-def get_df_table_schema(df: pd.DataFrame):
-    fields = []
-    for cname in df.columns:
-        fields.append(
-            {
-                "name": cname,
-                "data_type": df[cname].dtype.name,
-                "is_nullable": (df[cname].isna() | df[cname].isnull()).any(),
-            }
-        )
-    return {"fields": fields}
-
-
-def delete_file(filepath: str) -> str:
-    if not os.path.exists(filepath):
-        return
-    logging.debug(f"DELETING {filepath}")
-    make_file_writable(file_path=filepath)
-    os.remove(filepath)
-
-
-class ByteSerializer:
-    mediatype = None
-    suffix = None
-
-    def dumps(data: object, **kwargs) -> bytes:
-        raise NotImplementedError()
-
-    def loads(data: bytes, **kwargs) -> object:
-        raise NotImplementedError()
-
-
-class CsvSerializer(ByteSerializer):
-    mediatype = "text/csv"
-    suffix = ".csv"
-
-    def dumps(
-        self,
-        data: object,
-        encoding="utf-8",
-        sep=",",
-        lineterminator="\n",
-        **kwargs,
-    ) -> bytes:
-        buf = io.BytesIO()
-        pd.DataFrame(data, **kwargs).to_csv(
-            buf,
-            index=False,
-            encoding=encoding,
-            sep=sep,
-            lineterminator=lineterminator,
-            **kwargs,
-        )
-        bdata = buf.getvalue()
-        return bdata
-
-    def loads(self, data: bytes, encoding="utf-8", sep=",", **kwargs) -> object:
-        buf = io.BytesIO(data)
-        return pd.read_csv(buf, encoding=encoding, sep=sep, **kwargs)
-
-
-class JsonSerializer(ByteSerializer):
-    mediatype = "application/json"
-    suffix = ".json"
-
-    def dumps(self, data: object, **kwargs) -> bytes:
-        return json.dumps(data, **kwargs).encode()
-
-    def loads(self, data: bytes, **kwargs) -> object:
-        return json.loads(data, **kwargs)
-
-
-class PickleSerializer(ByteSerializer):
-    mediatype = "application/x-pickle"
-    suffix = ".pickle"
-
-    def dumps(self, data: object, **kwargs) -> bytes:
-        return pickle.dumps(data, **kwargs)
-
-    def loads(self, data: bytes, **kwargs) -> object:
-        return pickle.loads(data, **kwargs)
-
-
-def get_sql_uri(connection_string_uri: str, sql_query: str) -> str:
-    sql_query = normalize_sql_query(sql_query)
-
-    if "?" in connection_string_uri:
-        connection_string_uri += "&"
-    else:
-        connection_string_uri += "?"
-    uri = connection_string_uri + PARAM_SQL_QUERY + "=" + quote(sql_query)
-
-    return uri
-
-
-def get_suffix(path: str) -> str:
-    suffix = ""
-    while True:
-        path, ext = os.path.splitext(path)
-        if not ext:
-            break
-        suffix = ext + suffix
-    return suffix
-
-
-def get_byte_serializer(suffix: str) -> ByteSerializer:
-    if suffix == ".json":
-        return JsonSerializer()
-    elif suffix == ".csv":
-        return CsvSerializer()
-    elif suffix in (".pickle", ".pkl"):
-        return PickleSerializer()
-    else:
-        raise KeyError(suffix)
-
-
-def df_to_values(df: pd.DataFrame) -> list:
-    """get values from DataFrame, replace nans with None
-
-    Parameters
-    ----------
-    df : pd.DataFrame
-        data
-
-    Returns
-    -------
-    list
-        list of dicts
-    """
-    df = df.astype(object)  # None values need object type
-    df = df.where(~df.isna(), other=None)
-    data = df.to_dict(orient="records")
-    return data
-
-
-def get_err_message(err: Exception) -> str:
-    try:
-        return err["message"]
-    except Exception:
-        pass
-
-    try:
-        return err.message
-    except Exception:
-        pass
-
-    return str(err)
+import atexit
+import csv
+import datetime
+import inspect
+import io
+import json
+import logging
+import os
+import pickle
+import re
+import socket
+import sys
+import time
+from contextlib import ExitStack as _ExitStack
+from io import BufferedReader
+from pathlib import Path
+from typing import Iterable, Union
+from urllib.parse import quote, unquote, unquote_plus, urlsplit
+
+import chardet
+import numpy as np
+import pandas as pd
+import requests
+import sqlparse
+import tzlocal
+import unidecode
+
+from .constants import (
+    ANONYMOUS_USER,
+    DATE_FMT,
+    DATETIMETZ_FMT,
+    DEFAULT_BUFFER_SIZE,
+    FILEMOD_WRITE,
+    LOCALHOST,
+    PARAM_SQL_QUERY,
+    TIME_FMT,
+)
+
+
+def get_pandas_version() -> tuple:
+    return tuple(int(x) for x in pd.__version__.split("."))
+
+
+class ExitStack(_ExitStack):
+    __singleton_instance = None
+
+    def __new__(cls, *args, **kwargs):
+        if not cls.__singleton_instance:
+            cls.__singleton_instance = super().__new__(cls, *args, **kwargs)
+
+            print("register exit stack")
+
+            # register __exit__ on normal exit
+            atexit.register(cls.__singleton_instance.__exit__, None, None, None)
+
+            # register on unhandled Exception exit
+            sys.excepthook = cls.__singleton_instance.__exit__
+
+        return cls.__singleton_instance
+
+    def __exit__(self, exc_cls, exc_inst, exc_trace):
+        # do regular cleanup
+        super().__exit__(exc_cls, exc_inst, exc_trace)
+        if exc_inst:
+            raise exc_inst
+
+
+def normalize_sql_query(query: str) -> str:
+    """
+    Prettify an SQL query.
+
+    Args:
+        query (str): The SQL query to be prettified.
+
+    Returns:
+        str: The prettified SQL query.
+    """
+    query = sqlparse.format(
+        query,
+        reindent=False,
+        keyword_case="upper",
+        strip_comments=True,
+        strip_whitespace=True,
+    )
+    return query
+
+
+def get_free_port() -> int:
+    """Get a free port by binding to port 0 and releasing it.
+
+    Returns:
+        int: free port
+    """
+    sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    sock.bind((LOCALHOST, 0))
+    _, port = sock.getsockname()
+    sock.close()
+    return port
+
+
+def wait_for_server(url, timeout_s=30) -> None:
+    """Wait for server to be responsive"""
+    wait_s = 0.5
+
+    time_start = time.time()
+    while True:
+        try:
+            requests.head(url)
+            logging.debug(f"Server is online: {url}")
+            return True
+        except requests.exceptions.ConnectionError:
+            pass
+
+        time_waited = time.time() - time_start
+        logging.debug(f"checking server ({time_waited}): {url}")
+        if timeout_s is not None and time_waited >= timeout_s:
+            break
+        time.sleep(wait_s)
+    raise Exception("Timeout")
+
+
+def uri_to_data_path(uri: str) -> str:
+    url_parts = urlsplit(uri)
+
+    # start with netloc
+    path = url_parts.netloc or ""
+    if path:
+        path = remove_port_from_url_netloc(path)
+        path = remove_auth_from_url_netloc(path)
+
+    # add actual path
+    path = path + (url_parts.path or "")
+
+    # add fragment
+    path = path + (url_parts.fragment or "")
+
+    path = unquote_plus(path)
+
+    return path
+
+
+def get_resource_path_name(path: str) -> str:
+    """should be all lowercase ascii
+    * uri: remove query
+
+    """
+    _path = path
+
+    path = path.lower()
+    for cin, cout in [
+        ("ä", "ae"),
+        ("ö", "oe"),
+        ("ü", "ue"),
+        ("ß", "ss"),
+    ]:
+        path = path.replace(cin, cout)
+    path = unidecode.unidecode(path)
+    path = re.sub(r":", "", path)
+    path = re.sub(r"[^a-z0-9/_.\-]+", " ", path)
+    path = path.strip()
+    path = re.sub(r"\s+", "_", path)
+    path = re.sub(r"_+", "_", path)
+    path = re.sub(r"/+", "/", path)
+    path = path.strip("/")
+
+    if not path:
+        raise ValueError(_path)
+
+    return path
+
+
+def get_query_arg(kwargs: dict, key: str, default=None) -> str:
+    """query args only come as lists, we want single value"""
+    values = kwargs.get(key)
+    if not values:
+        return default
+    if len(values) > 1:
+        logging.warning("multiple values defined")
+    value = values[0]
+    return unquote_plus(value)
+
+
+def get_hostname() -> str:
+    return socket.gethostname()
+
+
+def get_fqhostname() -> str:
+    """fully qualified hostname (with domain)"""
+    return socket.getfqdn()
+
+
+def get_username() -> str:
+    # getpass.getuser() does not always work
+    return os.environ.get("USERNAME") or os.environ.get("USER") or ANONYMOUS_USER
+
+
+def get_user_w_host() -> str:
+    return f"{get_username()}@{get_fqhostname()}"
+
+
+def get_now() -> datetime.datetime:
+    # my local timezone, e.g.  DstTzInfo 'Europe/Berlin' LMT+0:53:00 STD
+    tz_local = tzlocal.get_localzone()
+    # timezone as current utc offset (does not know about dst),
+    # e.g. datetime.timezone(datetime.timedelta(seconds=3600))
+    now = datetime.datetime.now()
+    # convert unaware datetime to proper timezone...
+    now_tz = now.replace(tzinfo=tz_local)
+    return now_tz
+
+
+def get_now_str() -> str:
+    now = get_now()
+    now_str = now.strftime(DATETIMETZ_FMT)
+    # add ":" in offset
+    now_str = re.sub("([+-][0-9]{2})([0-9]{2})$", r"\1:\2", now_str)
+    return now_str
+
+
+def platform_is_windows() -> bool:
+    # os.name: 'posix', 'nt', 'java'
+    return os.name == "nt"
+
+
+def platform_is_unix() -> bool:
+    return not platform_is_windows()
+
+
+def make_file_readonly(file_path: str) -> None:
+    """Note: in WIndows, this also prevents delete
+    but not in Linux
+    """
+    current_permissions = os.stat(file_path).st_mode
+    readonly_permissions = current_permissions & ~FILEMOD_WRITE
+    os.chmod(file_path, readonly_permissions)
+
+
+def is_file_readonly(file_path: str) -> None:
+    current_permissions = os.stat(file_path).st_mode
+    return not (current_permissions & FILEMOD_WRITE)
+
+
+def make_file_writable(file_path: str) -> None:
+    current_permissions = os.stat(file_path).st_mode
+    readonly_permissions = current_permissions | FILEMOD_WRITE
+    os.chmod(file_path, readonly_permissions)
+
+
+def is_uri(source: str):
+    return bool(re.match(".+://", source))
+
+
+def as_uri(source: str) -> str:
+    if not is_uri(source):
+        # assume local path
+        # uri must be absolute path
+        filepath_abs = Path(source).absolute()
+        uri = filepath_abs_to_uri(filepath_abs=filepath_abs)
+        logging.debug(f"Translate {source} => {uri}")
+    else:
+        uri = source
+    return uri
+
+
+def filepath_abs_to_uri(filepath_abs: Path) -> str:
+    """
+    Args:
+        abspath(Path): must be already absolute path!
+    """
+    uri = filepath_abs.as_uri()
+    url_parts = urlsplit(uri)
+
+    if not url_parts.netloc:
+        url_parts = url_parts._replace(netloc=get_hostname())
+
+    uri = url_parts.geturl()  # unsplit
+
+    # we dont want it quoted
+    uri = unquote(uri)
+
+    return uri
+
+
+def uri_to_filepath_abs(uri: str) -> str:
+    url = urlsplit(uri)
+
+    # if url.scheme != "file":
+    #    raise Exception(f"Not a file path: {uri}")
+
+    is_local = url.netloc == get_hostname()
+    is_win = re.match("/[a-zA-Z]:/", url.path) or (not is_local)
+
+    filepath_abs = url.path
+    if is_win:
+        if is_local:
+            # remove starting /
+            filepath_abs = filepath_abs.lstrip("/")
+
+        else:  # unc share
+            filepath_abs = f"//{url.netloc}{filepath_abs}"
+        filepath_abs = filepath_abs.replace("/", "\\")
+    else:  # posix
+        if not is_local:
+            raise NotImplementedError(f"unc share in posix: {uri}")
+        pass
+
+    return filepath_abs
+
+
+def remove_auth_from_uri_or_path(uri_or_path):
+    """remove username:password@ from uri"""
+    if not is_uri(uri_or_path):
+        return uri_or_path
+    url_parts = urlsplit(uri_or_path)
+    if url_parts.netloc:
+        url_parts = url_parts._replace(
+            netloc=remove_auth_from_url_netloc(url_parts.netloc)
+        )
+    if not url_parts.netloc:
+        # usually, netloc is empty, and so geturl() drops the "//"" at the beginning
+        url_parts = url_parts._replace(path="//" + url_parts.path)
+    return url_parts.geturl()
+
+
+def remove_auth_from_url_netloc(url_netloc: str) -> str:
+    """
+
+    url_path(str): path part of url
+    """
+    return re.sub("[^/@]+@", "", url_netloc)
+
+
+def remove_port_from_url_netloc(url_netloc: str) -> str:
+    """
+
+    url_path(str): path part of url
+    """
+    return re.sub(":[0-9]+$", "", url_netloc)
+
+
+def parse_cli_metadata(metadata_key_vals):
+    """cli: list of key=value"""
+    metadata = {}
+    for key_value in metadata_key_vals:
+        parts = key_value.split("=")
+        key = parts[0]
+        value = "=".join(parts[1:])
+        key = key.strip()
+        value = value.strip()
+        try:
+            value = json.loads(value)
+        except Exception:
+            pass
+        metadata[key] = value
+    return metadata
+
+
+def parse_content_type(ctype: str) -> dict:
+    result = {}
+    parts = [x.strip() for x in ctype.split(";")]
+    result["mediatype"] = parts[0]
+    for key_value in parts[1:]:
+        try:
+            key, value = key_value.split("=")
+            key = key.strip()
+            key = {"charset": "encoding"}.get(key, key)
+            value = value.strip()
+            result[key] = value
+        except Exception:
+            logging.warning(f"cannot parse {key_value}")
+
+    return result
+
+
+def json_serialize(x):
+    if isinstance(x, datetime.datetime):
+        return x.strftime(DATETIMETZ_FMT)
+    elif isinstance(x, datetime.date):
+        return x.strftime(DATE_FMT)
+    elif isinstance(x, datetime.time):
+        return x.strftime(TIME_FMT)
+    elif isinstance(x, np.bool_):
+        return bool(x)
+    elif inspect.isclass(x):
+        # classname
+        return x.__name__
+    else:
+        raise NotImplementedError(f"{x.__class__}: {x}")
+
+
+def as_byte_iterator(data: Union[bytes, Iterable, BufferedReader]) -> Iterable[bytes]:
+    if isinstance(data, bytes):
+        yield data
+    elif isinstance(data, BufferedReader):
+        while True:
+            chunk = data.read(DEFAULT_BUFFER_SIZE)
+            logging.debug(f"read {len(chunk)} bytes")
+            if not chunk:
+                break
+            yield chunk
+        try:
+            data.close()
+        except Exception as exc:
+            logging.warning(f"could not close BufferedReader: {exc}")
+    elif isinstance(data, Iterable):
+        yield from data
+    else:
+        raise NotImplementedError(type(data))
+
+
+def detect_encoding(sample_data: bytes) -> str:
+    result = chardet.detect(sample_data)
+    if result["confidence"] < 1:
+        logging.warning(f"Chardet encoding detection < 100%: {result}")
+    return result["encoding"]
+
+
+def detect_csv_dialect(sample_data: str) -> dict:
+    dialect = csv.Sniffer().sniff(sample_data)
+    dialect_dict = dict(
+        (k, v)
+        for k, v in dialect.__dict__.items()
+        if k
+        in [
+            "lineterminator",
+            "quoting",
+            "doublequote",
+            "delimiter",
+            "quotechar",
+            "skipinitialspace",
+        ]
+    )
+    return dialect_dict
+
+
+def get_sql_table_schema(cursor):
+    fields = [
+        {"name": name, "data_type": data_type, "is_nullable": is_nullable}
+        for (
+            name,
+            data_type,
+            _display_size,
+            _internal_size,
+            _precision,
+            _scale,
+            is_nullable,
+        ) in cursor.description
+    ]
+    return {"fields": fields}
+
+
+def get_df_table_schema(df: pd.DataFrame):
+    fields = []
+    for cname in df.columns:
+        fields.append(
+            {
+                "name": cname,
+                "data_type": df[cname].dtype.name,
+                "is_nullable": (df[cname].isna() | df[cname].isnull()).any(),
+            }
+        )
+    return {"fields": fields}
+
+
+def delete_file(filepath: str) -> str:
+    if not os.path.exists(filepath):
+        return
+    logging.debug(f"DELETING {filepath}")
+    make_file_writable(file_path=filepath)
+    os.remove(filepath)
+
+
+class ByteSerializer:
+    mediatype = None
+    suffix = None
+
+    def dumps(data: object, **kwargs) -> bytes:
+        raise NotImplementedError()
+
+    def loads(data: bytes, **kwargs) -> object:
+        raise NotImplementedError()
+
+
+class CsvSerializer(ByteSerializer):
+    mediatype = "text/csv"
+    suffix = ".csv"
+
+    def dumps(
+        self,
+        data: object,
+        encoding="utf-8",
+        sep=",",
+        lineterminator="\n",
+        **kwargs,
+    ) -> bytes:
+        buf = io.BytesIO()
+        to_csv_kwargs = {
+            "index": False,
+            "encoding": encoding,
+            "sep": sep,
+            "lineterminator": lineterminator,
+        }
+        if get_pandas_version() < (1, 5):
+            to_csv_kwargs["line_terminator"] = to_csv_kwargs.pop("lineterminator")
+
+        pd.DataFrame(data, **kwargs).to_csv(
+            buf,
+            **to_csv_kwargs,
+            **kwargs,
+        )
+
+        bdata = buf.getvalue()
+        return bdata
+
+    def loads(self, data: bytes, encoding="utf-8", sep=",", **kwargs) -> object:
+        buf = io.BytesIO(data)
+        return pd.read_csv(buf, encoding=encoding, sep=sep, **kwargs)
+
+
+class JsonSerializer(ByteSerializer):
+    mediatype = "application/json"
+    suffix = ".json"
+
+    def dumps(self, data: object, **kwargs) -> bytes:
+        return json.dumps(data, **kwargs).encode()
+
+    def loads(self, data: bytes, **kwargs) -> object:
+        return json.loads(data, **kwargs)
+
+
+class PickleSerializer(ByteSerializer):
+    mediatype = "application/x-pickle"
+    suffix = ".pickle"
+
+    def dumps(self, data: object, **kwargs) -> bytes:
+        return pickle.dumps(data, **kwargs)
+
+    def loads(self, data: bytes, **kwargs) -> object:
+        return pickle.loads(data, **kwargs)
+
+
+def get_sql_uri(connection_string_uri: str, sql_query: str) -> str:
+    sql_query = normalize_sql_query(sql_query)
+
+    if "?" in connection_string_uri:
+        connection_string_uri += "&"
+    else:
+        connection_string_uri += "?"
+    uri = connection_string_uri + PARAM_SQL_QUERY + "=" + quote(sql_query)
+
+    return uri
+
+
+def get_suffix(path: str) -> str:
+    suffix = ""
+    while True:
+        path, ext = os.path.splitext(path)
+        if not ext:
+            break
+        suffix = ext + suffix
+    return suffix
+
+
+def get_byte_serializer(suffix: str) -> ByteSerializer:
+    if suffix == ".json":
+        return JsonSerializer()
+    elif suffix == ".csv":
+        return CsvSerializer()
+    elif suffix in (".pickle", ".pkl"):
+        return PickleSerializer()
+    else:
+        raise KeyError(suffix)
+
+
+def df_to_values(df: pd.DataFrame) -> list:
+    """get values from DataFrame, replace nans with None
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        data
+
+    Returns
+    -------
+    list
+        list of dicts
+    """
+    df = df.astype(object)  # None values need object type
+    df = df.where(~df.isna(), other=None)
+    data = df.to_dict(orient="records")
+    return data
+
+
+def get_err_message(err: Exception) -> str:
+    try:
+        return err["message"]
+    except Exception:
+        pass
+
+    try:
+        return err.message
+    except Exception:
+        pass
+
+    return str(err)
```

### Comparing `wingechr-datatools-0.8.0/setup.py` & `wingechr-datatools-0.9.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from setuptools import setup
-
-if __name__ == "__main__":
-    setup(
-        packages=["datatools"],
-        keywords=[],
-        install_requires=[
-            "appdirs",
-            "click",
-            "coloredlogs",
-            "jsonpath-ng>=1.5",
-            "requests",
-            "tzlocal",
-            "unidecode",
-            "sqlalchemy>=2.0",
-            "sqlparse",
-            "pyodbc",
-            "numpy",
-            "pandas",
-            "chardet",
-            "frictionless<5",  # frictionless no longer works with python3.7
-            "jsonschema",
-            "xarray",
-            "openpyxl",
-            "genson",
-        ],
-        install_recommends=[  # this does not do anything, just for information
-            "geopandas",
-            "h5netcdf",
-            "netCDF4",
-            "scipy",
-            "lxml",
-            "rioxarray",
-            "beautifulsoup4",
-            "openpyxl",
-            "rioxarray",
-            "pyproj",
-            "gdal",
-        ],
-        name="wingechr-datatools",
-        description=None,
-        long_description=None,
-        long_description_content_type="text/markdown",
-        version="0.8.0",
-        author="Christian Winger",
-        author_email="c@wingechr.de",
-        url="https://github.com/wingechr/datatools",
-        platforms=["any"],
-        license="Public Domain",
-        project_urls={"Bug Tracker": "https://github.com/wingechr/datatools"},
-        classifiers=[
-            "Programming Language :: Python :: 3",
-            "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
-            "Operating System :: OS Independent",
-        ],
-        entry_points={"console_scripts": ["datatools = datatools.__main__:main"]},
-    )
+from setuptools import setup
+
+if __name__ == "__main__":
+    setup(
+        packages=["datatools"],
+        keywords=[],
+        install_requires=[
+            "appdirs",
+            "click",
+            "coloredlogs",
+            "jsonpath-ng>=1.5",
+            "requests",
+            "tzlocal",
+            "unidecode",
+            "sqlalchemy>=2.0",
+            "sqlparse",
+            "pyodbc",
+            "numpy",
+            "pandas",
+            "chardet",
+            "frictionless<5",  # frictionless no longer works with python3.7
+            "jsonschema",
+            "xarray",
+            "openpyxl",
+            "genson",
+        ],
+        install_recommends=[  # this does not do anything, just for information
+            "geopandas",
+            "h5netcdf",
+            "netCDF4",
+            "scipy",
+            "lxml",
+            "rioxarray",
+            "beautifulsoup4",
+            "openpyxl",
+            "rioxarray",
+            "pyproj",
+            "gdal",
+        ],
+        name="wingechr-datatools",
+        description=None,
+        long_description=None,
+        long_description_content_type="text/markdown",
+        version="0.9.0",
+        author="Christian Winger",
+        author_email="c@wingechr.de",
+        url="https://github.com/wingechr/datatools",
+        platforms=["any"],
+        license="Public Domain",
+        project_urls={"Bug Tracker": "https://github.com/wingechr/datatools"},
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
+            "Operating System :: OS Independent",
+        ],
+        entry_points={"console_scripts": ["datatools = datatools.__main__:main"]},
+    )
```

### Comparing `wingechr-datatools-0.8.0/tests/test_frictionless.py` & `wingechr-datatools-0.9.0/tests/test_frictionless.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,228 +1,228 @@
-"""
-Have a look at the specs at
-* https://json-schema.org/draft/2019-09/json-schema-validation.html#rfc.section.6.1
-* https://specs.frictionlessdata.io/table-schema/#field-descriptors
-* https://github.com/frictionlessdata/specs
-
-"""
-
-import unittest
-
-from datatools.exceptions import SchemaError, ValidationError
-from datatools.schema import validate_resource
-
-
-class TestFrictionless(unittest.TestCase):
-    """Frictionless validators return a list of errors"""
-
-    @staticmethod
-    def create_single_val_resource(value, **field_specs):
-        scm = {
-            "name": "res1",
-            "schema": {"fields": [{"name": "field1"}]},
-            "profile": "tabular-data-resource",
-            "data": [{"field1": value}],
-        }
-        scm["schema"]["fields"][0].update(field_specs)
-        return scm
-
-    def test_resource(self):
-        self.assertRaises(
-            ValidationError, validate_resource, {"name": "name"}
-        )  # must have data (or path)
-        self.assertRaises(
-            ValidationError, validate_resource, {"name": "name", "data": [[]]}
-        )  # empty data is also an error
-        validate_resource({"name": "name", "data": [[99]]})
-
-    def test_type(self):
-        """
-        IMPORTANT:
-            * canonical strings that can be cast as target type are valid.
-            * key constraints are not validated (but unique/required is)
-
-        """
-
-        # numbers
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource("aaa", type="integer"),
-        )
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource(99.9, type="integer"),
-        )
-        validate_resource(self.create_single_val_resource("99", type="integer"))
-        validate_resource(self.create_single_val_resource(99, type="integer"))
-        validate_resource(self.create_single_val_resource("99.9", type="number"))
-        validate_resource(self.create_single_val_resource(99.9, type="number"))
-
-        # strings
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource(99, type="string"),
-        )
-        validate_resource(self.create_single_val_resource("99", type="string"))
-
-        # string + format
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource("abc", type="string", format="uri"),
-        )
-        validate_resource(
-            self.create_single_val_resource(
-                "http://abc.de", type="string", format="uri"
-            )
-        )
-
-        # boolean
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource("aaaa", type="boolean"),
-        )
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource(0, type="boolean"),
-        )
-        validate_resource(self.create_single_val_resource("true", type="boolean"))
-        validate_resource(self.create_single_val_resource(True, type="boolean"))
-
-        # boolean + trueValues
-        validate_resource(
-            self.create_single_val_resource(
-                "1",
-                type="boolean",
-                trueValues=["1", "TRUE"],
-                falseValues=["0", "FALSE"],
-            )
-        )
-
-        # date/times
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource("01.01.1970", type="date"),
-        )
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource("1970-01", type="date"),
-        )
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource("1970-02-31", type="date"),
-        )
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource(0, type="date"),
-        )
-        validate_resource(self.create_single_val_resource("1970-01-01", type="date"))
-
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource("10:11", type="time"),
-        )
-        validate_resource(self.create_single_val_resource("10:11:12", type="time"))
-        validate_resource(
-            self.create_single_val_resource("10:11:12.13", type="time")
-        )  # milliseconds ok too
-
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource("1970-01", type="datetime"),
-        )
-        validate_resource(
-            self.create_single_val_resource("1970-01-01 10:11:12", type="datetime")
-        )
-        validate_resource(
-            self.create_single_val_resource("1970-01-01T10:11:12", type="datetime")
-        )  # T or space is ok
-        validate_resource(
-            self.create_single_val_resource(
-                "1970-01-01 10:11:12+00:10", type="datetime"
-            )
-        )  # offset is ok too
-        validate_resource(
-            self.create_single_val_resource("1970-01-01 10:11:12+0010", type="datetime")
-        )  # this too
-        validate_resource(
-            self.create_single_val_resource("1970-01-01 10:11:12Z", type="datetime")
-        )  # this too
-
-        # IMPORTANT: does not allow for multiple types
-        self.assertRaises(
-            SchemaError,
-            validate_resource,
-            self.create_single_val_resource(True, type=["boolean", "null"]),
-        )
-
-    def test_constraints(self):
-        # missing/required
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource(
-                None, type="string", constraints={"required": True}
-            ),
-        )
-        self.assertRaises(
-            ValidationError,
-            validate_resource,
-            self.create_single_val_resource(
-                "", type="string", constraints={"required": True}
-            ),
-        )
-
-        # minLength/maxLength
-        res = self.create_single_val_resource(
-            "09111", type="string", constraints={"minLength": 5, "maxLength": 5}
-        )
-        validate_resource(res)
-        res["data"][0][0] = "1234"
-        self.assertRaises(ValidationError, validate_resource, res)
-
-        # minimum / maximum
-        res = self.create_single_val_resource(
-            "1980-01-01",
-            type="date",
-            constraints={"minimum": "1970-01-01", "maximum": "2020-01-01"},
-        )
-        validate_resource(res)
-        res["data"][0][0] = "1900-01-01"
-        self.assertRaises(ValidationError, validate_resource, res)
-
-        # pattern
-        res = self.create_single_val_resource(
-            "a1x", type="string", constraints={"pattern": "^a[0-9]{1,2}.*$"}
-        )
-        validate_resource(res)
-        res["data"][0][0] = "ax"
-        self.assertRaises(ValidationError, validate_resource, res)
-
-        # enum
-        res = self.create_single_val_resource(
-            "a", type="string", constraints={"enum": ["a", "b"]}
-        )
-        validate_resource(res)
-        res["data"][0][0] = "c"
-        self.assertRaises(ValidationError, validate_resource, res)
-
-        # unique
-        res = self.create_single_val_resource(
-            10, type="integer", constraints={"unique": True}
-        )
-        validate_resource(res)
-        res["data"].append({"field1": 11})
-        validate_resource(res)
-        res["data"].append({"field1": 10})
-        self.assertRaises(ValidationError, validate_resource, res)
+"""
+Have a look at the specs at
+* https://json-schema.org/draft/2019-09/json-schema-validation.html#rfc.section.6.1
+* https://specs.frictionlessdata.io/table-schema/#field-descriptors
+* https://github.com/frictionlessdata/specs
+
+"""
+
+import unittest
+
+from datatools.exceptions import ValidationError
+from datatools.schema import validate_resource
+
+
+class TestFrictionless(unittest.TestCase):
+    """Frictionless validators return a list of errors"""
+
+    @staticmethod
+    def create_single_val_resource(value, **field_specs):
+        scm = {
+            "name": "res1",
+            "schema": {"fields": [{"name": "field1"}]},
+            "profile": "tabular-data-resource",
+            "data": [{"field1": value}],
+        }
+        scm["schema"]["fields"][0].update(field_specs)
+        return scm
+
+    def test_resource(self):
+        self.assertRaises(
+            ValidationError, validate_resource, {"name": "name"}
+        )  # must have data (or path)
+        self.assertRaises(
+            ValidationError, validate_resource, {"name": "name", "data": [[]]}
+        )  # empty data is also an error
+        validate_resource({"name": "name", "data": [[99]]})
+
+    def test_type(self):
+        """
+        IMPORTANT:
+            * canonical strings that can be cast as target type are valid.
+            * key constraints are not validated (but unique/required is)
+
+        """
+
+        # numbers
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource("aaa", type="integer"),
+        )
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource(99.9, type="integer"),
+        )
+        validate_resource(self.create_single_val_resource("99", type="integer"))
+        validate_resource(self.create_single_val_resource(99, type="integer"))
+        validate_resource(self.create_single_val_resource("99.9", type="number"))
+        validate_resource(self.create_single_val_resource(99.9, type="number"))
+
+        # strings
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource(99, type="string"),
+        )
+        validate_resource(self.create_single_val_resource("99", type="string"))
+
+        # string + format
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource("abc", type="string", format="uri"),
+        )
+        validate_resource(
+            self.create_single_val_resource(
+                "http://abc.de", type="string", format="uri"
+            )
+        )
+
+        # boolean
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource("aaaa", type="boolean"),
+        )
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource(0, type="boolean"),
+        )
+        validate_resource(self.create_single_val_resource("true", type="boolean"))
+        validate_resource(self.create_single_val_resource(True, type="boolean"))
+
+        # boolean + trueValues
+        validate_resource(
+            self.create_single_val_resource(
+                "1",
+                type="boolean",
+                trueValues=["1", "TRUE"],
+                falseValues=["0", "FALSE"],
+            )
+        )
+
+        # date/times
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource("01.01.1970", type="date"),
+        )
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource("1970-01", type="date"),
+        )
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource("1970-02-31", type="date"),
+        )
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource(0, type="date"),
+        )
+        validate_resource(self.create_single_val_resource("1970-01-01", type="date"))
+
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource("10:11", type="time"),
+        )
+        validate_resource(self.create_single_val_resource("10:11:12", type="time"))
+        validate_resource(
+            self.create_single_val_resource("10:11:12.13", type="time")
+        )  # milliseconds ok too
+
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource("1970-01", type="datetime"),
+        )
+        validate_resource(
+            self.create_single_val_resource("1970-01-01 10:11:12", type="datetime")
+        )
+        validate_resource(
+            self.create_single_val_resource("1970-01-01T10:11:12", type="datetime")
+        )  # T or space is ok
+        validate_resource(
+            self.create_single_val_resource(
+                "1970-01-01 10:11:12+00:10", type="datetime"
+            )
+        )  # offset is ok too
+        validate_resource(
+            self.create_single_val_resource("1970-01-01 10:11:12+0010", type="datetime")
+        )  # this too
+        validate_resource(
+            self.create_single_val_resource("1970-01-01 10:11:12Z", type="datetime")
+        )  # this too
+
+        # IMPORTANT: does not allow for multiple types
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource(True, type=["boolean", "null"]),
+        )
+
+    def test_constraints(self):
+        # missing/required
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource(
+                None, type="string", constraints={"required": True}
+            ),
+        )
+        self.assertRaises(
+            ValidationError,
+            validate_resource,
+            self.create_single_val_resource(
+                "", type="string", constraints={"required": True}
+            ),
+        )
+
+        # minLength/maxLength
+        res = self.create_single_val_resource(
+            "09111", type="string", constraints={"minLength": 5, "maxLength": 5}
+        )
+        validate_resource(res)
+        res["data"][0][0] = "1234"
+        self.assertRaises(ValidationError, validate_resource, res)
+
+        # minimum / maximum
+        res = self.create_single_val_resource(
+            "1980-01-01",
+            type="date",
+            constraints={"minimum": "1970-01-01", "maximum": "2020-01-01"},
+        )
+        validate_resource(res)
+        res["data"][0][0] = "1900-01-01"
+        self.assertRaises(ValidationError, validate_resource, res)
+
+        # pattern
+        res = self.create_single_val_resource(
+            "a1x", type="string", constraints={"pattern": "^a[0-9]{1,2}.*$"}
+        )
+        validate_resource(res)
+        res["data"][0][0] = "ax"
+        self.assertRaises(ValidationError, validate_resource, res)
+
+        # enum
+        res = self.create_single_val_resource(
+            "a", type="string", constraints={"enum": ["a", "b"]}
+        )
+        validate_resource(res)
+        res["data"][0][0] = "c"
+        self.assertRaises(ValidationError, validate_resource, res)
+
+        # unique
+        res = self.create_single_val_resource(
+            10, type="integer", constraints={"unique": True}
+        )
+        validate_resource(res)
+        res["data"].append({"field1": 11})
+        validate_resource(res)
+        res["data"].append({"field1": 10})
+        self.assertRaises(ValidationError, validate_resource, res)
```

### Comparing `wingechr-datatools-0.8.0/tests/test_jsonschema.py` & `wingechr-datatools-0.9.0/tests/test_jsonschema.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-"""
-Have a look at the specs at
-* https://json-schema.org/draft/2019-09/json-schema-validation.html#rfc.section.6.1
-* https://specs.frictionlessdata.io/table-schema/#field-descriptors
-* https://github.com/frictionlessdata/specs
-
-"""
-
-import unittest
-
-from datatools.exceptions import SchemaError, ValidationError
-from datatools.schema import get_jsonschema_validator
-
-
-class TestJsonSchema(unittest.TestCase):
-    def test_invalid_schema(self):
-        self.assertRaises(
-            SchemaError,
-            get_jsonschema_validator,
-            {"type": "invalid"},
-        )
-
-    def test_type(self):
-        """
-        The value of this keyword MUST be either a string or an array.
-        If it is an array, elements of the array MUST be strings and MUST be unique.
-
-        Options: "null", "boolean", "object", "array", "number", "string", "integer"
-        """
-
-        validator = get_jsonschema_validator({"type": ["string", "boolean"]})
-        validator("i am string")
-        validator(True)
-        self.assertRaises(ValidationError, validator, 1)
-
-        validator = get_jsonschema_validator({"type": "integer"})
-        self.assertRaises(ValidationError, validator, "100")
-        validator(100)
-
-    def test_enum(self):
-        """
-        The value of this keyword MUST be an array. This array SHOULD have at least one
-        element. Elements in the array SHOULD be unique.
-        """
-
-        validator = get_jsonschema_validator({"enum": ["v1", "v2"]})
-        validator("v1")
-        self.assertRaises(ValidationError, validator, "V2")
-
-    def test_maximum_minimum(self):
-        """
-        The value of "maximum" MUST be a number, representing an inclusive upper limit
-        for a numeric instance.
-        The value of "exclusiveMaximum" MUST be number, representing an exclusive upper
-        limit for a numeric instance.
-
-        Note: this ONLY validates numbers, other values are ok
-        """
-
-        validator = get_jsonschema_validator({"maximum": 100})
-        validator(-1)
-        validator(100)
-        self.assertRaises(ValidationError, validator, 100.01)
-
-        validator = get_jsonschema_validator({"exclusiveMaximum": 100})
-        validator(-1)
-        self.assertRaises(ValidationError, validator, 100)
-
-        validator = get_jsonschema_validator({"exclusiveMinimum": float("-inf")})
-        validator(0)
-        self.assertRaises(ValidationError, validator, float("-inf"))
-
-        # non numeric are ok
-        validator = get_jsonschema_validator({"maximum": 100})
-        validator("1000000")
-
-    def test_min_max_length(self):
-        """
-        The value of this keyword MUST be a non-negative integer.
-        A string instance is valid against this keyword if its length is less than, or
-        equal to, the value of this keyword.
-
-        Note: this ONLY validates strings, other values are ok
-        """
-
-        validator = get_jsonschema_validator({"minLength": 5, "maxLength": 5})
-        validator("09112")
-        self.assertRaises(ValidationError, validator, "9112")
-
-        # non string are ok
-        validator(9112)
-
-    def test_min_max_items(self):
-        """
-        The value of this keyword MUST be a non-negative integer.
-        An array instance is valid against "maxItems" if its size is less than, or equal
-        to, the value of this keyword.
-        """
-
-        validator = get_jsonschema_validator({"minItems": 1, "maxItems": 2})
-        validator(None)  # only tests arrays
-        validator([1])
-        validator([1, None])
-        self.assertRaises(ValidationError, validator, [])
-        self.assertRaises(ValidationError, validator, [1, 2, 3])
-
-    def test_required(self):
-        """
-        The value of this keyword MUST be an array.
-        Elements of this array, if any, MUST be strings, and MUST be unique.
-
-        An object instance is valid against this keyword if every item in the array is
-        the name of a property in the instance.
-        """
-
-        validator = get_jsonschema_validator({"required": ["a", "b"]})
-        validator({"a": 1, "b": 2, "c": 3})
-        self.assertRaises(ValidationError, validator, {"a": 1, "c": 3})
-
-    def test_pattern(self):
-        """
-        The value of this keyword MUST be a string.
-        This string SHOULD be a valid regular expression, according to the
-        ECMA 262 regular expression dialect.
-        """
-
-        validator = get_jsonschema_validator({"pattern": "^a.*$"})
-        validator("aa")
-        self.assertRaises(ValidationError, validator, "Aa")  # case sensitive
-
-        validator = get_jsonschema_validator({"pattern": "a[0-9]{1,2}"})
-        validator("a1x")
-        validator("a11x")
-        self.assertRaises(ValidationError, validator, "ax")
-
-    def test_additional_properties(self):
-        validator_wo_add_prop = get_jsonschema_validator(
-            {
-                "type": "object",
-                "additionalProperties": False,
-                "properties": {"x": {"type": "integer"}},
-            }
-        )
-        validator_w_add_prop = get_jsonschema_validator(
-            {
-                "type": "object",
-                "properties": {"x": {"type": "integer"}},
-            }
-        )
-        validator_w_add_prop({"x": 1})
-        validator_wo_add_prop({"x": 1})
-        validator_w_add_prop({"x": 1, "y": 2})
-        self.assertRaises(ValidationError, validator_wo_add_prop, {"x": 1, "y": 2})
+"""
+Have a look at the specs at
+* https://json-schema.org/draft/2019-09/json-schema-validation.html#rfc.section.6.1
+* https://specs.frictionlessdata.io/table-schema/#field-descriptors
+* https://github.com/frictionlessdata/specs
+
+"""
+
+import unittest
+
+from datatools.exceptions import SchemaError, ValidationError
+from datatools.schema import get_jsonschema_validator
+
+
+class TestJsonSchema(unittest.TestCase):
+    def test_invalid_schema(self):
+        self.assertRaises(
+            SchemaError,
+            get_jsonschema_validator,
+            {"type": "invalid"},
+        )
+
+    def test_type(self):
+        """
+        The value of this keyword MUST be either a string or an array.
+        If it is an array, elements of the array MUST be strings and MUST be unique.
+
+        Options: "null", "boolean", "object", "array", "number", "string", "integer"
+        """
+
+        validator = get_jsonschema_validator({"type": ["string", "boolean"]})
+        validator("i am string")
+        validator(True)
+        self.assertRaises(ValidationError, validator, 1)
+
+        validator = get_jsonschema_validator({"type": "integer"})
+        self.assertRaises(ValidationError, validator, "100")
+        validator(100)
+
+    def test_enum(self):
+        """
+        The value of this keyword MUST be an array. This array SHOULD have at least one
+        element. Elements in the array SHOULD be unique.
+        """
+
+        validator = get_jsonschema_validator({"enum": ["v1", "v2"]})
+        validator("v1")
+        self.assertRaises(ValidationError, validator, "V2")
+
+    def test_maximum_minimum(self):
+        """
+        The value of "maximum" MUST be a number, representing an inclusive upper limit
+        for a numeric instance.
+        The value of "exclusiveMaximum" MUST be number, representing an exclusive upper
+        limit for a numeric instance.
+
+        Note: this ONLY validates numbers, other values are ok
+        """
+
+        validator = get_jsonschema_validator({"maximum": 100})
+        validator(-1)
+        validator(100)
+        self.assertRaises(ValidationError, validator, 100.01)
+
+        validator = get_jsonschema_validator({"exclusiveMaximum": 100})
+        validator(-1)
+        self.assertRaises(ValidationError, validator, 100)
+
+        validator = get_jsonschema_validator({"exclusiveMinimum": float("-inf")})
+        validator(0)
+        self.assertRaises(ValidationError, validator, float("-inf"))
+
+        # non numeric are ok
+        validator = get_jsonschema_validator({"maximum": 100})
+        validator("1000000")
+
+    def test_min_max_length(self):
+        """
+        The value of this keyword MUST be a non-negative integer.
+        A string instance is valid against this keyword if its length is less than, or
+        equal to, the value of this keyword.
+
+        Note: this ONLY validates strings, other values are ok
+        """
+
+        validator = get_jsonschema_validator({"minLength": 5, "maxLength": 5})
+        validator("09112")
+        self.assertRaises(ValidationError, validator, "9112")
+
+        # non string are ok
+        validator(9112)
+
+    def test_min_max_items(self):
+        """
+        The value of this keyword MUST be a non-negative integer.
+        An array instance is valid against "maxItems" if its size is less than, or equal
+        to, the value of this keyword.
+        """
+
+        validator = get_jsonschema_validator({"minItems": 1, "maxItems": 2})
+        validator(None)  # only tests arrays
+        validator([1])
+        validator([1, None])
+        self.assertRaises(ValidationError, validator, [])
+        self.assertRaises(ValidationError, validator, [1, 2, 3])
+
+    def test_required(self):
+        """
+        The value of this keyword MUST be an array.
+        Elements of this array, if any, MUST be strings, and MUST be unique.
+
+        An object instance is valid against this keyword if every item in the array is
+        the name of a property in the instance.
+        """
+
+        validator = get_jsonschema_validator({"required": ["a", "b"]})
+        validator({"a": 1, "b": 2, "c": 3})
+        self.assertRaises(ValidationError, validator, {"a": 1, "c": 3})
+
+    def test_pattern(self):
+        """
+        The value of this keyword MUST be a string.
+        This string SHOULD be a valid regular expression, according to the
+        ECMA 262 regular expression dialect.
+        """
+
+        validator = get_jsonschema_validator({"pattern": "^a.*$"})
+        validator("aa")
+        self.assertRaises(ValidationError, validator, "Aa")  # case sensitive
+
+        validator = get_jsonschema_validator({"pattern": "a[0-9]{1,2}"})
+        validator("a1x")
+        validator("a11x")
+        self.assertRaises(ValidationError, validator, "ax")
+
+    def test_additional_properties(self):
+        validator_wo_add_prop = get_jsonschema_validator(
+            {
+                "type": "object",
+                "additionalProperties": False,
+                "properties": {"x": {"type": "integer"}},
+            }
+        )
+        validator_w_add_prop = get_jsonschema_validator(
+            {
+                "type": "object",
+                "properties": {"x": {"type": "integer"}},
+            }
+        )
+        validator_w_add_prop({"x": 1})
+        validator_wo_add_prop({"x": 1})
+        validator_w_add_prop({"x": 1, "y": 2})
+        self.assertRaises(ValidationError, validator_wo_add_prop, {"x": 1, "y": 2})
```

### Comparing `wingechr-datatools-0.8.0/tests/test_storage.py` & `wingechr-datatools-0.9.0/tests/test_storage.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-import hashlib
-import json
-import logging
-import os
-import pickle
-import sqlite3
-import subprocess as sp
-import sys
-import unittest
-from tempfile import TemporaryDirectory
-
-from datatools.constants import DEFAULT_HASH_METHOD
-from datatools.exceptions import DataDoesNotExists, DataExists
-from datatools.storage import Storage
-from datatools.utils import (
-    get_free_port,
-    make_file_writable,
-    platform_is_unix,
-    wait_for_server,
-)
-
-from . import objects_euqal
-
-
-class MyTemporaryDirectory(TemporaryDirectory):
-    def __init__(self, *args, **kwargs):
-        self.tempdir = TemporaryDirectory(*args, **kwargs)
-
-    def __enter__(self):
-        return self.tempdir.__enter__()
-
-    def __exit__(self, *args):
-        # make files writable so cleanup can delete them
-        path = self.tempdir.name
-        for rt, _ds, fs in os.walk(path):
-            for f in fs:
-                filepath = f"{rt}/{f}"
-                make_file_writable(filepath)
-                logging.debug(f"FILE: {filepath}")
-        # delete dir
-        self.tempdir.__exit__(*args)
-        logging.debug(f"DELETING {path}: {not os.path.exists(path)}")
-
-
-class TestBase(unittest.TestCase):
-    def setUp(self) -> None:
-        self.tempdir1 = MyTemporaryDirectory()
-        path_tempdir1 = self.tempdir1.__enter__()  # exit_stack.enter_context()
-        self.storage = Storage(location=path_tempdir1)
-
-        # set up static file server
-        self.tempdir2 = TemporaryDirectory()
-        self.static_dir = self.tempdir2.__enter__()  # exit_stack.enter_context()
-        port = get_free_port()
-        self.static_url = f"http://localhost:{port}"
-        self.http_proc = sp.Popen(
-            [
-                sys.executable,
-                "-m",
-                "http.server",
-                str(port),
-                "--directory",
-                self.static_dir,
-            ],
-            stdout=sp.DEVNULL,  # do not show server startup message
-            stderr=sp.DEVNULL,  # do not show server request logging
-        )
-        wait_for_server(self.static_url)
-
-    def tearDown(self) -> None:
-        self.http_proc.terminate()  # or kill
-        self.http_proc.wait()
-
-        self.tempdir1.__exit__(None, None, None)
-        self.tempdir2.__exit__(None, None, None)
-
-
-class TestLocalStorage(TestBase):
-    def test_storage(self):
-        # create local instance in temporary dir
-
-        data = b"hello world"
-        data_path_user = "data:///My/path"
-
-        res = self.storage.resource(data_path_user)
-        self.assertFalse(res.exists())
-
-        logging.debug("save data")
-        res.write(data)
-        self.assertTrue(res.exists())
-        self.assertEqual(res.name, "my/path")
-
-        logging.debug("save again will fail")
-        self.assertRaises(DataExists, res.write, data)
-
-        logging.debug("read data")
-        with res.open() as file:
-            _data = file.read()
-        self.assertEqual(data, _data)
-
-        logging.debug("delete (twice, which is allowed)")
-        res.delete()
-        # reading now will raise error
-        self.assertRaises((DataDoesNotExists, NotImplementedError), res.open)
-        res.delete()
-
-        logging.debug("save again")
-        res.write(data)
-
-        logging.debug("save metadata")
-        metadata = {"a": [1, 2, 3], "b.c[0]": "test"}
-        res.metadata.update(metadata)
-
-        logging.debug("update metadata")
-        metadata = {"b.c[1]": "test2"}
-        res.metadata.update(metadata)
-
-        logging.debug("get metadata")
-
-        metadata_b_c = res.metadata.get("b.c")
-        self.assertTrue(objects_euqal(metadata_b_c, ["test", "test2"]), metadata_b_c)
-        metadata_all = res.metadata.get()
-        self.assertTrue(
-            metadata_all["hash"][DEFAULT_HASH_METHOD],
-            getattr(hashlib, DEFAULT_HASH_METHOD)(data).hexdigest,
-        )
-        self.assertTrue(metadata_all["size"], len(data))
-
-    def test_cache_decorator(self):
-        context = {"counter": 0}
-
-        @self.storage.cache()
-        def test_fun_sum(a, b):
-            logging.debug("running test_fun_sum")
-            context["counter"] += 1
-            return a + b
-
-        self.assertEqual(context["counter"], 0)
-        self.assertEqual(test_fun_sum(1, 1), 2)
-        # counted up, because first try
-        self.assertEqual(context["counter"], 1)
-        self.assertEqual(test_fun_sum(1, 1), 2)
-        # not counted up, because cache
-        self.assertEqual(context["counter"], 1)
-        self.assertEqual(test_fun_sum(1, 2), 3)
-        # counted up, because new signature
-        self.assertEqual(context["counter"], 2)
-
-
-class TestResource(TestBase):
-    def test_resource(self):
-        # in memory sqlite3 database
-        query = "select cast(101 as int) as value;"
-        uri = f"sqlite:///:memory:?q={query}#/testquery.pickle"
-        res = self.storage.resource(uri)
-        with res.open() as file:
-            bdata = file.read()
-        data = pickle.loads(bdata)
-        self.assertEqual(data[0]["value"], 101)
-
-        # sqlite file
-        db_filepath = self.static_dir + "/test.db"
-
-        con = sqlite3.connect(db_filepath)
-        cur = con.cursor()
-        cur.execute("create table test(value int);")
-        cur.execute("insert into test values(102);")
-        cur.close()
-        con.commit()
-        con.close()
-
-        # file should be created by sqlalchemy
-        # only for sqlite:
-        # in need an additional slash in linux for abs path
-        if platform_is_unix:
-            db_filepath = "/" + db_filepath
-        uri = f"sqlite://{db_filepath}?q=select value from test#/testquery.pickle"
-
-        res = self.storage.resource(uri)
-        with res.open() as file:
-            bdata = file.read()
-        data = pickle.loads(bdata)
-
-        self.assertEqual(data[0]["value"], 102)
-
-        # create files in static dir
-        fpath = os.path.join(self.static_dir, "testfile.json")
-        with open(fpath, "w", encoding="utf-8") as file:
-            json.dump({"value": 103}, file, ensure_ascii=False)
-
-        # load from path
-        uri = fpath
-        res = self.storage.resource(uri)
-        with res.open() as file:
-            data = json.load(file)
-        self.assertEqual(data["value"], 103)
-
-        # load from webserver
-
-        uri = self.static_url + "/testfile.json"
-        res = self.storage.resource(uri)
-        with res.open() as file:
-            data = json.load(file)
-        self.assertEqual(data["value"], 103)
+import hashlib
+import json
+import logging
+import os
+import pickle
+import sqlite3
+import subprocess as sp
+import sys
+import unittest
+from tempfile import TemporaryDirectory
+
+from datatools.constants import DEFAULT_HASH_METHOD
+from datatools.exceptions import DataDoesNotExists, DataExists
+from datatools.storage import Storage
+from datatools.utils import (
+    get_free_port,
+    make_file_writable,
+    platform_is_unix,
+    wait_for_server,
+)
+
+from . import objects_euqal
+
+
+class MyTemporaryDirectory(TemporaryDirectory):
+    def __init__(self, *args, **kwargs):
+        self.tempdir = TemporaryDirectory(*args, **kwargs)
+
+    def __enter__(self):
+        return self.tempdir.__enter__()
+
+    def __exit__(self, *args):
+        # make files writable so cleanup can delete them
+        path = self.tempdir.name
+        for rt, _ds, fs in os.walk(path):
+            for f in fs:
+                filepath = f"{rt}/{f}"
+                make_file_writable(filepath)
+                logging.debug(f"FILE: {filepath}")
+        # delete dir
+        self.tempdir.__exit__(*args)
+        logging.debug(f"DELETING {path}: {not os.path.exists(path)}")
+
+
+class TestBase(unittest.TestCase):
+    def setUp(self) -> None:
+        self.tempdir1 = MyTemporaryDirectory()
+        path_tempdir1 = self.tempdir1.__enter__()  # exit_stack.enter_context()
+        self.storage = Storage(location=path_tempdir1)
+
+        # set up static file server
+        self.tempdir2 = TemporaryDirectory()
+        self.static_dir = self.tempdir2.__enter__()  # exit_stack.enter_context()
+        port = get_free_port()
+        self.static_url = f"http://localhost:{port}"
+        self.http_proc = sp.Popen(
+            [
+                sys.executable,
+                "-m",
+                "http.server",
+                str(port),
+                "--directory",
+                self.static_dir,
+            ],
+            stdout=sp.DEVNULL,  # do not show server startup message
+            stderr=sp.DEVNULL,  # do not show server request logging
+        )
+        wait_for_server(self.static_url)
+
+    def tearDown(self) -> None:
+        self.http_proc.terminate()  # or kill
+        self.http_proc.wait()
+
+        self.tempdir1.__exit__(None, None, None)
+        self.tempdir2.__exit__(None, None, None)
+
+
+class TestLocalStorage(TestBase):
+    def test_storage(self):
+        # create local instance in temporary dir
+
+        data = b"hello world"
+        data_path_user = "data:///My/path"
+
+        res = self.storage.resource(data_path_user)
+        self.assertFalse(res.exists())
+
+        logging.debug("save data")
+        res.write(data)
+        self.assertTrue(res.exists())
+        self.assertEqual(res.name, "my/path")
+
+        logging.debug("save again will fail")
+        self.assertRaises(DataExists, res.write, data)
+
+        logging.debug("read data")
+        with res.open() as file:
+            _data = file.read()
+        self.assertEqual(data, _data)
+
+        logging.debug("delete (twice, which is allowed)")
+        res.delete()
+        # reading now will raise error
+        self.assertRaises((DataDoesNotExists, NotImplementedError), res.open)
+        res.delete()
+
+        logging.debug("save again")
+        res.write(data)
+
+        logging.debug("save metadata")
+        metadata = {"a": [1, 2, 3], "b.c[0]": "test"}
+        res.metadata.update(metadata)
+
+        logging.debug("update metadata")
+        metadata = {"b.c[1]": "test2"}
+        res.metadata.update(metadata)
+
+        logging.debug("get metadata")
+
+        metadata_b_c = res.metadata.get("b.c")
+        self.assertTrue(objects_euqal(metadata_b_c, ["test", "test2"]), metadata_b_c)
+        metadata_all = res.metadata.get()
+        self.assertTrue(
+            metadata_all["hash"][DEFAULT_HASH_METHOD],
+            getattr(hashlib, DEFAULT_HASH_METHOD)(data).hexdigest,
+        )
+        self.assertTrue(metadata_all["size"], len(data))
+
+    def test_cache_decorator(self):
+        context = {"counter": 0}
+
+        @self.storage.cache()
+        def test_fun_sum(a, b):
+            logging.debug("running test_fun_sum")
+            context["counter"] += 1
+            return a + b
+
+        self.assertEqual(context["counter"], 0)
+        self.assertEqual(test_fun_sum(1, 1), 2)
+        # counted up, because first try
+        self.assertEqual(context["counter"], 1)
+        self.assertEqual(test_fun_sum(1, 1), 2)
+        # not counted up, because cache
+        self.assertEqual(context["counter"], 1)
+        self.assertEqual(test_fun_sum(1, 2), 3)
+        # counted up, because new signature
+        self.assertEqual(context["counter"], 2)
+
+
+class TestResource(TestBase):
+    def test_resource(self):
+        # in memory sqlite3 database
+        query = "select cast(101 as int) as value;"
+        uri = f"sqlite:///:memory:?q={query}#/testquery.pickle"
+        res = self.storage.resource(uri)
+        with res.open() as file:
+            bdata = file.read()
+        data = pickle.loads(bdata)
+        self.assertEqual(data[0]["value"], 101)
+
+        # sqlite file
+        db_filepath = self.static_dir + "/test.db"
+
+        con = sqlite3.connect(db_filepath)
+        cur = con.cursor()
+        cur.execute("create table test(value int);")
+        cur.execute("insert into test values(102);")
+        cur.close()
+        con.commit()
+        con.close()
+
+        # file should be created by sqlalchemy
+        # only for sqlite:
+        # in need an additional slash in linux for abs path
+        if platform_is_unix:
+            db_filepath = "/" + db_filepath
+        uri = f"sqlite://{db_filepath}?q=select value from test#/testquery.pickle"
+
+        res = self.storage.resource(uri)
+        with res.open() as file:
+            bdata = file.read()
+        data = pickle.loads(bdata)
+
+        self.assertEqual(data[0]["value"], 102)
+
+        # create files in static dir
+        fpath = os.path.join(self.static_dir, "testfile.json")
+        with open(fpath, "w", encoding="utf-8") as file:
+            json.dump({"value": 103}, file, ensure_ascii=False)
+
+        # load from path
+        uri = fpath
+        res = self.storage.resource(uri)
+        with res.open() as file:
+            data = json.load(file)
+        self.assertEqual(data["value"], 103)
+
+        # load from webserver
+
+        uri = self.static_url + "/testfile.json"
+        res = self.storage.resource(uri)
+        with res.open() as file:
+            data = json.load(file)
+        self.assertEqual(data["value"], 103)
```

