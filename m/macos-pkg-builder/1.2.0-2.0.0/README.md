# Comparing `tmp/macos_pkg_builder-1.2.0-py3-none-any.whl.zip` & `tmp/macos_pkg_builder-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,13 @@
-Zip file size: 7688 bytes, number of entries: 6
--rw-r--r--  2.0 unx     1113 b- defN 24-Apr-17 22:15 macos_pkg_builder/__init__.py
--rw-r--r--  2.0 unx    22014 b- defN 24-Apr-17 22:15 macos_pkg_builder/core.py
--rw-r--r--  2.0 unx     6476 b- defN 24-Apr-17 22:15 macos_pkg_builder-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-17 22:15 macos_pkg_builder-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-17 22:15 macos_pkg_builder-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      507 b- defN 24-Apr-17 22:15 macos_pkg_builder-1.2.0.dist-info/RECORD
-6 files, 30220 bytes uncompressed, 6766 bytes compressed:  77.6%
+Zip file size: 12401 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1155 b- defN 24-Apr-23 21:45 macos_pkg_builder/__init__.py
+-rw-r--r--  2.0 unx     8838 b- defN 24-Apr-23 21:45 macos_pkg_builder/core.py
+-rw-r--r--  2.0 unx     7922 b- defN 24-Apr-23 21:45 macos_pkg_builder/distribution_pkg.py
+-rw-r--r--  2.0 unx     8342 b- defN 24-Apr-23 21:45 macos_pkg_builder/flat_pkg.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 21:45 macos_pkg_builder/utilities/__init__.py
+-rw-r--r--  2.0 unx     1866 b- defN 24-Apr-23 21:45 macos_pkg_builder/utilities/signing.py
+-rw-r--r--  2.0 unx     2747 b- defN 24-Apr-23 21:45 macos_pkg_builder/utilities/subprocess_wrapper.py
+-rw-r--r--  2.0 unx     8475 b- defN 24-Apr-23 21:45 macos_pkg_builder-2.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 21:45 macos_pkg_builder-2.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-23 21:45 macos_pkg_builder-2.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      980 b- defN 24-Apr-23 21:45 macos_pkg_builder-2.0.0.dist-info/RECORD
+11 files, 40435 bytes uncompressed, 10715 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -1,19 +1,34 @@
 Filename: macos_pkg_builder/__init__.py
 Comment: 
 
 Filename: macos_pkg_builder/core.py
 Comment: 
 
-Filename: macos_pkg_builder-1.2.0.dist-info/METADATA
+Filename: macos_pkg_builder/distribution_pkg.py
 Comment: 
 
-Filename: macos_pkg_builder-1.2.0.dist-info/WHEEL
+Filename: macos_pkg_builder/flat_pkg.py
 Comment: 
 
-Filename: macos_pkg_builder-1.2.0.dist-info/top_level.txt
+Filename: macos_pkg_builder/utilities/__init__.py
 Comment: 
 
-Filename: macos_pkg_builder-1.2.0.dist-info/RECORD
+Filename: macos_pkg_builder/utilities/signing.py
+Comment: 
+
+Filename: macos_pkg_builder/utilities/subprocess_wrapper.py
+Comment: 
+
+Filename: macos_pkg_builder-2.0.0.dist-info/METADATA
+Comment: 
+
+Filename: macos_pkg_builder-2.0.0.dist-info/WHEEL
+Comment: 
+
+Filename: macos_pkg_builder-2.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: macos_pkg_builder-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## macos_pkg_builder/__init__.py

```diff
@@ -15,17 +15,17 @@
     >>>     },
     >>> )
 
     >>> assert pkg_obj.build() is True
 """
 
 __title__:        str = "macos_pkg_builder"
-__version__:      str = "1.2.0"
-__description__:  str = "macOS Package Builder Library, wrapping the `pkgbuild` and `productbuild` tools."
+__version__:      str = "2.0.0"
+__description__:  str = "macOS Package Builder Library, wrapping Apple's 'pkgbuild' and 'productbuild' utilities."
 __url__:          str = "https://github.com/ripeda/macOS-Pkg-Builder"
 __author__:       str = "RIPEDA Consulting"
 __author_email__: str = "info@ripeda.com"
 __status__:       str = "Production/Stable"
 __all__:         list = ["Packages"]
 
 
-from .core import Packages
+from .core import DistributionPackage, FlatPackage, Packages
```

