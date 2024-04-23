# Comparing `tmp/nepattern-0.7.0.tar.gz` & `tmp/nepattern-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nepattern-0.7.0.tar", last modified: Sun Apr 21 14:44:42 2024, max compression
+gzip compressed data, was "nepattern-0.7.1.tar", last modified: Tue Apr 23 09:40:33 2024, max compression
```

## Comparing `nepattern-0.7.0.tar` & `nepattern-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1091 2024-02-24 17:08:26.922234 nepattern-0.7.0/LICENSE
--rw-r--r--   0        0        0      943 2024-02-24 17:08:26.923232 nepattern-0.7.0/README.md
--rw-r--r--   0        0        0     2658 2024-04-21 14:43:28.345665 nepattern-0.7.0/nepattern/__init__.py
--rw-r--r--   0        0        0    29406 2024-04-21 14:34:15.607956 nepattern-0.7.0/nepattern/base.py
--rw-r--r--   0        0        0     4148 2024-02-24 17:08:26.923232 nepattern-0.7.0/nepattern/context.py
--rw-r--r--   0        0        0     1507 2024-04-21 13:33:39.317700 nepattern-0.7.0/nepattern/context.pyi
--rw-r--r--   0        0        0    29177 2024-04-21 13:54:20.184287 nepattern-0.7.0/nepattern/core.py
--rw-r--r--   0        0        0    23609 2024-04-21 13:54:38.849885 nepattern-0.7.0/nepattern/core.pyi
--rw-r--r--   0        0        0       63 2024-02-24 17:08:26.924232 nepattern-0.7.0/nepattern/exception.py
--rw-r--r--   0        0        0       26 2024-02-24 17:08:26.924232 nepattern-0.7.0/nepattern/i18n/.config.json
--rw-r--r--   0        0        0      481 2024-02-24 17:08:26.924232 nepattern-0.7.0/nepattern/i18n/en-US.json
--rw-r--r--   0        0        0      470 2024-02-24 17:08:26.924232 nepattern-0.7.0/nepattern/i18n/zh-CN.json
--rw-r--r--   0        0        0     5579 2024-04-21 14:18:56.246589 nepattern-0.7.0/nepattern/main.py
--rw-r--r--   0        0        0     2186 2024-04-21 13:37:01.346873 nepattern-0.7.0/nepattern/main.pyi
--rw-r--r--   0        0        0     1073 2024-02-24 18:59:34.297506 nepattern-0.7.0/nepattern/util.py
--rw-r--r--   0        0        0     2056 2024-04-21 14:44:42.254194 nepattern-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nepattern-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-02-24 17:08:26.922234 nepattern-0.7.1/LICENSE
+-rw-r--r--   0        0        0      943 2024-02-24 17:08:26.923232 nepattern-0.7.1/README.md
+-rw-r--r--   0        0        0     2658 2024-04-21 14:43:28.345665 nepattern-0.7.1/nepattern/__init__.py
+-rw-r--r--   0        0        0    29438 2024-04-23 09:22:22.663290 nepattern-0.7.1/nepattern/base.py
+-rw-r--r--   0        0        0     4148 2024-02-24 17:08:26.923232 nepattern-0.7.1/nepattern/context.py
+-rw-r--r--   0        0        0     1507 2024-04-21 13:33:39.317700 nepattern-0.7.1/nepattern/context.pyi
+-rw-r--r--   0        0        0    29733 2024-04-23 09:37:19.191429 nepattern-0.7.1/nepattern/core.py
+-rw-r--r--   0        0        0    31324 2024-04-23 09:33:16.089736 nepattern-0.7.1/nepattern/core.pyi
+-rw-r--r--   0        0        0       63 2024-02-24 17:08:26.924232 nepattern-0.7.1/nepattern/exception.py
+-rw-r--r--   0        0        0       26 2024-02-24 17:08:26.924232 nepattern-0.7.1/nepattern/i18n/.config.json
+-rw-r--r--   0        0        0      481 2024-02-24 17:08:26.924232 nepattern-0.7.1/nepattern/i18n/en-US.json
+-rw-r--r--   0        0        0      470 2024-02-24 17:08:26.924232 nepattern-0.7.1/nepattern/i18n/zh-CN.json
+-rw-r--r--   0        0        0     5611 2024-04-23 09:38:29.355325 nepattern-0.7.1/nepattern/main.py
+-rw-r--r--   0        0        0     2186 2024-04-21 13:37:01.346873 nepattern-0.7.1/nepattern/main.pyi
+-rw-r--r--   0        0        0     1073 2024-02-24 18:59:34.297506 nepattern-0.7.1/nepattern/util.py
+-rw-r--r--   0        0        0     2056 2024-04-23 09:40:33.481176 nepattern-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1693 1970-01-01 00:00:00.000000 nepattern-0.7.1/PKG-INFO
```

### Comparing `nepattern-0.7.0/LICENSE` & `nepattern-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.0/README.md` & `nepattern-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.0/nepattern/__init__.py` & `nepattern-0.7.1/nepattern/__init__.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.0/nepattern/base.py` & `nepattern-0.7.1/nepattern/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
     def __calc_eq__(self, other):  # pragma: no cover
         return isinstance(other, SwitchPattern) and self.switch == other.switch
 
 
 class ForwardRefPattern(BasePattern[Any, Any, Literal[MatchMode.TYPE_CONVERT]]):
     def __init__(self, ref: ForwardRef):
         self.ref = ref
