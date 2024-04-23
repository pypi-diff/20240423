# Comparing `tmp/owimetadatabase_preprocessor-0.7.0b5.tar.gz` & `tmp/owimetadatabase_preprocessor-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owimetadatabase_preprocessor-0.7.0b5.tar", max compression
+gzip compressed data, was "owimetadatabase_preprocessor-0.8.0.tar", max compression
```

## Comparing `owimetadatabase_preprocessor-0.7.0b5.tar` & `owimetadatabase_preprocessor-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     1347 2024-03-14 08:41:05.276804 owimetadatabase_preprocessor-0.7.0b5/README.md
--rw-r--r--   0        0        0     2572 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/pyproject.toml
--rw-r--r--   0        0        0       91 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/__init__.py
--rw-r--r--   0        0        0       40 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/geometry/__init__.py
--rw-r--r--   0        0        0    10398 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/geometry/io.py
--rw-r--r--   0        0        0    38307 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/geometry/processing.py
--rw-r--r--   0        0        0    24884 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/geometry/structures.py
--rw-r--r--   0        0        0     7067 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/io.py
--rw-r--r--   0        0        0       41 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/locations/__init__.py
--rw-r--r--   0        0        0     8155 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/locations/io.py
--rw-r--r--   0        0        0        0 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/soil/__init__.py
--rw-r--r--   0        0        0    89735 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/soil/io.py
--rw-r--r--   0        0        0     6548 2024-03-14 08:41:05.280804 owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/utils.py
--rw-r--r--   0        0        0     3643 1970-01-01 00:00:00.000000 owimetadatabase_preprocessor-0.7.0b5/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-23 13:42:33.936551 owimetadatabase_preprocessor-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1471 2024-04-23 13:42:33.936551 owimetadatabase_preprocessor-0.8.0/README.md
+-rw-r--r--   0        0        0     2535 2024-04-23 13:42:33.936551 owimetadatabase_preprocessor-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/fatigue/__init__.py
+-rw-r--r--   0        0        0    34147 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/fatigue/data_objects.py
+-rw-r--r--   0        0        0    24890 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/fatigue/io.py
+-rw-r--r--   0        0        0       40 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/__init__.py
+-rw-r--r--   0        0        0    11835 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/io.py
+-rw-r--r--   0        0        0    38307 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/processing.py
+-rw-r--r--   0        0        0    24884 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/structures.py
+-rw-r--r--   0        0        0     7067 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/io.py
+-rw-r--r--   0        0        0       41 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/locations/__init__.py
+-rw-r--r--   0        0        0     8155 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/locations/io.py
+-rw-r--r--   0        0        0        0 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/soil/__init__.py
+-rw-r--r--   0        0        0    87680 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/soil/io.py
+-rw-r--r--   0        0        0     7268 2024-04-23 13:42:33.940551 owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/utils.py
+-rw-r--r--   0        0        0     3748 1970-01-01 00:00:00.000000 owimetadatabase_preprocessor-0.8.0/PKG-INFO
```

### Comparing `owimetadatabase_preprocessor-0.7.0b5/README.md` & `owimetadatabase_preprocessor-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 
 In your desired virtual environment and directory with Python 3 and pip installed:
 
 ``git clone <repo-github-address>``
 
 ``pip install <repo-local-name>``
 
+## Installation (beta)
+
+In case you want to try the latest beta-version (if it is more advanced than the latest stable one):
+
+``pip install owimetadatabase-preprocessor --pre``
+
 ## Contributing
 
 If you want to contribute to the development of the package, you can, in your desired virtual environment and directory with Python 3 and pip installed:
 
 ``git clone <repo-address>``
 
 ``pip install -e <repo-name>/[dev]``
@@ -34,8 +40,8 @@
 
 ## Acknowledgements
 
 This package was developed as part of the ETF Smartlife (FOD165) and WILLOW (EUAR157) projects.
 
 ## License
 
-The package is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).
+The package is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
```

### Comparing `owimetadatabase_preprocessor-0.7.0b5/pyproject.toml` & `owimetadatabase_preprocessor-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "owimetadatabase-preprocessor"
-version = "0.7.0-beta.5"
+version = "0.8.0"
 description = "Package for preprocessing data from owimetadatabase."
 authors = ["arsmlnkv <melnikov.arsene@gmail.com>"]
 readme = "README.md"
 homepage = "https://owi-lab.github.io/owimetadatabase-preprocessor/"
 repository = "https://github.com/OWI-Lab/owimetadatabase-preprocessor"
-license = "Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License"
+license = "GNU General Public License v3.0"
 keywords = ["owimetadatabase"]
 
 
 [tool.poetry.dependencies]
 # Main and dev dependencies are separated but dev dependencies are not grouped 
 # and put into optional to fascilitate pip usage. 
 # Main dependencies
@@ -19,14 +19,15 @@
 requests = ">=2.30.0, <3.0.0"
 matplotlib = "^3.8.0"
 numpy = "^1.26.0"
 pandas = "^2.0.0"
 groundhog = ">=0.11.0"
 pyproj = ">=3.6.0, <4.0.0"
 scipy = "^1.12.0"
+tqdm = ">=4.66.2"
 python-dotenv = "^1.0.0"
 
 
 # Development dependencies
 pytest = { version = "^8.0.0", optional = true }
 pytest-mock = { version = "*", optional = true }
 pytest-xdist = { version = "*", optional = true }