## macos_pkg_builder/core.py

```diff
@@ -2,32 +2,20 @@
 
 """
 macOS Package Builder
 
 Designed to simplify package creation through native tooling, ex. pkgbuild, productbuild, etc.
 """
 
-
 import logging
-import markdown
-import plistlib
-import tempfile
-import subprocess
-
-import xml.etree.ElementTree as ET
 
 from pathlib import Path
 
-
-PKGBUILD:     str = "/usr/bin/pkgbuild"
-PRODUCTBUILD: str = "/usr/bin/productbuild"
-PRODUCTSIGN:  str = "/usr/bin/productsign"
-SECURITY:     str = "/usr/bin/security"
-CHMOD:        str = "/bin/chmod"
-CP:           str = "/bin/cp"
+from .flat_pkg import FlatPackage
+from .distribution_pkg import DistributionPackage
 
 
 class Packages:
 
     def __init__(self,
                  pkg_output:              str,
                  pkg_bundle_id:           str,
@@ -167,365 +155,53 @@
             self._pkg_background,
             self._pkg_background_dark
         ]
 
         if self._pkg_as_distribution is False and any(_requires_distribution):
             raise Exception("Distribution files require 'pkg_as_distribution' to be True.")
 
-        # If a dark background is not provided, use the light background.
-        if self._pkg_background is not None and self._pkg_background_dark is None:
-            self._pkg_background_dark = self._pkg_background
-
-        self._pkg_temp_directory      = tempfile.TemporaryDirectory()
-        self._pkg_temp_directory      = Path(self._pkg_temp_directory.name)
-        self._pkg_build_directory     = Path(self._pkg_temp_directory, "build")
-        self._pkg_scripts_directory   = Path(self._pkg_temp_directory, "scripts")
-        self._pkg_output_directory    = Path(self._pkg_temp_directory, "output")
-        self._pkg_resources_directory = Path(self._pkg_temp_directory, "resources")
-
-        self._markdown_file_mapping = {
-            self._pkg_welcome: "WELCOME.html",
-            self._pkg_readme:  "README.html",
-            self._pkg_license: "LICENSE.html"
-        }
-
-        self._background_mapping = {
-            "light": {
-                "property": self._pkg_background,
-                "file": f"BACKGROUND{Path(self._pkg_background).suffix if self._pkg_background is not None else ''}",
-                "label": "background",
-            },
-            "dark": {
-                "property": self._pkg_background_dark,
-                "file": f"BACKGROUND-DARK{Path(self._pkg_background_dark).suffix if self._pkg_background_dark is not None else ''}",
-                "label": "background-darkAqua",
-            }
-        }
-
-
-    def _prepare_scripts(self) -> None:
-        """
-        Adjusts naming and permissions of scripts to match pkgbuild requirements.
-        """
-
-        if self._pkg_preinstall_script is not None:
-            self._pkg_scripts_directory.mkdir(parents=True, exist_ok=True)
-            if not Path(self._pkg_preinstall_script).exists():
-                raise FileNotFoundError(f"Preinstall script not found: {self._pkg_preinstall_script}")
-            subprocess.run([CP, self._pkg_preinstall_script, self._pkg_scripts_directory.joinpath("preinstall")])
-            subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath("preinstall")])
-
-        if self._pkg_preflight_script is not None:
-            self._pkg_scripts_directory.mkdir(parents=True, exist_ok=True)
-            if not Path(self._pkg_preflight_script).exists():
-                raise FileNotFoundError(f"Preflight script not found: {self._pkg_preflight_script}")
-            subprocess.run([CP, self._pkg_preflight_script, self._pkg_scripts_directory.joinpath("preflight")])
-            subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath("preflight")])
-
-        if self._pkg_postinstall_script is not None:
-            self._pkg_scripts_directory.mkdir(parents=True, exist_ok=True)
-            if not Path(self._pkg_postinstall_script).exists():
-                raise FileNotFoundError(f"Postinstall script not found: {self._pkg_postinstall_script}")
-            subprocess.run([CP, self._pkg_postinstall_script, self._pkg_scripts_directory.joinpath("postinstall")])
-            subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath("postinstall")])
-
-        if self._pkg_postflight_script is not None:
-            self._pkg_scripts_directory.mkdir(parents=True, exist_ok=True)
-            if not Path(self._pkg_postflight_script).exists():
-                raise FileNotFoundError(f"Postflight script not found: {self._pkg_postflight_script}")
-            subprocess.run([CP, self._pkg_postflight_script, self._pkg_scripts_directory.joinpath("postflight")])
-            subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath("postflight")])
-
-        if self._pkg_script_resources is not None:
-            for resources in self._pkg_script_resources:
-                if not Path(resources).exists():
-                    raise FileNotFoundError(f"Script resource not found: {resources}")
-                subprocess.run([CP, resources, self._pkg_scripts_directory])
-                subprocess.run([CHMOD, "+x", self._pkg_scripts_directory.joinpath(Path(resources).name)])
-
-
-    def _prepare_file_structure(self) -> None:
-        """
-        Adjusts file structure to match pkgbuild requirements.
-        """
-
-        self._pkg_build_directory.mkdir(parents=True, exist_ok=True)
-
-        if self._pkg_file_structure is None:
-            return
-
-        for source, destination in self._pkg_file_structure.items():
-            if not Path(source).exists():
-                raise FileNotFoundError(f"Source file does not exist: {source}")
-
-            internal_destination = Path(f"{self._pkg_build_directory}{destination}")
-
-            if not internal_destination.parent.exists():
-                internal_destination.parent.mkdir(parents=True, exist_ok=True)
-
-            subprocess.run([CP, "-R", source, internal_destination])
-
-
-    def _prepare_distribution_resources(self) -> None:
-        """
-        Prepare resources for the distribution package.
-        """
-        if self._pkg_as_distribution is False:
-            return
-
-        self._prepare_markdown_resources()
-        self._prepare_background_resources()
-
-
-    def _prepare_background_resources(self) -> None:
-        """
-        Prepare background resources for the distribution package.
-        """
-        # Check if light and dark are the same, if so, only copy one.
-        if self._background_mapping["light"]["property"] == self._background_mapping["dark"]["property"]:
-            self._background_mapping["dark"]["property"] = None
-            self._background_mapping["dark"]["file"] = self._background_mapping["light"]["file"]
-
-        for background in self._background_mapping:
-            if self._background_mapping[background]["property"] is None:
-                continue
-            if not Path(self._background_mapping[background]["property"]).exists():
-                raise FileNotFoundError(f"Background image not found: {self._background_mapping[background]['property']}")
-
-            Path(self._pkg_resources_directory).mkdir(parents=True, exist_ok=True)
-            subprocess.run([CP, self._background_mapping[background]["property"], self._pkg_resources_directory.joinpath(self._background_mapping[background]["file"])])
-
-
-    def _prepare_markdown_resources(self) -> None:
-        """
-        Convert content from markdown to HTML, then save it to the resources directory.
-        """
-        for file in self._markdown_file_mapping:
-            if file is None:
-                continue
-
-            Path(self._pkg_resources_directory).mkdir(parents=True, exist_ok=True)
-
-            with open(self._pkg_resources_directory / self._markdown_file_mapping[file], "w") as f:
-                f.write("<!DOCTYPE html>\n<html>\n<head>\n<style>\nbody { font-family: -apple-system; }\n</style>\n</head>\n<body>\n")
-                f.write(markdown.markdown(file))
-                f.write("</body>\n</html>\n")
-
-
-    def _generate_component_file(self) -> None:
-        """
-        Generate a component file to prevent the relocation of the embedded application(s).
-        """
-
-        bundle=""
-        file = self._pkg_build_directory.parent / "component.plist"
-
-        # Find anything with an Info.plist embedded, needs to be a valid bundle for pkgbuild.
-        for source, destination in self._pkg_file_structure.items():
-            if Path(source, "Contents", "Info.plist").exists():
-                bundle = destination
-                break
-
-        contents = [{
-            "BundleHasStrictIdentifier": True,
-            "BundleIsRelocatable": self._pkg_allow_relocation,
-            "BundleIsVersionChecked": True,
-            "BundleOverwriteAction": "upgrade",
-            "RootRelativeBundlePath": bundle,
-        }]
-        plistlib.dump(contents, file.open("wb"))
-
-
-    def _generate_pkg_arguments(self) -> list:
-        """
-        Generate pkgbuild arguments according to the provided configuration.
-        """
-
-        args = [
-            PKGBUILD,
-            "--identifier", self._pkg_project_identifier,
-            "--version", self._pkg_project_version,
-            "--root", self._pkg_build_directory
-        ]
-
-        if self._pkg_scripts_directory.exists():
-            args.extend(["--scripts", self._pkg_scripts_directory])
-
-        if self._pkg_file_structure is not None:
-            args.extend(["--install-location", self._pkg_install_location])
-            if self._pkg_allow_relocation is False:
-                self._generate_component_file()
-                args.extend(["--component-plist", self._pkg_build_directory.parent / "component.plist"])
-        else:
-            args.extend(["--nopayload"])
-
-
-        args.extend([self._pkg_build_directory.parent / self._pkg_file_name])
-
-        return args
-
 
-    def _sync_distribution_file(self, input_file: tempfile.NamedTemporaryFile) -> None:
-        """
-        Sync the distribution file with the provided content.
-        """
-        tree = ET.parse(input_file.name)
-        root = tree.getroot()
-
-        if self._pkg_title is not None:
-            element = ET.Element("title")
-            element.text = self._pkg_title
-            root.append(element)
-
-        # Check if light and dark are the same, if so, only copy one.
-        for background in self._background_mapping:
-            element = ET.Element(self._background_mapping[background]["label"], file=self._background_mapping[background]["file"], alignment="bottomleft", scaling="tofit")
-            root.append(element)
-
-        for file in self._markdown_file_mapping:
-            if file is not None:
-                element_name = self._markdown_file_mapping[file].split(".")[0].lower()
-                element = ET.Element(element_name, file=self._markdown_file_mapping[file], mimetype="text/html")
-                root.append(element)
-
-        tree.write(input_file.name)
-
-
-    def _build_pkg(self) -> bool:
+    def build(self) -> bool:
         """
         Build the application package.
         """
-        result = subprocess.run(self._generate_pkg_arguments(), capture_output=True)
-        if result.returncode != 0:
-            logging.info(result.stderr.decode("utf-8"))
-            return False
-
-        return True
-
-
-    def _is_identity_valid(self) -> bool:
-        """
-        Check if the provided signing identity is valid.
-        """
-        if self._pkg_signing_identity is None:
-            return False
-
-        args = [
-            SECURITY,
-            "find-identity",
-            "-v",
-        ]
-
-        result = subprocess.run(args, capture_output=True)
-        if result.returncode != 0:
-            logging.info(result.stderr.decode("utf-8"))
-            return False
-
-        if self._pkg_signing_identity not in result.stdout.decode("utf-8"):
-            logging.info(f"Signing identity not found: {self._pkg_signing_identity}")
-            return False
-
-        return True
-
-
-    def _sign_pkg(self) -> bool:
-        """
-        Sign application package.
-        """
-        if self._pkg_signing_identity is None:
-            return True
 
-        if self._is_identity_valid() is False:
-            return False
+        result = FlatPackage(
+            pkg_output=self._pkg_output,
+            pkg_bundle_id=self._pkg_project_identifier,
+            pkg_version=self._pkg_project_version,
+            pkg_install_location=self._pkg_install_location,
+            pkg_allow_relocation=self._pkg_allow_relocation,
+            pkg_file_structure=self._pkg_file_structure,
+            pkg_preinstall_script=self._pkg_preinstall_script,
+            pkg_preflight_script=self._pkg_preflight_script,
+            pkg_postinstall_script=self._pkg_postinstall_script,
+            pkg_postflight_script=self._pkg_postflight_script,
+            pkg_script_resources=self._pkg_script_resources,
+            pkg_signing_identity=self._pkg_signing_identity
+        ).build()
 
-        args = [
-            PRODUCTSIGN,
-            "--sign", self._pkg_signing_identity,
-            self._pkg_build_directory.parent / self._pkg_file_name,
-            self._pkg_build_directory.parent / Path(self._pkg_file_name + ".signed")
-        ]
-        result = subprocess.run(args, capture_output=True)
-        if result.returncode != 0:
-            logging.info(result.stderr.decode("utf-8"))
+        if result is False:
             return False
 
-        # Replace the original package with the signed one.
-        Path(self._pkg_build_directory.parent / self._pkg_file_name).unlink()
-        Path(self._pkg_build_directory.parent / Path(self._pkg_file_name + ".signed")).rename(self._pkg_build_directory.parent / self._pkg_file_name)
-
-        return True
-
-
-    def _convert_to_product_archive(self) -> bool:
-        """
-        Convert the package to a product archive.
-        """
         if self._pkg_as_distribution is False:
             return True
 
-        # First, synthesize the product archive.
-        distribution_file = tempfile.NamedTemporaryFile(delete=False)
-        args = [
-            PRODUCTBUILD,
-            "--synthesize",
-            "--package", self._pkg_build_directory.parent / self._pkg_file_name,
-            distribution_file.name
-        ]
-
-        result = subprocess.run(args, capture_output=True)
-        if result.returncode != 0:
-            logging.info(result.stderr.decode("utf-8"))
-            return False
+        logging.info("Converting to distribution package.")
 
-        self._sync_distribution_file(distribution_file)
+        result = DistributionPackage(
+            pkg_output=self._pkg_output,
+            pkg_inputs=[self._pkg_output],
+            pkg_bundle_id=self._pkg_project_identifier,
+            pkg_version=self._pkg_project_version,
+            pkg_title=self._pkg_title,
+            pkg_welcome=self._pkg_welcome,
+            pkg_readme=self._pkg_readme,
+            pkg_license=self._pkg_license,
+            pkg_background=self._pkg_background,
+            pkg_background_dark=self._pkg_background_dark,
+            pkg_signing_identity=self._pkg_signing_identity
+        ).build()
 
-        args = [
-            PRODUCTBUILD,
-            "--distribution", distribution_file.name,
-            "--resources", self._pkg_resources_directory,
-            "--package-path", self._pkg_build_directory.parent,
-            self._pkg_build_directory.parent / Path(self._pkg_file_name + ".product")
-        ]
-
-        result = subprocess.run(args, capture_output=True)
-        if result.returncode != 0:
-            logging.info(result.stderr.decode("utf-8"))
-            return False
-
-        # Replace the original package with the product archive.
-        Path(self._pkg_build_directory.parent / self._pkg_file_name).unlink()
-        Path(self._pkg_build_directory.parent / Path(self._pkg_file_name + ".product")).rename(self._pkg_build_directory.parent / self._pkg_file_name)
-
-        return self._sign_pkg()
-
-
-    def build(self) -> bool:
-        """
-        Build the application package.
-        """
-
-        if all([self._pkg_file_structure is None, self._pkg_preinstall_script is None, self._pkg_postinstall_script is None]):
-            raise Exception("Cannot build a package!")
-
-        if Path(self._pkg_output).exists():
-            logging.info(f"Removing existing package: {self._pkg_output}")
-            Path(self._pkg_output).unlink()
-
-        self._prepare_scripts()
-        self._prepare_file_structure()
-        self._prepare_distribution_resources()
-        if self._build_pkg() is False:
-            logging.info("Package build failed.")
-            return False
-        if self._sign_pkg() is False:
-            logging.info("Package signing failed.")
-            return False
-        if self._convert_to_product_archive() is False:
-            logging.info("Package conversion failed.")
-            return False
+        return result
 
-        if not Path(self._pkg_output).parent.exists():
-            Path(self._pkg_output).mkdir(parents=True, exist_ok=True)
 
-        subprocess.run([CP, self._pkg_build_directory.parent / self._pkg_file_name, self._pkg_output])
-        logging.info(f"Package built: {self._pkg_output}")
-        return True
```