-        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=Any, alias=ref.__forward_arg__)
+        super().__init__(mode=MatchMode.TYPE_CONVERT, origin=Any, converter=lambda _, x: eval(x), alias=ref.__forward_arg__)
 
     def match(self, input_: Any):
         if isinstance(input_, str) and input_ == self.ref.__forward_arg__:
             return input_
         _main = sys.modules["__main__"]
         if sys.version_info < (3, 9):  # pragma: no cover
             origin = self.ref._evaluate(_main.__dict__, _main.__dict__)
```

### Comparing `nepattern-0.7.0/nepattern/context.py` & `nepattern-0.7.1/nepattern/context.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.0/nepattern/context.pyi` & `nepattern-0.7.1/nepattern/context.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.0/nepattern/core.py` & `nepattern-0.7.1/nepattern/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,14 @@
 TVRF = TypeVar("TVRF", bound=ResultFlag)
 TMM = TypeVar("TMM", bound=MatchMode)
 
 
 class ValidateResult(Generic[TVOrigin, TVRF]):
     """参数表达式验证结果"""
 
-    def __new__(cls, *args, **kwargs):
-        return object.__new__(cls)
-
     def __init__(
         self,
         value: TVOrigin | type[Empty] = Empty,
         error: Exception | type[Empty] = Empty,
         flag: TVRF = ResultFlag.VALID,
     ):
         self._value = value
@@ -330,47 +327,45 @@
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
 def _type_convert_no_previous_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
-    if generic_isinstance(input_, self.origin):
-        return input_
     if not self.accept(input_):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
+    if generic_isinstance(input_, self.origin):
+        return input_
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
 def _type_convert_type_no_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
-    res = self.converter(self, input_)
-    if res is None and not generic_isinstance(res := self.converter(self, self.previous.match(input_)), self.origin):
+    if (res := self.converter(self, input_)) is None and (res := self.converter(self, self.previous.match(input_))) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
 def _type_convert_type_no_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
     if generic_isinstance(input_, self.origin):
         return input_
-    res = self.converter(self, input_)
-    if res is None and not generic_isinstance(res := self.converter(self, self.previous.match(input_)), self.origin):
+    if (res := self.converter(self, input_)) is None and (res := self.converter(self, self.previous.match(input_))) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
 def _type_convert_type_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
@@ -378,35 +373,33 @@
         assert self.previous
     if not self.accept(input_) and not self.accept(input_ := self.previous.match(input_)):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
-    res = self.converter(self, input_)
-    if res is None and not generic_isinstance(res := self.converter(self, self.previous.match(input_)), self.origin):
+    if (res := self.converter(self, input_)) is None and (res := self.converter(self, self.previous.match(input_))) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
 def _type_convert_type_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
-    if generic_isinstance(input_, self.origin):
-        return input_
     if not self.accept(input_) and not self.accept(input_ := self.previous.match(input_)):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
