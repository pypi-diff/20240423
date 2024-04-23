# Comparing `tmp/rpi_libcamera-0.1a3.tar.gz` & `tmp/rpi_libcamera-0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_libcamera-0.1a3.tar", last modified: Fri Feb 23 12:28:52 2024, max compression
+gzip compressed data, was "rpi_libcamera-0.1a4.tar", last modified: Tue Apr 23 12:53:02 2024, max compression
```

## Comparing `rpi_libcamera-0.1a3.tar` & `rpi_libcamera-0.1a4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       29 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/.gitignore
--rw-r--r--   0        0        0     5100 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/README.md
--rwxr-xr-x   0        0        0    71520 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/check-version
--rw-r--r--   0        0        0      136 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/check-version.cpp
--rwxr-xr-x   0        0        0      107 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/check-version.sh
--rwxr-xr-x   0        0        0      115 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/clone-libcamera.sh
--rw-r--r--   0        0        0     1991 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/meson.build
--rw-r--r--   0        0        0      698 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/meson_options.txt
--rw-r--r--   0        0        0      785 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/pypatch.patch
--rw-r--r--   0        0        0      558 2023-11-29 11:54:53.000000 rpi_libcamera-0.1a3/pyproject.toml
--rw-r--r--   0        0        0     5373 2024-02-23 12:28:52.101871 rpi_libcamera-0.1a3/PKG-INFO
+-rw-r--r--   0        0        0       29 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/.gitignore
+-rw-r--r--   0        0        0     5167 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/README.md
+-rw-r--r--   0        0        0      136 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/check-version.cpp
+-rwxr-xr-x   0        0        0      107 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/check-version.sh
+-rwxr-xr-x   0        0        0      115 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/clone-libcamera.sh
+-rw-r--r--   0        0        0     1991 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/meson.build
+-rw-r--r--   0        0        0      698 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/meson_options.txt
+-rw-r--r--   0        0        0      785 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/pypatch.patch
+-rw-r--r--   0        0        0      559 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     2186 2024-02-23 12:32:28.000000 rpi_libcamera-0.1a4/update-version.py
+-rw-r--r--   0        0        0     5440 2024-04-23 12:53:02.887582 rpi_libcamera-0.1a4/PKG-INFO
```

### Comparing `rpi_libcamera-0.1a3/README.md` & `rpi_libcamera-0.1a4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 To update your installation (which may be required when you update your version of libcamera) you can run `pip install --upgrade rpi-libcamera` to update to the latest version.
 
 ### If you get a version error
 If you get the error `This package works with libcamera version ..., but you have version ... installed`, then this means the version strings are not matching. If you have built your own version of libcamera, then just pass `-C setup-args="-Dversion=unknown"` to skip this check and follow the instructions in the next section. If you have a system installed version of libcamera then you will need to check this table for the correct pip package version to install, based on the version of libcamera you have installed. You can see your currently installed version of libcamera by running `rpicam-hello --version`. These are the common versions found on Raspberry Pis.
 
 | System and Date | libcamera Reported Version | Pip Package Version |
 | --------------- | -------------------------- | ------------------- |
+| Raspberry Pi Bookworm 18/04/2024 | v0.2.0+120-eb00c13d | 0.1a4 |
 | Raspberry Pi Bookworm 15/02/2024 | v0.2.0+46-075b54d5 | 0.1a3 |
 | Raspberry Pi Bookworm 22/11/2023 | v0.1.0+118-563cd78e | 0.1a2 |
 
 ### If that doesn't work...
 
 If you have built your own version of libcamera, or your system has a version which is not compatible with a release version, then you may need to pass the repository and revision to meson. The arguments to do this are `-C setup-args="-Drepository=https://my.repository.git"` for the repository and `-C setup-args="-Drevision=branch"` for the revision. These are passed directly into `git clone` and `git checkout` respectively, so and strings that work with those will work here. The `-C, --config-settings` argument require an up to date version of `pip>=23.1` so you may first need to run `pip install --upgrade pip`