```

### Comparing `owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/geometry/io.py` & `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,48 @@
         """
         url_params = {}  # type: Dict[str, str]
         url_data_type = "materials"
         output_type = "list"
         df, df_add = self.process_data(url_data_type, url_params, output_type)
         return {"data": df, "exists": df_add["existance"]}
 
+    def get_subassembly_objects(
+        self, turbine: str, subassembly: str = None
+    ) -> Dict[str, SubAssembly]:
+        """Get all subassemblies for a given turbine, divided by type.
+
+        :param turbine: Turbine title (e.g. 'BBC01')
+        :param subassembly: Sub-assembly type (e.g. 'MP', 'TW', 'TP')
+        :return: Dictionary with the following keys:
+
+            - "TW": SubAssembly object for the tower
+            - "TP": SubAssembly object for the transition piece
+            - "MP": SubAssembly object for the monopile
+        """
+        url_data_type = "subassemblies"
+        if subassembly is not None:
+            url_params = {"asset__title": turbine, "subassembly_type": subassembly}
+        else:
+            url_params = {"asset__title": turbine}
+        resp = self.send_request(url_data_type, url_params)
+        self.check_request_health(resp)
+        if not resp.json():
+            raise ValueError("No subassemblies found for " + str(turbine))
+
+        material_data = self.get_materials()
+        if material_data["exists"]:
+            materials = material_data["data"]
+        else:
+            raise ValueError("No materials found in the database.")
+
+        sas = [SubAssembly(materials, item, api_object=self) for item in resp.json()]
+        sas_types = [j["subassembly_type"] for j in resp.json()]
+        subassemblies = {k: v for (k, v) in zip(sas_types, sas)}
+        return subassemblies
+
     def get_owt_geometry_processor(
         self,
         turbines: Union[str, List[str]],
         tower_base: Union[float, List[float], None] = None,
         monopile_head: Union[float, List[float], None] = None,
     ) -> OWTs:
         """Return the required processing class.
```

### Comparing `owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/geometry/processing.py` & `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/processing.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/geometry/structures.py` & `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/geometry/structures.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/io.py` & `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/locations/io.py` & `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/locations/io.py`

 * *Files identical despite different names*

### Comparing `owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/soil/io.py` & `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/soil/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         while True:
             url_params["offset"] = radius
             url_data_type = api_url
             output_type = "list"
             df, df_add = self.process_data(url_data_type, url_params, output_type)
             if df_add["existance"]:
                 break
-            warnings.warn("Expanding search radius to")
             radius *= 2
             warnings.warn(f"Expanding search radius to {radius: .1f}km")
             if radius > radius_max:
                 raise ValueError(
                     f"No locations found within {radius_max}km radius. Check your input information."
                 )
         return df
@@ -181,18 +180,18 @@
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, str, float, None]]:
         """Get the entity closest to a certain point in 2D with optional query arguments (cylindrical search area).
 
         :param api_url: End-point for the API
         :param latitude: Latitude of the central point in decimal format
         :param longitude: Longitude of the central point in decimal format
-        :param initialradius: Initial search radius around the central point in km, the search radius is increased
+        :param radius_init: Initial search radius around the central point in km, the search radius is increased
             until locations are found
         :param target_srid: SRID for the offset calculation in meters
-        :param **kwargs: Optional keyword arguments e.g. ``campaign__projectsite__title__icontains='HKN'``
+        :param kwargs: Optional keyword arguments e.g. ``campaign__projectsite__title__icontains='HKN'``
         :return:  Dictionary with the following keys:
 
             - 'data': Pandas dataframe with the test location data for each location in the specified search area
             - 'id': ID of the closest test location
             - 'title': Title of the closest test location
             - 'offset [m]': Offset in meters from the specified point
         """
@@ -210,31 +209,31 @@
 
     def get_closest_entity_3d(
         self,
         api_url: str,
         latitude: float,
         longitude: float,
         depth: float,
-        radius_init: int = 1,
+        radius_init: float = 1.0,
         target_srid: str = "25831",
         sampletest: bool = True,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, str, float, None]]:
         """Get the entity closest to a certain point in 3D (spherical search area) with optional query arguments.
 
         :param api_url: End-point for the API
         :param latitude: Latitude of the central point in decimal format
         :param longitude: Longitude of the central point in decimal format
-        :param depth of the central point in meters below seabed
-        :param initialradius: Initial search radius around the central point in km, the search radius is increased
+        :param depth: of the central point in meters below seabed
+        :param radius_init: Initial search radius around the central point in km, the search radius is increased
             until locations are found
         :param target_srid: SRID for the offset calculation in meters
         :param sampletest: Boolean indicating whether a sample or sample test needs to be retrieved
             (default is True to search for sample tests)
-        :param **kwargs: Optional keyword arguments e.g. ``campaign__projectsite__title__icontains='HKN'``
+        :param kwargs: Optional keyword arguments e.g. ``campaign__projectsite__title__icontains='HKN'``
         :return: Dictionary with the following keys:
 
             - 'data': Pandas dataframe with the test location data for each location in the specified search area
             - 'id': ID of the closest test location
             - 'title': Title of the closest test location
             - 'offset [m]': Offset in meters from the specified point
         """