-    res = self.converter(self, input_)
-    if res is None and not generic_isinstance(res := self.converter(self, self.previous.match(input_)), self.origin):
+    if generic_isinstance(input_, self.origin):
+        return input_
+    if (res := self.converter(self, input_)) is None and (res := self.converter(self, self.previous.match(input_))) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
 def _type_convert_value_no_accepts_any(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
@@ -450,24 +443,24 @@
         )
     return res  # type: ignore
 
 
 def _type_convert_value_accepts_other(self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], input_: Any) -> TOrigin:
     if TYPE_CHECKING:
         assert self.previous
-    if generic_isinstance(input_, self.origin):
-        return input_
     if self.accept(input_):
         input_ = self.previous.match(input_)
     elif not self.accept(input_ := self.previous.match(input_)):
         raise MatchFailed(
             lang.require("nepattern", "type_error").format(
                 type=input_.__class__, target=input_, expected=self.alias
             )
         )
+    if generic_isinstance(input_, self.origin):
+        return input_
     if (res := self.converter(self, input_)) is None:
         raise MatchFailed(
             lang.require("nepattern", "content_error").format(target=input_, expected=self.alias)
         )
     return res  # type: ignore
 
 
@@ -574,38 +567,54 @@
 
     def __new__(cls, *args, **kwargs):
         cls.__eq__ = cls.__calc_eq__
         return super().__new__(cls)
 
     def __init__(
         self,
-        pattern: str = ".+",
-        mode: TMM = MatchMode.REGEX_MATCH,
-        origin: type[TOrigin] = str,
+        pattern: str | None = None,
+        mode: TMM | None = None,
+        origin: type[TOrigin] | None = None,
         converter: Callable[[BasePattern, Any], TOrigin | None] | None = None,
         alias: str | None = None,
         previous: BasePattern | None = None,
         accepts: Any = None,
         addition_accepts: BasePattern | None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ):
         """
         初始化参数匹配表达式
         """
-        if pattern.startswith("^") or pattern.endswith("$"):
-            raise ValueError(lang.require("nepattern", "pattern_head_or_tail_error").format(target=pattern))
-        self.pattern = pattern
-        self.regex_pattern = re.compile(f"^{pattern}$")
-        self.mode = MatchMode(mode)
-        self.origin = origin
+        if pattern is None:
+            _origin = origin or Any
+            self.mode = MatchMode(mode or MatchMode.KEEP)
+            self.pattern = ""
+            self.regex_pattern = re.compile("")
+        else:
+            if pattern.startswith("^") or pattern.endswith("$"):
+                raise ValueError(lang.require("nepattern", "pattern_head_or_tail_error").format(target=pattern))
+            self.pattern = pattern
+            self.regex_pattern = re.compile(f"^{pattern}$")
+            self.mode = MatchMode(mode or MatchMode.REGEX_MATCH)
+            _origin = origin or str
+        self.origin: type[TOrigin] = _origin  # type: ignore
         self.alias = alias
         self.previous = previous
-        self.converter = converter or (
-            lambda _, x: (get_origin(origin) or origin)(x) if mode == MatchMode.TYPE_CONVERT else eval(x[0])
-        )
+        if TYPE_CHECKING:
+            assert self.origin is not None
+        if self.mode == MatchMode.TYPE_CONVERT:
+            if not converter and (not origin or origin is Any):
+                raise ValueError(origin)
+            self.converter = converter or (lambda _, x: (get_origin(self.origin) or self.origin)(x))
+        elif self.mode == MatchMode.VALUE_OPERATE:
+            if not converter:
+                raise ValueError(converter)
+            self.converter = converter
+        else:
+            self.converter = converter or (lambda _, x: eval(x[0]))
         self.validators = validators or []
         if accepts is Any or not accepts:
             _accepts = Any
             self._accepts = ()
         else:
             _accepts = get_args(accepts) or accepts
             self._accepts = get_args(accepts) or (accepts,)
@@ -705,15 +714,15 @@
                 raise MatchFailed(lang.require("nepattern", "validate_error").format(target=input_))
             return ValidateResult(value=res, flag=ResultFlag.VALID)
         except Exception as e:
             if default is Empty:
                 return ValidateResult(error=e, flag=ResultFlag.ERROR)
             return ValidateResult(default, flag=ResultFlag.DEFAULT)  # type: ignore
 