```

### Comparing `rpi_libcamera-0.1a3/meson.build` & `rpi_libcamera-0.1a4/meson.build`

 * *Files identical despite different names*

### Comparing `rpi_libcamera-0.1a3/meson_options.txt` & `rpi_libcamera-0.1a4/meson_options.txt`

 * *Files identical despite different names*

### Comparing `rpi_libcamera-0.1a3/pypatch.patch` & `rpi_libcamera-0.1a4/pypatch.patch`

 * *Files identical despite different names*

### Comparing `rpi_libcamera-0.1a3/pyproject.toml` & `rpi_libcamera-0.1a4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 build-backend = 'mesonpy'
 requires = ['meson-python', 'pyyaml', 'pybind11']
 
 [project]
 name = 'rpi-libcamera'
-version = '0.1a3'
+version = '0.1a4'
 description = 'libcamera python bindings'
 readme = 'README.md'
 
 [project.urls]
 Source = "https://github.com/raspberrypi/pylibcamera"
 "RPi libcamera Source" = "https://github.com/raspberrypi/libcamera"
 
 [tool.meson-python.args]
 setup = [
-    '-Drevision=v0.2.0+rpt20240215',
+    '-Drevision=v0.2.0+rpt20240418',
     '-Drepository=https://github.com/raspberrypi/libcamera.git',
-    '-Dversion=v0.2.0+46-075b54d5'
+    '-Dversion=v0.2.0+120-eb00c13d'
 ]
 
 [tool.flit.module]
 name = "libcamera"
```

### Comparing `rpi_libcamera-0.1a3/PKG-INFO` & `rpi_libcamera-0.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-libcamera
-Version: 0.1a3
+Version: 0.1a4
 Summary: libcamera python bindings
 Project-URL: Source, https://github.com/raspberrypi/pylibcamera
 Project-URL: Rpi libcamera source, https://github.com/raspberrypi/libcamera
 Description-Content-Type: text/markdown
 
 # Pylibcamera
 This package is for the libcamera python bindings only. It requires you to already have installed a version of libcamera onto your system.
@@ -36,14 +36,15 @@
 To update your installation (which may be required when you update your version of libcamera) you can run `pip install --upgrade rpi-libcamera` to update to the latest version.
 
 ### If you get a version error
 If you get the error `This package works with libcamera version ..., but you have version ... installed`, then this means the version strings are not matching. If you have built your own version of libcamera, then just pass `-C setup-args="-Dversion=unknown"` to skip this check and follow the instructions in the next section. If you have a system installed version of libcamera then you will need to check this table for the correct pip package version to install, based on the version of libcamera you have installed. You can see your currently installed version of libcamera by running `rpicam-hello --version`. These are the common versions found on Raspberry Pis.
 
 | System and Date | libcamera Reported Version | Pip Package Version |
 | --------------- | -------------------------- | ------------------- |
+| Raspberry Pi Bookworm 18/04/2024 | v0.2.0+120-eb00c13d | 0.1a4 |
 | Raspberry Pi Bookworm 15/02/2024 | v0.2.0+46-075b54d5 | 0.1a3 |
 | Raspberry Pi Bookworm 22/11/2023 | v0.1.0+118-563cd78e | 0.1a2 |
 
 ### If that doesn't work...
 
 If you have built your own version of libcamera, or your system has a version which is not compatible with a release version, then you may need to pass the repository and revision to meson. The arguments to do this are `-C setup-args="-Drepository=https://my.repository.git"` for the repository and `-C setup-args="-Drevision=branch"` for the revision. These are passed directly into `git clone` and `git checkout` respectively, so and strings that work with those will work here. The `-C, --config-settings` argument require an up to date version of `pip>=23.1` so you may first need to run `pip install --upgrade pip`
```