@@ -269,16 +268,16 @@
         url_data_type = "surveycampaign"
         output_type = "list"
         df, df_add = self.process_data(url_data_type, url_params, output_type)
         return {"data": df, "exists": df_add["existance"]}
 
     def get_surveycampaign_detail(
         self,
-        projectsite: Union[str, None] = None,
-        campaign: Union[str, None] = None,
+        projectsite: str,
+        campaign: str,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, bool, int, None]]:
         """Get details for a specific survey campaign.
 
         :param projectsite: Name of the projectsite (e.g. "Nobelwind")
         :param campaign: Title of the survey campaign (e.g. "Borehole campaign")
         :return: Dictionary with the following keys:
@@ -315,15 +314,15 @@
             **kwargs,
         )
 
     def get_closest_testlocation(
         self,
         latitude: float,
         longitude: float,
-        radius_init: float = 1,
+        radius: float = 1.0,
         target_srid: str = "25831",
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, str, float, None]]:
         """Get the soil test location closest to a certain point with the name containing a certain string.
 
         :param latitude: Latitude of the central point in decimal format
         :param longitude: Longitude of the central point in decimal format
@@ -334,59 +333,56 @@
             - 'title': Title of the closest test location
             - 'offset [m]': Offset in meters from the specified point
         """
         return self.get_closest_entity_2d(
             api_url="testlocationproximity",
             latitude=latitude,
             longitude=longitude,
-            initialradius=radius_init,
+            radius_init=radius,
             target_srid=target_srid,
             **kwargs,
         )
 
     def get_testlocations(
         self,
         projectsite: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        location: Union[str, None] = None,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, bool, None]]:
         """Get the geotechnical test locations corresponding to the given search criteria.
 
-        :param projectsite: Name of the projectsite under consideration (e.g. "Nobelwind")
+        :param projectsite: Name of the projectsite under consideration (e.g. "Nobelwind", optional, default is None)
         :param campaign: Name of the survey campaign (optional, default is None to return all locations in a projectsite)
-        :param location: Name of a specific location (optional, default is None to return all locations in a projectsite)
         :return: Dictionary with the following keys:
 
             - 'data': Pandas dataframe with the test location data for each location meeting the specified search criteria
             - 'exists': Boolean indicating whether matching records are found
         """
         url_params = {
             "projectsite": projectsite,
             "campaign": campaign,
-            "location": location,
         }
         url_params = {**url_params, **kwargs}
         url_data_type = "testlocation"
         output_type = "list"
         df, df_add = self.process_data(url_data_type, url_params, output_type)
         return {"data": df, "exists": df_add["existance"]}
 
     def get_testlocation_detail(
         self,
+        location: str,
         projectsite: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        location: Union[str, None] = None,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, bool, None]]:
         """Get the detailed information for a geotechnical test location.
 
-        :param projectsite: Name of the projectsite under consideration (e.g. "Nobelwind")
-        :param campaign: Name of the survey campaign (optional, default is None to return all locations in a projectsite)
-        :param location: Name of a specific location (optional, default is None to return all locations in a projectsite)
+        :param location: Name of a specific location (e.g. "CPT-888")
+        :param projectsite: Optional, name of the projectsite under consideration (e.g. "Nobelwind")
+        :param campaign: Optional, name of the survey campaign (e.g. "Borehole campaign")
         :return: Dictionary with the following keys:
 
             - 'id': id of the selected test location
             - 'data': Pandas dataframe with the test location data for each location meeting the specified search criteria
             - 'exists': Boolean indicating whether matching records are found
         """
         url_params = {
@@ -398,50 +394,24 @@
         url_data_type = "testlocation"
         output_type = "single"
         df, df_add = self.process_data(url_data_type, url_params, output_type)
         return {"id": df_add["id"], "data": df, "exists": df_add["existance"]}
 
     def testlocation_exists(
         self,
+        location: str,
         projectsite: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        location: Union[str, None] = None,
         **kwargs,
     ) -> Union[int, bool]:
         """Checks if the test location answering to the search criteria exists.
 
-        :param projectsite: Name of the projectsite under consideration (e.g. "Nobelwind")
-        :param campaign: Name of the survey campaign (optional, default is None to return all locations in a projectsite)
-        :param location: Name of a specific location (optional, default is None to return all locations in a projectsite)
-        :return: Returns the id if test location exists, False otherwise
-        """
-        url_params = {
-            "projectsite": projectsite,
-            "campaign": campaign,
-            "location": location,
-        }
-        url_params = {**url_params, **kwargs}
-        url_data_type = "testlocation"
-        output_type = "single"
-        _, df_add = self.process_data(url_data_type, url_params, output_type)
-        return df_add["id"] if df_add["existance"] else False
-
-    def testlocation_location_exists(
-        self,
-        projectsite: Union[str, None] = None,
-        campaign: Union[str, None] = None,
-        location: Union[str, None] = None,
-        **kwargs,
-    ) -> Union[int, bool]:
-        """Checks if the location answering to the search criteria for the test location exists.
-        If the test location id is required, run the method ``testlocation_exists`` instead.
-
-        :param projectsite: Name of the projectsite under consideration (e.g. "Nobelwind")
-        :param campaign: Name of the survey campaign (optional, default is None to return all locations in a projectsite)
-        :param location: Name of a specific location (optional, default is None to return all locations in a projectsite)
+        :param location: Name of a specific location (e.g. "CPT-888")
+        :param projectsite: Optional, name of the projectsite under consideration (e.g. "Nobelwind")
+        :param campaign: Optional, name of the survey campaign (e.g. "Borehole campaign")
         :return: Returns the id if test location exists, False otherwise
         """
         url_params = {
             "projectsite": projectsite,
             "campaign": campaign,
             "location": location,
         }
@@ -483,35 +453,33 @@
         :return: Dataframe with the available InSituTestType records
         """
         url_data_type = "insitutesttype"
         output_type = "list"
         df, df_add = self.process_data(url_data_type, {}, output_type)
         return {"data": df, "exists": df_add["existance"]}
 
