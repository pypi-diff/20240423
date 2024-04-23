# Comparing `tmp/envzy-0.2.4.tar.gz` & `tmp/envzy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envzy-0.2.4.tar", max compression
+gzip compressed data, was "envzy-0.3.0.tar", max compression
```

## Comparing `envzy-0.2.4.tar` & `envzy-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      227 2024-01-26 11:07:00.875796 envzy-0.2.4/AUTHORS
--rw-r--r--   0        0        0     1868 2024-01-26 11:07:00.875796 envzy-0.2.4/CONTRIBUTING
--rw-r--r--   0        0        0      578 2024-01-26 11:07:00.879796 envzy-0.2.4/LICENSE
--rw-r--r--   0        0        0     1727 2024-01-26 11:07:00.879796 envzy-0.2.4/README.md
--rw-r--r--   0        0        0      375 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/__init__.py
--rw-r--r--   0        0        0     5487 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/auto.py
--rw-r--r--   0        0        0      541 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/base.py
--rw-r--r--   0        0        0    17568 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/classify.py
--rw-r--r--   0        0        0      118 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/exceptions.py
--rw-r--r--   0        0        0      636 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/packages.py
--rw-r--r--   0        0        0        0 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/py.typed
--rw-r--r--   0        0        0     4896 2024-01-26 11:07:00.879796 envzy-0.2.4/envzy/pypi.py
--rw-r--r--   0        0        0     6706 2024-01-26 11:07:00.883796 envzy-0.2.4/envzy/search.py
--rw-r--r--   0        0        0     8969 2024-04-15 08:19:12.388985 envzy-0.2.4/envzy/utils.py
--rw-r--r--   0        0        0      234 2024-01-26 11:07:00.883796 envzy-0.2.4/envzy/version.py
--rw-r--r--   0        0        0     1369 2024-04-15 08:20:00.149436 envzy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 envzy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-01-26 11:07:00.875796 envzy-0.3.0/AUTHORS
+-rw-r--r--   0        0        0     1868 2024-01-26 11:07:00.875796 envzy-0.3.0/CONTRIBUTING
+-rw-r--r--   0        0        0      578 2024-01-26 11:07:00.879796 envzy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1727 2024-01-26 11:07:00.879796 envzy-0.3.0/README.md
+-rw-r--r--   0        0        0      432 2024-04-23 13:52:07.289451 envzy-0.3.0/envzy/__init__.py
+-rw-r--r--   0        0        0     6820 2024-04-23 13:52:07.289451 envzy-0.3.0/envzy/auto.py
+-rw-r--r--   0        0        0      592 2024-04-23 13:52:07.289451 envzy-0.3.0/envzy/base.py
+-rw-r--r--   0        0        0    18048 2024-04-23 13:52:07.293451 envzy-0.3.0/envzy/classify.py
+-rw-r--r--   0        0        0      118 2024-01-26 11:07:00.879796 envzy-0.3.0/envzy/exceptions.py
+-rw-r--r--   0        0        0      666 2024-04-23 13:52:07.293451 envzy-0.3.0/envzy/packages.py
+-rw-r--r--   0        0        0        0 2024-01-26 11:07:00.879796 envzy-0.3.0/envzy/py.typed
+-rw-r--r--   0        0        0     4896 2024-04-18 15:39:31.723734 envzy-0.3.0/envzy/pypi.py
+-rw-r--r--   0        0        0     6706 2024-01-26 11:07:00.883796 envzy-0.3.0/envzy/search.py
+-rw-r--r--   0        0        0      472 2024-04-23 13:52:07.293451 envzy-0.3.0/envzy/spec.py
+-rw-r--r--   0        0        0     8969 2024-04-15 08:19:12.388985 envzy-0.3.0/envzy/utils.py
+-rw-r--r--   0        0        0      234 2024-01-26 11:07:00.883796 envzy-0.3.0/envzy/version.py
+-rw-r--r--   0        0        0     1369 2024-04-23 13:53:29.061848 envzy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 envzy-0.3.0/PKG-INFO
```

### Comparing `envzy-0.2.4/CONTRIBUTING` & `envzy-0.3.0/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `envzy-0.2.4/LICENSE` & `envzy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `envzy-0.2.4/README.md` & `envzy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `envzy-0.2.4/envzy/auto.py` & `envzy-0.3.0/envzy/auto.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import sys
 from dataclasses import dataclass, field
+from operator import attrgetter
 from logging import getLogger
 from typing import List, Type, TypeVar, Tuple, Union, Sequence
 
-from .base import BaseExplorer, ModulePathsList, PackagesDict
+from .base import BaseExplorer
 from .classify import ModuleClassifier
 from .search import VarsNamespace, get_transitive_namespace_dependencies
+from .spec import ModulePathsList, PackagesDict, EnvironmentSpec
 from .packages import (
     BrokenModules,
     LocalPackage,
     BasePackage,
     PypiDistribution,
     LocalDistribution
 )
@@ -29,16 +31,18 @@
     pypi_index_url: str = PYPI_INDEX_URL_DEFAULT
     extra_index_urls: Sequence[str] = ()
     additional_pypi_packages: PackagesDict = field(default_factory=dict)
     target_python: PythonVersion = sys.version_info[:2]
     search_stop_list: Sequence[str] = ()
 
     def get_local_module_paths(self, namespace: VarsNamespace) -> ModulePathsList:
-        packages = self._get_packages(namespace, LocalPackage)
+        packages = self._get_packages(namespace)
+        return self._get_local_module_paths(self._filter(packages, LocalPackage))
 
+    def _get_local_module_paths(self, packages: List[LocalPackage]) -> ModulePathsList:
         filtered: List[LocalPackage] = []
         binary: List[LocalPackage] = []
         nonbinary: List[LocalPackage] = []
 
         for package in packages:
             if package.name in self.additional_pypi_packages:
                 array = filtered
@@ -83,19 +87,21 @@
         if nonbinary:
             logger.debug(
                 "Next dependency packages were classified as local packages "
                 "and will be transfered to a remote host: %s",
                 nonbinary
             )
 
-        return list(set().union(*(p.paths for p in nonbinary)))
+        return sorted(set().union(*(p.paths for p in nonbinary)))
 
     def get_pypi_packages(self, namespace: VarsNamespace) -> PackagesDict:
-        packages = self._get_packages(namespace, PypiDistribution)
+        packages = self._get_packages(namespace)
+        return self._get_pypi_packages(self._filter(packages, PypiDistribution))
 
+    def _get_pypi_packages(self, packages: List[PypiDistribution]) -> PackagesDict:
         overrided: List[PypiDistribution] = []
         bad_platform: List[PypiDistribution] = []
         good: List[PypiDistribution] = []
 
         for package in packages:
             if package.name in self.additional_pypi_packages:
                 array = overrided
@@ -125,19 +131,42 @@
             )
 
         return {
             **{p.name: p.version for p in good},
             **self.additional_pypi_packages
         }
 
+    def get_environment_spec(self, namespace: VarsNamespace) -> EnvironmentSpec:
+        packages = self._get_packages(namespace)
+
+        local_packages = self._filter(packages, LocalPackage)
+        local_module_paths = self._get_local_module_paths(local_packages)
+        console_scripts = self._get_console_scripts(local_packages)
+
+        pypi_packages = self._get_pypi_packages(self._filter(packages, PypiDistribution))
+
+        return EnvironmentSpec(
+            packages=sorted(packages, key=attrgetter('name')),
+            local_module_paths=sorted(local_module_paths),
+            console_scripts=sorted(console_scripts),
+            pypi_packages=pypi_packages
+        )
+
+    def _get_console_scripts(self, packages: List[LocalPackage]) -> List[str]:
+        return list(
+            frozenset().union(*(p.console_scripts for p in packages))
+        )
+
+    def _filter(self, packages: List[BasePackage], filter_class: Type[P]) -> List[P]:
+        return [p for p in packages if isinstance(p, filter_class)]
+
     def _get_packages(
         self,
         namespace: VarsNamespace,
-        filter_class: Type[P],
-    ) -> List[P]:
+    ) -> List[BasePackage]:
         stop_list = frozenset(self.search_stop_list)
         modules = get_transitive_namespace_dependencies(namespace, stop_list=stop_list)
 
         classifier = ModuleClassifier(
             self.pypi_index_url,
             extra_index_urls=tuple(self.extra_index_urls),
             target_python=self.target_python
@@ -147,8 +176,8 @@
         broken = [p for p in packages if isinstance(p, BrokenModules)]
         if broken:
             logger.warning(
                 'while exploring local environment we failed to classify some modules '
                 'so these moduels will be omitted: %s', broken
             )
 
-        return [p for p in packages if isinstance(p, filter_class)]
+        return list(packages)
```