-    def copy(self):
+    def copy(self) -> Self:
         return deepcopy(self)
 
     def __rrshift__(self, other):
         return self.validate(other)
 
     def __rmatmul__(self, other) -> Self:  # pragma: no cover
         if isinstance(other, str):
```

### Comparing `nepattern-0.7.0/nepattern/core.pyi` & `nepattern-0.7.1/nepattern/core.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 T = TypeVar("T")
 T1 = TypeVar("T1")
 TInput = TypeVar("TInput")
 TInput1 = TypeVar("TInput1")
 TInput2 = TypeVar("TInput2")
 TInput3 = TypeVar("TInput3")
+TInput4 = TypeVar("TInput4")
 TOrigin = TypeVar("TOrigin")
 TOrigin1 = TypeVar("TOrigin1")
 TVOrigin = TypeVar("TVOrigin")
 TDefault = TypeVar("TDefault")
 TVRF = TypeVar("TVRF", bound=ResultFlag)
 TMM = TypeVar("TMM", bound=MatchMode)
 
@@ -134,81 +135,80 @@
     ): ...
     @overload
     def __init__(
         self: BasePattern[TInput, TInput, Literal[MatchMode.KEEP]],
         *,
         mode: Literal[MatchMode.KEEP],
         accepts: type[TInput],
-        origin: None = None,
+        origin: Any = None,
         alias: str | None = None,
         previous: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TInput], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TInput1, TInput1, Literal[MatchMode.KEEP]],
         *,
         mode: Literal[MatchMode.KEEP],
         addition_accepts: BasePattern[Any, TInput1, Any],
-        origin: None = None,
+        origin: Any = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         validators: list[Callable[[TInput1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TInput1 | TInput2, TInput1 | TInput2, Literal[MatchMode.KEEP]],
         *,
         mode: Literal[MatchMode.KEEP],
         accepts: type[TInput1],
         addition_accepts: BasePattern[Any, TInput2, Any],
-        origin: None = None,
+        origin: Any = None,
         alias: str | None = None,
         previous: None = None,
         validators: list[Callable[[TInput1 | TInput2], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TInput1, TInput1, Literal[MatchMode.KEEP]],
         *,
         mode: Literal[MatchMode.KEEP],
         accepts: type[TInput1],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
-        origin: None = None,
+        origin: Any = None,
         alias: str | None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TInput1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TInput1, TInput1, Literal[MatchMode.KEEP]],
         *,
         mode: Literal[MatchMode.KEEP],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
         addition_accepts: BasePattern[Any, TInput1, Any],
-        origin: None = None,
+        origin: Any = None,
         alias: str | None = None,
         accepts: None = None,
         validators: list[Callable[[TInput1], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TInput1 | TInput2, TInput1 | TInput2, Literal[MatchMode.KEEP]],
         *,
         mode: Literal[MatchMode.KEEP],
         accepts: type[TInput1],
         previous: BasePattern[TInput1 | TInput2, TInput1 | TInput2, Literal[MatchMode.VALUE_OPERATE]],
         addition_accepts: BasePattern[Any, TInput2, Any],
-        origin: None = None,
+        origin: Any = None,
         alias: str | None = None,
         validators: list[Callable[[TInput1 | TInput2], bool]] | None = None,
     ): ...
-
     @overload
     def __init__(
         self: BasePattern[str, str, Literal[MatchMode.REGEX_MATCH]],
         pattern: str,
         mode: Literal[MatchMode.REGEX_MATCH],
         origin: type[str] = str,
         converter: None = None,
@@ -240,15 +240,14 @@
         origin: type[str] = str,
         converter: None = None,
         alias: str | None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
         validators: list[Callable[[str], bool]] | None = None,
     ): ...
-
     @overload
     def __init__(
         self: BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]],
         pattern: str,
         mode: Literal[MatchMode.REGEX_CONVERT],
         origin: type[TOrigin],
         converter: Callable[[BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]], TOrigin | None]
@@ -283,62 +282,87 @@
         converter: Callable[[BasePattern[TOrigin, str | TOrigin, Literal[MatchMode.REGEX_CONVERT]], re.Match[str]], TOrigin | None]
         | None = None,
         alias: str | None = None,
         accepts: type[str] = str,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