-    def insitutest_type_exists(
-        self, testtype: Union[str, None] = None, **kwargs
-    ) -> Union[int, bool]:
+    def insitutest_type_exists(self, testtype: str, **kwargs) -> Union[int, bool]:
         """Checks if the in-situ test type answering to the search criteria exists and returns the id.
 
         :param testtype: Title of the in-situ test type (e.g. "Downhole PCPT")
         :return: Returns the id if the in-situ test type exists, False otherwise
         """
         url_params = {"testtype": testtype}
         url_params = {**url_params, **kwargs}
         url_data_type = "insitutesttype"
         output_type = "single"
         _, df_add = self.process_data(url_data_type, url_params, output_type)
         return df_add["id"] if df_add["existance"] else False
 
     def get_insitutests(
         self,
-        projectsite: str = None,
-        location: str = None,
-        testtype: str = None,
-        insitutest: str = None,
+        projectsite: Union[str, None] = None,
+        location: Union[str, None] = None,
+        testtype: Union[str, None] = None,
+        insitutest: Union[str, None] = None,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, bool, None]]:
         """Get the detailed information (measurement data) for an in-situ test of given type.
 
         :param projectsite: Name of the projectsite (e.g. "Nobelwind")
         :param location: Name of the test location (e.g. "CPT-7C")
         :param testtype: Name of the test type (e.g. "PCPT")
@@ -554,38 +522,38 @@
             **kwargs,
         )
 
     def get_closest_insitutest(
         self,
         latitude: float,
         longitude: float,
-        radius_init: float = 1,
+        radius: float = 1.0,
         target_srid: str = "25831",
         **kwargs,
     ):
         """Get the in-situ test closest to a certain point with the name containing a certain string.
 
         :param latitude: Latitude of the central point in decimal format
         :param longitude: Longitude of the central point in decimal format
-        :param initialradius: Initial search radius around the central point in km, the search radius is increased
+        :param radius: Initial search radius around the central point in km, the search radius is increased
             until locations are found
         :param target_srid: SRID for the offset calculation in meters
-        :param **kwargs: Optional keyword arguments e.g. ``campaign__projectsite__title__icontains='HKN'``
+        :param kwargs: Optional keyword arguments e.g. ``campaign__projectsite__title__icontains='HKN'``
         :return: Dictionary with the following keys:
 
             - 'data': Pandas dataframe with the in-situ test data for each in-situ test in the specified search area
             - 'id': ID of the closest in-situ test
             - 'title': Title of the closest in-situ test
             - 'offset [m]': Offset in meters from the specified point
         """
         return self.get_closest_entity_2d(
             api_url="insitutestproximity",
             latitude=latitude,
             longitude=longitude,
-            initialradius=radius_init,
+            radius_init=radius,
             target_srid=target_srid,
             **kwargs,
         )
 
     def _process_insitutest_dfs(self, df, cols):
         dfs = {k: None for k in cols}
         for col in cols:
@@ -626,27 +594,27 @@
             return cpt
         except Exception as err:
             warnings.warn(f"ERROR: PCPTProcessing object not created - {err}")
             return None
 
     def get_insitutest_detail(
         self,
+        insitutest: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         testtype: Union[str, None] = None,
-        insitutest: Union[str, None] = None,
         combine: bool = False,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, bool, requests.Response, None]]:
         """Get the detailed information (measurement data) for an in-situ test of give type.
 
+        :param insitutest: Name of the in-situ test
         :param projectsite: Name of the projectsite (e.g. "Nobelwind")
         :param location: Name of the test location (e.g. "CPT-7C")
         :param testtype: Name of the test type (e.g. "PCPT")
-        :param insitutest: Name of the in-situ test
         :param combine: Boolean indicating whether raw and processed data needs to be combined (default=False).
             If true, processed data columns are appended to the rawdata dataframe
         :param kwargs: Optional keyword arguments for further queryset filtering based on model attributes.
         :return: Dictionary with the following keys:
 
             - 'id': id of the selected test
             - 'insitutestsummary': Metadata of the insitu tests
@@ -670,40 +638,42 @@
         df_detail, df_add_detail = self.process_data(
             url_data_type, url_params, output_type
         )
         cols = ["rawdata", "processeddata", "conditions"]
         dfs = self._process_insitutest_dfs(df_detail, cols)
         if combine:
             df_raw = self._combine_dfs(dfs)