### Comparing `envzy-0.2.4/envzy/classify.py` & `envzy-0.3.0/envzy/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import json
 import os
 import site
+import sys
 from functools import lru_cache
+from pathlib import Path
 from typing import FrozenSet, Set, Dict, cast, Iterable, Tuple, Union, List, Optional
 from types import ModuleType
 
 from importlib.machinery import ExtensionFileLoader
 
 from typing_extensions import assert_never
 from packaging.tags import PythonVersion
@@ -56,14 +58,16 @@
 
         self.stdlib_module_names = get_stdlib_module_names()
         self.builtin_module_names = get_builtin_module_names()
         self.files_to_distributions = get_files_to_distributions()
         self.names_to_distributions = get_names_to_distributions()
         self.requirements_to_meta_packages = get_requirements_to_meta_packages()
 
+        self.scripts_directory = Path(sys.prefix).resolve() / 'bin'
+
         self.bad_prefixes = frozenset([
             site.getusersitepackages()
         ]) | set(site.getsitepackages())
 
     def classify(self, modules: Iterable[ModuleType]) -> FrozenSet[BasePackage]:
         distributions: DistributionSet = set()
         binary_distributions: DistributionSet = set()
@@ -102,14 +106,16 @@
             # so we are generally not interested about it.
             # It can be namespace modules or strange virtual modules as the `six.moves.*`.
             # It's totally okay that we are skipping it and don't require any warning,
             # because we should process such distributions by other properties.
             if not filename:
                 continue
 