-
     @overload
     def __init__(
         self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
-        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None] | None = None,
+        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None],
+        origin:  None = None,
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | Any, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
-        origin: type[TOrigin],
-        previous: BasePattern[Any, TInput1, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None] | None = None,
+        accepts: type[TInput1],
+        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
+        origin:  None = None,
         alias: str | None = None,
-        accepts: None = None,
+        previous: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput1 | Any, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
+        addition_accepts: BasePattern[Any, TInput1, Any],
+        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
+        origin:  None = None,
+        alias: str | None = None,
+        previous: None = None,
+        accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
+        accepts: type[TInput1],
+        addition_accepts: BasePattern[Any, TInput2, Any],
+        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput2], TOrigin | None],
+        origin:  None = None,
+        alias: str | None = None,
+        previous: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
-        previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None] | None = None,
+        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], Any], TOrigin | None] | None = None,
         alias: str | None = None,
+        previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
-        self: BasePattern[TOrigin, TInput, Literal[MatchMode.TYPE_CONVERT]],
+        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
-        accepts: type[TInput],
-        converter: Callable[[BasePattern[TOrigin, TInput, Literal[MatchMode.REGEX_CONVERT]], TInput], TOrigin | None] | None = None,
+        accepts: type[TInput1],
+        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
         alias: str | None = None,
         previous: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
@@ -365,22 +389,100 @@
         | None = None,
         alias: str | None = None,
         previous: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
+        self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
+        previous: BasePattern[TInput1, Any, Literal[MatchMode.TYPE_CONVERT]],
+        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None],
+        alias: str | None = None,
+        origin: None = None,
+        accepts: None = None,
+        addition_accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
+        origin: type[TOrigin],
+        previous: BasePattern[TInput1, Any, Literal[MatchMode.TYPE_CONVERT]],
+        converter: Callable[[BasePattern[TOrigin, Any, Literal[MatchMode.TYPE_CONVERT]], TInput1 | Any], TOrigin | None] | None = None,
+        alias: str | None = None,
+        accepts: None = None,
+        addition_accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
+        previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
+        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
+        alias: str | None = None,
+        origin: None = None,
+        accepts: None = None,
+        addition_accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
+        origin: type[TOrigin],
+        previous:  BasePattern[TOrigin | TInput1, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
+        converter: Callable[[BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
+        alias: str | None = None,
+        accepts: None = None,
+        addition_accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
+        accepts: type[TInput1],
+        previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4], TOrigin | None],
+        alias: str | None = None,
+        origin: None = None,
+        addition_accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
-        previous: BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
+        previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4], TOrigin | None] | None = None,
+        alias: str | None = None,
+        addition_accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
+        accepts: type[TInput1],
+        previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
+        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
         alias: str | None = None,
+        origin:  None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
@@ -394,54 +496,106 @@
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
+        addition_accepts: BasePattern[Any, TInput1, Any],
+        previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4], TOrigin | None],
+        alias: str | None = None,
+        origin: None = None,
+        accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         addition_accepts: BasePattern[Any, TInput1, Any],
-        previous: BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
+        previous: BasePattern[TInput4 | TInput1, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput4], TOrigin | None] | None = None,
         alias: str | None = None,
         accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
+        addition_accepts: BasePattern[Any, TInput1, Any],
+        previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
+        converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None],
+        alias: str | None = None,
+        origin: None = None,
+        accepts: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         addition_accepts: BasePattern[Any, TInput1, Any],
         previous: BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
         converter: Callable[[BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]], TInput1], TOrigin | None] | None = None,
         alias: str | None = None,
         accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