+        else:
+            df_raw = dfs["rawdata"]
         return {
             "id": df_add_detail["id"],
             "insitutestsummary": df_sum,
             "rawdata": df_raw,
             "processeddata": dfs["processeddata"],
             "conditions": dfs["conditions"],
             "response": df_add_detail["response"],
             "exists": df_add_sum["existance"],
         }
 
     def get_cpttest_detail(
         self,
+        insitutest: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         testtype: Union[str, None] = None,
-        insitutest: Union[str, None] = None,
         combine: bool = False,
         cpt: bool = True,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, bool, requests.Response, None]]:
         """Get the detailed information (measurement data) for an in-situ test of CPT type (seabed or downhole CPT)
 
+        :param insitutest: Name of the in-situ test
         :param projectsite: Name of the projectsite (e.g. "Nobelwind")
         :param location: Name of the test location (e.g. "CPT-7C")
         :param testtype: Name of the test type (e.g. "PCPT")
-        :param insitutest: Name of the in-situ test
         :param combine: Boolean indicating whether raw and processed data needs to be combined (default=False).
             If true, processed data columns are appended to the rawdata dataframe
         :param cpt: Boolean determining whether the in-situ test is a CPT or not.
             If True (default), a PCPTProcessing object is returned.
         :param kwargs: Optional keyword arguments for the cpt data loading.
             Note that further queryset filtering based on model attributes is not possible with this method.
             The in-situ test needs to be fully defined by the required arguments.
@@ -731,14 +701,16 @@
         df_detail, df_add_detail = self.process_data(
             url_data_type, url_params, output_type
         )
         cols = ["rawdata", "processeddata", "conditions"]
         dfs = self._process_insitutest_dfs(df_detail, cols)
         if combine:
             df_raw = self._combine_dfs(dfs)
+        else:
+            df_raw = dfs["rawdata"]
         dict_ = {
             "id": df_add_detail["id"],
             "insitutestsummary": df_sum,
             "rawdata": df_raw,
             "processeddata": dfs["processeddata"],
             "conditions": dfs["conditions"],
             "response": df_add_detail["response"],
@@ -749,26 +721,26 @@
             if cpt_ is not None:
                 dict_["cpt"] = cpt_
             return dict_
         return dict_
 
     def insitutest_exists(
         self,
+        insitutest: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         testtype: Union[str, None] = None,
-        insitutest: Union[str, None] = None,
         **kwargs,
     ) -> Union[int, bool]:
         """Checks if the in-situ test answering to the search criteria exists.
 
+        :param insitutest: Name of the in-situ test
         :param projectsite: Name of the projectsite (e.g. "Nobelwind")
         :param location: Name of the test location (e.g. "CPT-7C")
         :param testtype: Name of the test type (e.g. "PCPT")
-        :param insitutest: Name of the in-situ test
         :return: Returns the id if the in-situ test exists, False otherwise
         """
         url_params = {
             "projectsite": projectsite,
             "location": location,
             "testtype": testtype,
             "insitutest": insitutest,
@@ -828,38 +800,38 @@
             **kwargs,
         )
 
     def get_closest_soilprofile(
         self,
         latitude: float,
         longitude: float,
-        initialradius: float = 1.0,
+        radius: float = 1.0,
         target_srid: str = "25831",
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, str, float, None]]:
         """Get the soil profile closest to a certain point with additional conditions as optional keyword arguments.
 
         :param latitude: Latitude of the central point in decimal format
         :param longitude: Longitude of the central point in decimal format
-        :param initialradius: Initial search radius around the central point in km, the search radius is increased
+        :param radius: Initial search radius around the central point in km, the search radius is increased
             until locations are found
         :param target_srid: SRID for the offset calculation in meters
-        :param **kwargs: Optional keyword arguments e.g. ``location__title__icontains='HKN'``
+        :param kwargs: Optional keyword arguments e.g. ``location__title__icontains='HKN'``
         :return: Dictionary with the following keys:
 
             - 'data': Pandas dataframe with the soil profile data for each soil profile in the specified search area
             - 'id': ID of the closest in-situ test
             - 'title': Title of the closest in-situ test
             - 'offset [m]': Offset in meters from the specified point
         """
         return self.get_closest_entity_2d(
             api_url="soilprofileproximity",
             latitude=latitude,
             longitude=longitude,
-            initialradius=initialradius,
+            radius_init=radius,
             target_srid=target_srid,
             **kwargs,
         )
 
     def _convert_to_profile(self, df_sum, df_detail, profile_title, drop_info_cols):
         try:
             soilprofile_df = (
@@ -970,15 +942,15 @@
     ) -> pd.DataFrame:
         """Converts dataframes with soil profile data to a format suitable for PISA analysis.
 
         :param soil_profile: Groundhog SoilProfile object obtained through the get_soilprofile_detail method
         :param pw: Sea water density (default=1.025 t/m3)
         :param sbl: Sea bed level in mLAT coordinates
         :return: Dataframe containing soil model to carry out FE analysis through ```owi_monopylat``` of monopile
-        following PISA guidance.
+            following PISA guidance.
         """
         required_keys = [
             "Depth from [m]",
             "Depth to [m]",
             "Soil type",
             "Gmax from [kPa]",
             "Gmax to [kPa]",
@@ -1015,57 +987,55 @@
             },
             inplace=True,
         )
         return pisa_profile
 
     def soilprofile_exists(
         self,
+        soilprofile: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
-        soilprofile: Union[str, None] = None,
         **kwargs,
     ) -> Union[int, bool]:
-        """Checks if the in-situ test answering to the search criteria exists.
+        """Checks if the specific soil profile  exists.
 
+        :param soilprofile: Title of the soil profile (e.g. "Borehole log")
         :param projectsite: Name of the projectsite (e.g. "Nobelwind")
         :param location: Name of the test location (e.g. "CPT-7C")
-        :param soilprofile: Title of the soil profile (e.g. "Borehole log")
         :return: Returns the id if soil profile exists, False otherwise
         """
         url_params = {
             "projectsite": projectsite,
             "location": location,
             "soilprofile": soilprofile,
         }
         url_params = {**url_params, **kwargs}
         url_data_type = "soilprofiledetail"
         output_type = "single"
         _, df_add = self.process_data(url_data_type, url_params, output_type)
         return df_add["id"] if df_add["existance"] else False
 