## Comparing `macos_pkg_builder-1.2.0.dist-info/METADATA` & `macos_pkg_builder-2.0.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: macos_pkg_builder
-Version: 1.2.0
-Summary: macOS Package Builder Library, wrapping the `pkgbuild` and `productbuild` tools.
+Version: 2.0.0
+Summary: macOS Package Builder Library, wrapping Apple's 'pkgbuild' and 'productbuild' utilities.
 Home-page: https://github.com/ripeda/macOS-Pkg-Builder
 Author: RIPEDA Consulting
 Author-email: info@ripeda.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: markdown
 
 # macOS-Pkg-Builder
 
-Python module for creating macOS packages more easily through native tooling (pkgbuild). Primarily developed as an alternative to [WhiteBox's Packages](http://s.sudre.free.fr/Software/Packages/about.html) for easier CI/CD integration.
+Python module for creating macOS packages more easily through native tooling (pkgbuild and productbuild). Primarily developed as an alternative to [WhiteBox's Packages](http://s.sudre.free.fr/Software/Packages/about.html) for easier CI/CD integration.
 
 * [GitHub](https://github.com/ripeda/macOS-Pkg-Builder)
 * [PyPi](https://pypi.org/project/macos-pkg-builder)
 
+
 ## Usage
 
 Installation:
-```
+```bash
+# Requires Python 3.6+ and macOS host with pkgbuild and productbuild available
 pip3 install macos-pkg-builder
 ```
 
 Sample invocation:
 ```py
 from macos_pkg_builder import Packages
 
@@ -37,14 +39,20 @@
         "Samples/MyApp/MyLaunchDaemon.plist": "/Library/LaunchDaemons/com.myapp.plist",
     },
 )
 
 assert pkg_obj.build() is True
 ```
 
+Supported classes:
+* `Packages` - For building single packages, either flat or distribution.
+  * Recommended for most use cases. Internally uses `FlatPackage` and `DistributionPackage` classes.
+* `FlatPackage` - For building flat packages.
+* `DistributionPackage` - For building distribution packages.
+
 
 Format of `Packages` constructor:
 ```py
 """
     pkg_output:             Path to where the package will be saved.
                             Required.
 
@@ -150,20 +158,54 @@
         "Samples/MyWallpaperConfigurator/Snow Leopard Server.jpg": "/Library/Desktop Pictures/Snow Leopard Server.jpg",
     },
     pkg_preinstall_script="Samples/MyWallpaperConfigurator/PrepareDirectory.sh",
     pkg_postinstall_script="Samples/MyWallpaperConfigurator/SetWallpaper.sh",
     pkg_script_resources=[
         "Samples/MyWallpaperConfigurator/desktoppr",
     ],
-),
+)
 ```
 
 #### Building a simple uninstaller
 
 Useful for when you have a single script you need to execute to remove your application:
 ```py
 Packages(
     pkg_output="Sample-Uninstall.pkg",
     pkg_bundle_id="com.myapp.uninstaller",
     pkg_preinstall_script="Samples/MyUninstaller/MyPreinstall.sh",
+)
+```
+
+#### Building installers with welcome, readme, licensing and background image
+
+Uses the markdown formatting to provide a more polished installer experience with little effort.
+
+Notes:
+* Requires package to be built as a distribution package.
+* Optional `pkg_background` parameter to provide a background image for the distribution package.
+  * Image recommended to be
+  * Optional `pkg_background_dark` parameter to provide a dark mode background image.
+    * If not provided, `pkg_background` will be used for both light and dark mode.
+* Optional `pkg_title` parameter to provide a title for the distribution package.
+  * Configures as follows in the distribution package:
+    * Header: `Install {title}`
+    * Welcome: `Welcome to the {title} Installer`
+* Optional `pkg_welcome`, `pkg_readme` and `pkg_license` parameters to provide markdown content for the respective pages in the distribution package.
+
+```py
+Packages(
+    pkg_output="Sample-Install.pkg",
+    pkg_bundle_id="com.myapp.installer",
+    pkg_file_structure={
+        "Samples/MyApp/MyApp.app": "/Applications/MyApp.app",
+    },
+    pkg_as_distribution=True,
+    pkg_welcome="# Welcome\n\nThis is a sample welcome message written in markdown.",
+    pkg_readme="# Read Me\n\nThis is a sample README written in markdown.",
+    pkg_license="# License\n\nThis is a sample license written in markdown.",
+    pkg_title="RIPEDA's Sample App",
+    pkg_background="Samples/MyApp/MyBackground.png",
 ),
 ```
+
+<img src="https://raw.githubusercontent.com/ripeda/macOS-Pkg-Builder/main/Samples/Demos/Markdown-Welcome.png" width="768" />
```

