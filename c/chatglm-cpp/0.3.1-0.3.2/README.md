# Comparing `tmp/chatglm-cpp-0.3.1.tar.gz` & `tmp/chatglm_cpp-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-cpp-0.3.1.tar", last modified: Sat Jan 20 15:19:44 2024, max compression
+gzip compressed data, was "chatglm_cpp-0.3.2.tar", last modified: Tue Apr 23 15:34:59 2024, max compression
```

## Comparing `chatglm-cpp-0.3.1.tar` & `chatglm_cpp-0.3.2.tar`

### file list

```diff
@@ -1,391 +1,391 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.773129 chatglm-cpp-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28238 2024-01-20 15:19:44.773129 chatglm-cpp-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27154 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    63819 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    48046 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.705129 chatglm-cpp-0.3.1/chatglm_cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm_cpp/_C.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm_cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21569 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm_cpp/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm_cpp/langchain_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8409 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm_cpp/openai_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.773129 chatglm-cpp-0.3.1/chatglm_cpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28238 2024-01-20 15:19:44.000000 chatglm-cpp-0.3.1/chatglm_cpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17820 2024-01-20 15:19:44.000000 chatglm-cpp-0.3.1/chatglm_cpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-20 15:19:44.000000 chatglm-cpp-0.3.1/chatglm_cpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-20 15:19:44.000000 chatglm-cpp-0.3.1/chatglm_cpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-20 15:19:44.000000 chatglm-cpp-0.3.1/chatglm_cpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm_pybind.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    69902 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/chatglm_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.705129 chatglm-cpp-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    13359 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/main.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-20 15:19:44.773129 chatglm-cpp-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.705129 chatglm-cpp-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/tests/test_chatglm_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)    28333 2024-01-20 15:19:29.000000 chatglm-cpp-0.3.1/tests/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.701129 chatglm-cpp-0.3.1/third_party/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-20 15:19:30.000000 chatglm-cpp-0.3.1/third_party/ggml/.git
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/build.zig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/cmake/BuildTypes.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/cmake/GitVars.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/examples/dolly-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/dolly-v2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/dolly-v2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-2/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-j/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-j/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-j/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-neox/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-neox/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-neox/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/examples/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/mnist/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/mnist/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.709129 chatglm-cpp-0.3.1/third_party/ggml/examples/mpt/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/mpt/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/mpt/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.713129 chatglm-cpp-0.3.1/third_party/ggml/examples/python/
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.713129 chatglm-cpp-0.3.1/third_party/ggml/examples/replit/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/replit/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.713129 chatglm-cpp-0.3.1/third_party/ggml/examples/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/sam/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/sam/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.713129 chatglm-cpp-0.3.1/third_party/ggml/examples/starcoder/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/starcoder/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/starcoder/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.713129 chatglm-cpp-0.3.1/third_party/ggml/examples/whisper/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/whisper/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/examples/whisper/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/ggml.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.697129 chatglm-cpp-0.3.1/third_party/ggml/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.713129 chatglm-cpp-0.3.1/third_party/ggml/include/ggml/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/include/ggml/ggml-alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/include/ggml/ggml-backend.h
--rw-r--r--   0 runner    (1001) docker     (127)    76877 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/include/ggml/ggml.h
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.717129 chatglm-cpp-0.3.1/third_party/ggml/src/
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22783 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-alloc.c
--rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-backend.c
--rw-r--r--   0 runner    (1001) docker     (127)   294413 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-cuda.h
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-metal.h
--rw-r--r--   0 runner    (1001) docker     (127)    81148 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-metal.m
--rw-r--r--   0 runner    (1001) docker     (127)    91862 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-metal.metal
--rw-r--r--   0 runner    (1001) docker     (127)    71169 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-opencl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml-opencl.h
--rw-r--r--   0 runner    (1001) docker     (127)   735658 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/src/ggml.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.717129 chatglm-cpp-0.3.1/third_party/ggml/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/ggml/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.717129 chatglm-cpp-0.3.1/third_party/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.697129 chatglm-cpp-0.3.1/third_party/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.721129 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.721129 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (127)    28518 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (127)    53480 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (127)    17859 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (127)    28221 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (127)    48364 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.721129 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eigen/common.h
--rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (127)    79725 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (127)   126706 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (127)    98455 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (127)    29897 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    21733 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.725129 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.729129 chatglm-cpp-0.3.1/third_party/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-01-20 15:19:32.000000 chatglm-cpp-0.3.1/third_party/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.729129 chatglm-cpp-0.3.1/third_party/sentencepiece/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-20 15:19:31.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/.git
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.729129 chatglm-cpp-0.3.1/third_party/sentencepiece/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)    46672 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/cmake/ios.toolchain.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.729129 chatglm-cpp-0.3.1/third_party/sentencepiece/python/
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/python/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/sentencepiece.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.753129 chatglm-cpp-0.3.1/third_party/sentencepiece/src/
--rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model.h
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model_trainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model_trainer.h
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model_trainer_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18686 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/builder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/builder.h
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/builder_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.753129 chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/
--rw-r--r--   0 runner    (1001) docker     (127)    35154 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
--rw-r--r--   0 runner    (1001) docker     (127)    40648 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/sentencepiece.pb.h
--rw-r--r--   0 runner    (1001) docker     (127)   136631 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
--rw-r--r--   0 runner    (1001) docker     (127)   200094 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model.h
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model_trainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model_trainer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model_trainer_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/compile_charsmap_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/error.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/filesystem.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/filesystem_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/freelist.h
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/freelist_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/init.h
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/init_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_factory.cc
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_factory.h
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_factory_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_interface.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_interface_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)  7198605 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/normalization_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/normalizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/normalizer.h
--rw-r--r--   0 runner    (1001) docker     (127)    16156 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/normalizer_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/pretokenizer_for_training.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/pretokenizer_for_training.h
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/pretokenizer_for_training_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece.proto
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_model.proto
--rw-r--r--   0 runner    (1001) docker     (127)    37639 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_processor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_processor.h
--rw-r--r--   0 runner    (1001) docker     (127)    54189 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_processor_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_trainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_trainer.h
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_trainer_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/spec_parser.h
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_decode_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_encode_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_export_vocab_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_normalize_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_train_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/test_main.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/testharness.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/testharness.h
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_factory.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_factory.h
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_factory_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_interface.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)    20727 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_interface_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unicode_script.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unicode_script.h
--rw-r--r--   0 runner    (1001) docker     (127)   106446 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unicode_script_map.h
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unicode_script_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    34126 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model.h
--rw-r--r--   0 runner    (1001) docker     (127)    32283 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)    20993 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model_trainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model_trainer.h
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model_trainer_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/util.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/util.h
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/util_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model.h
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model_test.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model_trainer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model_trainer.h
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model_trainer_test.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.753129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.753129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.753129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/container/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/container/flat_hash_map.h
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/container/flat_hash_set.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.753129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/flags/
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/flags/flag.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/flags/flag.h
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/flags/parse.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.753129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/memory/
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/memory/memory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.757129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/random/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/random/distributions.h
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/random/random.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.757129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/ascii.h
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/match.h
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/numbers.h
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_cat.h
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_format.h
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_join.h
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_replace.h
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_split.h
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/string_view.h
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/strip.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.757129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/darts_clone/
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/darts_clone/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    51750 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/darts_clone/darts.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.757129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/esaxx/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/esaxx/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/esaxx/esa.hxx
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/esaxx/sais.hxx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.761129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/arena.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/arenastring.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/bytestream.cc
--rw-r--r--   0 runner    (1001) docker     (127)    30847 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/coded_stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/common.cc
--rw-r--r--   0 runner    (1001) docker     (127)    82338 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/extension_set.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
--rw-r--r--   0 runner    (1001) docker     (127)    30000 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.701129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.769129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
--rw-r--r--   0 runner    (1001) docker     (127)    29756 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
--rw-r--r--   0 runner    (1001) docker     (127)    96637 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
--rw-r--r--   0 runner    (1001) docker     (127)    78585 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
--rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
--rw-r--r--   0 runner    (1001) docker     (127)    31313 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.769129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
--rw-r--r--   0 runner    (1001) docker     (127)    69376 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
--rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
--rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
--rw-r--r--   0 runner    (1001) docker     (127)    48107 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
--rw-r--r--   0 runner    (1001) docker     (127)    24921 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
--rw-r--r--   0 runner    (1001) docker     (127)    31973 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
--rw-r--r--   0 runner    (1001) docker     (127)    27172 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
--rw-r--r--   0 runner    (1001) docker     (127)    32754 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
--rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
--rw-r--r--   0 runner    (1001) docker     (127)   101600 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-20 15:19:44.773129 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
--rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
--rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    31213 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
--rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
--rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
--rw-r--r--   0 runner    (1001) docker     (127)    39629 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
--rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
--rw-r--r--   0 runner    (1001) docker     (127)    83648 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/int128.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/io_win32.cc
--rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/message_lite.cc
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/parse_context.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/repeated_field.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/status.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/statusor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/stringprintf.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26415 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
--rw-r--r--   0 runner    (1001) docker     (127)    88575 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/time.cc
--rw-r--r--   0 runner    (1001) docker     (127)    27892 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-01-20 15:19:33.000000 chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.500085 chatglm_cpp-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28808 2024-04-23 15:34:59.500085 chatglm_cpp-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27724 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    79831 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    42969 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.424084 chatglm_cpp-0.3.2/chatglm_cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm_cpp/_C.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm_cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22943 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm_cpp/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm_cpp/langchain_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm_cpp/openai_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.496085 chatglm_cpp-0.3.2/chatglm_cpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28808 2024-04-23 15:34:59.000000 chatglm_cpp-0.3.2/chatglm_cpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17820 2024-04-23 15:34:59.000000 chatglm_cpp-0.3.2/chatglm_cpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:34:59.000000 chatglm_cpp-0.3.2/chatglm_cpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 15:34:59.000000 chatglm_cpp-0.3.2/chatglm_cpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 15:34:59.000000 chatglm_cpp-0.3.2/chatglm_cpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm_pybind.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    71267 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/chatglm_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.424084 chatglm_cpp-0.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13376 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:34:59.500085 chatglm_cpp-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.424084 chatglm_cpp-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/tests/test_chatglm_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32271 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/tests/test_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.420084 chatglm_cpp-0.3.2/third_party/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.428084 chatglm_cpp-0.3.2/third_party/ggml/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 15:34:45.000000 chatglm_cpp-0.3.2/third_party/ggml/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/build.zig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.428084 chatglm_cpp-0.3.2/third_party/ggml/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/cmake/BuildTypes.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/cmake/GitVars.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.428084 chatglm_cpp-0.3.2/third_party/ggml/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.428084 chatglm_cpp-0.3.2/third_party/ggml/examples/dolly-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/dolly-v2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/dolly-v2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.428084 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-2/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.428084 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-j/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-j/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-j/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.428084 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-neox/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-neox/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-neox/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.428084 chatglm_cpp-0.3.2/third_party/ggml/examples/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/mnist/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/mnist/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.432084 chatglm_cpp-0.3.2/third_party/ggml/examples/mpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/mpt/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/mpt/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.432084 chatglm_cpp-0.3.2/third_party/ggml/examples/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/python/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.432084 chatglm_cpp-0.3.2/third_party/ggml/examples/replit/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/replit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.432084 chatglm_cpp-0.3.2/third_party/ggml/examples/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/sam/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/sam/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.432084 chatglm_cpp-0.3.2/third_party/ggml/examples/starcoder/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/starcoder/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/starcoder/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.432084 chatglm_cpp-0.3.2/third_party/ggml/examples/whisper/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/whisper/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/examples/whisper/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/ggml.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.416084 chatglm_cpp-0.3.2/third_party/ggml/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.432084 chatglm_cpp-0.3.2/third_party/ggml/include/ggml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/include/ggml/ggml-alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/include/ggml/ggml-backend.h
+-rw-r--r--   0 runner    (1001) docker     (127)    76877 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/include/ggml/ggml.h
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.436084 chatglm_cpp-0.3.2/third_party/ggml/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22783 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-alloc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-backend.c
+-rw-r--r--   0 runner    (1001) docker     (127)   294413 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-cuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-metal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    81148 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-metal.m
+-rw-r--r--   0 runner    (1001) docker     (127)    91862 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-metal.metal
+-rw-r--r--   0 runner    (1001) docker     (127)    71169 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-opencl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml-opencl.h
+-rw-r--r--   0 runner    (1001) docker     (127)   735658 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/src/ggml.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.436084 chatglm_cpp-0.3.2/third_party/ggml/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13108 2024-04-23 15:34:48.000000 chatglm_cpp-0.3.2/third_party/ggml/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.436084 chatglm_cpp-0.3.2/third_party/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.416084 chatglm_cpp-0.3.2/third_party/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.440084 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)    24334 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67312 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8458 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.440084 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)    28518 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (127)    53480 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17859 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28221 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48364 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eigen/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32135 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13459 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4731 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    79725 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (127)   126706 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (127)    98455 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29897 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21733 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.444084 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.448084 chatglm_cpp-0.3.2/third_party/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1311 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14449 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-23 15:34:49.000000 chatglm_cpp-0.3.2/third_party/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.448084 chatglm_cpp-0.3.2/third_party/sentencepiece/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 15:34:47.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/.git
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.448084 chatglm_cpp-0.3.2/third_party/sentencepiece/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)    46672 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/cmake/ios.toolchain.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.448084 chatglm_cpp-0.3.2/third_party/sentencepiece/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/python/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/sentencepiece.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.476085 chatglm_cpp-0.3.2/third_party/sentencepiece/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model_trainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model_trainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model_trainer_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18686 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/builder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/builder_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.476085 chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/
+-rw-r--r--   0 runner    (1001) docker     (127)    35154 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    40648 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/sentencepiece.pb.h
+-rw-r--r--   0 runner    (1001) docker     (127)   136631 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   200094 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model_trainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model_trainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model_trainer_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/compile_charsmap_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/error.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/filesystem.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/filesystem_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/freelist.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/freelist_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/init.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/init_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_factory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_factory_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_interface.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_interface_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)  7198605 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/normalization_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/normalizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/normalizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16156 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/normalizer_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/pretokenizer_for_training.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/pretokenizer_for_training.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/pretokenizer_for_training_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_model.proto
+-rw-r--r--   0 runner    (1001) docker     (127)    37639 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_processor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_processor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    54189 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_processor_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_trainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_trainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_trainer_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10925 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/spec_parser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_decode_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_encode_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_export_vocab_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_normalize_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_train_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/test_main.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/testharness.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/testharness.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_factory.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_factory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_factory_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_interface.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20727 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_interface_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unicode_script.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unicode_script.h
+-rw-r--r--   0 runner    (1001) docker     (127)   106446 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unicode_script_map.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unicode_script_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    34126 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7324 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32283 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20993 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model_trainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model_trainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model_trainer_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/util.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/util_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model_test.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model_trainer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model_trainer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model_trainer_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.476085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.476085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.476085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/container/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/container/flat_hash_map.h
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/container/flat_hash_set.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.476085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/flags/
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/flags/flag.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/flags/flag.h
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/flags/parse.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.476085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/memory/memory.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.480085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/random/distributions.h
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/random/random.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.480085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/ascii.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/match.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/numbers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_cat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_format.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_join.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_replace.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_split.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/string_view.h
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/strip.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.480085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/darts_clone/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/darts_clone/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    51750 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/darts_clone/darts.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.480085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/esaxx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/esaxx/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/esaxx/esa.hxx
+-rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/esaxx/sais.hxx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.488085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15726 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/arena.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/arenastring.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/bytestream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    30847 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/coded_stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/common.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    82338 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/extension_set.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    30000 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.420084 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.492085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29756 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15918 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
+-rw-r--r--   0 runner    (1001) docker     (127)    96637 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    78585 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31313 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.492085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    69376 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10258 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16950 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48107 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24921 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31973 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27172 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32754 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20834 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
+-rw-r--r--   0 runner    (1001) docker     (127)   101600 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:34:59.496085 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11769 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31213 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8558 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17861 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    39629 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14401 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)    83648 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/int128.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13526 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/io_win32.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/message_lite.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/parse_context.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/repeated_field.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/status.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/statusor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/stringprintf.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26415 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    88575 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/time.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    27892 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-04-23 15:34:51.000000 chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
```

### Comparing `chatglm-cpp-0.3.1/CMakeLists.txt` & `chatglm_cpp-0.3.2/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,27 @@
 set(SPM_ENABLE_SHARED OFF CACHE BOOL "chatglm: disable sentencepiece shared libraries by default")
 set(SPM_ENABLE_TCMALLOC OFF CACHE BOOL "chatglm: disable tcmalloc by default")
 include_directories(third_party/sentencepiece/src)
 add_subdirectory(third_party/sentencepiece)
 
 if (GGML_CUBLAS)
     add_compile_definitions(GGML_USE_CUBLAS)
-    set(CUDA_ARCHITECTURES "52;61;70;75;80;86" CACHE STRING "chatglm: cuda architectures to compile")
+    enable_language(CUDA)
+    # ref: https://stackoverflow.com/questions/28932864/which-compute-capability-is-supported-by-which-cuda-versions
+    set(CUDA_ARCH_LIST "52;61;70;75")
+    if (CMAKE_CUDA_COMPILER_VERSION VERSION_GREATER_EQUAL "11.0")
+        set(CUDA_ARCH_LIST "${CUDA_ARCH_LIST};80")
+    endif ()
+    if (CMAKE_CUDA_COMPILER_VERSION VERSION_GREATER_EQUAL "11.1")
+        set(CUDA_ARCH_LIST "${CUDA_ARCH_LIST};86")
+    endif ()
+    if (CMAKE_CUDA_COMPILER_VERSION VERSION_GREATER_EQUAL "11.8")
+        set(CUDA_ARCH_LIST "${CUDA_ARCH_LIST};89;90")
+    endif ()
+    set(CUDA_ARCHITECTURES ${CUDA_ARCH_LIST} CACHE STRING "chatglm: cuda architectures to compile")
     set_property(TARGET ggml PROPERTY CUDA_ARCHITECTURES ${CUDA_ARCHITECTURES})
 endif ()
 
 if (GGML_METAL)
     add_compile_definitions(GGML_USE_METAL)
     configure_file(third_party/ggml/src/ggml-metal.metal ${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/ggml-metal.metal COPYONLY)
 endif ()
@@ -102,14 +114,23 @@
     ${PROJECT_SOURCE_DIR}/convert.py
     ${PROJECT_SOURCE_DIR}/setup.py)
 add_custom_target(lint
     COMMAND clang-format -i ${CPP_SOURCES}
     COMMAND isort ${PY_SOURCES}
     COMMAND black ${PY_SOURCES} --verbose)
 
+# check all
+add_custom_target(check
+    COMMAND cmake --build build -j
+    COMMAND ./build/bin/chatglm_test
+    COMMAND python3 setup.py develop
+    COMMAND python3 -m pytest tests/test_chatglm_cpp.py -v
+    WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}
+)
+
 # mypy
 add_custom_target(mypy
     mypy chatglm_cpp examples --exclude __init__.pyi
     WORKING_DIRECTORY ${PROJECT_SOURCE_DIR}
 )
 
 # stub
```

### Comparing `chatglm-cpp-0.3.1/LICENSE` & `chatglm_cpp-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/PKG-INFO` & `chatglm_cpp-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatglm-cpp
-Version: 0.3.1
+Version: 0.3.2
 Summary: C++ implementation of ChatGLM family models and more LLMs
 Author-email: Jiahao Li <liplus17@163.com>
 Maintainer-email: Jiahao Li <liplus17@163.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/li-plus/chatglm.cpp
 Project-URL: Repository, https://github.com/li-plus/chatglm.cpp.git
 Keywords: ChatGLM,ChatGLM2,ChatGLM3,Large Language Model