-    def soiltype_exists(
-        self, soiltype: Union[str, None] = None, **kwargs
-    ) -> Union[int, bool]:
+    def soiltype_exists(self, soiltype: str, **kwargs) -> Union[int, bool]:
         """Checks if a soiltype with a given name exists.
 
         :param soiltype: Name of the soil type
         :return: id of the soil type if it exists, False otherwise
         """
         url_params = {"soiltype": soiltype}
         url_params = {**url_params, **kwargs}
         url_data_type = "soiltype"
         output_type = "single"
         _, df_add = self.process_data(url_data_type, url_params, output_type)
         return df_add["id"] if df_add["existance"] else False
 
     def soilunit_exists(
         self,
+        soilunit: str,
         projectsite: Union[str, None] = None,
         soiltype: Union[str, None] = None,
-        soilunit: Union[str, None] = None,
         **kwargs,
     ) -> Union[int, bool]:
         """Checks if a certain soil unit exists.
 
         :param projectsite: Name of the project site
         :param soiltype: Name of the soil type
         :param soilunit: Name of the soil unit
@@ -1154,15 +1124,15 @@
         url_params = {**url_params, **kwargs}
         url_data_type = "batchlabtestsummary"
         output_type = "list"
         df, df_add = self.process_data(url_data_type, url_params, output_type)
         return {"data": df, "exists": df_add["existance"]}
 
     def batchlabtesttype_exists(
-        self, batchlabtesttype: Union[str, None] = None, **kwargs
+        self, batchlabtesttype: str, **kwargs
     ) -> Union[int, bool]:
         """Checks if the geotechnical sample type answering to the search criteria exists.
 
         :param batchlabtesttype: Title of the batch lab test type
         :return: Returns the id if the sample type exists, False otherwise
         """
         url_params = {"testtype": batchlabtesttype}
@@ -1194,49 +1164,49 @@
             **kwargs,
         )
 
     def get_closest_batchlabtest(
         self,
         latitude: float,
         longitude: float,
-        initialradius: float = 1.0,
+        radius: float = 1.0,
         target_srid: str = "25831",
         **kwargs,
     ):
         """Gets the batch lab test closest to a certain point with the name containing a certain string.
 
         :param latitude: Latitude of the central point in decimal format
         :param longitude: Longitude of the central point in decimal format
-        :param initialradius: Initial search radius around the central point in km, the search radius is increased
+        :param radius: Initial search radius around the central point in km, the search radius is increased
             until locations are found
         :param target_srid: SRID for the offset calculation in meters
-        :param **kwargs: Optional keyword arguments e.g. ``location__title__icontains='BH'``
+        :param kwargs: Optional keyword arguments e.g. ``location__title__icontains='BH'``
         :return: Dictionary with the following keys:
 
             - 'data': Pandas dataframe with the batch lab test data for each batch lab test in the specified search area
             - 'id': ID of the closest batch lab test
             - 'title': Title of the closest batch lab test
             - 'offset [m]': Offset in meters from the specified point
         """
         return self.get_closest_entity_2d(
             api_url="batchlabtestproximity",
             latitude=latitude,
             longitude=longitude,
-            initialradius=initialradius,
+            radius_init=radius,
             target_srid=target_srid,
             **kwargs,
         )
 
     def get_batchlabtest_detail(
         self,
+        batchlabtest: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         testtype: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        batchlabtest: Union[str, None] = None,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, bool, requests.Response, None]]:
         """Retrieves detailed data for a specific batch lab test.
 
         :param projectsite: Title of the project site
         :param campaign: Title of the survey campaign
         :param location: Title of the test location