+            filename = str(Path(filename).resolve())
+
             # We also not interested in standard modules
             if (
                 top_level in self.stdlib_module_names or
                 top_level in self.builtin_module_names
             ):
                 continue
 
@@ -165,22 +171,23 @@
             return PypiDistribution(
                 name=distribution.name,
                 version=distribution.version,
                 pypi_index_url=pypi_index_url,
                 have_server_supported_tags=have_server_supported_tags,
             )
 
-        paths, bad_paths = self._get_distribution_paths(distribution)
+        paths, console_scripts, bad_paths = self._get_distribution_paths(distribution)
         is_binary = distribution in binary_distributions
         return LocalDistribution(
             name=distribution.name,
             version=distribution.version,
             paths=paths,
             is_binary=is_binary,
             bad_paths=bad_paths,
+            console_scripts=console_scripts,
         )
 
     def _classify_modules_without_distributions(
         self,
         modules_without_distribution: ModulesSet
     ) -> Set[BasePackage]:
         """
@@ -214,15 +221,16 @@
             package = BrokenModules(name='packages_with_bad_path', modules_paths=tuple(broken.items()))
             result.add(package)
 
         for top_level, paths in fake_distributions.items():
             package = LocalPackage(
                 name=top_level,
                 paths=frozenset(paths),
-                is_binary=top_level in binary_distributions
+                is_binary=top_level in binary_distributions,
+                console_scripts=frozenset(),
             )
             result.add(package)
 
         return result
 
     def _process_meta_package_distributions(
         self,
@@ -390,37 +398,43 @@
             name=name,
             version=version,
             target_python=target_python,
         )
 
     def _get_distribution_paths(
         self, distribution: Distribution
-    ) -> Tuple[FrozenSet[str], FrozenSet[str]]:
+    ) -> Tuple[FrozenSet[str], FrozenSet[str], FrozenSet[str]]:
         """
         If Distribution files are foo/bar, foo/baz and foo1,
         we want to return {<site-packages>/foo, <site-packages>/foo1}
         """
 
         paths = set()
         bad_paths = set()
+        console_scripts = set()
 
         base_path = distribution.locate_file('').resolve()
 
         for path in distribution.files or ():
             abs_path = distribution.locate_file(path).resolve()
+
+            if self.scripts_directory in abs_path.parents:
+                console_scripts.add(str(abs_path))
+                continue
+
             if base_path not in abs_path.parents:
                 bad_paths.add(str(abs_path))
                 continue
 
             rel_path = abs_path.relative_to(base_path)
             first_part = rel_path.parts[0]
             result_path = base_path / first_part
             paths.add(str(result_path))
 
-        return frozenset(paths), frozenset(bad_paths)
+        return frozenset(paths), frozenset(console_scripts), frozenset(bad_paths)
 
     def _check_module_is_binary(self, module: ModuleType) -> bool:
         loader = getattr(module, '__loader__', None)
         return bool(loader and isinstance(loader, ExtensionFileLoader))
 
     def _get_top_level_path(self, module: ModuleType) -> Optional[str]:
         """
```

### Comparing `envzy-0.2.4/envzy/packages.py` & `envzy-0.3.0/envzy/packages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import FrozenSet, Dict, Tuple
+from typing import FrozenSet, Tuple
 
 
 @dataclass(frozen=True)
 class BasePackage:
     name: str
 
 
 @dataclass(frozen=True)
 class LocalPackage(BasePackage):
     paths: FrozenSet[str]
+    console_scripts: FrozenSet[str]
     is_binary: bool
 
 
 @dataclass(frozen=True)
 class LocalDistribution(LocalPackage):
     version: str
     bad_paths: FrozenSet[str]
```

### Comparing `envzy-0.2.4/envzy/pypi.py` & `envzy-0.3.0/envzy/pypi.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.4/envzy/search.py` & `envzy-0.3.0/envzy/search.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.4/envzy/utils.py` & `envzy-0.3.0/envzy/utils.py`

 * *Files identical despite different names*

### Comparing `envzy-0.2.4/pyproject.toml` & `envzy-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "envzy"
-version = "0.2.4"
+version = "0.3.0"
 description = "A library that explores dependencies from a given module or namespace in a local Python environment, then classifies these dependencies."
 license = "Apache-2.0"
 authors = ["Vladimir Lipkin <lipkin@yandex-team.ru>"]
 readme = "README.md"
 homepage = "https://github.com/lambdazy/envzy"
 repository = "https://github.com/lambdazy/envzy"
 include = ["AUTHORS", "CONTRIBUTING"]
```

### Comparing `envzy-0.2.4/PKG-INFO` & `envzy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envzy
-Version: 0.2.4
+Version: 0.3.0
 Summary: A library that explores dependencies from a given module or namespace in a local Python environment, then classifies these dependencies.
 Home-page: https://github.com/lambdazy/envzy
 License: Apache-2.0
 Author: Vladimir Lipkin
 Author-email: lipkin@yandex-team.ru
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