@@ -37,22 +37,25 @@
 ![demo](docs/demo.gif)
 
 ## Features
 
 Highlights:
 * Pure C++ implementation based on [ggml](https://github.com/ggerganov/ggml), working in the same way as [llama.cpp](https://github.com/ggerganov/llama.cpp).
 * Accelerated memory-efficient CPU inference with int4/int8 quantization, optimized KV cache and parallel computing.
+* P-Tuning v2 and LoRA finetuned models support.
 * Streaming generation with typewriter effect.
 * Python binding, web demo, api servers and more possibilities.
 
 Support Matrix:
 * Hardwares: x86/arm CPU, NVIDIA GPU, Apple Silicon GPU
 * Platforms: Linux, MacOS, Windows
 * Models: [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B), [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B), [ChatGLM3-6B](https://github.com/THUDM/ChatGLM3), [CodeGeeX2](https://github.com/THUDM/CodeGeeX2), [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B), [Baichuan-7B](https://github.com/baichuan-inc/Baichuan-7B), [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B), [Baichuan2](https://github.com/baichuan-inc/Baichuan2), [InternLM](https://github.com/InternLM/InternLM)
 
+**NOTE**: Baichuan & InternLM model series are deprecated in favor of [llama.cpp](https://github.com/ggerganov/llama.cpp).
+
 ## Getting Started
 
 **Preparation**
 
 Clone the ChatGLM.cpp repository into your local machine:
 ```sh
 git clone --recursive https://github.com/li-plus/chatglm.cpp.git && cd chatglm.cpp
@@ -88,15 +91,17 @@
 * `q4_1`: 4-bit integer quantization with fp16 scales and minimum values.
 * `q5_0`: 5-bit integer quantization with fp16 scales.
 * `q5_1`: 5-bit integer quantization with fp16 scales and minimum values.
 * `q8_0`: 8-bit integer quantization with fp16 scales.
 * `f16`: half precision floating point weights without quantization.
 * `f32`: single precision floating point weights without quantization.
 
-For LoRA model, add `-l <lora_model_name_or_path>` flag to merge your LoRA weights into the base model.
+For LoRA models, add `-l <lora_model_name_or_path>` flag to merge your LoRA weights into the base model. For example, run `python3 chatglm_cpp/convert.py -i THUDM/chatglm3-6b -t q4_0 -o chatglm3-ggml-lora.bin -l shibing624/chatglm3-6b-csc-chinese-lora` to merge public LoRA weights from Hugging Face.
+
+For P-Tuning v2 models using the [official finetuning script](https://github.com/THUDM/ChatGLM3/tree/main/finetune_demo), additional weights are automatically detected by `convert.py`. If `past_key_values` is on the output weight list, the P-Tuning checkpoint is successfully converted.
 
 **Build & Run**
 
 Compile the project using CMake:
 ```sh
 cmake -B build
 cmake --build build -j --config Release
@@ -294,15 +299,15 @@
 
 By default, all kernels will be compiled for all possible CUDA architectures and it takes some time. To run on a specific type of device, you may specify `CUDA_ARCHITECTURES` to speed up the nvcc compilation. For example:
 ```sh
 cmake -B build -DGGML_CUBLAS=ON -DCUDA_ARCHITECTURES="80"       # for A100
 cmake -B build -DGGML_CUBLAS=ON -DCUDA_ARCHITECTURES="70;75"    # compatible with both V100 and T4
 ```
 
-To find out the CUDA architecture of your GPU device, see [Matching CUDA arch and CUDA gencode for various NVIDIA architectures](https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/).
+To find out the CUDA architecture of your GPU device, see [Your GPU Compute Capability](https://developer.nvidia.com/cuda-gpus).
 
 **Metal**
 
 MPS (Metal Performance Shaders) allows computation to run on powerful Apple Silicon GPU. Add the CMake flag `-DGGML_METAL=ON` to enable it.
 ```sh
 cmake -B build -DGGML_METAL=ON && cmake --build build -j
 ```
```

### Comparing `chatglm-cpp-0.3.1/README.md` & `chatglm_cpp-0.3.2/chatglm_cpp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: chatglm-cpp
+Version: 0.3.2
+Summary: C++ implementation of ChatGLM family models and more LLMs
+Author-email: Jiahao Li <liplus17@163.com>
+Maintainer-email: Jiahao Li <liplus17@163.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/li-plus/chatglm.cpp
+Project-URL: Repository, https://github.com/li-plus/chatglm.cpp.git
+Keywords: ChatGLM,ChatGLM2,ChatGLM3,Large Language Model
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: api
+Requires-Dist: fastapi[all]; extra == "api"
+Requires-Dist: sse-starlette; extra == "api"
+
 # ChatGLM.cpp
 
 [![CMake](https://github.com/li-plus/chatglm.cpp/actions/workflows/cmake.yml/badge.svg)](https://github.com/li-plus/chatglm.cpp/actions/workflows/cmake.yml)
 [![Python package](https://github.com/li-plus/chatglm.cpp/actions/workflows/python-package.yml/badge.svg)](https://github.com/li-plus/chatglm.cpp/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/chatglm-cpp)](https://pypi.org/project/chatglm-cpp/)
 ![Python](https://img.shields.io/pypi/pyversions/chatglm-cpp)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
@@ -11,22 +37,25 @@
 ![demo](docs/demo.gif)
 
 ## Features
 
 Highlights:
 * Pure C++ implementation based on [ggml](https://github.com/ggerganov/ggml), working in the same way as [llama.cpp](https://github.com/ggerganov/llama.cpp).
 * Accelerated memory-efficient CPU inference with int4/int8 quantization, optimized KV cache and parallel computing.
+* P-Tuning v2 and LoRA finetuned models support.
 * Streaming generation with typewriter effect.
 * Python binding, web demo, api servers and more possibilities.
 
 Support Matrix:
 * Hardwares: x86/arm CPU, NVIDIA GPU, Apple Silicon GPU
 * Platforms: Linux, MacOS, Windows
 * Models: [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B), [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B), [ChatGLM3-6B](https://github.com/THUDM/ChatGLM3), [CodeGeeX2](https://github.com/THUDM/CodeGeeX2), [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B), [Baichuan-7B](https://github.com/baichuan-inc/Baichuan-7B), [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B), [Baichuan2](https://github.com/baichuan-inc/Baichuan2), [InternLM](https://github.com/InternLM/InternLM)
 
+**NOTE**: Baichuan & InternLM model series are deprecated in favor of [llama.cpp](https://github.com/ggerganov/llama.cpp).
+
 ## Getting Started
 
 **Preparation**
 
 Clone the ChatGLM.cpp repository into your local machine:
 ```sh
 git clone --recursive https://github.com/li-plus/chatglm.cpp.git && cd chatglm.cpp
@@ -62,15 +91,17 @@
 * `q4_1`: 4-bit integer quantization with fp16 scales and minimum values.
 * `q5_0`: 5-bit integer quantization with fp16 scales.
 * `q5_1`: 5-bit integer quantization with fp16 scales and minimum values.
 * `q8_0`: 8-bit integer quantization with fp16 scales.
 * `f16`: half precision floating point weights without quantization.
 * `f32`: single precision floating point weights without quantization.
 
-For LoRA model, add `-l <lora_model_name_or_path>` flag to merge your LoRA weights into the base model.
+For LoRA models, add `-l <lora_model_name_or_path>` flag to merge your LoRA weights into the base model. For example, run `python3 chatglm_cpp/convert.py -i THUDM/chatglm3-6b -t q4_0 -o chatglm3-ggml-lora.bin -l shibing624/chatglm3-6b-csc-chinese-lora` to merge public LoRA weights from Hugging Face.
+
+For P-Tuning v2 models using the [official finetuning script](https://github.com/THUDM/ChatGLM3/tree/main/finetune_demo), additional weights are automatically detected by `convert.py`. If `past_key_values` is on the output weight list, the P-Tuning checkpoint is successfully converted.
 
 **Build & Run**
 
 Compile the project using CMake:
 ```sh
 cmake -B build
 cmake --build build -j --config Release
@@ -268,15 +299,15 @@
 
 By default, all kernels will be compiled for all possible CUDA architectures and it takes some time. To run on a specific type of device, you may specify `CUDA_ARCHITECTURES` to speed up the nvcc compilation. For example:
 ```sh
 cmake -B build -DGGML_CUBLAS=ON -DCUDA_ARCHITECTURES="80"       # for A100
 cmake -B build -DGGML_CUBLAS=ON -DCUDA_ARCHITECTURES="70;75"    # compatible with both V100 and T4
 ```
 
-To find out the CUDA architecture of your GPU device, see [Matching CUDA arch and CUDA gencode for various NVIDIA architectures](https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/).
+To find out the CUDA architecture of your GPU device, see [Your GPU Compute Capability](https://developer.nvidia.com/cuda-gpus).
 
 **Metal**
 
 MPS (Metal Performance Shaders) allows computation to run on powerful Apple Silicon GPU. Add the CMake flag `-DGGML_METAL=ON` to enable it.
 ```sh
 cmake -B build -DGGML_METAL=ON && cmake --build build -j
 ```
```

### Comparing `chatglm-cpp-0.3.1/chatglm.cpp` & `chatglm_cpp-0.3.2/chatglm.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     }
 
     ggml_graph_compute(graph, &plan);
 }
 
 // for debugging purpose
 [[maybe_unused]] static inline ggml_tensor *add_zero(ggml_context *ctx, ggml_tensor *tensor) {
-    ggml_tensor *zeros = ggml_new_tensor(ctx, tensor->type, tensor->n_dims, tensor->ne);
+    ggml_tensor *zeros = ggml_new_tensor(ctx, GGML_TYPE_F32, tensor->n_dims, tensor->ne);
     ggml_set_f32(zeros, 0);
     tensor_to_device(zeros);
     ggml_tensor *out = tensor_assign_buffers(ggml_add(ctx, tensor, zeros));
     return out;
 }
 
 void ModelContext::init_device_context() {
@@ -445,14 +445,43 @@
     ggml_context *gctx = ctx->ctx_b.get();
     auto ggml_rms_norm_fn = inplace ? ggml_rms_norm_inplace : ggml_rms_norm;
     ggml_tensor *output = tensor_assign_buffers(ggml_rms_norm_fn(gctx, input, eps));
     output = tensor_assign_buffers(ggml_mul_inplace(gctx, output, weight));
     return output;
 }
 
+static ggml_tensor *apply_activation_inplace(ggml_context *ctx, ggml_tensor *hidden_states, ActivationType hidden_act) {
+    switch (hidden_act) {
+    case ActivationType::GELU:
+        return tensor_assign_buffers(ggml_gelu_inplace(ctx, hidden_states));
+    case ActivationType::SILU:
+        return tensor_assign_buffers(ggml_silu_inplace(ctx, hidden_states));
+    default:
+        CHATGLM_THROW << "Unknown activation type " << (int)hidden_act;
+    }
+}
+
+ggml_tensor *BasicMLP::forward(ModelContext *ctx, ggml_tensor *hidden_states) const {
+    ggml_context *gctx = ctx->ctx_b.get();
+    hidden_states = dense_h_to_4h.forward(ctx, hidden_states);
+    hidden_states = apply_activation_inplace(gctx, hidden_states, hidden_act);
+    hidden_states = dense_4h_to_h.forward(ctx, hidden_states);
+    return hidden_states;
+}
+
+ggml_tensor *BasicGLU::forward(ModelContext *ctx, ggml_tensor *hidden_states) const {
+    ggml_context *gctx = ctx->ctx_b.get();
+    ggml_tensor *gate = gate_proj.forward(ctx, hidden_states);
+    gate = apply_activation_inplace(gctx, gate, hidden_act);
+    hidden_states = up_proj.forward(ctx, hidden_states);
+    hidden_states = tensor_assign_buffers(ggml_mul_inplace(gctx, hidden_states, gate));
+    hidden_states = down_proj.forward(ctx, hidden_states);
+    return hidden_states;
+}
+
 // Adapted from https://github.com/ggerganov/llama.cpp/blob/master/examples/common.cpp
 int get_num_physical_cores() {
     unsigned int n_threads = std::thread::hardware_concurrency();
     return n_threads > 0 ? (n_threads <= 4 ? n_threads : n_threads / 2) : 4;
 }
 
 int get_default_num_threads() {
@@ -478,21 +507,257 @@
     case ModelType::INTERNLM:
         return "InternLM";
     default:
         CHATGLM_THROW << "unknown model type " << (int)model_type;
     }
 }
 
+static ggml_tensor *apply_rotary_emb_basic(ModelContext *ctx, ggml_tensor *layer, ggml_tensor *position_ids, int n_ctx,
+                                           RopeType rope_type, float rope_theta, int dim_scale) {
+    // tensor a (activation) is of shape [s, #h, d]
+    // tensor b (position_ids) is of shape [s]
+    ggml_context *gctx = ctx->ctx_b.get();
+#ifdef GGML_USE_CUBLAS
+    if (!ggml_is_contiguous(layer)) {
+        layer = tensor_assign_buffers(ggml_cont(gctx, layer));
+    }
+#endif
+    const int head_size = layer->ne[0];
+    const int rope_dim = head_size / dim_scale;
+    layer = tensor_assign_buffers(ggml_rope_custom_inplace(gctx, layer, position_ids, rope_dim, (int)rope_type, n_ctx,
+                                                           rope_theta, 1.f)); // [s, #h, d]
+    return layer;
+}
+
+static ggml_tensor *apply_rotary_emb_glm(ModelContext *ctx, ggml_tensor *layer, ggml_tensor *position_ids, int n_ctx) {
+    // tensor a (activation) is of shape [s, #h, d]
+    // tensor b (position_ids) is of shape [2 * s]
+    ggml_context *gctx = ctx->ctx_b.get();
+
+    const int head_size = layer->ne[0];
+    const int num_heads = layer->ne[1];
+    const int qlen = layer->ne[2];
+    const int rope_dim = head_size / 2;
+
+    ggml_tensor *b1 = ggml_view_1d(gctx, position_ids, qlen, 0);
+    ggml_tensor *b2 = ggml_view_1d(gctx, position_ids, qlen, qlen * ggml_element_size(position_ids));
+
+    ggml_tensor *a1 = ggml_view_3d(gctx, layer, head_size / 2, num_heads, qlen, layer->nb[1], layer->nb[2], 0);
+    ggml_tensor *a2 = ggml_view_3d(gctx, layer, head_size / 2, num_heads, qlen, layer->nb[1], layer->nb[2],
+                                   head_size / 2 * ggml_element_size(layer));
+
+    ggml_tensor *a1_rope = a1;
+    ggml_tensor *a2_rope = a2;
+#ifdef GGML_USE_CUBLAS
+    a1_rope = tensor_assign_buffers(ggml_cont(gctx, a1_rope));
+    a2_rope = tensor_assign_buffers(ggml_cont(gctx, a2_rope));
+#endif
+
+    a1_rope = tensor_assign_buffers(
+        ggml_rope_inplace(gctx, a1_rope, b1, rope_dim, (int)RopeType::NEOX, n_ctx)); // [s, #h, d/2]
+    a2_rope = tensor_assign_buffers(
+        ggml_rope_inplace(gctx, a2_rope, b2, rope_dim, (int)RopeType::NEOX, n_ctx)); // [s, #h, d/2]
+
+#ifdef GGML_USE_CUBLAS
+    a1_rope = ggml_cpy(gctx, a1_rope, a1);
+    a2_rope = ggml_cpy(gctx, a2_rope, a2);
+#endif
+    ggml_build_forward_expand(&ctx->gf, a1_rope);
+    ggml_build_forward_expand(&ctx->gf, a2_rope);
+
+    return layer;
+}
+
+[[maybe_unused]] static ggml_tensor *apply_rotary_emb_glm2(ModelContext *ctx, ggml_tensor *layer,
+                                                           ggml_tensor *position_ids) {
+    // layer: [s, #h, d], position_ids: [s]
+    ggml_context *gctx = ctx->ctx_b.get();
+#ifdef GGML_USE_CUBLAS
+    if (!ggml_is_contiguous(layer)) {
+        layer = tensor_assign_buffers(ggml_cont(gctx, layer));
+    }
+#endif
+    const int head_size = layer->ne[0];
+    const int rope_dim = head_size / 2;
+    ggml_tensor *roped_layer =
+        tensor_assign_buffers(ggml_rope(gctx, layer, position_ids, rope_dim, (int)RopeType::GPTJ, 0)); // [s, #h, d]
+
+    ggml_tensor *roped_layer_view = tensor_assign_buffers(
+        ggml_view_3d(gctx, roped_layer, rope_dim, roped_layer->ne[1], roped_layer->ne[2], roped_layer->nb[1],
+                     roped_layer->nb[2], rope_dim * roped_layer->nb[0])); // [s, #h, d/2]
+
+    ggml_tensor *layer_view =
+        tensor_assign_buffers(ggml_view_3d(gctx, layer, rope_dim, layer->ne[1], layer->ne[2], layer->nb[1],
+                                           layer->nb[2], rope_dim * layer->nb[0])); // [s, #h, d/2]
+
+    ggml_build_forward_expand(&ctx->gf, ggml_cpy(gctx, layer_view, roped_layer_view));
+
+    return roped_layer;
+}
+
+static ggml_tensor *apply_rotary_emb(ModelContext *ctx, ggml_tensor *layer, ggml_tensor *position_ids, int n_ctx,
+                                     RopeType rope_type, float rope_theta, int dim_scale) {
+    switch (rope_type) {
+    case RopeType::GPTJ:
+    case RopeType::NEOX:
+        return apply_rotary_emb_basic(ctx, layer, position_ids, n_ctx, rope_type, rope_theta, dim_scale);
+    case RopeType::CHATGLM:
+        return apply_rotary_emb_glm(ctx, layer, position_ids, n_ctx);
+    // case RopeType::CHATGLM2:
+    //     return apply_rotary_emb_glm2(ctx, layer, position_ids);
+    case RopeType::DISABLED:
+        return layer;
+    default:
+        CHATGLM_THROW << "Unknown rope type " << (int)rope_type;
+    }
+}
+
+static inline ggml_tensor *apply_attention_mask_causal(ModelContext *ctx, ggml_tensor *attn_scores, int n_past) {
+    return tensor_assign_buffers(ggml_diag_mask_inf_inplace(ctx->ctx_b.get(), attn_scores, n_past));
+}
+
+static ggml_tensor *apply_attention_mask_glm(ModelContext *ctx, ggml_tensor *attn_scores, int n_past) {
+    // attn_scores: [#h, s, kvs]
+    // semantic: attn_scores[:, :-1, -1] = -inf
+    ggml_context *gctx = ctx->ctx_b.get();
+    const int kvlen = attn_scores->ne[0];
+    const int qlen = attn_scores->ne[1];
+    const int num_attention_heads = attn_scores->ne[2];
+    ggml_tensor *inf = ggml_new_tensor_3d(gctx, attn_scores->type, 1, qlen - 1, num_attention_heads);
+    ggml_set_f32(inf, -INFINITY);
+    tensor_to_device(inf); // TODO: optimize
+    ggml_tensor *masked_attn_scores =
+        tensor_assign_buffers(ggml_view_3d(gctx, attn_scores, 1, qlen - 1, num_attention_heads, attn_scores->nb[1],
+                                           attn_scores->nb[2], (kvlen - 1) * attn_scores->nb[0]));
+    ggml_build_forward_expand(&ctx->gf, ggml_cpy(gctx, inf, masked_attn_scores));
+    return attn_scores;
+}
+
+static ggml_tensor *apply_attention_mask(ModelContext *ctx, ggml_tensor *attn_scores, int n_past,
+                                         AttentionMaskType attn_mask_type) {
+    switch (attn_mask_type) {
+    case AttentionMaskType::CAUSAL:
+        return apply_attention_mask_causal(ctx, attn_scores, n_past);
+    case AttentionMaskType::CHATGLM:
+        return apply_attention_mask_glm(ctx, attn_scores, n_past);
+    default:
+        CHATGLM_THROW << "Unknown attention mask type " << (int)attn_mask_type;
+    }
+}
+
+ggml_tensor *BasicAttention::forward(ModelContext *ctx, ggml_tensor *hidden_states, ggml_tensor *position_ids,
+                                     int n_past, int n_ctx) const {
+    ggml_context *gctx = ctx->ctx_b.get();
+
+    const int hidden_size = hidden_states->ne[0];
+    const int qlen = hidden_states->ne[1];
+    const int head_size = hidden_size / num_attention_heads;
+    const int num_shared_q_heads = num_attention_heads / num_kv_heads;
+    const bool is_gqa = num_shared_q_heads > 1;
+
+    ggml_tensor *qkv = query_key_value.forward(ctx, hidden_states); // [sq, (#h + 2 * #kvh) * d]
+
+    // split mixed qkv into separate query, key and value
+    ggml_tensor *query_layer; // [s, #h, d]
+    ggml_tensor *key_layer;   // [s, #kvh, d]
+    ggml_tensor *value_layer; // [s, #kvh, d]
+
+    if (interleaved_qkv) {
+        CHATGLM_CHECK(!is_gqa) << "interleaved qkv is not supported for GQA";
+        query_layer = ggml_view_3d(gctx, qkv, head_size, num_attention_heads, qlen,
+                                   3 * head_size * ggml_element_size(qkv), qkv->nb[1], 0);
+        key_layer =
+            ggml_view_3d(gctx, qkv, head_size, num_attention_heads, qlen, 3 * head_size * ggml_element_size(qkv),
+                         qkv->nb[1], head_size * ggml_element_size(qkv));
+        value_layer =
+            ggml_view_3d(gctx, qkv, head_size, num_attention_heads, qlen, 3 * head_size * ggml_element_size(qkv),
+                         qkv->nb[1], 2 * head_size * ggml_element_size(qkv));
+    } else {
+        query_layer = ggml_view_3d(gctx, qkv, head_size, num_attention_heads, qlen, head_size * ggml_element_size(qkv),
+                                   qkv->nb[1], 0);
+        key_layer = ggml_view_3d(gctx, qkv, head_size, num_kv_heads, qlen, head_size * ggml_element_size(qkv),
+                                 qkv->nb[1], hidden_size * ggml_element_size(qkv));
+        value_layer = ggml_view_3d(gctx, qkv, head_size, num_kv_heads, qlen, head_size * ggml_element_size(qkv),
+                                   qkv->nb[1], (hidden_size + head_size * num_kv_heads) * ggml_element_size(qkv));
+    }
+
+    query_layer = apply_rotary_emb(ctx, query_layer, position_ids, n_ctx, rope_type, rope_theta, rope_dim_scale);
+    key_layer = apply_rotary_emb(ctx, key_layer, position_ids, n_ctx, rope_type, rope_theta, rope_dim_scale);
+
+    query_layer = tensor_assign_buffers(ggml_cont(gctx, ggml_permute(gctx, query_layer, 0, 2, 1, 3))); // [#h, s, d]
+    if (num_shared_q_heads > 1) {
+        query_layer = tensor_assign_buffers(ggml_reshape_3d(gctx, query_layer, head_size, num_shared_q_heads * qlen,
+                                                            num_kv_heads)); // [#kvh, (#h/#kvh) * s, d]
+    }
+
+    key_layer = tensor_assign_buffers(ggml_permute(gctx, key_layer, 0, 2, 1, 3));     // [#kvh, s, d]
+    value_layer = tensor_assign_buffers(ggml_permute(gctx, value_layer, 1, 2, 0, 3)); // [#kvh, d, s]
+
+    // store key & value to cache
+    ggml_tensor *k_cache_view = tensor_assign_buffers(
+        ggml_view_3d(gctx, k_cache, head_size, qlen, num_kv_heads, k_cache->nb[1], k_cache->nb[2],
+                     (num_virtual_tokens + n_past) * head_size * ggml_element_size(k_cache))); // [#kvh, s, d]
+    ggml_build_forward_expand(&ctx->gf, ggml_cpy(gctx, key_layer, k_cache_view));
+    ggml_tensor *v_cache_view =
+        tensor_assign_buffers(ggml_view_3d(gctx, v_cache, qlen, head_size, num_kv_heads, v_cache->nb[1], v_cache->nb[2],
+                                           (num_virtual_tokens + n_past) * ggml_element_size(v_cache))); // [#kvh, d, s]
+    ggml_build_forward_expand(&ctx->gf, ggml_cpy(gctx, value_layer, v_cache_view));
+
+    // concat key & value with past kv
+    key_layer = tensor_assign_buffers(ggml_view_3d(gctx, k_cache, head_size, num_virtual_tokens + n_past + qlen,
+                                                   num_kv_heads, k_cache->nb[1], k_cache->nb[2],
+                                                   0)); // [#kvh, kvs, d]
+    value_layer = tensor_assign_buffers(ggml_view_3d(gctx, v_cache, num_virtual_tokens + n_past + qlen, head_size,
+                                                     num_kv_heads, v_cache->nb[1], v_cache->nb[2],
+                                                     0)); // [#kvh, d, kvs]
+
+    // attention
+    ggml_tensor *attn_scores =
+        tensor_assign_buffers(ggml_mul_mat(gctx, key_layer, query_layer)); // [#kvh, (#h/#kvh) * s, kvs]
+    attn_scores =
+        tensor_assign_buffers(ggml_scale_inplace(gctx, attn_scores, ggml_new_f32(gctx, 1.f / std::sqrt(head_size))));
+    if (use_alibi) {
+        attn_scores = tensor_assign_buffers(ggml_alibi(gctx, attn_scores, n_past, num_attention_heads, 8));
+    }
+    if (n_past == 0) {
+        // build attention mask for context input
+        if (num_shared_q_heads > 1) {
+            attn_scores = ggml_reshape_3d(gctx, attn_scores, num_virtual_tokens + n_past + qlen, qlen,
+                                          num_attention_heads); // [#h, s, kvs]
+        }
+        attn_scores = apply_attention_mask(ctx, attn_scores, num_virtual_tokens + n_past, attn_mask_type);
+        if (num_shared_q_heads > 1) {
+            attn_scores =
+                ggml_reshape_3d(gctx, attn_scores, num_virtual_tokens + n_past + qlen, num_shared_q_heads * qlen,
+                                num_kv_heads); // [#kvh, (#h/#kvh) * s, kvs]
+        }
+    }
+    ggml_tensor *attn_probs =
+        tensor_assign_buffers(ggml_soft_max_inplace(gctx, attn_scores)); // [#kvh, (#h/#kvh) * s, kvs]
+
+    ggml_tensor *context_layer =
+        tensor_assign_buffers(ggml_mul_mat(gctx, value_layer, attn_probs)); // [#kvh, (#h/#kvh) * s, d]
+    if (num_shared_q_heads > 1) {
+        context_layer = ggml_reshape_3d(gctx, context_layer, head_size, qlen,
+                                        num_attention_heads); // [#h, s, d]
+    }
+    context_layer = tensor_assign_buffers(ggml_cont(gctx, ggml_permute(gctx, context_layer, 0, 2, 1, 3))); // [s, #h, d]
+    context_layer = tensor_assign_buffers(ggml_reshape_2d(gctx, context_layer, hidden_size, qlen)); // [s, #h * d]
+
+    ggml_tensor *attn_output = dense.forward(ctx, context_layer);
+    return attn_output;
+}
+
 BaseModelForCausalLM::BaseModelForCausalLM(ModelConfig config, size_t mem_size, size_t scratch_size, size_t num_weights)
     : config(config) {
     ctx_.dtype = config.dtype;
     const size_t ctx_w_size = num_weights * ggml_tensor_overhead();
     const size_t ctx_kv_size = 2 * config.num_hidden_layers *
-                               (config.max_length * config.hidden_size / config.num_attention_heads *
-                                    config.num_kv_heads * ggml_type_size(GGML_TYPE_F16) +
+                               ((config.max_length + config.num_virtual_tokens) * config.hidden_size /
+                                    config.num_attention_heads * config.num_kv_heads * ggml_type_size(GGML_TYPE_F16) +
                                 ggml_tensor_overhead());
     ctx_.ctx_w = make_unique_ggml_context(ctx_w_size, nullptr, true);
     ctx_.ctx_kv = make_unique_ggml_context(ctx_kv_size + 1 * MB, nullptr, false); // 1MB extra for MPS
 
     ctx_.compute_buffer.resize(mem_size);
     ctx_.scratch_buffer.resize(scratch_size);
     ctx_.scratch = {0, ctx_.scratch_buffer.size(), ctx_.scratch_buffer.data()};
@@ -658,15 +923,15 @@
         p->score *= inv_sum;
     }
 }
 
 std::vector<int> BaseModelForCausalLM::generate(const std::vector<int> &input_ids, const GenerationConfig &gen_config,
                                                 BaseStreamer *streamer) {
     CHATGLM_CHECK(gen_config.max_length <= config.max_length)
-        << "requested max_length (" << gen_config.max_length << ") is larger than model's max_length ("
+        << "Requested max_length (" << gen_config.max_length << ") exceeds pre-configured model max_length ("
         << config.max_length << ")";
 
     std::vector<int> output_ids;
     output_ids.reserve(gen_config.max_length);
     output_ids = input_ids;
     if (streamer) {
         streamer->put(input_ids);
@@ -837,29 +1102,14 @@
     }
     // punctuations
     output = replace_punctuations(output);
 
     return output;
 }
 
-ggml_tensor *GLMContextMasker::operator()(ModelContext *ctx, ggml_tensor *attn_scores, int n_past) const {
-    // attn_scores is of shape [heads, qlen, klen]
-    ggml_context *gctx = ctx->ctx_b.get();
-    const int qlen = attn_scores->ne[1];
-    const int num_attention_heads = attn_scores->ne[2];
-    ggml_tensor *inf = ggml_new_tensor_3d(gctx, attn_scores->type, 1, qlen - 1, num_attention_heads);
-    ggml_set_f32(inf, -INFINITY);
-    tensor_to_device(inf); // TODO: optimize
-    ggml_tensor *masked_attn_scores = tensor_assign_buffers(
-        ggml_view_3d(gctx, attn_scores, 1, qlen - 1, num_attention_heads, qlen * ggml_element_size(attn_scores),
-                     qlen * qlen * ggml_element_size(attn_scores), (qlen - 1) * ggml_element_size(attn_scores)));
-    ggml_build_forward_expand(&ctx->gf, ggml_cpy(gctx, inf, masked_attn_scores));
-    return attn_scores;
-}
-
 ggml_tensor *GLMBlock::forward(ModelContext *ctx, ggml_tensor *hidden_states, ggml_tensor *position_ids, int n_past,
                                int n_ctx) const {
     ggml_context *gctx = ctx->ctx_b.get();
 
     ggml_tensor *alpha = ggml_new_f32(gctx, alpha_value);
 
     ggml_tensor *attn_input = input_layernorm.forward(ctx, hidden_states);
@@ -991,14 +1241,29 @@
 
 ChatGLM2ForCausalLM::ChatGLM2ForCausalLM(const ModelConfig &config)
     : BasicModelForCausalLM(config, MEM_SIZE, SCRATCH_SIZE, num_weights(config.num_hidden_layers)) {
     state_dict_ = state_dict();
 }
 
 void ChatGLM2ForCausalLM::load(ModelLoader &loader) {
+    if (config.num_virtual_tokens > 0) {
+        const int head_size = config.hidden_size / config.num_attention_heads;
+        auto prefix_cache_ctx = make_unique_ggml_context(
+            ggml_tensor_overhead() + config.num_hidden_layers * 2 * config.num_kv_heads * config.num_virtual_tokens *
+                                         head_size * ggml_type_size(GGML_TYPE_F16),
+            nullptr, false);
+        ggml_tensor *past_key_values =
+            ggml_new_tensor_4d(prefix_cache_ctx.get(), GGML_TYPE_F16, head_size, config.num_virtual_tokens,
+                               config.num_kv_heads, config.num_hidden_layers * 2);
+        CHATGLM_CHECK(ggml_used_mem(prefix_cache_ctx.get()) == ggml_get_mem_size(prefix_cache_ctx.get()))
+            << "corrupted prefix cache";
+        loader.read_tensor("past_key_values", past_key_values);
+        load_prefix_cache(past_key_values);
+    }
+
     std::unordered_map<std::string, std::string> glu_name_map;
     for (int i = 0; i < config.num_hidden_layers; i++) {
         std::string layer_prefix = "transformer.encoder.layers." + std::to_string(i) + '.';
         glu_name_map.emplace(layer_prefix + "mlp.gate_proj.weight", layer_prefix + "mlp.dense_h_to_4h.weight");
         glu_name_map.emplace(layer_prefix + "mlp.up_proj.weight", layer_prefix + "mlp.dense_h_to_4h.weight");
     }
 
@@ -1420,97 +1685,119 @@
         } else {
             oss_prompt << msg.content << "<eoa>\n";
         }
     }
     return oss_prompt.str();
 }
 
-template <typename InternLMModel>
-InternLMForCausalLM<InternLMModel>::InternLMForCausalLM(const ModelConfig &config)
-    : BasicModelForCausalLM<InternLMModel>(config, MEM_SIZE, SCRATCH_SIZE, num_weights(config.num_hidden_layers)) {
-    this->state_dict_ = state_dict();
+InternLMForCausalLM::InternLMForCausalLM(const ModelConfig &config)
+    : BasicModelForCausalLM(config, MEM_SIZE, SCRATCH_SIZE, num_weights(config.num_hidden_layers, config.hidden_size)) {
+    state_dict_ = state_dict();
 }
 
-template <typename InternLMModel>
-void InternLMForCausalLM<InternLMModel>::load(ModelLoader &loader) {
-    for (auto &item : this->state_dict_) {
+void InternLMForCausalLM::load(ModelLoader &loader) {
+    for (auto &item : state_dict_) {
         const std::string &name = item.first;
         ggml_tensor *tensor = item.second;
         loader.read_tensor(name, tensor);
     }
 
-    this->to_device();
+    to_device();
 
-    this->ctx_.weight_buffer = std::string_view(loader.data, loader.size);
-    this->ctx_.init_device_context();
+    ctx_.weight_buffer = std::string_view(loader.data, loader.size);
+    ctx_.init_device_context();
 }
 
-template <typename InternLMModel>
-StateDict InternLMForCausalLM<InternLMModel>::state_dict() const {
+StateDict InternLMForCausalLM::state_dict() const {
     StateDict sd;
-    sd.reserve(num_weights(this->config.num_hidden_layers));
-    sd.emplace_back("model.embed_tokens.weight", this->transformer.word_embeddings.weight);
-    for (int i = 0; i < this->config.num_hidden_layers; i++) {
+    sd.reserve(num_weights(config.num_hidden_layers, config.hidden_size));
+    sd.emplace_back("model.embed_tokens.weight", transformer.word_embeddings.weight);
+    for (int i = 0; i < config.num_hidden_layers; i++) {
         std::string layer_prefix = "model.layers." + std::to_string(i) + '.';
-        sd.emplace_back(layer_prefix + "input_layernorm.weight", this->transformer.layers[i].input_layernorm.weight);
+        sd.emplace_back(layer_prefix + "input_layernorm.weight", transformer.layers[i].input_layernorm.weight);
         sd.emplace_back(layer_prefix + "self_attn.qkv_proj.weight",
-                        this->transformer.layers[i].attention.query_key_value.weight);
-        if (this->transformer.layers[i].attention.query_key_value.bias) {
+                        transformer.layers[i].attention.query_key_value.weight);
+        if (transformer.layers[i].attention.query_key_value.bias) {
             sd.emplace_back(layer_prefix + "self_attn.qkv_proj.bias",
-                            this->transformer.layers[i].attention.query_key_value.bias);
+                            transformer.layers[i].attention.query_key_value.bias);
         }
-        sd.emplace_back(layer_prefix + "self_attn.o_proj.weight", this->transformer.layers[i].attention.dense.weight);
-        if (this->transformer.layers[i].attention.dense.bias) {
-            sd.emplace_back(layer_prefix + "self_attn.o_proj.bias", this->transformer.layers[i].attention.dense.bias);
+        sd.emplace_back(layer_prefix + "self_attn.o_proj.weight", transformer.layers[i].attention.dense.weight);
+        if (transformer.layers[i].attention.dense.bias) {
+            sd.emplace_back(layer_prefix + "self_attn.o_proj.bias", transformer.layers[i].attention.dense.bias);
         }
         sd.emplace_back(layer_prefix + "post_attention_layernorm.weight",
-                        this->transformer.layers[i].post_attention_layernorm.weight);
-        sd.emplace_back(layer_prefix + "mlp.gate_proj.weight", this->transformer.layers[i].mlp.gate_proj.weight);
-        sd.emplace_back(layer_prefix + "mlp.up_proj.weight", this->transformer.layers[i].mlp.up_proj.weight);
-        sd.emplace_back(layer_prefix + "mlp.down_proj.weight", this->transformer.layers[i].mlp.down_proj.weight);
+                        transformer.layers[i].post_attention_layernorm.weight);
+        sd.emplace_back(layer_prefix + "mlp.gate_proj.weight", transformer.layers[i].mlp.gate_proj.weight);
+        sd.emplace_back(layer_prefix + "mlp.up_proj.weight", transformer.layers[i].mlp.up_proj.weight);
+        sd.emplace_back(layer_prefix + "mlp.down_proj.weight", transformer.layers[i].mlp.down_proj.weight);
     }
-    sd.emplace_back("model.norm.weight", this->transformer.final_layernorm.weight);
-    sd.emplace_back("lm_head.weight", this->lm_head.weight);
+    sd.emplace_back("model.norm.weight", transformer.final_layernorm.weight);
+    sd.emplace_back("lm_head.weight", lm_head.weight);
     return sd;
 }
 
 // ===== pipeline =====
 
-Pipeline::Pipeline(const std::string &path) {
+Pipeline::Pipeline(const std::string &path, int max_length) {
+    auto _update_config_max_length = [](ModelConfig &config, int max_length) {
+        if (max_length > 0) {
+            CHATGLM_CHECK(max_length <= config.max_length)
+                << "Requested max_length (" << max_length << ") exceeds the max possible model sequence length ("
+                << config.max_length << ")";
+            config.max_length = max_length;
+        }
+    };
+
     mapped_file = std::make_unique<MappedFile>(path);
     ModelLoader loader(mapped_file->data, mapped_file->size);
 
     // load magic
     std::string magic = loader.read_string(4);
     CHATGLM_CHECK(magic == "ggml") << "model file is broken (bad magic)";
 
     // load model type
     ModelType model_type = (ModelType)loader.read_basic<int>();
     // load version
     int version = loader.read_basic<int>();
     if (model_type == ModelType::CHATGLM) {
-        CHATGLM_CHECK(version == 1) << "only support version 1 for now but got " << version;
-
         // load config
-        ModelConfig config(model_type, loader.read_basic<ConfigRecordV1>());
+        ModelConfig config;
+        if (version == 1) {
+            config = ModelConfig(model_type, loader.read_basic<ConfigRecordV1>(), 1e-5f, ActivationType::GELU, true,
+                                 true, true, false, RopeType::CHATGLM, 10000.f, -1, AttentionMaskType::CHATGLM, 0);
+        } else if (version == 2) {
+            config = ModelConfig(model_type, loader.read_basic<ConfigRecordV2>(), ActivationType::GELU, true, true,
+                                 true, false, RopeType::CHATGLM, -1, AttentionMaskType::CHATGLM);
+        } else {
+            CHATGLM_THROW << "only support version 1 or 2 for now but got " << version;
+        }
+        _update_config_max_length(config, max_length);
 
         // load tokenizer
         int proto_size = loader.read_basic<int>();
         std::string_view serialized_model_proto((char *)mapped_file->data + loader.tell(), proto_size);
         loader.seek(proto_size, SEEK_CUR);
         tokenizer = std::make_unique<ChatGLMTokenizer>(serialized_model_proto);
 
         // load model
         model = std::make_unique<ChatGLMForCausalLM>(config);
         model->load(loader);
     } else if (model_type == ModelType::CHATGLM2 || model_type == ModelType::CHATGLM3) {
-        CHATGLM_CHECK(version == 1) << "only support version 1 for now but got " << version;
-
         // load config
-        ModelConfig config(model_type, loader.read_basic<ConfigRecordV2>());
+        ModelConfig config;
+        if (version == 1) {
+            config = ModelConfig(model_type, loader.read_basic<ConfigRecordV1GQA>(), 1e-5f, ActivationType::SILU, true,
+                                 false, false, false, RopeType::GPTJ, 10000.f, 2, AttentionMaskType::CAUSAL, 0);
+        } else if (version == 2) {
+            config = ModelConfig(model_type, loader.read_basic<ConfigRecordV2>(), ActivationType::SILU, true, false,
+                                 false, false, RopeType::GPTJ, 2, AttentionMaskType::CAUSAL);
+        } else {
+            CHATGLM_THROW << "only support version 1 or 2 for now but got " << version;
+        }
+        _update_config_max_length(config, max_length);
 
         // load tokenizer
         int proto_size = loader.read_basic<int>();
         std::string_view serialized_model_proto((char *)mapped_file->data + loader.tell(), proto_size);
         loader.seek(proto_size, SEEK_CUR);
 
         if (model_type == ModelType::CHATGLM2) {
@@ -1522,64 +1809,76 @@
             tokenizer = std::move(chatglm3_tokenizer);
             model = std::make_unique<ChatGLM3ForCausalLM>(config);
         }
 
         // load model
         model->load(loader);
     } else if (model_type == ModelType::BAICHUAN7B) {
+        std::cerr << "[WARN] Baichuan models are deprecated in favor of llama.cpp, and will be removed in next major "
+                     "version of chatglm.cpp\n";
         CHATGLM_CHECK(version == 1) << "only support version 1 for now but got " << version;
 
         // load config
-        ModelConfig config(model_type, loader.read_basic<ConfigRecordV1>());
-        config.norm_eps = 1e-6;
+        ModelConfig config(model_type, loader.read_basic<ConfigRecordV1>(), 1e-6f, ActivationType::SILU, false, false,
+                           false, false, RopeType::NEOX, 10000.f, 1, AttentionMaskType::CAUSAL, 0);
+        _update_config_max_length(config, max_length);
 
         // load tokenizer
         int proto_size = loader.read_basic<int>();
         std::string_view serialized_model_proto((char *)mapped_file->data + loader.tell(), proto_size);
         loader.seek(proto_size, SEEK_CUR);
         tokenizer = std::make_unique<BaichuanTokenizer>(serialized_model_proto);
 
         // load model
         model = std::make_unique<Baichuan7BForCausalLM>(config);
         model->load(loader);
     } else if (model_type == ModelType::BAICHUAN13B) {
+        std::cerr << "[WARN] Baichuan models are deprecated in favor of llama.cpp, and will be removed in next major "
+                     "version of chatglm.cpp\n";
         CHATGLM_CHECK(version == 1) << "only support version 1 for now but got " << version;
 
         // load config
-        ModelConfig config(model_type, loader.read_basic<ConfigRecordV1>());
-        config.norm_eps = 1e-6;
+        ModelConfig config(model_type, loader.read_basic<ConfigRecordV1>(), 1e-6f, ActivationType::SILU, false, false,
+                           false, true, RopeType::DISABLED, 10000.f, -1, AttentionMaskType::CAUSAL, 0);
+        _update_config_max_length(config, max_length);
 
         // load tokenizer
         int proto_size = loader.read_basic<int>();
         std::string_view serialized_model_proto((char *)mapped_file->data + loader.tell(), proto_size);
         loader.seek(proto_size, SEEK_CUR);
         tokenizer = std::make_unique<BaichuanTokenizer>(serialized_model_proto);
 
         // load model
         model = std::make_unique<Baichuan13BForCausalLM>(config);
         model->load(loader);
     } else if (model_type == ModelType::INTERNLM) {
+        std::cerr << "[WARN] InternLM models are deprecated in favor of llama.cpp, and will be removed in next major "
+                     "version of chatglm.cpp\n";
         CHATGLM_CHECK(version == 1) << "only support version 1 for now but got " << version;
 
         // load config
-        ModelConfig config(model_type, loader.read_basic<ConfigRecordV1>());
-        config.norm_eps = 1e-6;
+        auto rec = loader.read_basic<ConfigRecordV1>();
+        ModelConfig config;
+        if (rec.hidden_size == 4096) {
+            config = ModelConfig(model_type, rec, 1e-6f, ActivationType::SILU, true, true, false, false, RopeType::NEOX,
+                                 10000.f, 1, AttentionMaskType::CAUSAL, 0);
+        } else {
+            config = ModelConfig(model_type, rec, 1e-6f, ActivationType::SILU, false, false, false, false,
+                                 RopeType::NEOX, 10000.f, 1, AttentionMaskType::CAUSAL, 0);
+        }
+        _update_config_max_length(config, max_length);
 
         // load tokenizer
         int proto_size = loader.read_basic<int>();
         std::string_view serialized_model_proto((char *)mapped_file->data + loader.tell(), proto_size);
         loader.seek(proto_size, SEEK_CUR);
         tokenizer = std::make_unique<InternLMTokenizer>(serialized_model_proto);
 
         // load model
-        if (config.hidden_size == 4096) {
-            model = std::make_unique<InternLM7BForCausalLM>(config);
-        } else {
-            model = std::make_unique<InternLM20BForCausalLM>(config);
-        }
+        model = std::make_unique<InternLMForCausalLM>(config);
         model->load(loader);
     } else {
         CHATGLM_THROW << "invalid model type " << (int)model_type;
     }
 }
 
 std::vector<int> Pipeline::generate(const std::vector<int> &input_ids, const GenerationConfig &gen_config,
```

### Comparing `chatglm-cpp-0.3.1/chatglm.h` & `chatglm_cpp-0.3.2/chatglm.h`

 * *Files 21% similar despite different names*

```diff
@@ -72,55 +72,122 @@
     int bos_token_id;
     int eos_token_id;
     int pad_token_id;
     int sep_token_id;
 };
 
 // For compatibility
-struct ConfigRecordV2 : public ConfigRecordV1 {
+struct ConfigRecordV1GQA : public ConfigRecordV1 {
     int num_kv_heads;
 };
 
+// TODO: use json to serialize config
+struct ConfigRecordV2 {
+    ggml_type dtype;
+    int vocab_size;
+    int hidden_size;
+    int num_attention_heads;
+    int num_key_value_heads;
+    int num_hidden_layers;
+    int intermediate_size;
+    float norm_eps;
+    int num_virtual_tokens;
+    float rope_theta;
+    int max_length;
+    int eos_token_id;
+    int pad_token_id;
+};
+
+enum class ActivationType {
+    GELU,
+    SILU,
+};
+
+enum class RopeType {
+    GPTJ = 0,
+    NEOX = 2,
+    CHATGLM = 4,
+    CHATGLM2 = 8,
+    DISABLED = 10000,
+};
+
+enum class AttentionMaskType {
+    CAUSAL,
+    CHATGLM,
+};
+
 // Should save kv record of ModelConfig in the future
 class ModelConfig {
   public:
     ModelConfig() = default;
 
     ModelConfig(ModelType model_type, ggml_type dtype, int vocab_size, int hidden_size, int num_attention_heads,
-                int num_kv_heads, int num_hidden_layers, int intermediate_size, float norm_eps, int max_length,
-                int bos_token_id, int eos_token_id, int pad_token_id, int sep_token_id,
-                std::vector<int> extra_eos_token_ids)
+                int num_kv_heads, int num_hidden_layers, int intermediate_size, float norm_eps,
+                ActivationType hidden_act, bool use_qkv_bias, bool use_dense_bias, bool interleaved_qkv, bool use_alibi,
+                RopeType rope_type, float rope_theta, int rope_dim_scale, AttentionMaskType attn_mask_type,
+                int num_virtual_tokens, int max_length, int bos_token_id, int eos_token_id, int pad_token_id,
+                int sep_token_id, std::vector<int> extra_eos_token_ids)
         : model_type(model_type), dtype(dtype), vocab_size(vocab_size), hidden_size(hidden_size),
           num_attention_heads(num_attention_heads), num_kv_heads(num_kv_heads), num_hidden_layers(num_hidden_layers),
-          intermediate_size(intermediate_size), norm_eps(norm_eps), max_length(max_length), bos_token_id(bos_token_id),
+          intermediate_size(intermediate_size), norm_eps(norm_eps), hidden_act(hidden_act), use_qkv_bias(use_qkv_bias),
+          use_dense_bias(use_dense_bias), interleaved_qkv(interleaved_qkv), use_alibi(use_alibi), rope_type(rope_type),
+          rope_theta(rope_theta), rope_dim_scale(rope_dim_scale), attn_mask_type(attn_mask_type),
+          num_virtual_tokens(num_virtual_tokens), max_length(max_length), bos_token_id(bos_token_id),
           eos_token_id(eos_token_id), pad_token_id(pad_token_id), sep_token_id(sep_token_id),
           extra_eos_token_ids(std::move(extra_eos_token_ids)) {}
 
-    ModelConfig(ModelType model_type, const ConfigRecordV1 &rec)
+    ModelConfig(ModelType model_type, const ConfigRecordV1 &rec, float norm_eps, ActivationType hidden_act,
+                bool use_qkv_bias, bool use_dense_bias, bool interleaved_qkv, bool use_alibi, RopeType rope_type,
+                float rope_theta, int rope_dim_scale, AttentionMaskType attn_mask_type, int num_virtual_tokens)
         : ModelConfig(model_type, rec.dtype, rec.vocab_size, rec.hidden_size, rec.num_attention_heads,
-                      rec.num_attention_heads, rec.num_hidden_layers, rec.intermediate_size, 1e-5, rec.max_length,
-                      rec.bos_token_id, rec.eos_token_id, rec.pad_token_id, rec.sep_token_id, {}) {}
-
-    ModelConfig(ModelType model_type, const ConfigRecordV2 &rec)
+                      rec.num_attention_heads, rec.num_hidden_layers, rec.intermediate_size, norm_eps, hidden_act,
+                      use_qkv_bias, use_dense_bias, interleaved_qkv, use_alibi, rope_type, rope_theta, rope_dim_scale,
+                      attn_mask_type, num_virtual_tokens, rec.max_length, rec.bos_token_id, rec.eos_token_id,
+                      rec.pad_token_id, rec.sep_token_id, {}) {}
+
+    ModelConfig(ModelType model_type, const ConfigRecordV1GQA &rec, float norm_eps, ActivationType hidden_act,
+                bool use_qkv_bias, bool use_dense_bias, bool interleaved_qkv, bool use_alibi, RopeType rope_type,
+                float rope_theta, int rope_dim_scale, AttentionMaskType attn_mask_type, int num_virtual_tokens)
         : ModelConfig(model_type, rec.dtype, rec.vocab_size, rec.hidden_size, rec.num_attention_heads, rec.num_kv_heads,
-                      rec.num_hidden_layers, rec.intermediate_size, 1e-5, rec.max_length, rec.bos_token_id,
-                      rec.eos_token_id, rec.pad_token_id, rec.sep_token_id, {}) {}
+                      rec.num_hidden_layers, rec.intermediate_size, norm_eps, hidden_act, use_qkv_bias, use_dense_bias,
+                      interleaved_qkv, use_alibi, rope_type, rope_theta, rope_dim_scale, attn_mask_type,
+                      num_virtual_tokens, rec.max_length, rec.bos_token_id, rec.eos_token_id, rec.pad_token_id,
+                      rec.sep_token_id, {}) {}
+
+    ModelConfig(ModelType model_type, const ConfigRecordV2 &rec, ActivationType hidden_act, bool use_qkv_bias,
+                bool use_dense_bias, bool interleaved_qkv, bool use_alibi, RopeType rope_type, int rope_dim_scale,
+                AttentionMaskType attn_mask_type)
+        : ModelConfig(model_type, rec.dtype, rec.vocab_size, rec.hidden_size, rec.num_attention_heads,
+                      rec.num_key_value_heads, rec.num_hidden_layers, rec.intermediate_size, rec.norm_eps, hidden_act,
+                      use_qkv_bias, use_dense_bias, interleaved_qkv, use_alibi, rope_type, rec.rope_theta,
+                      rope_dim_scale, attn_mask_type, rec.num_virtual_tokens, rec.max_length, -1, rec.eos_token_id,
+                      rec.pad_token_id, -1, {}) {}
 
     std::string model_type_name() const { return to_string(model_type); }
 
   public:
     ModelType model_type;
     ggml_type dtype;
     int vocab_size;
     int hidden_size;
     int num_attention_heads;
     int num_kv_heads;
     int num_hidden_layers;
     int intermediate_size;
     float norm_eps;
+    ActivationType hidden_act;
+    bool use_qkv_bias;
+    bool use_dense_bias;
+    bool interleaved_qkv;
+    bool use_alibi;
+    RopeType rope_type;
+    float rope_theta;
+    int rope_dim_scale;
+    AttentionMaskType attn_mask_type;
+    int num_virtual_tokens;
     int max_length;
     int bos_token_id;
     int eos_token_id;
     int pad_token_id;
     int sep_token_id;
     std::vector<int> extra_eos_token_ids;
 };
@@ -312,297 +379,95 @@
 
   public:
     ggml_tensor *weight; // [normalized_shape]
     bool inplace;
     float eps;
 };
 
-enum class ActivationType {
-    GELU,
-    SILU,
-};
-
-template <ActivationType ACT_TYPE>
-static inline ggml_tensor *apply_activation_inplace(ggml_context *ctx, ggml_tensor *hidden_states) {
-    static_assert(ACT_TYPE == ActivationType::GELU || ACT_TYPE == ActivationType::SILU);
-    if constexpr (ACT_TYPE == ActivationType::GELU) {
-        hidden_states = tensor_assign_buffers(ggml_gelu_inplace(ctx, hidden_states));
-    } else if constexpr (ACT_TYPE == ActivationType::SILU) {
-        hidden_states = tensor_assign_buffers(ggml_silu_inplace(ctx, hidden_states));
-    } else {
-        CHATGLM_THROW << "Unknown activation type " << (int)ACT_TYPE;
-    }
-    return hidden_states;
-}
-
-template <ActivationType ACT_TYPE>
 class BasicMLP {
   public:
     BasicMLP() = default;
-    BasicMLP(ModelContext *ctx, int hidden_size, int intermediate_size)
-        : dense_h_to_4h(ctx, hidden_size, intermediate_size), dense_4h_to_h(ctx, intermediate_size, hidden_size) {}
+    BasicMLP(ModelContext *ctx, int hidden_size, int intermediate_size, ActivationType hidden_act)
+        : dense_h_to_4h(ctx, hidden_size, intermediate_size), dense_4h_to_h(ctx, intermediate_size, hidden_size),
+          hidden_act(hidden_act) {}
 
-    ggml_tensor *forward(ModelContext *ctx, ggml_tensor *hidden_states) const {
-        ggml_context *gctx = ctx->ctx_b.get();
-        hidden_states = dense_h_to_4h.forward(ctx, hidden_states);
-        hidden_states = apply_activation_inplace<ACT_TYPE>(gctx, hidden_states);
-        hidden_states = dense_4h_to_h.forward(ctx, hidden_states);
-        return hidden_states;
-    }
+    ggml_tensor *forward(ModelContext *ctx, ggml_tensor *hidden_states) const;
 
   public:
     Linear dense_h_to_4h;
     Linear dense_4h_to_h;
+    ActivationType hidden_act;
 };
 
-template <ActivationType ACT_TYPE, bool USE_BIAS>
 class BasicGLU {
   public:
     BasicGLU() = default;
-    BasicGLU(ModelContext *ctx, int hidden_size, int intermediate_size)
-        : gate_proj(ctx, hidden_size, intermediate_size, USE_BIAS),
-          up_proj(ctx, hidden_size, intermediate_size, USE_BIAS),
-          down_proj(ctx, intermediate_size, hidden_size, USE_BIAS) {}
+    BasicGLU(ModelContext *ctx, int hidden_size, int intermediate_size, ActivationType hidden_act)
+        : gate_proj(ctx, hidden_size, intermediate_size, false), up_proj(ctx, hidden_size, intermediate_size, false),
+          down_proj(ctx, intermediate_size, hidden_size, false), hidden_act(hidden_act) {}
 
-    ggml_tensor *forward(ModelContext *ctx, ggml_tensor *hidden_states) const {
-        ggml_context *gctx = ctx->ctx_b.get();
-        ggml_tensor *gate = gate_proj.forward(ctx, hidden_states);
-        gate = apply_activation_inplace<ACT_TYPE>(gctx, gate);
-        hidden_states = up_proj.forward(ctx, hidden_states);
-        hidden_states = tensor_assign_buffers(ggml_mul_inplace(gctx, hidden_states, gate));
-        hidden_states = down_proj.forward(ctx, hidden_states);
-        return hidden_states;
-    }
+    ggml_tensor *forward(ModelContext *ctx, ggml_tensor *hidden_states) const;
 
   public:
     Linear gate_proj;
     Linear up_proj;
     Linear down_proj;
+    ActivationType hidden_act;
 };
 
-struct CausalContextMasker {
-    ggml_tensor *operator()(ModelContext *ctx, ggml_tensor *attn_scores, int n_past) const {
-        return tensor_assign_buffers(ggml_diag_mask_inf_inplace(ctx->ctx_b.get(), attn_scores, n_past));
-    }
-};
-
-enum RopeType {
-    ROPE_TYPE_DEFAULT = 0,
-    ROPE_TYPE_NEOX = 2,
-    ROPE_TYPE_CHATGLM = 4,
-};
-
-struct NoopRoper {
-    ggml_tensor *operator()(ModelContext *ctx, ggml_tensor *a, ggml_tensor *b, int n_ctx) const { return a; }
-};
-
-template <RopeType MODE, int DIM_SCALE>
-struct BasicRoper {
-    ggml_tensor *operator()(ModelContext *ctx, ggml_tensor *a, ggml_tensor *b, int n_ctx) const {
-        // tensor a (activation) is of shape [qlen, heads, head_size]
-        // tensor b (position_ids) is of shape [qlen]
-        ggml_context *gctx = ctx->ctx_b.get();
-#ifdef GGML_USE_CUBLAS
-        if (!ggml_is_contiguous(a)) {
-            a = tensor_assign_buffers(ggml_cont(gctx, a));
-        }
-#endif
-        const int head_size = a->ne[0];
-        const int rope_dim = head_size / DIM_SCALE;
-        a = tensor_assign_buffers(ggml_rope_inplace(gctx, a, b, rope_dim, MODE, n_ctx)); // [qlen, heads, head_size]
-
-        return a;
-    }
-};
-
-struct GLMRoper {
-    ggml_tensor *operator()(ModelContext *ctx, ggml_tensor *a, ggml_tensor *b, int n_ctx) const {
-        // tensor a (activation) is of shape [qlen, heads, head_size]
-        // tensor b (position_ids) is of shape [2 * qlen]
-        ggml_context *gctx = ctx->ctx_b.get();
-
-        const int head_size = a->ne[0];
-        const int num_heads = a->ne[1];
-        const int qlen = a->ne[2];
-        const int rope_dim = head_size / 2;
-
-        ggml_tensor *b1 = ggml_view_1d(gctx, b, qlen, 0);
-        ggml_tensor *b2 = ggml_view_1d(gctx, b, qlen, qlen * ggml_element_size(b));
-
-        ggml_tensor *a1 = ggml_view_3d(gctx, a, head_size / 2, num_heads, qlen, a->nb[1], a->nb[2], 0);
-        ggml_tensor *a2 = ggml_view_3d(gctx, a, head_size / 2, num_heads, qlen, a->nb[1], a->nb[2],
-                                       head_size / 2 * ggml_element_size(a));
-
-        ggml_tensor *a1_rope = a1;
-        ggml_tensor *a2_rope = a2;
-#ifdef GGML_USE_CUBLAS
-        a1_rope = tensor_assign_buffers(ggml_cont(gctx, a1_rope));
-        a2_rope = tensor_assign_buffers(ggml_cont(gctx, a2_rope));
-#endif
-
-        a1_rope = tensor_assign_buffers(
-            ggml_rope_inplace(gctx, a1_rope, b1, rope_dim, ROPE_TYPE_NEOX, n_ctx)); // [qlen, heads, head_size/2]
-        a2_rope = tensor_assign_buffers(
-            ggml_rope_inplace(gctx, a2_rope, b2, rope_dim, ROPE_TYPE_NEOX, n_ctx)); // [qlen, heads, head_size/2]
-
-#ifdef GGML_USE_CUBLAS
-        a1_rope = ggml_cpy(gctx, a1_rope, a1);
-        a2_rope = ggml_cpy(gctx, a2_rope, a2);
-#endif
-        ggml_build_forward_expand(&ctx->gf, a1_rope);
-        ggml_build_forward_expand(&ctx->gf, a2_rope);
-
-        return a;
-    }
-};
-
-template <bool USE_QKV_BIAS, bool USE_DENSE_BIAS, bool INTERLEAVED_QKV, typename Roper, bool USE_ALIBI,
-          typename ContextMasker>
 class BasicAttention {
   public:
     BasicAttention() = default;
-    BasicAttention(ModelContext *ctx, int hidden_size, int num_attention_heads, int num_kv_heads, int max_length)
-        : num_attention_heads(num_attention_heads), num_kv_heads(num_kv_heads),
+    BasicAttention(ModelContext *ctx, int hidden_size, int num_attention_heads, int num_kv_heads, int max_length,
+                   bool use_qkv_bias, bool use_dense_bias, bool interleaved_qkv, bool use_alibi, RopeType rope_type,
+                   float rope_theta, int rope_dim_scale, AttentionMaskType attn_mask_type, int num_virtual_tokens)
+        : num_attention_heads(num_attention_heads), num_kv_heads(num_kv_heads), interleaved_qkv(interleaved_qkv),
+          use_alibi(use_alibi), rope_type(rope_type), rope_theta(rope_theta), rope_dim_scale(rope_dim_scale),
+          attn_mask_type(attn_mask_type), num_virtual_tokens(num_virtual_tokens),
           query_key_value(ctx, hidden_size, hidden_size + 2 * (hidden_size / num_attention_heads) * num_kv_heads,
-                          USE_QKV_BIAS),
-          dense(ctx, hidden_size, hidden_size, USE_DENSE_BIAS),
-          k_cache(ggml_new_tensor_3d(ctx->ctx_kv.get(), GGML_TYPE_F16, hidden_size / num_attention_heads, max_length,
-                                     num_kv_heads)),
-          v_cache(ggml_new_tensor_3d(ctx->ctx_kv.get(), GGML_TYPE_F16, max_length, hidden_size / num_attention_heads,
-                                     num_kv_heads)) {}
+                          use_qkv_bias),
+          dense(ctx, hidden_size, hidden_size, use_dense_bias),
+          k_cache(ggml_new_tensor_3d(ctx->ctx_kv.get(), GGML_TYPE_F16, hidden_size / num_attention_heads,
+                                     max_length + num_virtual_tokens, num_kv_heads)),
+          v_cache(ggml_new_tensor_3d(ctx->ctx_kv.get(), GGML_TYPE_F16, max_length + num_virtual_tokens,
+                                     hidden_size / num_attention_heads, num_kv_heads)) {}
 
     ggml_tensor *forward(ModelContext *ctx, ggml_tensor *hidden_states, ggml_tensor *position_ids, int n_past,
-                         int n_ctx) const {
-        ggml_context *gctx = ctx->ctx_b.get();
-
-        const int hidden_size = hidden_states->ne[0];
-        const int qlen = hidden_states->ne[1];
-        const int head_size = hidden_size / num_attention_heads;
-        const int num_shared_q_heads = num_attention_heads / num_kv_heads;
-        const bool is_gqa = num_shared_q_heads > 1;
-
-        ggml_tensor *qkv = query_key_value.forward(ctx, hidden_states); // [qlen, hidden + 2 * kv_hidden]
-
-        // split mixed qkv into separate query, key and value
-        ggml_tensor *query_layer; // [qlen, heads, head_size]
-        ggml_tensor *key_layer;   // [qlen, kv_heads, head_size]
-        ggml_tensor *value_layer; // [qlen, kv_heads, head_size]
-
-        if constexpr (INTERLEAVED_QKV) {
-            CHATGLM_CHECK(!is_gqa) << "interleaved qkv is not supported for GQA";
-            query_layer = ggml_view_3d(gctx, qkv, head_size, num_attention_heads, qlen,
-                                       3 * head_size * ggml_element_size(qkv), qkv->nb[1], 0);
-            key_layer =
-                ggml_view_3d(gctx, qkv, head_size, num_attention_heads, qlen, 3 * head_size * ggml_element_size(qkv),
-                             qkv->nb[1], head_size * ggml_element_size(qkv));
-            value_layer =
-                ggml_view_3d(gctx, qkv, head_size, num_attention_heads, qlen, 3 * head_size * ggml_element_size(qkv),
-                             qkv->nb[1], 2 * head_size * ggml_element_size(qkv));
-        } else {
-            query_layer = ggml_view_3d(gctx, qkv, head_size, num_attention_heads, qlen,
-                                       head_size * ggml_element_size(qkv), qkv->nb[1], 0);
-            key_layer = ggml_view_3d(gctx, qkv, head_size, num_kv_heads, qlen, head_size * ggml_element_size(qkv),
-                                     qkv->nb[1], hidden_size * ggml_element_size(qkv));
-            value_layer = ggml_view_3d(gctx, qkv, head_size, num_kv_heads, qlen, head_size * ggml_element_size(qkv),
-                                       qkv->nb[1], (hidden_size + head_size * num_kv_heads) * ggml_element_size(qkv));
-        }
-
-        query_layer = roper_(ctx, query_layer, position_ids, n_ctx);
-        key_layer = roper_(ctx, key_layer, position_ids, n_ctx);
-
-        query_layer = tensor_assign_buffers(
-            ggml_cont(gctx, ggml_permute(gctx, query_layer, 0, 2, 1, 3))); // [heads, qlen, head_size]
-        if (num_shared_q_heads > 1) {
-            query_layer =
-                tensor_assign_buffers(ggml_reshape_3d(gctx, query_layer, head_size, num_shared_q_heads * qlen,
-                                                      num_kv_heads)); // [kv_heads, shared_qheads * qlen, head_size]
-        }
-
-        key_layer = tensor_assign_buffers(ggml_permute(gctx, key_layer, 0, 2, 1, 3)); // [kv_heads, qlen, head_size]
-
-        value_layer = tensor_assign_buffers(ggml_permute(gctx, value_layer, 1, 2, 0, 3)); // [kv_heads, head_size, qlen]
-
-        // store key & value to cache
-        ggml_tensor *k_cache_view = tensor_assign_buffers(
-            ggml_view_3d(gctx, k_cache, head_size, qlen, num_kv_heads, k_cache->nb[1], k_cache->nb[2],
-                         n_past * head_size * ggml_element_size(k_cache))); // [kv_heads, qlen, head_size]
-        ggml_build_forward_expand(&ctx->gf, ggml_cpy(gctx, key_layer, k_cache_view));
-        ggml_tensor *v_cache_view = tensor_assign_buffers(
-            ggml_view_3d(gctx, v_cache, qlen, head_size, num_kv_heads, v_cache->nb[1], v_cache->nb[2],
-                         n_past * ggml_element_size(v_cache))); // [kv_heads, head_size, qlen]
-        ggml_build_forward_expand(&ctx->gf, ggml_cpy(gctx, value_layer, v_cache_view));
-
-        // concat key & value with past kv
-        key_layer = tensor_assign_buffers(ggml_view_3d(gctx, k_cache, head_size, n_past + qlen, num_kv_heads,
-                                                       k_cache->nb[1], k_cache->nb[2],
-                                                       0)); // [kv_heads, klen, head_size]
-        value_layer = tensor_assign_buffers(ggml_view_3d(gctx, v_cache, n_past + qlen, head_size, num_kv_heads,
-                                                         v_cache->nb[1], v_cache->nb[2],
-                                                         0)); // [kv_heads, head_size, klen]
-
-        // attention
-        ggml_tensor *attn_scores =
-            tensor_assign_buffers(ggml_mul_mat(gctx, key_layer, query_layer)); // [kv_heads, shared_qheads * qlen, klen]
-        attn_scores = tensor_assign_buffers(
-            ggml_scale_inplace(gctx, attn_scores, ggml_new_f32(gctx, 1.f / std::sqrt(head_size))));
-        if constexpr (USE_ALIBI) {
-            attn_scores = tensor_assign_buffers(ggml_alibi(gctx, attn_scores, n_past, num_attention_heads, 8));
-        }
-        if (n_past == 0) {
-            // build attention mask for context input
-            if (num_shared_q_heads > 1) {
-                attn_scores = ggml_reshape_3d(gctx, attn_scores, n_past + qlen, qlen,
-                                              num_attention_heads); // [heads, qlen, klen]
-            }
-            attn_scores = context_masker_(ctx, attn_scores, n_past);
-            if (num_shared_q_heads > 1) {
-                attn_scores = ggml_reshape_3d(gctx, attn_scores, n_past + qlen, num_shared_q_heads * qlen,
-                                              num_kv_heads); // [kv_heads, shared_qheads * qlen, klen]
-            }
-        }
-        ggml_tensor *attn_probs =
-            tensor_assign_buffers(ggml_soft_max_inplace(gctx, attn_scores)); // [kv_heads, shared_qheads * qlen, klen]
-
-        ggml_tensor *context_layer = tensor_assign_buffers(
-            ggml_mul_mat(gctx, value_layer, attn_probs)); // [kv_heads, shared_qheads * qlen, head_size]
-        if (num_shared_q_heads > 1) {
-            context_layer = ggml_reshape_3d(gctx, context_layer, head_size, qlen,
-                                            num_attention_heads); // [heads, qlen, head_size]
-        }
-        context_layer = tensor_assign_buffers(
-            ggml_cont(gctx, ggml_permute(gctx, context_layer, 0, 2, 1, 3))); // [qlen, heads, head_size]
-        context_layer =
-            tensor_assign_buffers(ggml_reshape_2d(gctx, context_layer, hidden_size, qlen)); // [qlen, hidden]
-
-        ggml_tensor *attn_output = dense.forward(ctx, context_layer);
-        return attn_output;
-    }
+                         int n_ctx) const;
 
   public:
     int num_attention_heads;
     int num_kv_heads;
+    bool interleaved_qkv;
+    bool use_alibi;
+    RopeType rope_type;
+    float rope_theta;
+    int rope_dim_scale;
+    AttentionMaskType attn_mask_type;
+    int num_virtual_tokens;
     Linear query_key_value;
     Linear dense;
-    ggml_tensor *k_cache; // [kv_heads, max_len, head_size]
-    ggml_tensor *v_cache; // [kv_heads, head_size, max_len]
-
-  private:
-    Roper roper_;
-    ContextMasker context_masker_;
+    ggml_tensor *k_cache; // [#kvh, s, d]
+    ggml_tensor *v_cache; // [#kvh, d, s]
 };
 
 template <typename Norm, typename Attention, typename MLP>
 class BasicBlock {
   public:
     BasicBlock() = default;
     BasicBlock(ModelContext *ctx, int hidden_size, int num_attention_heads, int num_kv_heads, int intermediate_size,
-               int max_length, float norm_eps)
+               int max_length, float norm_eps, ActivationType hidden_act, bool use_qkv_bias, bool use_dense_bias,
+               bool interleaved_qkv, bool use_alibi, RopeType rope_type, float rope_theta, int rope_dim_scale,
+               AttentionMaskType attn_mask_type, int num_virtual_tokens)
         : input_layernorm(ctx, hidden_size, false, norm_eps),
-          attention(ctx, hidden_size, num_attention_heads, num_kv_heads, max_length),
-          post_attention_layernorm(ctx, hidden_size, false, norm_eps), mlp(ctx, hidden_size, intermediate_size) {}
+          attention(ctx, hidden_size, num_attention_heads, num_kv_heads, max_length, use_qkv_bias, use_dense_bias,
+                    interleaved_qkv, use_alibi, rope_type, rope_theta, rope_dim_scale, attn_mask_type,
+                    num_virtual_tokens),
+          post_attention_layernorm(ctx, hidden_size, false, norm_eps),
+          mlp(ctx, hidden_size, intermediate_size, hidden_act) {}
 
     ggml_tensor *forward(ModelContext *ctx, ggml_tensor *hidden_states, ggml_tensor *position_ids, int n_past,
                          int n_ctx) const {
         ggml_context *gctx = ctx->ctx_b.get();
 
         ggml_tensor *residual = hidden_states;
         hidden_states = input_layernorm.forward(ctx, hidden_states);
@@ -683,22 +548,52 @@
         }
         ggml_scratch empty_scratch = {0, 0, nullptr};
         ggml_set_scratch(gctx, empty_scratch);
         hidden_states = final_layernorm.forward(ctx, hidden_states);
         return hidden_states;
     }
 
+    void load_prefix_cache(const ModelConfig &config, ggml_tensor *past_key_values) {
+        ggml_cgraph gf{};
+        auto ctx = make_unique_ggml_context(config.num_hidden_layers * 7 * ggml_tensor_overhead(), nullptr, false);
+        const int head_size = config.hidden_size / config.num_attention_heads;
+        for (size_t i = 0; i < layers.size(); i++) {
+            auto &attn = layers[i].attention;
+            ggml_tensor *virtual_key = ggml_view_3d(ctx.get(), past_key_values, head_size, config.num_virtual_tokens,
+                                                    config.num_kv_heads, past_key_values->nb[1], past_key_values->nb[2],
+                                                    i * 2 * past_key_values->nb[3]); // [#h, v, d]
+            ggml_tensor *k_cache_view =
+                ggml_view_3d(ctx.get(), attn.k_cache, head_size, config.num_virtual_tokens, config.num_kv_heads,
+                             attn.k_cache->nb[1], attn.k_cache->nb[2], 0); // [#h, v, d]
+            ggml_build_forward_expand(&gf, ggml_cpy(ctx.get(), virtual_key, k_cache_view));
+
+            ggml_tensor *virtual_value = ggml_view_3d(
+                ctx.get(), past_key_values, head_size, config.num_virtual_tokens, config.num_kv_heads,
+                past_key_values->nb[1], past_key_values->nb[2], (i * 2 + 1) * past_key_values->nb[3]); // [#h, v, d]
+            virtual_value = ggml_permute(ctx.get(), virtual_value, 1, 0, 2, 3);                        // [#h, d, v]
+            ggml_tensor *v_cache_view =
+                ggml_view_3d(ctx.get(), attn.v_cache, config.num_virtual_tokens, head_size, config.num_kv_heads,
+                             attn.v_cache->nb[1], attn.v_cache->nb[2], 0); // [#h, d, v]
+            ggml_build_forward_expand(&gf, ggml_cpy(ctx.get(), virtual_value, v_cache_view));
+        }
+        CHATGLM_CHECK(ggml_used_mem(ctx.get()) == ggml_get_mem_size(ctx.get())) << "corrupted prefix cache context";
+        std::vector<uninitialized_char> compute_buffer;
+        ggml_graph_compute_helper(compute_buffer, &gf, 0);
+    }
+
   private:
     std::vector<Block> build_layers(ModelContext *ctx, const ModelConfig &config) {
         std::vector<Block> layers;
         layers.reserve(config.num_hidden_layers);
         for (int layer_id = 0; layer_id < config.num_hidden_layers; layer_id++) {
-            // TODO: reduce max length? 32k might be too large for cpu inference
             layers.emplace_back(ctx, config.hidden_size, config.num_attention_heads, config.num_kv_heads,
-                                config.intermediate_size, config.max_length, config.norm_eps);
+                                config.intermediate_size, config.max_length, config.norm_eps, config.hidden_act,
+                                config.use_qkv_bias, config.use_dense_bias, config.interleaved_qkv, config.use_alibi,
+                                config.rope_type, config.rope_theta, config.rope_dim_scale, config.attn_mask_type,
+                                config.num_virtual_tokens);
         }
         return layers;
     }
 
   public:
     Embedding word_embeddings;
     std::vector<Block> layers;
@@ -909,14 +804,16 @@
                 ggml_view_1d(ctx->ctx_b.get(), transformer_outputs, config.hidden_size,
                              (input_ids->ne[0] - 1) * config.hidden_size * ggml_element_size(transformer_outputs)));
         }
         ggml_tensor *lm_logits = lm_head.forward(ctx, transformer_outputs);
         return lm_logits;
     }
 
+    void load_prefix_cache(ggml_tensor *past_key_values) { transformer.load_prefix_cache(config, past_key_values); }
+
   protected:
     void to_cpu() {
         for (auto &item : state_dict_) {
             tensor_to_cpu(item.second);
         }
 
         for (auto &layer : transformer.layers) {
@@ -976,27 +873,28 @@
     int pad_token_id;
 };
 
 struct GLMContextMasker {
     ggml_tensor *operator()(ModelContext *ctx, ggml_tensor *attn_scores, int n_past) const;
 };
 
-using GLMAttention = BasicAttention<true, true, true, GLMRoper, false, GLMContextMasker>;
-
-using GLMMLP = BasicMLP<ActivationType::GELU>;
-
 // NOTE: disable inplace norm since it causes nonsense on cuda when sequence length >= 144
-class GLMBlock : public BasicBlock<LayerNorm, GLMAttention, GLMMLP> {
+class GLMBlock : public BasicBlock<LayerNorm, BasicAttention, BasicMLP> {
   public:
     GLMBlock() = default;
     GLMBlock(ModelContext *ctx, int hidden_size, int num_attention_heads, int num_kv_heads, int intermediate_size,
-             int max_length, float norm_eps)
+             int max_length, float norm_eps, ActivationType hidden_act, bool use_qkv_bias, bool use_dense_bias,
+             bool interleaved_qkv, bool use_alibi, RopeType rope_type, float rope_theta, int rope_dim_scale,
+             AttentionMaskType attn_mask_type, int num_virtual_tokens)
         : BasicBlock(LayerNorm(ctx, hidden_size, false, norm_eps),
-                     GLMAttention(ctx, hidden_size, num_attention_heads, num_attention_heads, max_length),
-                     LayerNorm(ctx, hidden_size, false, norm_eps), GLMMLP(ctx, hidden_size, intermediate_size)),
+                     BasicAttention(ctx, hidden_size, num_attention_heads, num_attention_heads, max_length,
+                                    use_qkv_bias, use_dense_bias, interleaved_qkv, use_alibi, rope_type, rope_theta,
+                                    rope_dim_scale, attn_mask_type, num_virtual_tokens),
+                     LayerNorm(ctx, hidden_size, false, norm_eps),
+                     BasicMLP(ctx, hidden_size, intermediate_size, hidden_act)),
           alpha_value(std::sqrt(2.f * 28)) {}
 
     ggml_tensor *forward(ModelContext *ctx, ggml_tensor *hidden_states, ggml_tensor *position_ids, int n_past,
                          int n_ctx) const;
 
   public:
     float alpha_value;
@@ -1042,19 +940,15 @@
     int mask_token_id;
     int gmask_token_id;
     int smask_token_id;
     int sop_token_id;
     int eop_token_id;
 };
 
-using GLM2Attention = BasicAttention<true, false, false, BasicRoper<ROPE_TYPE_DEFAULT, 2>, false, CausalContextMasker>;
-
-using GLM2MLP = BasicGLU<ActivationType::SILU, false>;
-
-using GLM2Block = BasicBlock<RMSNorm, GLM2Attention, GLM2MLP>;
+using GLM2Block = BasicBlock<RMSNorm, BasicAttention, BasicGLU>;
 
 using ChatGLM2Model = BasicModel<GLM2Block, RMSNorm, BasicPositionIdsGenerator>;
 
 class ChatGLM2ForCausalLM : public BasicModelForCausalLM<ChatGLM2Model> {
   public:
     ChatGLM2ForCausalLM(const ModelConfig &config);
 
@@ -1141,20 +1035,15 @@
     int bos_token_id;
     int eos_token_id;
     int pad_token_id;
 };
 
 // ===== Baichuan-7B =====
 
-using Baichuan7BAttention =
-    BasicAttention<false, false, false, BasicRoper<ROPE_TYPE_NEOX, 1>, false, CausalContextMasker>;
-
-using Baichuan7BMLP = BasicGLU<ActivationType::SILU, false>;
-
-using Baichuan7BBlock = BasicBlock<RMSNorm, Baichuan7BAttention, Baichuan7BMLP>;
+using Baichuan7BBlock = BasicBlock<RMSNorm, BasicAttention, BasicGLU>;
 
 using Baichuan7BModel = BasicModel<Baichuan7BBlock, RMSNorm, BasicPositionIdsGenerator>;
 
 class Baichuan7BForCausalLM : public BasicModelForCausalLM<Baichuan7BModel> {
   public:
     Baichuan7BForCausalLM(const ModelConfig &config);
 
@@ -1168,19 +1057,15 @@
   public:
     static constexpr size_t MEM_SIZE = 1280 * MB;
     static constexpr size_t SCRATCH_SIZE = 1280 * MB;
 };
 
 // ===== Baichuan-13B =====
 
-using Baichuan13BAttention = BasicAttention<false, false, false, NoopRoper, true, CausalContextMasker>;
-
-using Baichuan13BMLP = BasicGLU<ActivationType::SILU, false>;
-
-using Baichuan13BBlock = BasicBlock<RMSNorm, Baichuan13BAttention, Baichuan13BMLP>;
+using Baichuan13BBlock = BasicBlock<RMSNorm, BasicAttention, BasicGLU>;
 
 using Baichuan13BModel = BasicModel<Baichuan13BBlock, RMSNorm, NoopPositionIdsGenerator>;
 
 class Baichuan13BForCausalLM : public BasicModelForCausalLM<Baichuan13BModel> {
   public:
     Baichuan13BForCausalLM(const ModelConfig &config);
 
@@ -1216,60 +1101,41 @@
   public:
     sentencepiece::SentencePieceProcessor sp;
     static constexpr int unk_token_id = 0;
     static constexpr int bos_token_id = 1;
     static constexpr int eos_token_id = 2;
 };
 
-using InternLM7BAttention =
-    BasicAttention<true, true, false, BasicRoper<ROPE_TYPE_NEOX, 1>, false, CausalContextMasker>;
-
-using InternLM7BMLP = BasicGLU<ActivationType::SILU, false>;
-
-using InternLM7BBlock = BasicBlock<RMSNorm, InternLM7BAttention, InternLM7BMLP>;
+using InternLMBlock = BasicBlock<RMSNorm, BasicAttention, BasicGLU>;
 
-using InternLM7BModel = BasicModel<InternLM7BBlock, RMSNorm, BasicPositionIdsGenerator>;
+using InternLMModel = BasicModel<InternLMBlock, RMSNorm, BasicPositionIdsGenerator>;
 
-using InternLM20BAttention =
-    BasicAttention<false, false, false, BasicRoper<ROPE_TYPE_NEOX, 1>, false, CausalContextMasker>;
-
-using InternLM20BMLP = BasicGLU<ActivationType::SILU, false>;
-
-using InternLM20BBlock = BasicBlock<RMSNorm, InternLM20BAttention, InternLM20BMLP>;
-
-using InternLM20BModel = BasicModel<InternLM20BBlock, RMSNorm, BasicPositionIdsGenerator>;
-
-template <typename InternLMModel>
 class InternLMForCausalLM : public BasicModelForCausalLM<InternLMModel> {
   public:
     InternLMForCausalLM(const ModelConfig &config);
 
     void load(ModelLoader &loader) override;
 
-    static int num_weights(int num_hidden_layers) {
-        return 3 + num_hidden_layers * (std::is_same_v<InternLMModel, InternLM7BModel> ? 9 : 7);
+    static int num_weights(int num_hidden_layers, int hidden_size) {
+        return 3 + num_hidden_layers * (hidden_size == 4096 ? 9 : 7);
     }
 
   private:
     StateDict state_dict() const;
 
   public:
     static constexpr size_t MEM_SIZE = 1280 * MB;
     static constexpr size_t SCRATCH_SIZE = 1280 * MB;
 };
 
-using InternLM7BForCausalLM = InternLMForCausalLM<InternLM7BModel>;
-
-using InternLM20BForCausalLM = InternLMForCausalLM<InternLM20BModel>;
-
 // ===== pipeline =====
 
 class Pipeline {
   public:
-    Pipeline(const std::string &path);
+    Pipeline(const std::string &path, int max_length = -1);
 
     std::vector<int> generate(const std::vector<int> &input_ids, const GenerationConfig &gen_config,
                               BaseStreamer *streamer = nullptr) const;
 
     std::string generate(const std::string &prompt, const GenerationConfig &gen_config,
                          BaseStreamer *streamer = nullptr) const;
```

### Comparing `chatglm-cpp-0.3.1/chatglm_cpp/_C.pyi` & `chatglm_cpp-0.3.2/chatglm_cpp/_C.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 ChatGLM.cpp python binding
 """
 from __future__ import annotations
 import typing
-__all__ = ['Baichuan13BForCausalLM', 'Baichuan7BForCausalLM', 'BaichuanTokenizer', 'BaseModelForCausalLM', 'BaseTokenizer', 'ChatGLM2ForCausalLM', 'ChatGLM2Tokenizer', 'ChatGLM3Tokenizer', 'ChatGLMForCausalLM', 'ChatGLMTokenizer', 'ChatMessage', 'CodeMessage', 'FunctionMessage', 'GenerationConfig', 'InternLM20BForCausalLM', 'InternLM7BForCausalLM', 'InternLMTokenizer', 'ModelConfig', 'ModelType', 'Pipeline', 'ToolCallMessage']
+__all__ = ['Baichuan13BForCausalLM', 'Baichuan7BForCausalLM', 'BaichuanTokenizer', 'BaseModelForCausalLM', 'BaseTokenizer', 'ChatGLM2ForCausalLM', 'ChatGLM2Tokenizer', 'ChatGLM3Tokenizer', 'ChatGLMForCausalLM', 'ChatGLMTokenizer', 'ChatMessage', 'CodeMessage', 'FunctionMessage', 'GenerationConfig', 'InternLMForCausalLM', 'InternLMTokenizer', 'ModelConfig', 'ModelType', 'Pipeline', 'ToolCallMessage']
 class Baichuan13BForCausalLM(BaseModelForCausalLM):
     pass
 class Baichuan7BForCausalLM(BaseModelForCausalLM):
     pass
 class BaichuanTokenizer(BaseTokenizer):
     pass
 class BaseModelForCausalLM:
@@ -70,17 +70,15 @@
     num_threads: int
     repetition_penalty: float
     temperature: float
     top_k: int
     top_p: float
     def __init__(self, max_length: int = 2048, max_new_tokens: int = -1, max_context_length: int = 512, do_sample: bool = True, top_k: int = 0, top_p: float = 0.7, temperature: float = 0.95, repetition_penalty: float = 1.0, num_threads: int = 0) -> None:
         ...
-class InternLM20BForCausalLM(BaseModelForCausalLM):
-    pass
-class InternLM7BForCausalLM(BaseModelForCausalLM):
+class InternLMForCausalLM(BaseModelForCausalLM):
     pass
 class InternLMTokenizer(BaseTokenizer):
     pass
 class ModelConfig:
     @property
     def bos_token_id(self) -> int:
         ...
@@ -172,15 +170,15 @@
     @property
     def name(self) -> str:
         ...
     @property
     def value(self) -> int:
         ...
 class Pipeline:
-    def __init__(self, path: str) -> None:
+    def __init__(self, path: str, max_length: int = -1) -> None:
         ...
     @property
     def model(self) -> BaseModelForCausalLM:
         ...
     @property
     def tokenizer(self) -> BaseTokenizer:
         ...
```

### Comparing `chatglm-cpp-0.3.1/chatglm_cpp/__init__.py` & `chatglm_cpp-0.3.2/chatglm_cpp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Union
 
 import chatglm_cpp._C as _C
 from chatglm_cpp._C import ChatMessage
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 
 @dataclass
 class DeltaMessage:
     role: str
     content: str
     token_ids: List[int]
@@ -23,28 +23,32 @@
         chat_message = ChatMessage(**message)
     else:
         raise TypeError(f"expect message type to be ChatMessage or dict, but got {type(message)}")
     return chat_message
 
 
 class Pipeline(_C.Pipeline):
-    def __init__(self, model_path: str, *, dtype: Optional[str] = None) -> None:
+    def __init__(self, model_path: str, *, max_length: Optional[int] = None, dtype: Optional[str] = None) -> None:
+        kwargs = {}
+        if max_length is not None:
+            kwargs.update(max_length=max_length)
+
         if Path(model_path).is_file():
             # load ggml model
-            super().__init__(str(model_path))
+            super().__init__(str(model_path), **kwargs)
         else:
             # convert hf model to ggml format
             from chatglm_cpp.convert import convert
 
             if dtype is None:
                 dtype = "q4_0"  # default dtype
 
             with tempfile.NamedTemporaryFile("wb") as f:
                 convert(f, model_path, dtype=dtype)
-                super().__init__(f.name)
+                super().__init__(f.name, **kwargs)
 
     def chat(
         self,
         messages: List[ChatMessage],
         *,
         max_length: int = 2048,
         max_new_tokens: int = -1,
```

### Comparing `chatglm-cpp-0.3.1/chatglm_cpp/convert.py` & `chatglm_cpp-0.3.2/chatglm_cpp/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Convert Hugging Face ChatGLM/ChatGLM2 models to GGML format
 """
+
 import argparse
 import platform
 import struct
 import sys
 from enum import Enum
 from pathlib import Path
 from typing import BinaryIO, Optional
@@ -123,16 +124,14 @@
     tensor = torch.cat(
         (scale.half().view(torch.int8), min_vals.half().view(torch.int8), qh[..., None].view(torch.int8), qs), dim=-1
     )
     return tensor
 
 
 def dump_tensor(f, name: str, tensor: torch.Tensor, ggml_type: GGMLType):
-    assert tensor.dtype == torch.float32
-
     # tensor name
     f.write(struct.pack("i", len(name.encode())))
     f.write(name.encode())
 
     # tensor shape & dtype
     f.write(struct.pack("i" * (2 + tensor.ndim), tensor.ndim, *tensor.shape, ggml_type.value))
 
@@ -160,15 +159,17 @@
     tensor.numpy().tofile(f)
 
 
 def dump_state_dict(f, weight_names, state_dict, quantization_bit, ggml_type):
     tensor_info = []
     for name in tqdm(weight_names, desc="Processing model states"):
         tensor = state_dict[name]
-        if tensor.ndim == 2:
+        if name == "past_key_values":
+            tensor_ggml_type = GGMLType.F16
+        elif tensor.ndim == 2:
             # 2d weight: should quantize it if needed
 
             # step 1: de-quantize it back to float32
             if tensor.dtype == torch.int8:
                 assert quantization_bit in [4, 8]
                 scale = state_dict[f"{name}_scale"].float()  # channel-wise scale
 
@@ -186,52 +187,69 @@
         else:
             # 1d weight: convert it to float32
             assert tensor.ndim == 1
             tensor = tensor.float()
             tensor_ggml_type = GGMLType.F32
 
         dump_tensor(f, name, tensor, tensor_ggml_type)
-        tensor_info.append((name, tensor.shape, tensor_ggml_type.name))
+        tensor_info.append((name, tuple(tensor.shape), tensor_ggml_type.name))
 
     print(tabulate(tensor_info, headers=["name", "shape", "dtype"], tablefmt="psql"))
 
 
 class BaseConverter:
     @classmethod
     def convert(cls, f, model, tokenizer, ggml_type):
         f.write(b"ggml")  # magic
-        f.write(struct.pack("ii", cls.MODEL_TYPE.value, 1))  # model type & version
+        f.write(struct.pack("i", cls.MODEL_TYPE.value))  # model type
         cls.dump_config(f, model.config, ggml_type)
         cls.dump_tokenizer(f, tokenizer)
         cls.dump_model(f, model, ggml_type)
 
 
+def get_prefix_cache(prefix_encoder, pre_seq_len, num_layers, num_kv_heads, head_size):
+    prefix_tokens = torch.arange(pre_seq_len, dtype=torch.long)
+    with torch.no_grad():
+        past_key_values = prefix_encoder(prefix_tokens)
+    past_key_values = (
+        past_key_values.to(torch.half)
+        .view(pre_seq_len, num_layers * 2, num_kv_heads, head_size)
+        .permute(1, 2, 0, 3)
+        .contiguous()
+    )
+    return past_key_values
+
+
 class ChatGLMConverter(BaseConverter):
     MODEL_TYPE = ModelType.CHATGLM
 
     @staticmethod
     def dump_config(f, config, ggml_type):
         assert config.position_encoding_2d, "unimplemented: position_encoding_2d should be True"
         assert (
             config.inner_hidden_size == 4 * config.hidden_size
         ), "unimplemented: inner_hidden_size should be 4 times hidden_size"
+
+        config_version = 2
         config_values = [
             ggml_type.value,
             config.vocab_size,
             config.hidden_size,
             config.num_attention_heads,
+            config.num_attention_heads,
             config.num_layers,
             config.inner_hidden_size,
+            config.layernorm_epsilon,
+            config.pre_seq_len if config.pre_seq_len is not None else 0,
+            10000.0,  # rope_theta
             config.max_sequence_length,
-            config.bos_token_id if config.bos_token_id is not None else -1,
             config.eos_token_id if config.eos_token_id is not None else -1,
             config.pad_token_id if config.pad_token_id is not None else -1,
-            config.sep_token_id if config.sep_token_id is not None else -1,
         ]
-        f.write(struct.pack("i" * len(config_values), *config_values))
+        f.write(struct.pack("iiiiiiiififiii", config_version, *config_values))
 
     @staticmethod
     def dump_tokenizer(f, tokenizer):
         serialized_model_proto = tokenizer.sp_tokenizer.text_tokenizer.sp.serialized_model_proto()
         f.write(struct.pack("i", len(serialized_model_proto)))
         f.write(serialized_model_proto)
 
@@ -263,96 +281,115 @@
         ]
         dump_state_dict(f, weight_names, model.state_dict(), model.config.quantization_bit, ggml_type)
 
 
 class ChatGLM2Converter(BaseConverter):
     MODEL_TYPE = ModelType.CHATGLM2
 
-    @staticmethod
-    def dump_config(f, config, ggml_type):
+    @classmethod
+    def dump_config(cls, f, config, ggml_type):
         assert config.add_bias_linear is False, "unimplemented: add_bias_linear must be false"
         assert config.add_qkv_bias is True, "unimplemented: add_qkv_bias must be true"
         assert (
             config.apply_residual_connection_post_layernorm is False
         ), "unimplemented: apply_residual_connection_post_layernorm must be false"
         assert (
             config.kv_channels * config.num_attention_heads == config.hidden_size
         ), "unimplemented: invalid kv_channels"
         assert config.multi_query_attention is True, "unimplemented: multi_query_attention must be true"
         assert config.original_rope is True, "unimplemented: original_rope must be true"
         assert config.post_layer_norm is True, "unimplemented: post_layer_norm must be true"
         assert config.rmsnorm is True, "unimplemented: rmsnorm must be true"
 
+        config_version = 2
         config_values = [
             ggml_type.value,
             config.padded_vocab_size,
             config.hidden_size,
             config.num_attention_heads,
+            config.multi_query_group_num,
             config.num_layers,
             config.ffn_hidden_size,
+            config.layernorm_epsilon,
+            config.pre_seq_len if config.pre_seq_len is not None else 0,
+            10000.0 * getattr(config, "rope_ratio", 1),  # rope_theta
             config.seq_length,
-            config.bos_token_id if config.bos_token_id is not None else -1,
             config.eos_token_id if config.eos_token_id is not None else -1,
             config.pad_token_id if config.pad_token_id is not None else -1,
-            config.sep_token_id if config.sep_token_id is not None else -1,
-            config.multi_query_group_num,
         ]
 
-        f.write(struct.pack("i" * len(config_values), *config_values))
+        f.write(struct.pack("iiiiiiiififiii", config_version, *config_values))
 
     @staticmethod
     def dump_tokenizer(f, tokenizer):
         serialized_model_proto = tokenizer.tokenizer.sp_model.serialized_model_proto()
         f.write(struct.pack("i", len(serialized_model_proto)))
         f.write(serialized_model_proto)
 
     @staticmethod
     def dump_model(f, model, ggml_type):
-        weight_names = ["transformer.embedding.word_embeddings.weight"]
-        for i in range(model.config.num_layers):
+        config = model.config
+
+        state_dict = model.state_dict()
+
+        weight_names = []
+        if config.pre_seq_len is not None and config.pre_seq_len > 0:
+            past_key_values = get_prefix_cache(
+                model.transformer.prefix_encoder,
+                config.pre_seq_len,
+                config.num_layers,
+                config.multi_query_group_num,
+                config.kv_channels,
+            )
+            state_dict["past_key_values"] = past_key_values
+            weight_names.append("past_key_values")
+
+        weight_names.append("transformer.embedding.word_embeddings.weight")
+        for i in range(config.num_layers):
             weight_names += [
                 f"transformer.encoder.layers.{i}.input_layernorm.weight",
                 f"transformer.encoder.layers.{i}.self_attention.query_key_value.weight",
                 f"transformer.encoder.layers.{i}.self_attention.query_key_value.bias",
                 f"transformer.encoder.layers.{i}.self_attention.dense.weight",
                 f"transformer.encoder.layers.{i}.post_attention_layernorm.weight",
                 f"transformer.encoder.layers.{i}.mlp.dense_h_to_4h.weight",
                 f"transformer.encoder.layers.{i}.mlp.dense_4h_to_h.weight",
             ]
         weight_names += [
             "transformer.encoder.final_layernorm.weight",
             "transformer.output_layer.weight",
         ]
-        dump_state_dict(f, weight_names, model.state_dict(), model.config.quantization_bit, ggml_type)
+        dump_state_dict(f, weight_names, state_dict, config.quantization_bit, ggml_type)
 
 
 class ChatGLM3Converter(ChatGLM2Converter):
     MODEL_TYPE = ModelType.CHATGLM3
 
 
 class BaichuanConverter(BaseConverter):
-    @staticmethod
-    def dump_config(f, config, ggml_type):
+    @classmethod
+    def dump_config(cls, f, config, ggml_type):
         assert config.hidden_act == "silu", "unimplemented: hidden_act must be silu"
 
+        config_version = 1
         config_values = [
             ggml_type.value,
             config.vocab_size,
             config.hidden_size,
             config.num_attention_heads,
             config.num_hidden_layers,
             config.intermediate_size,
             config.model_max_length,
             config.bos_token_id if config.bos_token_id is not None else -1,
             config.eos_token_id if config.eos_token_id is not None else -1,
             config.pad_token_id if config.pad_token_id is not None else -1,
             config.sep_token_id if config.sep_token_id is not None else -1,
         ]
 
-        f.write(struct.pack("i" * len(config_values), *config_values))
+        f.write(struct.pack("i" * (1 + len(config_values)), config_version, *config_values))
 
     @staticmethod
     def dump_tokenizer(f, tokenizer):
         serialized_model_proto = tokenizer.sp_model.serialized_model_proto()
         f.write(struct.pack("i", len(serialized_model_proto)))
         f.write(serialized_model_proto)
 
@@ -392,29 +429,30 @@
 class InternLMConverter(BaseConverter):
     MODEL_TYPE = ModelType.INTERNLM
 
     @staticmethod
     def dump_config(f, config, ggml_type):
         assert config.hidden_act == "silu", "unimplemented: hidden_act must be silu"
 
+        config_version = 1
         config_values = [
             ggml_type.value,
             config.vocab_size,
             config.hidden_size,
             config.num_attention_heads,
             config.num_hidden_layers,
             config.intermediate_size,
             config.max_position_embeddings,
             config.bos_token_id if config.bos_token_id is not None else -1,
             config.eos_token_id if config.eos_token_id is not None else -1,
             config.pad_token_id if config.pad_token_id is not None else -1,
             config.sep_token_id if config.sep_token_id is not None else -1,
         ]
 
-        f.write(struct.pack("i" * len(config_values), *config_values))
+        f.write(struct.pack("i" * (1 + len(config_values)), config_version, *config_values))
 
     @staticmethod
     def dump_tokenizer(f, tokenizer):
         serialized_model_proto = tokenizer.sp_model.serialized_model_proto()
         f.write(struct.pack("i", len(serialized_model_proto)))
         f.write(serialized_model_proto)
 
@@ -480,18 +518,21 @@
 
     if lora_model_name_or_path is not None:
         from peft import PeftModel
 
         model = PeftModel.from_pretrained(model, lora_model_name_or_path)
         model = model.merge_and_unload()
 
+    model = model.eval()
+
     if model.config.model_type == "chatglm":
         if hasattr(model.config, "multi_query_attention"):
-            # hack: ChatGLM3 shares the same architecture and model config with ChatGLM2, so I have to check transformers_version to discriminate one from the other
-            if model.config.transformers_version == "4.27.1":
+            # ChatGLM3 shares the same architecture and model config with ChatGLM2, but its tokenizer further supports system prompts,
+            # so we can check system token to discriminate ChatGLM3 from ChatGLM2.
+            if "<|system|>" not in tokenizer.tokenizer.special_tokens:
                 ChatGLM2Converter.convert(f, model, tokenizer, ggml_type)
             else:
                 ChatGLM3Converter.convert(f, model, tokenizer, ggml_type)
         else:
             ChatGLMConverter.convert(f, model, tokenizer, ggml_type)
     elif model.config.model_type == "baichuan":
         if model.config.hidden_size == 5120:
@@ -530,14 +571,14 @@
         type=str,
         choices=["f32", "f16", "q8_0", "q4_0", "q4_1", "q5_0", "q5_1"],
         help="GGML model quantization type",
     )
     args = parser.parse_args()
 
     with open(args.save_path, "wb") as f:
-        convert(f, args.model_name_or_path, dtype=args.type)
+        convert(f, args.model_name_or_path, args.lora_model_name_or_path, dtype=args.type)
 
     print(f"GGML model saved to {args.save_path}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `chatglm-cpp-0.3.1/chatglm_cpp/langchain_api.py` & `chatglm_cpp-0.3.2/chatglm_cpp/langchain_api.py`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/chatglm_cpp/openai_api.py` & `chatglm_cpp-0.3.2/chatglm_cpp/openai_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,17 @@
     temperature: float = Field(default=0.95, ge=0.0, le=2.0)
     top_p: float = Field(default=0.7, ge=0.0, le=1.0)
     stream: bool = False
     max_tokens: int = Field(default=2048, ge=0)
     tools: Optional[List[ChatCompletionTool]] = None
 
     model_config = {
-        "json_schema_extra": {"examples": [{"model": "default-model", "messages": [{"role": "user", "content": "你好"}]}]}
+        "json_schema_extra": {
+            "examples": [{"model": "default-model", "messages": [{"role": "user", "content": "你好"}]}]
+        }
     }
 
 
 class ChatCompletionResponseChoice(BaseModel):
     index: int = 0
     message: ChatMessage
     finish_reason: Literal["stop", "length", "function_call"]
@@ -104,15 +106,18 @@
                     "id": "chatcmpl",
                     "model": "default-model",
                     "object": "chat.completion",
                     "created": 1691166146,
                     "choices": [
                         {
                             "index": 0,
-                            "message": {"role": "assistant", "content": "你好👋！我是人工智能助手 ChatGLM2-6B，很高兴见到你，欢迎问我任何问题。"},
+                            "message": {
+                                "role": "assistant",
+                                "content": "你好👋！我是人工智能助手 ChatGLM2-6B，很高兴见到你，欢迎问我任何问题。",
+                            },
                             "finish_reason": "stop",
                         }
                     ],
                     "usage": {"prompt_tokens": 17, "completion_tokens": 29, "total_tokens": 46},
                 }
             ]
         }
```

### Comparing `chatglm-cpp-0.3.1/chatglm_cpp.egg-info/PKG-INFO` & `chatglm_cpp-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: chatglm-cpp
-Version: 0.3.1
-Summary: C++ implementation of ChatGLM family models and more LLMs
-Author-email: Jiahao Li <liplus17@163.com>
-Maintainer-email: Jiahao Li <liplus17@163.com>
-License: MIT License
-Project-URL: Homepage, https://github.com/li-plus/chatglm.cpp
-Project-URL: Repository, https://github.com/li-plus/chatglm.cpp.git
-Keywords: ChatGLM,ChatGLM2,ChatGLM3,Large Language Model
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Provides-Extra: api
-Requires-Dist: fastapi[all]; extra == "api"
-Requires-Dist: sse-starlette; extra == "api"
-
 # ChatGLM.cpp
 
 [![CMake](https://github.com/li-plus/chatglm.cpp/actions/workflows/cmake.yml/badge.svg)](https://github.com/li-plus/chatglm.cpp/actions/workflows/cmake.yml)
 [![Python package](https://github.com/li-plus/chatglm.cpp/actions/workflows/python-package.yml/badge.svg)](https://github.com/li-plus/chatglm.cpp/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/chatglm-cpp)](https://pypi.org/project/chatglm-cpp/)
 ![Python](https://img.shields.io/pypi/pyversions/chatglm-cpp)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
@@ -37,22 +11,25 @@
 ![demo](docs/demo.gif)
 
 ## Features
 
 Highlights:
 * Pure C++ implementation based on [ggml](https://github.com/ggerganov/ggml), working in the same way as [llama.cpp](https://github.com/ggerganov/llama.cpp).
 * Accelerated memory-efficient CPU inference with int4/int8 quantization, optimized KV cache and parallel computing.
+* P-Tuning v2 and LoRA finetuned models support.
 * Streaming generation with typewriter effect.
 * Python binding, web demo, api servers and more possibilities.
 
 Support Matrix:
 * Hardwares: x86/arm CPU, NVIDIA GPU, Apple Silicon GPU
 * Platforms: Linux, MacOS, Windows
 * Models: [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B), [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B), [ChatGLM3-6B](https://github.com/THUDM/ChatGLM3), [CodeGeeX2](https://github.com/THUDM/CodeGeeX2), [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B), [Baichuan-7B](https://github.com/baichuan-inc/Baichuan-7B), [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B), [Baichuan2](https://github.com/baichuan-inc/Baichuan2), [InternLM](https://github.com/InternLM/InternLM)
 
+**NOTE**: Baichuan & InternLM model series are deprecated in favor of [llama.cpp](https://github.com/ggerganov/llama.cpp).
+
 ## Getting Started
 
 **Preparation**
 
 Clone the ChatGLM.cpp repository into your local machine:
 ```sh
 git clone --recursive https://github.com/li-plus/chatglm.cpp.git && cd chatglm.cpp
@@ -88,15 +65,17 @@
 * `q4_1`: 4-bit integer quantization with fp16 scales and minimum values.
 * `q5_0`: 5-bit integer quantization with fp16 scales.
 * `q5_1`: 5-bit integer quantization with fp16 scales and minimum values.
 * `q8_0`: 8-bit integer quantization with fp16 scales.
 * `f16`: half precision floating point weights without quantization.
 * `f32`: single precision floating point weights without quantization.
 
-For LoRA model, add `-l <lora_model_name_or_path>` flag to merge your LoRA weights into the base model.
+For LoRA models, add `-l <lora_model_name_or_path>` flag to merge your LoRA weights into the base model. For example, run `python3 chatglm_cpp/convert.py -i THUDM/chatglm3-6b -t q4_0 -o chatglm3-ggml-lora.bin -l shibing624/chatglm3-6b-csc-chinese-lora` to merge public LoRA weights from Hugging Face.
+
+For P-Tuning v2 models using the [official finetuning script](https://github.com/THUDM/ChatGLM3/tree/main/finetune_demo), additional weights are automatically detected by `convert.py`. If `past_key_values` is on the output weight list, the P-Tuning checkpoint is successfully converted.
 
 **Build & Run**
 
 Compile the project using CMake:
 ```sh
 cmake -B build
 cmake --build build -j --config Release
@@ -294,15 +273,15 @@
 
 By default, all kernels will be compiled for all possible CUDA architectures and it takes some time. To run on a specific type of device, you may specify `CUDA_ARCHITECTURES` to speed up the nvcc compilation. For example:
 ```sh
 cmake -B build -DGGML_CUBLAS=ON -DCUDA_ARCHITECTURES="80"       # for A100
 cmake -B build -DGGML_CUBLAS=ON -DCUDA_ARCHITECTURES="70;75"    # compatible with both V100 and T4
 ```
 
-To find out the CUDA architecture of your GPU device, see [Matching CUDA arch and CUDA gencode for various NVIDIA architectures](https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/).
+To find out the CUDA architecture of your GPU device, see [Your GPU Compute Capability](https://developer.nvidia.com/cuda-gpus).
 
 **Metal**
 
 MPS (Metal Performance Shaders) allows computation to run on powerful Apple Silicon GPU. Add the CMake flag `-DGGML_METAL=ON` to enable it.
 ```sh
 cmake -B build -DGGML_METAL=ON && cmake --build build -j
 ```
```

### Comparing `chatglm-cpp-0.3.1/chatglm_cpp.egg-info/SOURCES.txt` & `chatglm_cpp-0.3.2/chatglm_cpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/chatglm_pybind.cpp` & `chatglm_cpp-0.3.2/chatglm_pybind.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -151,20 +151,18 @@
 
     py::class_<Baichuan13BForCausalLM, BaseModelForCausalLM>(m, "Baichuan13BForCausalLM");
 
     // ===== InternLM =====
 
     py::class_<InternLMTokenizer, BaseTokenizer>(m, "InternLMTokenizer");
 
-    py::class_<InternLM7BForCausalLM, BaseModelForCausalLM>(m, "InternLM7BForCausalLM");
-
-    py::class_<InternLM20BForCausalLM, BaseModelForCausalLM>(m, "InternLM20BForCausalLM");
+    py::class_<InternLMForCausalLM, BaseModelForCausalLM>(m, "InternLMForCausalLM");
 
     // ===== Pipeline ====
 
     py::class_<Pipeline>(m, "Pipeline")
-        .def(py::init<const std::string &>(), "path"_a)
+        .def(py::init<const std::string &, int>(), "path"_a, "max_length"_a = -1)
         .def_property_readonly("model", [](const Pipeline &self) { return self.model.get(); })
         .def_property_readonly("tokenizer", [](const Pipeline &self) { return self.tokenizer.get(); });
 }
 
 } // namespace chatglm
```

### Comparing `chatglm-cpp-0.3.1/chatglm_test.cpp` & `chatglm_cpp-0.3.2/chatglm_test.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -18,19 +18,30 @@
 }
 
 static inline void expect_all_close(ggml_tensor *a, ggml_tensor *b, float atol = 1e-5f, float rtol = 0.f) {
     ASSERT_EQ(a->type, b->type);
     ASSERT_EQ(a->type, GGML_TYPE_F32);
     ASSERT_EQ(ggml_nelements(a), ggml_nelements(b));
     int64_t numel = ggml_nelements(a);
+    float max_abs_diff = 0.f;
+    int64_t num_mismatch = 0;
     for (int64_t i = 0; i < numel; i++) {
         float ai = ((float *)a->data)[i];
         float bi = ((float *)b->data)[i];
-        EXPECT_LT(std::abs(ai - bi), atol + rtol * std::abs(bi)) << "diff " << ai << " vs " << bi;
+        float abs_diff = std::abs(ai - bi);
+        max_abs_diff = std::max(max_abs_diff, abs_diff);
+        if (abs_diff >= atol + rtol * std::abs(bi)) {
+            num_mismatch++;
+        }
     }
+    EXPECT_EQ(num_mismatch, 0) << "Tensors are not close!\n\n"
+                               << "Mismatched elements: " << num_mismatch << " / " << numel << " ("
+                               << num_mismatch * 100 / numel << "%)\n"
+                               << "Greatest absolute difference: " << max_abs_diff << " (up to " << std::scientific
+                               << atol << " allowed)\n";
 }
 
 static inline char *read_tensor_data(char *ptr, ggml_tensor *tensor) {
     memcpy(tensor->data, ptr, ggml_nbytes(tensor));
     return ptr + ggml_nbytes(tensor);
 }
 
@@ -273,69 +284,79 @@
 #endif
     }
 
     float perf_cpu_graph_compute() { return _perf_graph_compute_impl<true>(); }
     float perf_device_graph_compute() { return _perf_graph_compute_impl<false>(); }
 
     template <typename Model>
-    void test_model(const Model &model, const ModelConfig &config, const fs::path &data_path, int seq_len,
+    void test_model(Model &model, const ModelConfig &config, const fs::path &data_path, int seq_len,
                     const std::vector<ggml_tensor *> &all_weights) {
         ASSERT_EQ(config.num_hidden_layers, 1);
 
         MappedFile mapped_file(data_path.string());
         char *ptr = mapped_file.data;
 
-        tensor_to_device(model.layers[0].attention.k_cache);
-        tensor_to_device(model.layers[0].attention.v_cache);
-
         ggml_tensor *x1 = ggml_new_tensor_1d(ctx.ctx_b.get(), GGML_TYPE_I32, seq_len);
         ggml_tensor *ref_y1 = ggml_new_tensor_2d(ctx.ctx_b.get(), GGML_TYPE_F32, config.hidden_size, seq_len);
         ggml_tensor *x2 = ggml_new_tensor_1d(ctx.ctx_b.get(), GGML_TYPE_I32, 1);
         ggml_tensor *ref_y2 = ggml_new_tensor_1d(ctx.ctx_b.get(), GGML_TYPE_F32, config.hidden_size);
         ggml_tensor *x3 = ggml_new_tensor_1d(ctx.ctx_b.get(), GGML_TYPE_I32, 1);
         ggml_tensor *ref_y3 = ggml_new_tensor_1d(ctx.ctx_b.get(), GGML_TYPE_F32, config.hidden_size);
 
         std::vector<ggml_tensor *> all_tensors = all_weights;
         all_tensors.insert(all_tensors.end(), {x1, ref_y1, x2, ref_y2, x3, ref_y3});
 
         std::vector<ggml_tensor *> cpu_tensors{model.word_embeddings.weight, x1, x2, x3};
 
+        if (config.num_virtual_tokens > 0) {
+            const int head_size = config.hidden_size / config.num_attention_heads;
+            ggml_tensor *past_key_values =
+                ggml_new_tensor_4d(ctx.ctx_b.get(), GGML_TYPE_F16, head_size, config.num_virtual_tokens,
+                                   config.num_kv_heads, config.num_hidden_layers * 2); // [l * 2, #h, v, d]
+            ptr = read_tensor_data(ptr, past_key_values);
+            model.load_prefix_cache(config, past_key_values);
+        }
+
+        tensor_to_device(model.layers[0].attention.k_cache);
+        tensor_to_device(model.layers[0].attention.v_cache);
+
         for (auto tensor : all_tensors) {
             ptr = read_tensor_data(ptr, tensor);
             if (std::find(cpu_tensors.begin(), cpu_tensors.end(), tensor) == cpu_tensors.end()) {
                 tensor_to_device(tensor);
             }
         }
 
         ASSERT_EQ(ptr, mapped_file.data + mapped_file.size);
 
         // self attention
         {
+            reset_cgraph();
             ggml_tensor *out_y1 = model.forward(&ctx, x1, 0, seq_len);
             EXPECT_EQ(out_y1->backend, ref_y1->backend);
             out_y1->backend = GGML_BACKEND_CPU;
             ggml_build_forward_expand(&ctx.gf, out_y1);
             device_graph_compute(1);
 
             expect_all_close(ref_y1, out_y1, 5e-4);
         }
 
         // cross attention
-        reset_cgraph();
         {
+            reset_cgraph();
             ggml_tensor *out_y2 = model.forward(&ctx, x2, seq_len, seq_len);
             EXPECT_EQ(out_y2->backend, ref_y2->backend);
             out_y2->backend = GGML_BACKEND_CPU;
             ggml_build_forward_expand(&ctx.gf, out_y2);
             device_graph_compute(1);
 
             expect_all_close(ref_y2, out_y2, 5e-4);
         }
-        reset_cgraph();
         {
+            reset_cgraph();
             ggml_tensor *out_y3 = model.forward(&ctx, x3, seq_len + 1, seq_len);
             EXPECT_EQ(out_y3->backend, ref_y3->backend);
             out_y3->backend = GGML_BACKEND_CPU;
             ggml_build_forward_expand(&ctx.gf, out_y3);
             device_graph_compute(1);
 
             expect_all_close(ref_y3, out_y3, 5e-4);
@@ -577,23 +598,23 @@
         tensor_to_cpu(tensor);
     }
 }
 
 TEST_F(ChatGLMTest, GLMModel) {
     fs::path data_path = fs::path(__FILE__).parent_path() / "tests/data/glm_model.data";
 
-    ModelConfig config;
-    config.hidden_size = 32;
-    config.num_attention_heads = 8;
-    config.num_kv_heads = 2;
-    config.intermediate_size = config.hidden_size * 4;
-    config.num_hidden_layers = 1;
-    config.vocab_size = 5;
-    config.max_length = 8;
-    config.norm_eps = 1e-5;
+    ModelConfig config(
+        ModelType::CHATGLM, GGML_TYPE_F32, /*vocab_size=*/5, /*hidden_size=*/32, /*num_attention_heads=*/8,
+        /*num_kv_heads=*/8, /*num_hidden_layers=*/1, /*intermediate_size=*/128, /*norm_eps=*/1e-5f,
+        /*hidden_act=*/ActivationType::GELU, /*use_qkv_bias=*/true, /*use_dense_bias=*/true,
+        /*interleaved_qkv=*/true, /*use_alibi=*/false, /*rope_type=*/RopeType::CHATGLM, /*rope_theta=*/10000.f,
+        /*rope_dim_scale=*/-1,
+        /*attn_mask_type=*/AttentionMaskType::CHATGLM, /*num_virtual_tokens=*/0,
+        /*max_length=*/8, /*bos_token_id=*/-1, /*eos_token_id=*/-1, /*pad_token_id=*/-1, /*sep_token_id=*/-1,
+        /*extra_eos_token_ids=*/{});
 
     constexpr int seq_len = 3;
 
     ChatGLMModel model(&ctx, config);
 
     std::vector<ggml_tensor *> all_weights{model.word_embeddings.weight,
                                            model.layers[0].input_layernorm.weight,
@@ -610,194 +631,128 @@
                                            model.layers[0].mlp.dense_4h_to_h.bias,
                                            model.final_layernorm.weight,
                                            model.final_layernorm.bias};
 
     test_model(model, config, data_path, seq_len, all_weights);
 }
 
-// TEST_F(ChatGLMTest, BenchmarkGLMBlock) {
-//     constexpr int hidden_size = 4096;
-//     constexpr int num_attention_heads = 32;
-//     constexpr int num_hidden_layers = 28;
-//     constexpr int max_length = 2048;
-//     constexpr int seq_len = 64;
-
-//     ggml_type dtypes[]{GGML_TYPE_F32, GGML_TYPE_F16, GGML_TYPE_Q8_0, GGML_TYPE_Q4_0};
-//     for (const auto dtype : dtypes) {
-//         SetUp();
-
-//         ctx.dtype = dtype;
-//         GLMBlock model(&ctx, hidden_size, num_attention_heads, num_hidden_layers, max_length);
-
-//         ggml_tensor *self_attn_x = ggml_new_tensor_2d(ctx.ctx_b.get(), GGML_TYPE_F32, hidden_size, seq_len);
-//         ggml_tensor *cross_attn_x = ggml_new_tensor_1d(ctx.ctx_b.get(), GGML_TYPE_F32, hidden_size);
-
-//         std::vector<ggml_tensor *> all_tensors{model.input_layernorm.weight,
-//                                                model.input_layernorm.bias,
-//                                                model.attention.query_key_value.weight,
-//                                                model.attention.query_key_value.bias,
-//                                                model.attention.dense.weight,
-//                                                model.attention.dense.bias,
-//                                                model.post_attention_layernorm.weight,
-//                                                model.post_attention_layernorm.bias,
-//                                                model.mlp.dense_h_to_4h.weight,
-//                                                model.mlp.dense_h_to_4h.bias,
-//                                                model.mlp.dense_4h_to_h.weight,
-//                                                model.mlp.dense_4h_to_h.bias,
-//                                                self_attn_x,
-//                                                cross_attn_x};
-
-//         for (auto tensor : all_tensors) {
-//             random_fill(tensor);
-//             tensor_to_device(tensor);
-//         }
-
-//         // self attention
-//         reset_cgraph();
-//         {
-//             ggml_tensor *self_attn_y = model.forward(&ctx, self_attn_x, 0, seq_len);
-//             ggml_build_forward_expand(&ctx.gf, self_attn_y);
-//             std::cout << "[Benchmark] GLMBlock " << ggml_type_name(dtype)
-//                       << " self attn time: " << perf_cpu_graph_compute() << " ms\n";
-//         }
-
-//         // cross attention
-//         reset_cgraph();
-//         {
-//             ggml_tensor *cross_attn_y = model.forward(&ctx, cross_attn_x, seq_len, seq_len);
-//             ggml_build_forward_expand(&ctx.gf, cross_attn_y);
-//             std::cout << "[Benchmark] GLMBlock " << ggml_type_name(dtype)
-//                       << " cross attn time: " << perf_device_graph_compute() << " ms\n";
-//         }
-
-//         for (auto tensor : all_tensors) {
-//             tensor_to_cpu(tensor);
-//         }
-//     }
-// }
+TEST_F(ChatGLMTest, GLMPTuningV2Model) {
+    fs::path data_path = fs::path(__FILE__).parent_path() / "tests/data/glm_ptuning_v2_model.data";
+
+    ModelConfig config(
+        ModelType::CHATGLM, GGML_TYPE_F32, /*vocab_size=*/5, /*hidden_size=*/32, /*num_attention_heads=*/8,
+        /*num_kv_heads=*/8, /*num_hidden_layers=*/1, /*intermediate_size=*/128, /*norm_eps=*/1e-5f,
+        /*hidden_act=*/ActivationType::GELU, /*use_qkv_bias=*/true, /*use_dense_bias=*/true,
+        /*interleaved_qkv=*/true, /*use_alibi=*/false, /*rope_type=*/RopeType::CHATGLM, /*rope_theta=*/10000.f,
+        /*rope_dim_scale=*/-1,
+        /*attn_mask_type=*/AttentionMaskType::CHATGLM, /*num_virtual_tokens=*/5,
+        /*max_length=*/8, /*bos_token_id=*/-1, /*eos_token_id=*/-1, /*pad_token_id=*/-1, /*sep_token_id=*/-1,
+        /*extra_eos_token_ids=*/{});
+
+    constexpr int seq_len = 3;
+
+    ChatGLMModel model(&ctx, config);
+
+    std::vector<ggml_tensor *> all_weights{model.word_embeddings.weight,
+                                           model.layers[0].input_layernorm.weight,
+                                           model.layers[0].input_layernorm.bias,
+                                           model.layers[0].attention.query_key_value.weight,
+                                           model.layers[0].attention.query_key_value.bias,
+                                           model.layers[0].attention.dense.weight,
+                                           model.layers[0].attention.dense.bias,
+                                           model.layers[0].post_attention_layernorm.weight,
+                                           model.layers[0].post_attention_layernorm.bias,
+                                           model.layers[0].mlp.dense_h_to_4h.weight,
+                                           model.layers[0].mlp.dense_h_to_4h.bias,
+                                           model.layers[0].mlp.dense_4h_to_h.weight,
+                                           model.layers[0].mlp.dense_4h_to_h.bias,
+                                           model.final_layernorm.weight,
+                                           model.final_layernorm.bias};
+
+    test_model(model, config, data_path, seq_len, all_weights);
+}
 
 TEST_F(ChatGLMTest, GLM2Model) {
     fs::path data_path = fs::path(__FILE__).parent_path() / "tests/data/glm2_model.data";
 
-    ModelConfig config;
-    config.vocab_size = 5;
-    config.hidden_size = 32;
-    config.num_attention_heads = 8;
-    config.num_kv_heads = 2;
-    config.num_hidden_layers = 1;
-    config.intermediate_size = 48;
-    config.norm_eps = 1e-5;
-    config.max_length = 8;
+    ModelConfig config(
+        ModelType::CHATGLM2, GGML_TYPE_F32, /*vocab_size=*/5, /*hidden_size=*/32, /*num_attention_heads=*/8,
+        /*num_kv_heads=*/2, /*num_hidden_layers=*/1, /*intermediate_size=*/48, /*norm_eps=*/1e-5f,
+        /*hidden_act=*/ActivationType::SILU, /*use_qkv_bias=*/true, /*use_dense_bias=*/false,
+        /*interleaved_qkv=*/false, /*use_alibi=*/false, /*rope_type=*/RopeType::GPTJ, /*rope_theta=*/10000.f,
+        /*rope_dim_scale=*/2,
+        /*attn_mask_type=*/AttentionMaskType::CAUSAL, /*num_virtual_tokens=*/0,
+        /*max_length=*/8, /*bos_token_id=*/-1, /*eos_token_id=*/-1, /*pad_token_id=*/-1, /*sep_token_id=*/-1,
+        /*extra_eos_token_ids=*/{});
 
     constexpr int seq_len = 3;
 
     ChatGLM2Model model(&ctx, config);
 
-    tensor_to_device(model.layers[0].attention.k_cache);
-    tensor_to_device(model.layers[0].attention.v_cache);
-
     std::vector<ggml_tensor *> all_weights{model.word_embeddings.weight,
                                            model.layers[0].input_layernorm.weight,
                                            model.layers[0].attention.query_key_value.weight,
                                            model.layers[0].attention.query_key_value.bias,
                                            model.layers[0].attention.dense.weight,
                                            model.layers[0].post_attention_layernorm.weight,
                                            model.layers[0].mlp.gate_proj.weight,
                                            model.layers[0].mlp.up_proj.weight,
                                            model.layers[0].mlp.down_proj.weight,
                                            model.final_layernorm.weight};
 
     test_model(model, config, data_path, seq_len, all_weights);
 }
 
-// TEST_F(ChatGLMTest, BenchmarkGLM2Block) {
-//     constexpr int seq_len = 64;
-//     constexpr int hidden_size = 4096;
-//     constexpr int num_attention_heads = 32;
-//     constexpr int num_kv_heads = 2;
-//     constexpr int ffn_hidden_size = 13696;
-//     constexpr int max_length = 2048;
-
-// #ifdef GGML_USE_METAL
-//     ggml_type dtypes[]{GGML_TYPE_F16, GGML_TYPE_Q8_0, GGML_TYPE_Q4_1, GGML_TYPE_Q4_0};
-// #else
-//     ggml_type dtypes[]{GGML_TYPE_F32, GGML_TYPE_F16, GGML_TYPE_Q8_0, GGML_TYPE_Q4_0};
-// #endif
-//     for (const auto dtype : dtypes) {
-//         SetUp();
-
-//         ctx.dtype = dtype;
-//         GLM2Block model(&ctx, hidden_size, num_attention_heads, num_kv_heads, ffn_hidden_size, max_length, 1e-5);
-//         tensor_to_device(model.attention.k_cache);
-//         tensor_to_device(model.attention.v_cache);
-
-//         ggml_tensor *self_attn_x = ggml_new_tensor_2d(ctx.ctx_b.get(), GGML_TYPE_F32, hidden_size, seq_len);
-//         ggml_tensor *cross_attn_x = ggml_new_tensor_1d(ctx.ctx_b.get(), GGML_TYPE_F32, hidden_size);
-
-//         std::vector<ggml_tensor *> all_tensors{model.input_layernorm.weight,
-//                                                model.attention.query_key_value.weight,
-//                                                model.attention.query_key_value.bias,
-//                                                model.attention.dense.weight,
-//                                                model.post_attention_layernorm.weight,
-//                                                model.mlp.gate_proj.weight,
-//                                                model.mlp.up_proj.weight,
-//                                                model.mlp.down_proj.weight,
-//                                                self_attn_x,
-//                                                cross_attn_x};
-
-//         for (auto tensor : all_tensors) {
-//             random_fill(tensor);
-//             tensor_to_device(tensor);
-//         }
-
-//         // self attention
-//         reset_cgraph();
-//         {
-//             ggml_tensor *self_attn_y = model.forward(&ctx, self_attn_x, 0, seq_len);
-//             ggml_build_forward_expand(&ctx.gf, self_attn_y);
-//             std::cout << "[Benchmark] GLM2Block " << ggml_type_name(dtype)
-//                       << " self attn time: " << perf_device_graph_compute() << " ms\n";
-//         }
-
-//         // cross attention
-//         reset_cgraph();
-//         {
-//             ggml_tensor *cross_attn_y = model.forward(&ctx, cross_attn_x, seq_len, seq_len);
-//             ggml_build_forward_expand(&ctx.gf, cross_attn_y);
-//             std::cout << "[Benchmark] GLM2Block " << ggml_type_name(dtype)
-//                       << " cross attn time: " << perf_device_graph_compute() << " ms\n";
-//         }
-
-//         for (auto tensor : all_tensors) {
-//             tensor_to_cpu(tensor);
-//         }
-//         tensor_to_cpu(model.attention.k_cache);
-//         tensor_to_cpu(model.attention.v_cache);
-//     }
-// }
-
 TEST_F(ChatGLMTest, GLM3Model) {
     fs::path data_path = fs::path(__FILE__).parent_path() / "tests/data/glm3_model.data";
 
-    ModelConfig config;
-    config.vocab_size = 5;
-    config.hidden_size = 32;
-    config.num_attention_heads = 8;
-    config.num_kv_heads = 2;
-    config.num_hidden_layers = 1;
-    config.intermediate_size = 48;
-    config.norm_eps = 1e-5;
-    config.max_length = 8;
+    ModelConfig config(
+        ModelType::CHATGLM3, GGML_TYPE_F32, /*vocab_size=*/5, /*hidden_size=*/32, /*num_attention_heads=*/8,
+        /*num_kv_heads=*/2, /*num_hidden_layers=*/1, /*intermediate_size=*/48, /*norm_eps=*/1e-5f,
+        /*hidden_act=*/ActivationType::SILU, /*use_qkv_bias=*/true, /*use_dense_bias=*/false,
+        /*interleaved_qkv=*/false, /*use_alibi=*/false, /*rope_type=*/RopeType::GPTJ, /*rope_theta=*/10000.f,
+        /*rope_dim_scale=*/2,
+        /*attn_mask_type=*/AttentionMaskType::CAUSAL, /*num_virtual_tokens=*/0,
+        /*max_length=*/8, /*bos_token_id=*/-1, /*eos_token_id=*/-1, /*pad_token_id=*/-1, /*sep_token_id=*/-1,
+        /*extra_eos_token_ids=*/{});
 
     constexpr int seq_len = 3;
 
     ChatGLM3Model model(&ctx, config);
 
-    tensor_to_device(model.layers[0].attention.k_cache);
-    tensor_to_device(model.layers[0].attention.v_cache);
+    std::vector<ggml_tensor *> all_weights{model.word_embeddings.weight,
+                                           model.layers[0].input_layernorm.weight,
+                                           model.layers[0].attention.query_key_value.weight,
+                                           model.layers[0].attention.query_key_value.bias,
+                                           model.layers[0].attention.dense.weight,
+                                           model.layers[0].post_attention_layernorm.weight,
+                                           model.layers[0].mlp.gate_proj.weight,
+                                           model.layers[0].mlp.up_proj.weight,
+                                           model.layers[0].mlp.down_proj.weight,
+                                           model.final_layernorm.weight};
+
+    test_model(model, config, data_path, seq_len, all_weights);
+}
+
+TEST_F(ChatGLMTest, GLM3PTuningV2Model) {
+    fs::path data_path = fs::path(__FILE__).parent_path() / "tests/data/glm3_ptuning_v2_model.data";
+
+    ModelConfig config(
+        ModelType::CHATGLM3, GGML_TYPE_F32, /*vocab_size=*/5, /*hidden_size=*/32, /*num_attention_heads=*/8,
+        /*num_kv_heads=*/2, /*num_hidden_layers=*/1, /*intermediate_size=*/48, /*norm_eps=*/1e-5f,
+        /*hidden_act=*/ActivationType::SILU, /*use_qkv_bias=*/true, /*use_dense_bias=*/false,
+        /*interleaved_qkv=*/false, /*use_alibi=*/false, /*rope_type=*/RopeType::GPTJ, /*rope_theta=*/10000.f,
+        /*rope_dim_scale=*/2,
+        /*attn_mask_type=*/AttentionMaskType::CAUSAL, /*num_virtual_tokens=*/5,
+        /*max_length=*/8, /*bos_token_id=*/-1, /*eos_token_id=*/-1, /*pad_token_id=*/-1, /*sep_token_id=*/-1,
+        /*extra_eos_token_ids=*/{});
+
+    constexpr int seq_len = 3;
+
+    ChatGLM3Model model(&ctx, config);
 
     std::vector<ggml_tensor *> all_weights{model.word_embeddings.weight,
                                            model.layers[0].input_layernorm.weight,
                                            model.layers[0].attention.query_key_value.weight,
                                            model.layers[0].attention.query_key_value.bias,
                                            model.layers[0].attention.dense.weight,
                                            model.layers[0].post_attention_layernorm.weight,
@@ -808,23 +763,23 @@
 
     test_model(model, config, data_path, seq_len, all_weights);
 }
 
 TEST_F(ChatGLMTest, Baichuan7BModel) {
     fs::path data_path = fs::path(__FILE__).parent_path() / "tests/data/baichuan7b_model.data";
 
-    ModelConfig config;
-    config.hidden_size = 32;
-    config.num_attention_heads = 8;
-    config.num_kv_heads = config.num_attention_heads;
-    config.intermediate_size = config.hidden_size * 3;
-    config.num_hidden_layers = 1;
-    config.vocab_size = 5;
-    config.max_length = 8;
-    config.norm_eps = 1e-6;
+    ModelConfig config(
+        ModelType::BAICHUAN7B, GGML_TYPE_F32, /*vocab_size=*/5, /*hidden_size=*/32, /*num_attention_heads=*/8,
+        /*num_kv_heads=*/8, /*num_hidden_layers=*/1, /*intermediate_size=*/32 * 3, /*norm_eps=*/1e-6f,
+        /*hidden_act=*/ActivationType::SILU, /*use_qkv_bias=*/false, /*use_dense_bias=*/false,
+        /*interleaved_qkv=*/false, /*use_alibi=*/false, /*rope_type=*/RopeType::NEOX, /*rope_theta=*/10000.f,
+        /*rope_dim_scale=*/1,
+        /*attn_mask_type=*/AttentionMaskType::CAUSAL, /*num_virtual_tokens=*/0,
+        /*max_length=*/8, /*bos_token_id=*/-1, /*eos_token_id=*/-1, /*pad_token_id=*/-1, /*sep_token_id=*/-1,
+        /*extra_eos_token_ids=*/{});
 
     constexpr int seq_len = 3;
 
     Baichuan7BModel model(&ctx, config);
 
     std::vector<ggml_tensor *> all_weights{model.word_embeddings.weight,
                                            model.layers[0].input_layernorm.weight,
@@ -838,23 +793,23 @@
 
     test_model(model, config, data_path, seq_len, all_weights);
 }
 
 TEST_F(ChatGLMTest, Baichuan13BModel) {
     fs::path data_path = fs::path(__FILE__).parent_path() / "tests/data/baichuan13b_model.data";
 
-    ModelConfig config;
-    config.hidden_size = 32;
-    config.num_attention_heads = 8;
-    config.num_kv_heads = config.num_attention_heads;
-    config.intermediate_size = config.hidden_size * 3;
-    config.num_hidden_layers = 1;
-    config.vocab_size = 5;
-    config.max_length = 8;
-    config.norm_eps = 1e-6;
+    ModelConfig config(
+        ModelType::BAICHUAN13B, GGML_TYPE_F32, /*vocab_size=*/5, /*hidden_size=*/32, /*num_attention_heads=*/8,
+        /*num_kv_heads=*/8, /*num_hidden_layers=*/1, /*intermediate_size=*/32 * 3, /*norm_eps=*/1e-6f,
+        /*hidden_act=*/ActivationType::SILU, /*use_qkv_bias=*/false, /*use_dense_bias=*/false,
+        /*interleaved_qkv=*/false, /*use_alibi=*/true, /*rope_type=*/RopeType::DISABLED, /*rope_theta=*/10000.f,
+        /*rope_dim_scale=*/-1,
+        /*attn_mask_type=*/AttentionMaskType::CAUSAL, /*num_virtual_tokens=*/0,
+        /*max_length=*/8, /*bos_token_id=*/-1, /*eos_token_id=*/-1, /*pad_token_id=*/-1, /*sep_token_id=*/-1,
+        /*extra_eos_token_ids=*/{});
 
     constexpr int seq_len = 3;
 
     Baichuan13BModel model(&ctx, config);
 
     std::vector<ggml_tensor *> all_weights{model.word_embeddings.weight,
                                            model.layers[0].input_layernorm.weight,
@@ -868,27 +823,27 @@
 
     test_model(model, config, data_path, seq_len, all_weights);
 }
 
 TEST_F(ChatGLMTest, InternLMModel) {
     fs::path data_path = fs::path(__FILE__).parent_path() / "tests/data/internlm_model.data";
 
-    ModelConfig config;
-    config.hidden_size = 32;
-    config.num_attention_heads = 8;
-    config.num_kv_heads = config.num_attention_heads;
-    config.intermediate_size = config.hidden_size * 3;
-    config.num_hidden_layers = 1;
-    config.vocab_size = 5;
-    config.max_length = 8;
-    config.norm_eps = 1e-6;
+    ModelConfig config(
+        ModelType::INTERNLM, GGML_TYPE_F32, /*vocab_size=*/5, /*hidden_size=*/32, /*num_attention_heads=*/8,
+        /*num_kv_heads=*/8, /*num_hidden_layers=*/1, /*intermediate_size=*/32 * 3, /*norm_eps=*/1e-6f,
+        /*hidden_act=*/ActivationType::SILU, /*use_qkv_bias=*/true, /*use_dense_bias=*/true,
+        /*interleaved_qkv=*/false, /*use_alibi=*/false, /*rope_type=*/RopeType::NEOX, /*rope_theta=*/10000.f,
+        /*rope_dim_scale=*/1,
+        /*attn_mask_type=*/AttentionMaskType::CAUSAL, /*num_virtual_tokens=*/0,
+        /*max_length=*/8, /*bos_token_id=*/-1, /*eos_token_id=*/-1, /*pad_token_id=*/-1, /*sep_token_id=*/-1,
+        /*extra_eos_token_ids=*/{});
 
     constexpr int seq_len = 3;
 
-    InternLM7BModel model(&ctx, config);
+    InternLMModel model(&ctx, config);
 
     std::vector<ggml_tensor *> all_weights{model.word_embeddings.weight,
                                            model.layers[0].input_layernorm.weight,
                                            model.layers[0].attention.query_key_value.weight,
                                            model.layers[0].attention.query_key_value.bias,
                                            model.layers[0].attention.dense.weight,
                                            model.layers[0].attention.dense.bias,
@@ -1257,50 +1212,54 @@
                                       "```");
             messages.emplace_back(std::move(output));
         }
         messages.emplace_back(ChatMessage::ROLE_OBSERVATION, "22");
         {
             ChatMessage output = pipeline.chat(messages, gen_config);
             EXPECT_EQ(output.role, ChatMessage::ROLE_ASSISTANT);
-            EXPECT_EQ(output.content, "根据您的要求，我使用随机数生成器API生成了一个在0和100之间的随机数，结果为22。");
+            EXPECT_EQ(output.content,
+                      "根据API调用结果，我为您生成了一个随机数，随机数的范围在0到100之间。这个随机数是22。");
         }
     }
 
     // code interpreter
     {
         GenerationConfig gen_config;
         gen_config.do_sample = false;
         std::vector<ChatMessage> messages{
             {ChatMessage::ROLE_SYSTEM, system_ci},
             {ChatMessage::ROLE_USER, "列出100以内的所有质数"},
         };
         {
             ChatMessage output = pipeline.chat(messages, gen_config);
             EXPECT_EQ(output.role, ChatMessage::ROLE_ASSISTANT);
-            EXPECT_EQ(output.content, "好的，我会为您列出100以内的所有质数。\n\n质数是指只能被1和它本身整除的大于1"
-                                      "的整数。例如，2、3、5、7等都是质数。\n\n让我们开始吧！");
+            EXPECT_EQ(output.content, R"(好的，我会为您列出100以内的所有质数。
+
+质数是指只能被1和它本身整除的正整数。例如，2、3、5、7等都是质数。
+
+让我们开始吧！)");
             EXPECT_EQ(output.tool_calls.front().code.input, R"(```python
+# Function to check if a number is prime
 def is_prime(n):
-    """Check if a number is prime."""
     if n <= 1:
         return False
     if n <= 3:
         return True
     if n % 2 == 0 or n % 3 == 0:
         return False
     i = 5
     while i * i <= n:
         if n % i == 0 or n % (i + 2) == 0:
             return False
         i += 6
     return True
 
 # Get all prime numbers up to 100
-primes_upto_100 = [i for i in range(2, 101) if is_prime(i)]
-primes_upto_100
+primes_up_to_100 = [i for i in range(2, 101) if is_prime(i)]
+primes_up_to_100
 ```)");
             messages.emplace_back(std::move(output));
         }
         messages.emplace_back(
             ChatMessage::ROLE_OBSERVATION,
             "[2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97]");
         {
@@ -1507,15 +1466,15 @@
 
 TEST(Pipeline, InternLM) {
     fs::path model_path = fs::path(__FILE__).parent_path() / "internlm-chat-7b-ggml.bin";
     if (!fs::exists(model_path)) {
         GTEST_SKIP() << "Skipping InternLM e2e test (ggml model not found)";
     }
     Pipeline pipeline(model_path.string());
-    EXPECT_TRUE(dynamic_cast<InternLM7BForCausalLM *>(pipeline.model.get()));
+    EXPECT_TRUE(dynamic_cast<InternLMForCausalLM *>(pipeline.model.get()));
 
     // tokenizer
     {
         std::vector<TokenizerTestCase> cases{
             {"你好", {1, 76379}},
             {"<|User|>:你好<eoh>\n<|Bot|>:你好，有什么我可以帮助你的吗？<eoa>\n<|User|>:晚上睡不着应该怎么办<eoh>\n<|"
              "Bot|>:",
```

### Comparing `chatglm-cpp-0.3.1/docs/README.md` & `chatglm_cpp-0.3.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/main.cpp` & `chatglm_cpp-0.3.2/main.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         std::cout << message.tool_calls.front().code.input << "\n";
     }
 }
 
 static void chat(Args &args) {
     ggml_time_init();
     int64_t start_load_us = ggml_time_us();
-    chatglm::Pipeline pipeline(args.model_path);
+    chatglm::Pipeline pipeline(args.model_path, args.max_length);
     int64_t end_load_us = ggml_time_us();
 
     std::string model_name = pipeline.model->config.model_type_name();
 
     auto text_streamer = std::make_shared<chatglm::TextStreamer>(std::cout, pipeline.tokenizer.get());
     auto perf_streamer = std::make_shared<chatglm::PerfStreamer>();
     std::vector<std::shared_ptr<chatglm::BaseStreamer>> streamers{perf_streamer};
```

### Comparing `chatglm-cpp-0.3.1/pyproject.toml` & `chatglm_cpp-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/setup.py` & `chatglm_cpp-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/tests/test_chatglm_cpp.py` & `chatglm_cpp-0.3.2/tests/test_chatglm_cpp.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,26 +32,51 @@
     if model_path == CHATGLM3_MODEL_PATH:
         # hack for ChatGLM3
         stream_output = stream_output.strip()
     assert stream_output == target
 
 
 @pytest.mark.skipif(not CHATGLM_MODEL_PATH.exists(), reason="model file not found")
+def test_pipeline_options():
+    # check max_length option
+    pipeline = chatglm_cpp.Pipeline(CHATGLM_MODEL_PATH)
+    assert pipeline.model.config.max_length == 2048
+    pipeline = chatglm_cpp.Pipeline(CHATGLM_MODEL_PATH, max_length=234)
+    assert pipeline.model.config.max_length == 234
+
+    # check if resources are properly released
+    for _ in range(100):
+        chatglm_cpp.Pipeline(CHATGLM_MODEL_PATH)
+
+
+@pytest.mark.skipif(not CHATGLM_MODEL_PATH.exists(), reason="model file not found")
 def test_chatglm_pipeline():
-    check_pipeline(model_path=CHATGLM_MODEL_PATH, prompt="你好", target="你好👋！我是人工智能助手 ChatGLM-6B，很高兴见到你，欢迎问我任何问题。")
+    check_pipeline(
+        model_path=CHATGLM_MODEL_PATH,
+        prompt="你好",
+        target="你好👋！我是人工智能助手 ChatGLM-6B，很高兴见到你，欢迎问我任何问题。",
+    )
 
 
 @pytest.mark.skipif(not CHATGLM2_MODEL_PATH.exists(), reason="model file not found")
 def test_chatglm2_pipeline():
-    check_pipeline(model_path=CHATGLM2_MODEL_PATH, prompt="你好", target="你好👋！我是人工智能助手 ChatGLM2-6B，很高兴见到你，欢迎问我任何问题。")
+    check_pipeline(
+        model_path=CHATGLM2_MODEL_PATH,
+        prompt="你好",
+        target="你好👋！我是人工智能助手 ChatGLM2-6B，很高兴见到你，欢迎问我任何问题。",
+    )
 
 
 @pytest.mark.skipif(not CHATGLM3_MODEL_PATH.exists(), reason="model file not found")
 def test_chatglm3_pipeline():
-    check_pipeline(model_path=CHATGLM3_MODEL_PATH, prompt="你好", target="你好👋！我是人工智能助手 ChatGLM3-6B，很高兴见到你，欢迎问我任何问题。")
+    check_pipeline(
+        model_path=CHATGLM3_MODEL_PATH,
+        prompt="你好",
+        target="你好👋！我是人工智能助手 ChatGLM3-6B，很高兴见到你，欢迎问我任何问题。",
+    )
 
 
 @pytest.mark.skipif(not CODEGEEX2_MODEL_PATH.exists(), reason="model file not found")
 def test_codegeex2_pipeline():
     prompt = "# language: Python\n# write a bubble sort function\n"
     target = """
```

### Comparing `chatglm-cpp-0.3.1/tests/test_convert.py` & `chatglm_cpp-0.3.2/tests/test_convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import sys
 from pathlib import Path
 
 import torch
 import torch.nn.functional as F
-from chatglm_cpp.convert import quantize_q4_0, quantize_q4_1, quantize_q5_0, quantize_q5_1, quantize_q8_0
+from chatglm_cpp.convert import (
+    get_prefix_cache,
+    quantize_q4_0,
+    quantize_q4_1,
+    quantize_q5_0,
+    quantize_q5_1,
+    quantize_q8_0,
+)
 
 HERE = Path(__file__).resolve().parent
 
 # generated by:
 #   torch.manual_seed(0)
 #   weight = torch.randn(2, 128)
 
@@ -164,18 +171,14 @@
            2,  -70,  -84,   12,  -65,  -14,  116,  103,   55,  -15,   55,  -23,
         -112,   47,   11,  -65,   46,  104,   84,  -26,   44,   12,    1,   98,
          -66,  -28,   77,  -44,  -18, -118,  122,  -74, -121,    6,   -7,   32]).view(q_tensor.shape)
     # fmt: on
     assert (q_tensor == ggml_q_tensor).all()
 
 
-CHATGLM_MODEL_PATH = Path(
-    "~/.cache/huggingface/hub/models--THUDM--chatglm-6b/snapshots/619e736c6d4cd139840579c5482063b75bed5666"
-).expanduser()
-
 CHATGLM2_MODEL_PATH = Path(
     "~/.cache/huggingface/hub/models--THUDM--chatglm2-6b/snapshots/b1502f4f75c71499a3d566b14463edd62620ce9f"
 ).expanduser()
 
 BAICHUAN7B_MODEL_PATH = Path(
     "~/.cache/huggingface/hub/models--baichuan-inc--Baichuan2-7B-Chat/snapshots/229e4eb1fab7f6aef90a2344c07085b680487597"
 ).expanduser()
@@ -238,14 +241,52 @@
     with open(HERE / "data/rms_norm.data", "wb") as f:
         m.weight.data.numpy().tofile(f)
         x.numpy().tofile(f)
         y.numpy().tofile(f)
 
 
 def make_data_glm_model():
+    def _forward_steps(model, seq_len):
+        # self attention
+        x1 = torch.arange(seq_len, dtype=torch.int64)[None, :]
+        position_ids = torch.tensor([[[0, 1, 1], [0, 0, 1]]])
+        attn_mask = torch.tensor([[0, 0, 1], [0, 0, 1], [0, 0, 0]], dtype=torch.bool)[None, None, :]
+        with torch.no_grad():
+            out = model(x1, position_ids=position_ids, attention_mask=attn_mask, use_cache=True)
+            y1 = out.last_hidden_state
+            kv_cache = out.past_key_values
+
+        # cross attention
+        x2 = torch.tensor([[seq_len]], dtype=torch.int64)
+        position_ids = torch.tensor([[[1], [2]]])
+        attn_mask = None
+        with torch.no_grad():
+            out = model(
+                x2, position_ids=position_ids, attention_mask=attn_mask, past_key_values=kv_cache, use_cache=True
+            )
+            y2 = out.last_hidden_state
+            kv_cache = out.past_key_values
+
+        # cross attention
+        x3 = torch.tensor([[seq_len + 1]], dtype=torch.int64)
+        position_ids = torch.tensor([[[1], [3]]])
+        attn_mask = None
+        with torch.no_grad():
+            out = model(
+                x3, position_ids=position_ids, attention_mask=attn_mask, past_key_values=kv_cache, use_cache=True
+            )
+            y3 = out.last_hidden_state
+            kv_cache = out.past_key_values
+
+        return x1, y1, x2, y2, x3, y3
+
+    CHATGLM_MODEL_PATH = Path(
+        "~/.cache/huggingface/hub/models--THUDM--chatglm-6b/snapshots/8b7d33596d18c5e83e2da052d05ca4db02e60620"
+    ).expanduser()
+
     sys.path.append(str(CHATGLM_MODEL_PATH))
     from modeling_chatglm import ChatGLMModel
     from transformers import AutoConfig
 
     config = AutoConfig.from_pretrained(CHATGLM_MODEL_PATH, trust_remote_code=True)
     config.hidden_size = 32
     config.num_attention_heads = 8
@@ -256,44 +297,62 @@
 
     m = ChatGLMModel(config, empty_init=False).float().eval()
     for param in m.parameters():
         param.data.uniform_(-0.5, 0.5)
 
     seq_len = 3
 
-    # self attention
-    x1 = torch.arange(seq_len, dtype=torch.int64)[None, :]
-    position_ids = torch.tensor([[[0, 1, 1], [0, 0, 1]]])
-    attn_mask = torch.tensor([[0, 0, 1], [0, 0, 1], [0, 0, 0]], dtype=torch.bool)[None, None, :]
-    with torch.no_grad():
-        out = m(x1, position_ids=position_ids, attention_mask=attn_mask, use_cache=True)
-        y1 = out.last_hidden_state
-        kv_cache = out.past_key_values
+    x1, y1, x2, y2, x3, y3 = _forward_steps(m, seq_len)
 
-    # cross attention
-    x2 = torch.tensor([[seq_len]], dtype=torch.int64)
-    position_ids = torch.tensor([[[1], [2]]])
-    attn_mask = None
-    with torch.no_grad():
-        out = m(x2, position_ids=position_ids, attention_mask=attn_mask, past_key_values=kv_cache, use_cache=True)
-        y2 = out.last_hidden_state
-        kv_cache = out.past_key_values
+    print(m)
 
-    # cross attention
-    x3 = torch.tensor([[seq_len + 1]], dtype=torch.int64)
-    position_ids = torch.tensor([[[1], [3]]])
-    attn_mask = None
-    with torch.no_grad():
-        out = m(x3, position_ids=position_ids, attention_mask=attn_mask, past_key_values=kv_cache, use_cache=True)
-        y3 = out.last_hidden_state
-        kv_cache = out.past_key_values
+    with open(HERE / "data/glm_model.data", "wb") as f:
+        m.word_embeddings.weight.data.numpy().tofile(f)
+        m.layers[0].input_layernorm.weight.data.numpy().tofile(f)
+        m.layers[0].input_layernorm.bias.data.numpy().tofile(f)
+        m.layers[0].attention.query_key_value.weight.data.numpy().tofile(f)
+        m.layers[0].attention.query_key_value.bias.data.numpy().tofile(f)
+        m.layers[0].attention.dense.weight.data.numpy().tofile(f)
+        m.layers[0].attention.dense.bias.data.numpy().tofile(f)
+        m.layers[0].post_attention_layernorm.weight.data.numpy().tofile(f)
+        m.layers[0].post_attention_layernorm.bias.data.numpy().tofile(f)
+        m.layers[0].mlp.dense_h_to_4h.weight.data.numpy().tofile(f)
+        m.layers[0].mlp.dense_h_to_4h.bias.data.numpy().tofile(f)
+        m.layers[0].mlp.dense_4h_to_h.weight.data.numpy().tofile(f)
+        m.layers[0].mlp.dense_4h_to_h.bias.data.numpy().tofile(f)
+        m.final_layernorm.weight.data.numpy().tofile(f)
+        m.final_layernorm.bias.data.numpy().tofile(f)
+
+        x1.int().numpy().tofile(f)
+        y1.data.numpy().tofile(f)
+        x2.int().numpy().tofile(f)
+        y2.data.numpy().tofile(f)
+        x3.int().numpy().tofile(f)
+        y3.data.numpy().tofile(f)
+
+    # p-tuning v2
+    config.pre_seq_len = 5
+    m = ChatGLMModel(config).float().eval()
+    for param in m.parameters():
+        param.data.uniform_(-0.5, 0.5)
+
+    x1, y1, x2, y2, x3, y3 = _forward_steps(m, seq_len)
 
     print(m)
 
-    with open(HERE / "data/glm_model.data", "wb") as f:
+    past_key_values = get_prefix_cache(
+        m.prefix_encoder,
+        config.pre_seq_len,
+        config.num_layers,
+        config.num_attention_heads,
+        config.hidden_size // config.num_attention_heads,
+    )
+
+    with open(HERE / "data/glm_ptuning_v2_model.data", "wb") as f:
+        past_key_values.data.numpy().tofile(f)
         m.word_embeddings.weight.data.numpy().tofile(f)
         m.layers[0].input_layernorm.weight.data.numpy().tofile(f)
         m.layers[0].input_layernorm.bias.data.numpy().tofile(f)
         m.layers[0].attention.query_key_value.weight.data.numpy().tofile(f)
         m.layers[0].attention.query_key_value.bias.data.numpy().tofile(f)
         m.layers[0].attention.dense.weight.data.numpy().tofile(f)
         m.layers[0].attention.dense.bias.data.numpy().tofile(f)
@@ -381,15 +440,52 @@
         x2.int().numpy().tofile(f)
         y2.numpy().tofile(f)
         x3.int().numpy().tofile(f)
         y3.numpy().tofile(f)
 
 
 def make_data_glm3_model():
-    CHATGLM3_MODEL_PATH = Path("./chatglm3-6b").expanduser()
+
+    def _forward_steps(model, seq_len):
+        # self attention
+        x1 = torch.arange(seq_len, dtype=torch.int64)[None, :]
+        position_ids = torch.arange(seq_len, dtype=torch.int64)[None, :]
+        attn_mask = torch.ones(1, seq_len, dtype=torch.int64)
+        with torch.no_grad():
+            out = model(x1, position_ids=position_ids, attention_mask=attn_mask, use_cache=True)
+            y1 = out.last_hidden_state
+            kv_cache = out.past_key_values
+
+        # cross attention
+        x2 = torch.tensor([[seq_len]], dtype=torch.int64)
+        position_ids = torch.tensor([[seq_len]], dtype=torch.int64)
+        attn_mask = torch.ones(1, seq_len + 1, dtype=torch.int64)
+        with torch.no_grad():
+            out = model(
+                x2, position_ids=position_ids, attention_mask=attn_mask, past_key_values=kv_cache, use_cache=True
+            )
+            y2 = out.last_hidden_state
+            kv_cache = out.past_key_values
+
+        # cross attention
+        x3 = torch.tensor([[seq_len + 1]], dtype=torch.int64)
+        position_ids = torch.tensor([[seq_len + 1]], dtype=torch.int64)
+        attn_mask = torch.ones(1, seq_len + 2, dtype=torch.int64)
+        with torch.no_grad():
+            out = model(
+                x3, position_ids=position_ids, attention_mask=attn_mask, past_key_values=kv_cache, use_cache=True
+            )
+            y3 = out.last_hidden_state
+            kv_cache = out.past_key_values
+
+        return x1, y1, x2, y2, x3, y3
+
+    CHATGLM3_MODEL_PATH = Path(
+        "~/.cache/huggingface/hub/models--THUDM--chatglm3-6b/snapshots/a5ba5501eb873d40d48bd0983bd2a8dd006bb838"
+    ).expanduser()
 
     sys.path.append(str(CHATGLM3_MODEL_PATH))
     from modeling_chatglm import ChatGLMModel
     from transformers import AutoConfig
 
     config = AutoConfig.from_pretrained(CHATGLM3_MODEL_PATH, trust_remote_code=True)
     config.hidden_size = 32
@@ -403,44 +499,52 @@
 
     m = ChatGLMModel(config).float().eval()
     for param in m.parameters():
         param.data.uniform_(-0.5, 0.5)
 
     seq_len = 3
 
-    # self attention
-    x1 = torch.arange(seq_len, dtype=torch.int64)[None, :]
-    position_ids = torch.arange(seq_len, dtype=torch.int64)[None, :]
-    attn_mask = torch.ones(1, seq_len, dtype=torch.int64)
-    with torch.no_grad():
-        out = m(x1, position_ids=position_ids, attention_mask=attn_mask, use_cache=True)
-        y1 = out.last_hidden_state
-        kv_cache = out.past_key_values
+    x1, y1, x2, y2, x3, y3 = _forward_steps(m, seq_len)
 
-    # cross attention
-    x2 = torch.tensor([[seq_len]], dtype=torch.int64)
-    position_ids = torch.tensor([[seq_len]], dtype=torch.int64)
-    attn_mask = torch.ones(1, seq_len + 1, dtype=torch.int64)
-    with torch.no_grad():
-        out = m(x2, position_ids=position_ids, attention_mask=attn_mask, past_key_values=kv_cache, use_cache=True)
-        y2 = out.last_hidden_state
-        kv_cache = out.past_key_values
+    print(m)
 
-    # cross attention
-    x3 = torch.tensor([[seq_len + 1]], dtype=torch.int64)
-    position_ids = torch.tensor([[seq_len + 1]], dtype=torch.int64)
-    attn_mask = torch.ones(1, seq_len + 2, dtype=torch.int64)
-    with torch.no_grad():
-        out = m(x3, position_ids=position_ids, attention_mask=attn_mask, past_key_values=kv_cache, use_cache=True)
-        y3 = out.last_hidden_state
-        kv_cache = out.past_key_values
+    with open(HERE / "data/glm3_model.data", "wb") as f:
+        m.embedding.word_embeddings.weight.data.numpy().tofile(f)
+        m.encoder.layers[0].input_layernorm.weight.data.numpy().tofile(f)
+        m.encoder.layers[0].self_attention.query_key_value.weight.data.numpy().tofile(f)
+        m.encoder.layers[0].self_attention.query_key_value.bias.data.numpy().tofile(f)
+        m.encoder.layers[0].self_attention.dense.weight.data.numpy().tofile(f)
+        m.encoder.layers[0].post_attention_layernorm.weight.data.numpy().tofile(f)
+        m.encoder.layers[0].mlp.dense_h_to_4h.weight.data.numpy().tofile(f)
+        m.encoder.layers[0].mlp.dense_4h_to_h.weight.data.numpy().tofile(f)
+        m.encoder.final_layernorm.weight.data.numpy().tofile(f)
+
+        x1.int().numpy().tofile(f)
+        y1.numpy().tofile(f)
+        x2.int().numpy().tofile(f)
+        y2.numpy().tofile(f)
+        x3.int().numpy().tofile(f)
+        y3.numpy().tofile(f)
+
+    # p-tuning v2
+    config.pre_seq_len = 5
+    m = ChatGLMModel(config).float().eval()
+    for param in m.parameters():
+        param.data.uniform_(-0.5, 0.5)
+
+    x1, y1, x2, y2, x3, y3 = _forward_steps(m, seq_len)
 
     print(m)
 
-    with open(HERE / "data/glm3_model.data", "wb") as f:
+    past_key_values = get_prefix_cache(
+        m.prefix_encoder, config.pre_seq_len, config.num_layers, config.multi_query_group_num, config.kv_channels
+    )
+
+    with open(HERE / "data/glm3_ptuning_v2_model.data", "wb") as f:
+        past_key_values.data.numpy().tofile(f)
         m.embedding.word_embeddings.weight.data.numpy().tofile(f)
         m.encoder.layers[0].input_layernorm.weight.data.numpy().tofile(f)
         m.encoder.layers[0].self_attention.query_key_value.weight.data.numpy().tofile(f)
         m.encoder.layers[0].self_attention.query_key_value.bias.data.numpy().tofile(f)
         m.encoder.layers[0].self_attention.dense.weight.data.numpy().tofile(f)
         m.encoder.layers[0].post_attention_layernorm.weight.data.numpy().tofile(f)
         m.encoder.layers[0].mlp.dense_h_to_4h.weight.data.numpy().tofile(f)
```

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/ggml/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/LICENSE` & `chatglm_cpp-0.3.2/third_party/ggml/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/build.zig` & `chatglm_cpp-0.3.2/third_party/ggml/build.zig`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/cmake/BuildTypes.cmake` & `chatglm_cpp-0.3.2/third_party/ggml/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/cmake/GitVars.cmake` & `chatglm_cpp-0.3.2/third_party/ggml/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/ggml/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/dolly-v2/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/dolly-v2/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-2/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-2/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-2/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-j/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-j/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/gpt-neox/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/gpt-neox/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/mnist/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/ggml/examples/mnist/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/mnist/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/mnist/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/mpt/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/mpt/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/python/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/python/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/sam/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/sam/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/starcoder/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/ggml/examples/starcoder/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/starcoder/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/starcoder/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/examples/whisper/README.md` & `chatglm_cpp-0.3.2/third_party/ggml/examples/whisper/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/include/ggml/ggml-alloc.h` & `chatglm_cpp-0.3.2/third_party/ggml/include/ggml/ggml-alloc.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/include/ggml/ggml-backend.h` & `chatglm_cpp-0.3.2/third_party/ggml/include/ggml/ggml-backend.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/include/ggml/ggml.h` & `chatglm_cpp-0.3.2/third_party/ggml/include/ggml/ggml.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/ggml/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-alloc.c` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-alloc.c`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-backend.c` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-backend.c`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-cuda.cu` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-cuda.h` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-metal.h` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-metal.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-metal.m` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-metal.m`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-metal.metal` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-metal.metal`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-opencl.cpp` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-opencl.cpp`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml-opencl.h` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/src/ggml.c` & `chatglm_cpp-0.3.2/third_party/ggml/src/ggml.c`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/ggml/tests/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/ggml/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/LICENSE` & `chatglm_cpp-0.3.2/third_party/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/attr.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/buffer_info.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/cast.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/chrono.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/complex.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/class.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/common.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/descr.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/init.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/internals.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/type_caster_base.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/detail/typeid.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eigen/matrix.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eigen/tensor.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/embed.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/eval.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/functional.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/gil.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/iostream.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/numpy.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/operators.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/options.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/pybind11.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/pytypes.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/stl/filesystem.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/stl.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/stl_bind.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h` & `chatglm_cpp-0.3.2/third_party/pybind11/include/pybind11/type_caster_pyobject_ptr.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tests/test_embed/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/FindCatch.cmake` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/FindEigen3.cmake` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/FindPythonLibsNew.cmake` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/JoinPaths.cmake` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/check-style.sh` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/cmake_uninstall.cmake.in` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/libsize.py` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/make_changelog.py` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11Common.cmake` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11Config.cmake.in` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11NewTools.cmake` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/pybind11Tools.cmake` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/setup_global.py.in` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/pybind11/tools/setup_main.py.in` & `chatglm_cpp-0.3.2/third_party/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/.gitignore` & `chatglm_cpp-0.3.2/third_party/sentencepiece/.gitignore`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/sentencepiece/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/CONTRIBUTING.md` & `chatglm_cpp-0.3.2/third_party/sentencepiece/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/LICENSE` & `chatglm_cpp-0.3.2/third_party/sentencepiece/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/README.md` & `chatglm_cpp-0.3.2/third_party/sentencepiece/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/cmake/ios.toolchain.cmake` & `chatglm_cpp-0.3.2/third_party/sentencepiece/cmake/ios.toolchain.cmake`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/python/README.md` & `chatglm_cpp-0.3.2/third_party/sentencepiece/python/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/CMakeLists.txt` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model_trainer.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model_trainer.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model_trainer.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/bpe_model_trainer_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/bpe_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/builder.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/builder.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/builder.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/builder.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/builder_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/builder_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/sentencepiece.pb.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/sentencepiece.pb.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/sentencepiece.pb.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/sentencepiece.pb.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model_trainer.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model_trainer.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model_trainer.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/char_model_trainer_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/char_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/common.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/common.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/compile_charsmap_main.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/compile_charsmap_main.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/error.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/error.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/filesystem.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/filesystem.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/filesystem.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/filesystem_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/filesystem_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/freelist.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/freelist.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/freelist_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/freelist_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/init.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/init.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/init_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/init_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_factory.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_factory.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_factory.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_factory.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_factory_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_factory_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_interface.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_interface.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_interface.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_interface.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/model_interface_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/model_interface_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/normalization_rule.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/normalization_rule.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/normalizer.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/normalizer.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/normalizer.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/normalizer.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/normalizer_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/normalizer_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/pretokenizer_for_training.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/pretokenizer_for_training.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/pretokenizer_for_training.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/pretokenizer_for_training.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/pretokenizer_for_training_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/pretokenizer_for_training_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece.proto` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece.proto`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_model.proto` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_model.proto`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_processor.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_processor.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_processor.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_processor.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_processor_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_processor_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_trainer.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_trainer.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_trainer.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_trainer.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/sentencepiece_trainer_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/sentencepiece_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/spec_parser.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/spec_parser.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_decode_main.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_decode_main.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_encode_main.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_encode_main.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_export_vocab_main.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_export_vocab_main.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_normalize_main.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_normalize_main.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/spm_train_main.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/spm_train_main.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/test_main.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/test_main.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/testharness.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/testharness.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/testharness.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/testharness.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_factory.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_factory.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_factory.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_factory.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_factory_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_factory_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_interface.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_interface.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_interface.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_interface.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/trainer_interface_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/trainer_interface_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unicode_script.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unicode_script.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unicode_script.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unicode_script.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unicode_script_map.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unicode_script_map.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unicode_script_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unicode_script_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model_trainer.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model_trainer.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model_trainer.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/unigram_model_trainer_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/unigram_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/util.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/util.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/util.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/util.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/util_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/util_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model_trainer.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model_trainer.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model_trainer.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/src/word_model_trainer_test.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/src/word_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/LICENSE` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/container/flat_hash_map.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/container/flat_hash_map.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/container/flat_hash_set.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/container/flat_hash_set.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/flags/flag.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/flags/flag.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/flags/flag.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/flags/flag.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/flags/parse.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/flags/parse.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/memory/memory.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/memory/memory.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/random/distributions.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/random/distributions.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/random/random.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/random/random.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/ascii.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/ascii.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/match.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/match.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/numbers.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/numbers.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_cat.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_cat.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_format.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_format.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_join.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_join.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_replace.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_replace.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/str_split.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/str_split.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/string_view.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/string_view.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/absl/strings/strip.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/absl/strings/strip.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/darts_clone/LICENSE` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/darts_clone/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/darts_clone/darts.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/darts_clone/darts.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/esaxx/LICENSE` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/esaxx/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/esaxx/esa.hxx` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/esaxx/esa.hxx`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/esaxx/sais.hxx` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/esaxx/sais.hxx`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/LICENSE` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/LICENSE`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/arena.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/arena.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/arenastring.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/arenastring.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/bytestream.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/bytestream.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/coded_stream.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/coded_stream.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/common.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/common.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/extension_set.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/extension_set.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/generated_message_util.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/generated_message_util.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/int128.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/int128.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/io_win32.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/io_win32.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/message_lite.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/message_lite.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/parse_context.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/parse_context.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/repeated_field.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/repeated_field.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/status.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/status.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/statusor.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/statusor.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/stringpiece.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/stringprintf.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/stringprintf.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/structurally_valid.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/structurally_valid.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/strutil.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/strutil.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/time.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/time.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc`

 * *Files identical despite different names*

### Comparing `chatglm-cpp-0.3.1/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc` & `chatglm_cpp-0.3.2/third_party/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc`

 * *Files identical despite different names*