@@ -1277,28 +1247,28 @@
             "processeddata": dfs["processeddata"],
             "conditions": dfs["conditions"],
             "exists": df_add_sum["existance"],
         }
 
     def batchlabtest_exists(
         self,
+        batchlabtest: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         testtype: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        batchlabtest: Union[str, None] = None,
         **kwargs,
     ) -> Union[int, bool]:
         """Checks if the batch lab test answering to the search criteria exists.
 
+        :param batchlabtest: Title of the batch lab test
         :param projectsite: Project site name (e.g. 'Nobelwind')
         :param campaign: Title of the survey campaign
         :param location: Title of the test location
         :param testtype: Title of the test type
-        :param batchlabtest: Title of the batch lab test
         :return: Returns the id if batch lab test exists, False otherwise
         """
         url_params = {
             "projectsite": projectsite,
             "campaign": campaign,
             "location": location,
             "testtype": testtype,
@@ -1307,15 +1277,15 @@
         url_params = {**url_params, **kwargs}
         url_data_type = "batchlabtestdetail"
         output_type = "single"
         _, df_add = self.process_data(url_data_type, url_params, output_type)
         return df_add["id"] if df_add["existance"] else False
 
     def geotechnicalsampletype_exists(
-        self, sampletype: Union[str, None] = None, **kwargs
+        self, sampletype: str, **kwargs
     ) -> Union[int, bool]:
         """Checks if the geotechnical sample type answering to the search criteria exists.
 
         :param sampletype: Title of the sample type
         :return: Returns the id if the sample type exists, False otherwise
         """
         url_params = {"sampletype": sampletype}
@@ -1382,62 +1352,62 @@
         )
 
     def get_closest_geotechnicalsample(
         self,
         latitude: float,
         longitude: float,
         depth: float,
-        initialradius: float = 1.0,
+        radius: float = 1.0,
         target_srid: str = "25831",
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, str, float, None]]:
         """Gets the geotechnical sample closest to a certain point with the name containing a certain string.
 
         :param latitude: Latitude of the central point in decimal format
         :param longitude: Longitude of the central point in decimal format
         :param depth: Depth of the central point in meters below seabed
-        :param initialradius: Initial search radius around the central point in km, the search radius is increased
+        :param radius: Initial search radius around the central point in km, the search radius is increased
             until locations are found
         :param target_srid: SRID for the offset calculation in meters
-        :param **kwargs: Optional keyword arguments e.g. ``location__title__icontains='BH'``
+        :param kwargs: Optional keyword arguments e.g. ``location__title__icontains='BH'``
         :return: Dictionary with the following keys:
 
             - 'data': Pandas dataframe with the geotechnical sample data for each geotechnical sample
                 in the specified search area
             - 'id': ID of the closest batch lab test
             - 'title': Title of the closest batch lab test
             - 'offset [m]': Offset in meters from the specified point
         """
         return self.get_closest_entity_3d(
             api_url="geotechnicalsampleproximity",
             latitude=latitude,
             longitude=longitude,
             depth=depth,
-            initialradius=initialradius,
+            radius_init=radius,
             target_srid=target_srid,
             sampletest=False,
             **kwargs,
         )
 
     def get_geotechnicalsample_detail(
         self,
+        sample: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         sampletype: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        sample: Union[str, None] = None,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, bool, requests.Response, None]]:
         """Retrieves detailed data for a specific sample.
 
+        :param sample: Title of the sample
         :param projectsite: Title of the project site
         :param campaign: Title of the survey campaign
         :param location: Title of the test location
         :param sampletype: Title of the sample type
-        :param sample: Title of the sample
         :return: Dictionary with the following keys:
 
             - 'id': id for the selected soil profile
             - 'data': Metadata for the batch lab test
             - 'response': Response text
             - 'exists': Boolean indicating whether a matching record is found
         """
@@ -1457,28 +1427,28 @@
             "data": df,
             "response": df_add["response"],
             "exists": df_add["existance"],
         }
 
     def geotechnicalsample_exists(
         self,
+        sample: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         sampletype: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        sample: Union[str, None] = None,
         **kwargs,
     ) -> Union[int, bool]:
         """Checks if the geotechnical sample answering to the search criteria exists.
 
+        :param sample: Title of the sample
         :param projectsite: Project site name (e.g. 'Nobelwind')
         :param campaign: Title of the survey campaign
         :param location: Title of the test location
         :param sampletype: Title of the sample type
-        :param sample: Title of the sample
         :return: Returns the id if the geotechnical sample exists, False otherwise
         """
         url_params = {
             "projectsite": projectsite,
             "campaign": campaign,
             "location": location,
             "sampletype": sampletype,
@@ -1549,47 +1519,45 @@
         )
 
     def get_closest_sampletest(
         self,
         latitude: float,
         longitude: float,
         depth: float,
-        initialradius: float = 1.0,
+        radius: float = 1.0,
         target_srid: str = "25831",
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, str, float, None]]:
         """Gets the sample test closest to a certain point.
 
         :param latitude: Latitude of the central point in decimal format
         :param longitude: Longitude of the central point in decimal format
         :param Depth: Depth of the central point in meters below seabed
-        :param initialradius: Initial search radius around the central point in km, the search radius is increased
+        :param radius: Initial search radius around the central point in km, the search radius is increased
             until locations are found
         :param target_srid: SRID for the offset calculation in meters
-        :param **kwargs: Optional keyword arguments e.g. ``sample__location__title__icontains='BH'``
+        :param kwargs: Optional keyword arguments e.g. ``sample__location__title__icontains='BH'``
         :return: Dictionary with the following keys:
 
             - 'data': Pandas dataframe with the sample test data for each sample test in the specified search area
             - 'id': ID of the closest sample test
             - 'title': Title of the closest sample test
             - 'offset [m]': Offset in meters from the specified point
         """
         return self.get_closest_entity_3d(
             api_url="sampletestproximity",
             latitude=latitude,
             longitude=longitude,
             depth=depth,
-            initialradius=initialradius,
+            radius_init=radius,
             target_srid=target_srid,
             **kwargs,
         )
 
-    def sampletesttype_exists(
-        self, sampletesttype: Union[str, None] = None, **kwargs
-    ) -> Union[int, bool]:
+    def sampletesttype_exists(self, sampletesttype: str, **kwargs) -> Union[int, bool]:
         """Checks if the sample test type answering to the search criteria exists.
 
         :param sampletesttype: Title of the sample test type
         :return: Returns the id if the sample test type exists, False otherwise
         """
         url_params = {"testtype": sampletesttype}
         url_params = {**url_params, **kwargs}