+        accepts: type[TInput1],
+        previous: BasePattern[TInput1 | TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]],
+        addition_accepts: BasePattern[Any, TInput3, Any],
+        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3], TOrigin | None],
+        alias: str | None = None,
+        origin: None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
         previous: BasePattern[TInput1 | TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TInput1, TInput2, Literal[MatchMode.TYPE_CONVERT]] | BasePattern[TInput3, TInput2, Literal[MatchMode.TYPE_CONVERT]],
         addition_accepts: BasePattern[Any, TInput3, Any],
         converter: Callable[[BasePattern[TOrigin, TInput1 | TInput2 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3], TOrigin | None]
         | None = None,
         alias: str | None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
         *,
         mode: Literal[MatchMode.TYPE_CONVERT],
+        accepts: type[TInput1],
+        previous: BasePattern[TInput1 | TInput3, TInput1 | TInput3, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput3, TInput3, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
+        addition_accepts: BasePattern[Any, TInput3, Any],
+        converter: Callable[[BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3], TOrigin | None],
+        origin: None = None,
+        alias: str | None = None,
+        validators: list[Callable[[TOrigin], bool]] | None = None,
+    ): ...
+    @overload
+    def __init__(
+        self: BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]],
+        *,
+        mode: Literal[MatchMode.TYPE_CONVERT],
         origin: type[TOrigin],
         accepts: type[TInput1],
         previous: BasePattern[TInput1 | TInput3, TInput1 | TInput3, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput3, TInput3, Literal[MatchMode.VALUE_OPERATE]] | BasePattern[TInput1, TInput1, Literal[MatchMode.VALUE_OPERATE]],
         addition_accepts: BasePattern[Any, TInput3, Any],
         converter: Callable[[BasePattern[TOrigin, TInput1 | TInput3, Literal[MatchMode.TYPE_CONVERT]], TInput1 | TInput3], TOrigin | None]
         | None = None,
         alias: str | None = None,
@@ -449,42 +603,42 @@
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
         origin: type[TOrigin],
-        converter: Callable[[BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None] | None = None,
+        converter: Callable[[BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None],
         alias: str | None = None,
         previous: None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
         origin: type[TOrigin],
         previous: BasePattern[TOrigin, TInput1, Literal[MatchMode.TYPE_CONVERT]],
-        converter: Callable[[BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None] | None = None,
+        converter: Callable[[BasePattern[TOrigin, TOrigin | TInput1, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None],
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     @overload
     def __init__(
         self: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
         *,
         mode: Literal[MatchMode.VALUE_OPERATE],
         origin: type[TOrigin],
         previous: BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]],
-        converter: Callable[[BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None] | None = None,
+        converter: Callable[[BasePattern[TOrigin, TOrigin, Literal[MatchMode.VALUE_OPERATE]], TOrigin], TOrigin | None],
         alias: str | None = None,
         accepts: None = None,
         addition_accepts: None = None,
         validators: list[Callable[[TOrigin], bool]] | None = None,
     ): ...
     def refresh(self): ...
     def __calc_hash__(self): ...
```

### Comparing `nepattern-0.7.0/nepattern/main.py` & `nepattern-0.7.1/nepattern/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,16 @@
     if getattr(item, "_is_protocol", False):
         return _protocol_parser(item)
     if isinstance(item, (FunctionType, MethodType, LambdaType)):
         if len((sig := inspect.signature(item)).parameters) not in (1, 2):  # pragma: no cover
             raise TypeError(f"{item} can only accept 1 or 2 argument")
         anno = list(sig.parameters.values())[-1].annotation
         return BasePattern(
-            accepts=Any if anno == inspect.Signature.empty else anno,
-            origin=(Any if sig.return_annotation == inspect.Signature.empty else sig.return_annotation),
+            accepts=Any if anno == inspect.Signature.empty else anno,  # type: ignore
+            origin=(Any if sig.return_annotation == inspect.Signature.empty else sig.return_annotation),  # type: ignore
             converter=item if len(sig.parameters) == 2 else lambda _, x: item(x),
             mode=MatchMode.TYPE_CONVERT,
         )
     if isinstance(item, TPattern):  # type: ignore
         return RegexPattern(item.pattern, alias=f"'{item.pattern}'")
     if isinstance(item, str):
         if item.startswith("re:"):
```

### Comparing `nepattern-0.7.0/nepattern/main.pyi` & `nepattern-0.7.1/nepattern/main.pyi`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.0/nepattern/util.py` & `nepattern-0.7.1/nepattern/util.py`

 * *Files identical despite different names*

### Comparing `nepattern-0.7.0/pyproject.toml` & `nepattern-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nepattern"
-version = "0.7.0"
+version = "0.7.1"
 description = "a complex pattern, support typing"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "typing-extensions>=4.5.0",
     "tarina>=0.4.1",
```

### Comparing `nepattern-0.7.0/PKG-INFO` & `nepattern-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nepattern
-Version: 0.7.0
+Version: 0.7.1
 Summary: a complex pattern, support typing
 Keywords: typing,pattern,converter,validator
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