@@ -1611,30 +1579,30 @@
         url_data_type = "sampletesttype"
         output_type = "list"
         df, df_add = self.process_data(url_data_type, kwargs, output_type)
         return {"data": df, "exists": df_add["existance"]}
 
     def get_sampletest_detail(
         self,
+        sampletest: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         testtype: Union[str, None] = None,
         sample: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        sampletest: Union[str, None] = None,
         **kwargs,
     ) -> Dict[str, Union[pd.DataFrame, int, bool, requests.Response, None]]:
         """Retrieves detailed information on a specific sample test based on the specified search criteria.
 
+        :param sampletest: Title of the sample test
         :param projectsite: Title of the project site
         :param campaign: Title of the survey campaign
         :param location: Title of the test location
         :param sample: Title of the sample
         :param testtype: Title of the test type
-        :param sampletest: Title of the sample test
         :return: Dictionary with the following keys:
 
             - 'id': id for the selected soil profile
             - 'summary': Metadata for the batch lab test
             - 'response': Response text
             - 'rawdata': Dataframe with the raw data
             - 'processeddata': Dataframe with the raw data
@@ -1667,30 +1635,30 @@
             "conditions": dfs["conditions"],
             "response": df_add_detail["response"],
             "exists": df_add_sum["existance"],
         }
 
     def sampletest_exists(
         self,
+        sampletest: str,
         projectsite: Union[str, None] = None,
         location: Union[str, None] = None,
         testtype: Union[str, None] = None,
         sample: Union[str, None] = None,
         campaign: Union[str, None] = None,
-        sampletest: Union[str, None] = None,
         **kwargs,
     ) -> Union[int, bool]:
         """Checks if the batch lab test answering to the search criteria exists.
 
+        :param sampletest: Title of the sample test
         :param projectsite: Title of the project site
         :param campaign: Title of the survey campaign
         :param location: Title of the test location
         :param sample: Title of the sample
         :param testtype: Title of the test type
-        :param sampletest: Title of the sample test
         :return: Returns the id if the sample test exists, False otherwise
         """
         url_params = {
             "projectsite": projectsite,
             "campaign": campaign,
             "location": location,
             "sample": sample,
```

### Comparing `owimetadatabase_preprocessor-0.7.0b5/src/owimetadatabase_preprocessor/utils.py` & `owimetadatabase_preprocessor-0.8.0/src/owimetadatabase_preprocessor/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -179,7 +179,29 @@
                 data[i]["outline"] = tuple(data[i]["outline"])
     elif isinstance(data, dict):
         if "outline" in data.keys() and data["outline"] is not None:
             data["outline"] = tuple(data["outline"])
     else:
         raise ValueError("Not supported data type.")
     return data
+
+
+def hex_to_dec(value):
+    """Return [red, green, blue, alpha] for the color given as #rrggbbaa."""
+
+    def _hex_to_dec(value):
+        value = value.lstrip("#") if value.startswith("#") else value
+        if len(value) != 6:
+            if len(value) != 8:
+                raise ValueError("len(value) != 6 or 8 (excluding #)")
+        col = value[0:6]
+        alpha = value[6:] / 100 if len(value) == 8 else 1
+        lv = len(col)
+        return list(
+            int(col[i : i + lv // 3], 16) / 255  # noqa: E203
+            for i in range(0, lv, lv // 3)
+        ) + [alpha]
+
+    if isinstance(value, str):
+        value = [value]
+    elif isinstance(value, list):
+        return [_hex_to_dec(_) for _ in value]
```

### Comparing `owimetadatabase_preprocessor-0.7.0b5/PKG-INFO` & `owimetadatabase_preprocessor-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: owimetadatabase-preprocessor
-Version: 0.7.0b5
+Version: 0.8.0
 Summary: Package for preprocessing data from owimetadatabase.
 Home-page: https://owi-lab.github.io/owimetadatabase-preprocessor/
-License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
+License: GNU General Public License v3.0
 Keywords: owimetadatabase
 Author: arsmlnkv
 Author-email: melnikov.arsene@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -38,14 +38,15 @@
 Requires-Dist: pytest-xdist ; extra == "dev"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: requests-mock ; extra == "dev"
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
 Requires-Dist: sphinx (>=7.0.0,<8.0.0) ; extra == "dev"
 Requires-Dist: sphinx_rtd_theme ; extra == "dev"
+Requires-Dist: tqdm (>=4.66.2)
 Requires-Dist: types-Pygments ; extra == "dev"
 Requires-Dist: types-colorama ; extra == "dev"
 Requires-Dist: types-requests ; extra == "dev"
 Requires-Dist: types-setuptools ; extra == "dev"
 Project-URL: Repository, https://github.com/OWI-Lab/owimetadatabase-preprocessor
 Description-Content-Type: text/markdown
 
@@ -63,14 +64,20 @@
 
 In your desired virtual environment and directory with Python 3 and pip installed:
 
 ``git clone <repo-github-address>``
 
 ``pip install <repo-local-name>``
 
+## Installation (beta)
+
+In case you want to try the latest beta-version (if it is more advanced than the latest stable one):
+
+``pip install owimetadatabase-preprocessor --pre``
+
 ## Contributing
 
 If you want to contribute to the development of the package, you can, in your desired virtual environment and directory with Python 3 and pip installed:
 
 ``git clone <repo-address>``
 
 ``pip install -e <repo-name>/[dev]``
@@ -85,8 +92,8 @@
 
 ## Acknowledgements
 
 This package was developed as part of the ETF Smartlife (FOD165) and WILLOW (EUAR157) projects.
 
 ## License
 
-The package is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).
+The package is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html).
```

