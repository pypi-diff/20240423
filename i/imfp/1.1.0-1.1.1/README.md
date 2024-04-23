# Comparing `tmp/imfp-1.1.0.tar.gz` & `tmp/imfp-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imfp-1.1.0.tar", max compression
+gzip compressed data, was "imfp-1.1.1.tar", max compression
```

## Comparing `imfp-1.1.0.tar` & `imfp-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      596 2023-04-29 21:06:07.370012 imfp-1.1.0/imfp/__init__.py
--rw-r--r--   0        0        0     2239 2023-04-29 21:06:07.415432 imfp-1.1.0/imfp/admin.py
--rw-r--r--   0        0        0    16124 2023-04-28 18:38:01.551682 imfp-1.1.0/imfp/data.py
--rw-r--r--   0        0        0     9577 2023-04-29 21:06:07.573604 imfp-1.1.0/imfp/utils.py
--rw-r--r--   0        0        0    11558 2023-03-25 14:05:34.578038 imfp-1.1.0/LICENSE
--rw-r--r--   0        0        0     1050 2023-04-29 21:09:08.385198 imfp-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    21042 2023-04-29 21:06:20.465633 imfp-1.1.0/README.md
--rw-r--r--   0        0        0    21358 1970-01-01 00:00:00.000000 imfp-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 19:52:28.684416 imfp-1.1.1/LICENSE
+-rw-r--r--   0        0        0    21040 2024-04-23 19:52:28.684416 imfp-1.1.1/README.md
+-rw-r--r--   0        0        0      571 2024-04-23 19:52:28.688416 imfp-1.1.1/imfp/__init__.py
+-rw-r--r--   0        0        0     2167 2024-04-23 19:52:28.688416 imfp-1.1.1/imfp/admin.py
+-rw-r--r--   0        0        0    15698 2024-04-23 19:52:28.688416 imfp-1.1.1/imfp/data.py
+-rw-r--r--   0        0        0     9115 2024-04-23 19:52:28.688416 imfp-1.1.1/imfp/utils.py
+-rw-r--r--   0        0        0      996 2024-04-23 19:52:28.688416 imfp-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    22062 1970-01-01 00:00:00.000000 imfp-1.1.1/PKG-INFO
```

### Comparing `imfp-1.1.0/imfp/admin.py` & `imfp-1.1.1/imfp/admin.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from os import environ
-from warnings import warn
-from typing import Union
-
-
-def set_imf_app_name(name: str = "imfp"):
-    """
-    Set the IMF Application Name.
-
-    Set a unique application name to be used in requests to the IMF API as an
-    environment variable.
-
-    Args:
-        name (str, optional): A string representing the application name.
-        Default is "imfp".
-
-    Returns:
-        None
-
-    Raises:
-        ValueError: If the provided name is not a valid string or contains
-        forbidden characters.
-
-    Examples:
-        imf_app_name("my_custom_app_name")
-    """
-
-    if not isinstance(name, str) or len(name) > 255:
-        raise ValueError(
-            "Please provide a valid string as the application "
-            "name (max length: 255 characters)."
-        )
-
-    if name == "imfp" or name == "":
-        warn(
-            "Best practice is to choose a unique app name. Use of a default "
-            "or empty app name may result in hitting API rate limits and "
-            "being blocked by the API.",
-            UserWarning,
-        )
-
-    forbidden_chars = set(range(32)) | {127}
-    if any(ord(c) in forbidden_chars for c in name):
-        raise ValueError(
-            "The application name contains forbidden characters. "
-            "Please remove control characters and non-printable "
-            "ASCII characters."
-        )
-
-    environ["IMF_APP_NAME"] = name
-
-    return None
-
-
-def set_imf_wait_time(wait_time: Union[int, float] = 1.5):
-    """
-    Set the IMF wait time as an environment variable.
-
-    Args:
-        wait_time (Union[int, float], optional): The wait time in seconds to be set as an environment variable. Defaults to 1.5.
-
-    Raises:
-        TypeError: If the provided wait_time is not a numeric value (int or float).
-        ValueError: If the provided wait_time is not greater than 0.
-    """
-    if not isinstance(wait_time, (int, float)):
-        raise TypeError("Rate limit wait time must be a numeric value (int or float).")
-
-    if wait_time >= 0:
-        environ["IMF_WAIT_TIME"] = str(wait_time)
-    else:
-        raise ValueError("Rate limit wait time must be greater than or equal to 0.")
+from os import environ
+from warnings import warn
+from typing import Union
+
+
+def set_imf_app_name(name: str = "imfp"):
+    """
+    Set the IMF Application Name.
+
+    Set a unique application name to be used in requests to the IMF API as an
+    environment variable.
+
+    Args:
+        name (str, optional): A string representing the application name.
+        Default is "imfp".
+
+    Returns:
+        None
+
+    Raises:
+        ValueError: If the provided name is not a valid string or contains
+        forbidden characters.
+
+    Examples:
+        imf_app_name("my_custom_app_name")
+    """
+
+    if not isinstance(name, str) or len(name) > 255:
+        raise ValueError(
+            "Please provide a valid string as the application "
+            "name (max length: 255 characters)."
+        )
+
+    if name == "imfp" or name == "":
+        warn(
+            "Best practice is to choose a unique app name. Use of a default "
+            "or empty app name may result in hitting API rate limits and "
+            "being blocked by the API.",
+            UserWarning,
+        )
+
+    forbidden_chars = set(range(32)) | {127}
+    if any(ord(c) in forbidden_chars for c in name):
+        raise ValueError(
+            "The application name contains forbidden characters. "
+            "Please remove control characters and non-printable "
+            "ASCII characters."
+        )
+
+    environ["IMF_APP_NAME"] = name
+
+    return None
+
+
+def set_imf_wait_time(wait_time: Union[int, float] = 1.5):
+    """
+    Set the IMF wait time as an environment variable.
+
+    Args:
+        wait_time (Union[int, float], optional): The wait time in seconds to be set as an environment variable. Defaults to 1.5.
+
+    Raises:
+        TypeError: If the provided wait_time is not a numeric value (int or float).
+        ValueError: If the provided wait_time is not greater than 0.
+    """
+    if not isinstance(wait_time, (int, float)):
+        raise TypeError("Rate limit wait time must be a numeric value (int or float).")
+
+    if wait_time >= 0:
+        environ["IMF_WAIT_TIME"] = str(wait_time)
+    else:
+        raise ValueError("Rate limit wait time must be greater than or equal to 0.")
```

### Comparing `imfp-1.1.0/imfp/data.py` & `imfp-1.1.1/imfp/data.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,426 +1,426 @@
-from pandas import DataFrame, Series, concat
-from warnings import warn
-from .utils import _download_parse, _imf_dimensions, _imf_metadata
-from urllib.parse import urlencode
-
-
-def imf_databases(times=3):
-    """
-    List IMF database IDs and descriptions
-
-    Returns a DataFrame with database_id and text description for each
-    database available through the IMF API endpoint.
-
-    Parameters
-    ----------
-    times : int, optional, default 3
-        Maximum number of API requests to attempt.
-
-    Returns
-    -------
-    pandas.DataFrame
-        DataFrame containing database_id and description columns.
-
-    Examples
-    --------
-    # Return first 6 IMF database IDs and descriptions
-    databases = imf_databases()
-    """
-    url = "http://dataservices.imf.org/REST/SDMX_JSON.svc/Dataflow"
-    raw_dl = _download_parse(url, times)
-
-    database_id = [
-        dataflow["KeyFamilyRef"]["KeyFamilyID"]
-        for dataflow in raw_dl["Structure"]["Dataflows"]["Dataflow"]
-    ]
-
-    description = [
-        dataflow["Name"]["#text"]
-        for dataflow in raw_dl["Structure"]["Dataflows"]["Dataflow"]
-    ]
-    database_list = DataFrame({"database_id": database_id, "description": description})
-    return database_list
-
-
-def imf_parameters(database_id, times=2):
-    """
-    List input parameters and available parameter values for use in
-    making API requests from a given IMF database.
-
-    Parameters
-    ----------
-    database_id : str
-        A database_id from imf_databases().
-    times : int, optional, default 3
-        Maximum number of API requests to attempt.
-
-    Returns
-    -------
-    dict
-        A dictionary of DataFrames, where each key corresponds to an input
-        parameter for API requests from the database. All values are DataFrames
-        with an 'input_code' column and a 'description' column. The
-        'input_code' column is a character list of all possible input codes for
-        that parameter when making requests from the IMF API endpoint. The
-        'descriptions' column is a character list of text descriptions of what
-        each input code represents.
-
-    Examples
-    --------
-    # Fetch the full list of indicator codes and descriptions for the Primary
-    # Commodity Price System database
-    params = imf_parameters(database_id='PCPS')
-    """
-    if not database_id:
-        raise ValueError("Must supply database_id. Use imf_databases to find.")
-
-    url = "http://dataservices.imf.org/REST/SDMX_JSON.svc/CodeList/"
-    try:
-        codelist = _imf_dimensions(database_id, times)
-    except ValueError as e:
-        if "There is an issue" in str(e):
-            raise ValueError(
-                f"{e}\n\nDid you supply a valid database_id? "
-                "Use imf_databases to find."
-            )
-        else:
-            raise ValueError(e)
-
-    def fetch_parameter_data(k, url, times):
-        if codelist.loc[k, "parameter"] == "freq":
-            return DataFrame(
-                {
-                    "input_code": ["A", "M", "Q"],
-                    "description": ["Annual", "Monthly", "Quarterly"],
-                }
-            )
-        else:
-            raw = _download_parse(url + codelist.loc[k, "code"], times)["Structure"][
-                "CodeLists"
-            ]["CodeList"]["Code"]
-            if isinstance(raw, list):
-                return DataFrame(
-                    {
-                        "input_code": [code["@value"] for code in raw],
-                        "description": [code["Description"]["#text"] for code in raw],
-                    }
-                )
-            else:
-                return DataFrame(
-                    {
-                        "input_code": [raw["@value"]],
-                        "description": [raw["Description"]["#text"]],
-                    }
-                )
-
-    parameter_list = {
-        codelist.loc[k, "parameter"]: fetch_parameter_data(k, url, times)
-        for k in range(codelist.shape[0])
-    }
-
-    return parameter_list
-
-
-def imf_parameter_defs(database_id, times=3, inputs_only=True):
-    """
-    Get text descriptions of input parameters used in making API
-    requests from a given IMF database
-
-    Parameters
-    ----------
-    database_id : str
-        A database_id from imf_databases().
-    times : int, optional, default 3
-        Maximum number of API requests to attempt.
-    inputs_only : bool, optional, default False
-        Whether to return only parameters used as inputs in API requests,
-        or also output variables.
-
-    Returns
-    -------
-    pandas.DataFrame
-        A DataFrame of input parameters used in making API requests
-        from a given IMF database, along with text descriptions or definitions
-        of those parameters. Useful in cases when parameter names returned by
-        imf_databases() are not self-explanatory. (Note that the usefulness
-        of text descriptions can be uneven, depending on the database design.)
-
-    Examples
-    --------
-    # Get names and text descriptions of parameters used in IMF API calls to
-    # the Primary Commodity Price System database
-    param_defs = imf_parameter_defs(database_id='PCPS')
-    """
-    if not database_id:
-        raise ValueError("Must supply database_id. Use imf_databases to find.")
-
-    try:
-        parameterlist = _imf_dimensions(database_id, times, inputs_only)[
-            ["parameter", "description"]
-        ]
-    except ValueError as e:
-        if "There is an issue" in str(e):
-            raise ValueError(
-                f"{e}\n\nDid you supply a valid database_id? "
-                "Use imf_databases to find."
-            )
-        else:
-            raise ValueError(e)
-
-    return parameterlist
-
-
-def imf_dataset(
-    database_id: str,
-    parameters: dict = None,
-    start_year: int = None,
-    end_year: int = None,
-    return_raw: bool = False,
-    print_url: bool = False,
-    times: int = 3,
-    include_metadata: bool = False,
-    **kwargs,
-):
-    """
-    Download a data series from the IMF.
-
-    Args:
-        database_id (str): Database ID for the database from which you would
-                           like to request data. Can be found using
-                           imf_databases().
-        parameters (dict): Dictionary of data frames providing input parameters
-                           for your API request. Retrieve dictionary of all
-                           possible input parameters using imf_parameters() and
-                           filter each data frame in the dictionary to reduce
-                           it to the inputs you want.
-        start_year (int, optional): Four-digit year. Earliest year for which
-                                    you would like to request data.
-        end_year (int, optional): Four-digit year. Latest year for which you
-                                  would like to request data.
-        return_raw (bool, optional): Whether to return the raw list returned by
-                                     the API instead of a cleaned-up data
-                                     frame.
-        print_url (bool, optional): Whether to print the URL used in the API
-                                    call.
-        times (int, optional): Maximum number of requests to attempt.
-        include_metadata (bool, optional): Whether to return the database
-                                           metadata header along with the data
-                                           series.
-        **kwargs: Additional keyword arguments for specifying parameters as
-                  separate arguments. Use imf_parameters() to identify which
-                  parameters to use for requests from a given database and to
-                  see all valid input codes for each parameter.
-
-    Returns:
-        If return_raw == False and include_metadata == False, returns a pandas
-        DataFrame with the data series. If return_raw == False but
-        include_metadata == True, returns a tuple whose first item is the
-        database header, and whose second item is the pandas DataFrame. If
-        return_raw == True, returns the raw JSON fetched from the API endpoint.
-    """
-
-    if database_id is None:
-        raise ValueError("Missing required database_id argument.")
-
-    if not isinstance(database_id, str):
-        raise ValueError("database_id must be a string.")
-
-    years = {}
-    if start_year is not None:
-        try:
-            start_year = str(start_year)
-            if start_year.isdigit() and len(start_year) == 4:
-                years["startPeriod"] = start_year
-            else:
-                raise ValueError(
-                    "start_year must be a four-digit number, "
-                    "either integer or string."
-                )
-        except Exception:
-            raise ValueError(
-                "start_year must be a four-digit number, either " "integer or string."
-            )
-    if end_year is not None:
-        try:
-            end_year = str(end_year)
-            if end_year.isdigit() and len(end_year) == 4:
-                years["endPeriod"] = end_year
-            else:
-                raise ValueError(
-                    "end_year must be a four-digit number, " "either integer or string"
-                )
-        except Exception:
-            raise ValueError(
-                "end_year must be a four-digit number, " "either integer or string"
-            )
-
-    data_dimensions = imf_parameters(database_id, times)
-
-    if parameters is not None:
-        if kwargs:
-            warn(
-                "Parameters list argument cannot be combined with character "
-                "vector parameters arguments. Character vector parameters "
-                "arguments will be ignored."
-            )
-        for key in parameters:
-            if key not in data_dimensions:
-                raise ValueError(
-                    f"{key} not valid parameter(s) for the "
-                    f"{database_id} database. Use "
-                    f"imf_parameters('{database_id}') to get "
-                    "valid parameters."
-                )
-            invalid_keys = []
-            for x in list(parameters[key]["input_code"]):
-                if x not in list(data_dimensions[key]["input_code"]):
-                    invalid_keys.append(x)
-            if len(invalid_keys) > 0:
-                warn(
-                    f"{invalid_keys} not valid value(s) for {key} and will "
-                    f"be ignored. Use imf_parameters('{database_id}') to get "
-                    "valid parameters."
-                )
-            if (
-                set(parameters[key]["input_code"])
-                == set(data_dimensions[key]["input_code"])
-                or len(parameters[key]) == 0
-            ):
-                data_dimensions[key] = data_dimensions[key].iloc[0:0]
-            data_dimensions[key] = data_dimensions[key].iloc[
-                [
-                    index
-                    for index, x in enumerate(data_dimensions[key]["input_code"])
-                    if x in list(parameters[key]["input_code"])
-                ]
-            ]
-        for key in data_dimensions:
-            if key not in parameters:
-                data_dimensions[key] = data_dimensions[key].iloc[0:0]
-
-    elif kwargs:
-        for key in kwargs:
-            if key not in data_dimensions:
-                raise ValueError(
-                    f"{key} not valid parameter(s) for the "
-                    f"{database_id} database. Use "
-                    f"imf_parameters('{database_id}') to get "
-                    "valid parameters."
-                )
-            invalid_vals = []
-            if not isinstance(kwargs[key], list):
-                kwargs[key] = [kwargs[key]]
-            for x in kwargs[key]:
-                if x not in data_dimensions[key]["input_code"].tolist():
-                    invalid_vals.append(x)
-            if len(invalid_vals) > 0:
-                warn(
-                    f"{invalid_vals} not valid value(s) for {key} and will "
-                    f"be ignored. Use imf_parameters('{database_id}') to get "
-                    "valid parameters."
-                )
-            if (
-                set(kwargs[key]) == set(data_dimensions[key]["input_code"].tolist())
-                or len(kwargs[key]) == 0
-            ):
-                data_dimensions[key] = data_dimensions[key].iloc[0:0]
-            data_dimensions[key] = data_dimensions[key].iloc[
-                [
-                    index
-                    for index, x in enumerate(data_dimensions[key]["input_code"])
-                    if x in kwargs[key]
-                ]
-            ]
-        for key in data_dimensions:
-            if key not in kwargs:
-                data_dimensions[key] = data_dimensions[key].iloc[0:0]
-
-    else:
-        print(
-            "User supplied no filter parameters for the API request. "
-            "imf_dataset will attempt to request the entire database."
-        )
-        for key in data_dimensions:
-            data_dimensions[key] = data_dimensions[key].iloc[0:0]
-
-    parameter_string = ".".join(
-        ["+".join(data_dimensions[key]["input_code"]) for key in data_dimensions]
-    )
-
-    url = (
-        f"http://dataservices.imf.org/REST/SDMX_JSON.svc/"
-        f"CompactData/{database_id}/{parameter_string}"
-    )
-    if years:
-        url += f"?{urlencode(years)}"
-
-    if print_url:
-        print(url)
-
-    raw_dl = _download_parse(url, times)["CompactData"]["DataSet"]
-    try:
-        raw_dl = raw_dl["Series"]
-    except Exception:
-        raise ValueError(
-            "No data found for that combination of parameters. "
-            "Try making your request less restrictive."
-        )
-    if raw_dl is None:
-        raise ValueError(
-            "No data found for that combination of parameters. "
-            "Try making your request less restrictive."
-        )
-
-    if return_raw:
-        if include_metadata:
-            metadata = _imf_metadata(url)
-            return metadata, raw_dl
-        else:
-            return raw_dl
-
-    # Function to check if a value is a scalar
-    def is_scalar(value):
-        return not isinstance(value, (list, tuple, set, Series))
-
-    # Function to return dictionary without 'Obs'
-    def without_obs(d, keys={"Obs"}):
-        return {x: d[x] for x in d if x not in keys}
-
-    # Check if raw_dl is a list, and if not, convert it to one
-    if not isinstance(raw_dl, list):
-        raw_dl = [raw_dl]
-
-    def process_data(item):
-        # Make a data frame of dict items excluding 'Obs'
-        if all(is_scalar(value) for value in without_obs(item).values()):
-            param_vals = DataFrame.from_dict([without_obs(item)])
-        else:
-            raise ValueError("Expected item to be scalar, but it's not.")
-
-        # Make a data frame from the dicts in 'Obs'
-        try:
-            if not isinstance(item["Obs"], list):
-                item["Obs"] = [item["Obs"]]
-        except:
-            raise ValueError(
-                "No observations found for that combination of parameters. "
-                "start_year and end_year may be outside the dataset's range."
-            )
-        series = DataFrame.from_dict(item["Obs"])
-
-        # Create a copy of param_vals for every row in series
-        param_vals = concat([param_vals] * len(series)).reset_index(drop=True)
-
-        # Column bind param_vals to series
-        output = concat([param_vals, series], axis=1)
-        return output
-
-    result = concat(list(map(process_data, raw_dl)))
-    result.columns = result.columns.str.replace("@", "")
-    result.columns = result.columns.str.lower()
-
-    if not include_metadata:
-        return result
-    else:
-        metadata = _imf_metadata(url)
-        return metadata, result
+from pandas import DataFrame, Series, concat
+from warnings import warn
+from .utils import _download_parse, _imf_dimensions, _imf_metadata
+from urllib.parse import urlencode
+
+
+def imf_databases(times=3):
+    """
+    List IMF database IDs and descriptions
+
+    Returns a DataFrame with database_id and text description for each
+    database available through the IMF API endpoint.
+
+    Parameters
+    ----------
+    times : int, optional, default 3
+        Maximum number of API requests to attempt.
+
+    Returns
+    -------
+    pandas.DataFrame
+        DataFrame containing database_id and description columns.
+
+    Examples
+    --------
+    # Return first 6 IMF database IDs and descriptions
+    databases = imf_databases()
+    """
+    url = "http://dataservices.imf.org/REST/SDMX_JSON.svc/Dataflow"
+    raw_dl = _download_parse(url, times)
+
+    database_id = [
+        dataflow["KeyFamilyRef"]["KeyFamilyID"]
+        for dataflow in raw_dl["Structure"]["Dataflows"]["Dataflow"]
+    ]
+
+    description = [
+        dataflow["Name"]["#text"]
+        for dataflow in raw_dl["Structure"]["Dataflows"]["Dataflow"]
+    ]
+    database_list = DataFrame({"database_id": database_id, "description": description})
+    return database_list
+
+
+def imf_parameters(database_id, times=2):
+    """
+    List input parameters and available parameter values for use in
+    making API requests from a given IMF database.
+
+    Parameters
+    ----------
+    database_id : str
+        A database_id from imf_databases().
+    times : int, optional, default 3
+        Maximum number of API requests to attempt.
+
+    Returns
+    -------
+    dict
+        A dictionary of DataFrames, where each key corresponds to an input
+        parameter for API requests from the database. All values are DataFrames
+        with an 'input_code' column and a 'description' column. The
+        'input_code' column is a character list of all possible input codes for
+        that parameter when making requests from the IMF API endpoint. The
+        'descriptions' column is a character list of text descriptions of what
+        each input code represents.
+
+    Examples
+    --------
+    # Fetch the full list of indicator codes and descriptions for the Primary
+    # Commodity Price System database
+    params = imf_parameters(database_id='PCPS')
+    """
+    if not database_id:
+        raise ValueError("Must supply database_id. Use imf_databases to find.")
+
+    url = "http://dataservices.imf.org/REST/SDMX_JSON.svc/CodeList/"
+    try:
+        codelist = _imf_dimensions(database_id, times)
+    except ValueError as e:
+        if "There is an issue" in str(e):
+            raise ValueError(
+                f"{e}\n\nDid you supply a valid database_id? "
+                "Use imf_databases to find."
+            )
+        else:
+            raise ValueError(e)
+
+    def fetch_parameter_data(k, url, times):
+        if codelist.loc[k, "parameter"] == "freq":
+            return DataFrame(
+                {
+                    "input_code": ["A", "M", "Q"],
+                    "description": ["Annual", "Monthly", "Quarterly"],
+                }
+            )
+        else:
+            raw = _download_parse(url + codelist.loc[k, "code"], times)["Structure"][
+                "CodeLists"
+            ]["CodeList"]["Code"]
+            if isinstance(raw, list):
+                return DataFrame(
+                    {
+                        "input_code": [code["@value"] for code in raw],
+                        "description": [code["Description"]["#text"] for code in raw],
+                    }
+                )
+            else:
+                return DataFrame(
+                    {
+                        "input_code": [raw["@value"]],
+                        "description": [raw["Description"]["#text"]],
+                    }
+                )
+
+    parameter_list = {
+        codelist.loc[k, "parameter"]: fetch_parameter_data(k, url, times)
+        for k in range(codelist.shape[0])
+    }
+
+    return parameter_list
+
+
+def imf_parameter_defs(database_id, times=3, inputs_only=True):
+    """
+    Get text descriptions of input parameters used in making API
+    requests from a given IMF database
+
+    Parameters
+    ----------
+    database_id : str
+        A database_id from imf_databases().
+    times : int, optional, default 3
+        Maximum number of API requests to attempt.
+    inputs_only : bool, optional, default False
+        Whether to return only parameters used as inputs in API requests,
+        or also output variables.
+
+    Returns
+    -------
+    pandas.DataFrame
+        A DataFrame of input parameters used in making API requests
+        from a given IMF database, along with text descriptions or definitions
+        of those parameters. Useful in cases when parameter names returned by
+        imf_databases() are not self-explanatory. (Note that the usefulness
+        of text descriptions can be uneven, depending on the database design.)
+
+    Examples
+    --------
+    # Get names and text descriptions of parameters used in IMF API calls to
+    # the Primary Commodity Price System database
+    param_defs = imf_parameter_defs(database_id='PCPS')
+    """
+    if not database_id:
+        raise ValueError("Must supply database_id. Use imf_databases to find.")
+
+    try:
+        parameterlist = _imf_dimensions(database_id, times, inputs_only)[
+            ["parameter", "description"]
+        ]
+    except ValueError as e:
+        if "There is an issue" in str(e):
+            raise ValueError(
+                f"{e}\n\nDid you supply a valid database_id? "
+                "Use imf_databases to find."
+            )
+        else:
+            raise ValueError(e)
+
+    return parameterlist
+
+
+def imf_dataset(
+    database_id: str,
+    parameters: dict = None,
+    start_year: int = None,
+    end_year: int = None,
+    return_raw: bool = False,
+    print_url: bool = False,
+    times: int = 3,
+    include_metadata: bool = False,
+    **kwargs,
+):
+    """
+    Download a data series from the IMF.
+
+    Args:
+        database_id (str): Database ID for the database from which you would
+                           like to request data. Can be found using
+                           imf_databases().
+        parameters (dict): Dictionary of data frames providing input parameters
+                           for your API request. Retrieve dictionary of all
+                           possible input parameters using imf_parameters() and
+                           filter each data frame in the dictionary to reduce
+                           it to the inputs you want.
+        start_year (int, optional): Four-digit year. Earliest year for which
+                                    you would like to request data.
+        end_year (int, optional): Four-digit year. Latest year for which you
+                                  would like to request data.
+        return_raw (bool, optional): Whether to return the raw list returned by
+                                     the API instead of a cleaned-up data
+                                     frame.
+        print_url (bool, optional): Whether to print the URL used in the API
+                                    call.
+        times (int, optional): Maximum number of requests to attempt.
+        include_metadata (bool, optional): Whether to return the database
+                                           metadata header along with the data
+                                           series.
+        **kwargs: Additional keyword arguments for specifying parameters as
+                  separate arguments. Use imf_parameters() to identify which
+                  parameters to use for requests from a given database and to
+                  see all valid input codes for each parameter.
+
+    Returns:
+        If return_raw == False and include_metadata == False, returns a pandas
+        DataFrame with the data series. If return_raw == False but
+        include_metadata == True, returns a tuple whose first item is the
+        database header, and whose second item is the pandas DataFrame. If
+        return_raw == True, returns the raw JSON fetched from the API endpoint.
+    """
+
+    if database_id is None:
+        raise ValueError("Missing required database_id argument.")
+
+    if not isinstance(database_id, str):
+        raise ValueError("database_id must be a string.")
+
+    years = {}
+    if start_year is not None:
+        try:
+            start_year = str(start_year)
+            if start_year.isdigit() and len(start_year) == 4:
+                years["startPeriod"] = start_year
+            else:
+                raise ValueError(
+                    "start_year must be a four-digit number, "
+                    "either integer or string."
+                )
+        except Exception:
+            raise ValueError(
+                "start_year must be a four-digit number, either " "integer or string."
+            )
+    if end_year is not None:
+        try:
+            end_year = str(end_year)
+            if end_year.isdigit() and len(end_year) == 4:
+                years["endPeriod"] = end_year
+            else:
+                raise ValueError(
+                    "end_year must be a four-digit number, " "either integer or string"
+                )
+        except Exception:
+            raise ValueError(
+                "end_year must be a four-digit number, " "either integer or string"
+            )
+
+    data_dimensions = imf_parameters(database_id, times)
+
+    if parameters is not None:
+        if kwargs:
+            warn(
+                "Parameters list argument cannot be combined with character "
+                "vector parameters arguments. Character vector parameters "
+                "arguments will be ignored."
+            )
+        for key in parameters:
+            if key not in data_dimensions:
+                raise ValueError(
+                    f"{key} not valid parameter(s) for the "
+                    f"{database_id} database. Use "
+                    f"imf_parameters('{database_id}') to get "
+                    "valid parameters."
+                )
+            invalid_keys = []
+            for x in list(parameters[key]["input_code"]):
+                if x not in list(data_dimensions[key]["input_code"]):
+                    invalid_keys.append(x)
+            if len(invalid_keys) > 0:
+                warn(
+                    f"{invalid_keys} not valid value(s) for {key} and will "
+                    f"be ignored. Use imf_parameters('{database_id}') to get "
+                    "valid parameters."
+                )
+            if (
+                set(parameters[key]["input_code"])
+                == set(data_dimensions[key]["input_code"])
+                or len(parameters[key]) == 0
+            ):
+                data_dimensions[key] = data_dimensions[key].iloc[0:0]
+            data_dimensions[key] = data_dimensions[key].iloc[
+                [
+                    index
+                    for index, x in enumerate(data_dimensions[key]["input_code"])
+                    if x in list(parameters[key]["input_code"])
+                ]
+            ]
+        for key in data_dimensions:
+            if key not in parameters:
+                data_dimensions[key] = data_dimensions[key].iloc[0:0]
+
+    elif kwargs:
+        for key in kwargs:
+            if key not in data_dimensions:
+                raise ValueError(
+                    f"{key} not valid parameter(s) for the "
+                    f"{database_id} database. Use "
+                    f"imf_parameters('{database_id}') to get "
+                    "valid parameters."
+                )
+            invalid_vals = []
+            if not isinstance(kwargs[key], list):
+                kwargs[key] = [kwargs[key]]
+            for x in kwargs[key]:
+                if x not in data_dimensions[key]["input_code"].tolist():
+                    invalid_vals.append(x)
+            if len(invalid_vals) > 0:
+                warn(
+                    f"{invalid_vals} not valid value(s) for {key} and will "
+                    f"be ignored. Use imf_parameters('{database_id}') to get "
+                    "valid parameters."
+                )
+            if (
+                set(kwargs[key]) == set(data_dimensions[key]["input_code"].tolist())
+                or len(kwargs[key]) == 0
+            ):
+                data_dimensions[key] = data_dimensions[key].iloc[0:0]
+            data_dimensions[key] = data_dimensions[key].iloc[
+                [
+                    index
+                    for index, x in enumerate(data_dimensions[key]["input_code"])
+                    if x in kwargs[key]
+                ]
+            ]
+        for key in data_dimensions:
+            if key not in kwargs:
+                data_dimensions[key] = data_dimensions[key].iloc[0:0]
+
+    else:
+        print(
+            "User supplied no filter parameters for the API request. "
+            "imf_dataset will attempt to request the entire database."
+        )
+        for key in data_dimensions:
+            data_dimensions[key] = data_dimensions[key].iloc[0:0]
+
+    parameter_string = ".".join(
+        ["+".join(data_dimensions[key]["input_code"]) for key in data_dimensions]
+    )
+
+    url = (
+        f"http://dataservices.imf.org/REST/SDMX_JSON.svc/"
+        f"CompactData/{database_id}/{parameter_string}"
+    )
+    if years:
+        url += f"?{urlencode(years)}"
+
+    if print_url:
+        print(url)
+
+    raw_dl = _download_parse(url, times)["CompactData"]["DataSet"]
+    try:
+        raw_dl = raw_dl["Series"]
+    except Exception:
+        raise ValueError(
+            "No data found for that combination of parameters. "
+            "Try making your request less restrictive."
+        )
+    if raw_dl is None:
+        raise ValueError(
+            "No data found for that combination of parameters. "
+            "Try making your request less restrictive."
+        )
+
+    if return_raw:
+        if include_metadata:
+            metadata = _imf_metadata(url)
+            return metadata, raw_dl
+        else:
+            return raw_dl
+
+    # Function to check if a value is a scalar
+    def is_scalar(value):
+        return not isinstance(value, (list, tuple, set, Series))
+
+    # Function to return dictionary without 'Obs'
+    def without_obs(d, keys={"Obs"}):
+        return {x: d[x] for x in d if x not in keys}
+
+    # Check if raw_dl is a list, and if not, convert it to one
+    if not isinstance(raw_dl, list):
+        raw_dl = [raw_dl]
+
+    def process_data(item):
+        # Make a data frame of dict items excluding 'Obs'
+        if all(is_scalar(value) for value in without_obs(item).values()):
+            param_vals = DataFrame.from_dict([without_obs(item)])
+        else:
+            raise ValueError("Expected item to be scalar, but it's not.")
+
+        # Make a data frame from the dicts in 'Obs'
+        try:
+            if not isinstance(item["Obs"], list):
+                item["Obs"] = [item["Obs"]]
+        except:
+            raise ValueError(
+                "No observations found for that combination of parameters. "
+                "start_year and end_year may be outside the dataset's range."
+            )
+        series = DataFrame.from_dict(item["Obs"])
+
+        # Create a copy of param_vals for every row in series
+        param_vals = concat([param_vals] * len(series)).reset_index(drop=True)
+
+        # Column bind param_vals to series
+        output = concat([param_vals, series], axis=1)
+        return output
+
+    result = concat(list(map(process_data, raw_dl)))
+    result.columns = result.columns.str.replace("@", "")
+    result.columns = result.columns.str.lower()
+
+    if not include_metadata:
+        return result
+    else:
+        metadata = _imf_metadata(url)
+        return metadata, result
```

### Comparing `imfp-1.1.0/imfp/utils.py` & `imfp-1.1.1/imfp/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,277 +1,273 @@
-from os import environ, path
-import hashlib
-from time import sleep, perf_counter
-from requests import get
-from json import loads, load, dump, JSONDecodeError
-from pandas import DataFrame
-from pkg_resources import get_distribution, DistributionNotFound
-import re
-
-
-def _min_wait_time_limited(default_wait_time=1.5):
-    def decorator(func):
-        last_called = [0.0]
-
-        def wrapper(*args, **kwargs):
-            min_wait_time = float(environ.get("IMF_WAIT_TIME", default_wait_time))
-            elapsed = perf_counter() - last_called[0]
-            left_to_wait = min_wait_time - elapsed
-            if left_to_wait > 0:
-                sleep(left_to_wait)
-            ret = func(*args, **kwargs)
-            last_called[0] = perf_counter()
-            return ret
-
-        return wrapper
-
-    return decorator
-
-
-@_min_wait_time_limited()
-def _imf_get(url, headers):
-    """
-    A rate-limited wrapper around the requests.get method.
-
-    Args:
-        url (str): The URL to send a GET request to.
-        headers (dict): The headers to use in the API request.
-
-    Returns:
-        requests.Response: The response object returned by requests.get.
-
-    Usage:
-        response = _imf_get(
-                'http://dataservices.imf.org/REST/SDMX_JSON.svc/Dataflow'
-            )
-        print(response.text)
-    """
-    return get(url, headers)
-
-
-_imf_use_cache = False
-_imf_save_response = False
-
-
-def _download_parse(URL, times=3):
-    """
-    (Internal) Download and parse JSON content from a URL with rate limiting
-    and retries.
-
-    This function is rate-limited and will perform a specified number of
-    retries in case of failure.
-
-    Args:
-        URL (str): The URL to download and parse the JSON content from.
-        times (int, optional): The number of times to retry the request in case
-        of failure. Defaults to 3.
-
-    Returns:
-        dict: The parsed JSON content as a Python dictionary.
-
-    Raises:
-        ValueError: If the content cannot be parsed as JSON after the specified
-        number of retries.
-    """
-
-    global _imf_use_cache, _imf_save_response
-    use_cache = _imf_use_cache
-    save_response = _imf_save_response
-
-    app_name = environ.get("IMF_APP_NAME")
-    if app_name:
-        app_name = app_name[:255]
-    else:
-        try:
-            app_name = f'imfp/{get_distribution("imfp").version}'
-        except DistributionNotFound:
-            app_name = "imfp"
-
-    headers = {"Accept": "application/json", "User-Agent": app_name}
-    for _ in range(times):
-        if use_cache:
-            cached_status, cached_content = _load_cached_response(URL)
-            if cached_content is not None:
-                content = cached_content
-                status = cached_status
-        else:
-            response = _imf_get(URL, headers=headers)
-            content = response.text
-            status = response.status_code
-
-        if save_response:
-            file_name = hashlib.sha256(URL.encode()).hexdigest()
-            file_path = f"tests/responses/{file_name}.json"
-            print(f"Saving response to: {file_path}")
-            with open(file_path, "w") as file:
-                dump({"status_code": status, "content": content}, file)
-
-        if status != 200 or ("<" in content and ">" in content):
-            matches = re.search("<[^>]+>(.*?)<\\/[^>]+>", content)
-            inner_text = matches.group(1)
-            output_string = re.sub(" GKey\\s*=\\s*[a-f0-9-]+", "", inner_text)
-
-            if "Rejected" in content or "Bandwidth" in content:
-                err_message = (
-                    f"API request failed. URL: '{URL}' "
-                    f"Status: '{status}', "
-                    f"Content: '{output_string}'\n\n"
-                    "API may be overwhelmed by too many "
-                    "requests. Take a break and try again."
-                )
-            elif "Service" in content:
-                err_message = (
-                    f"API request failed. URL: '{URL}' "
-                    f"Status: '{status}', "
-                    f"Content: '{output_string}'\n\n"
-                    "Your requested dataset may be too large. "
-                    "Try narrowing your request and try again."
-                )
-            elif status == 400:
-                err_message = (
-                    f"API request failed. URL: '{URL}' "
-                    f"Status: '{status}', "
-                    f"Content: '{output_string}'\n\n"
-                    "Too many parameters supplied. "
-                    "Please narrow the request and try again."
-                )
-            elif status == 500 and "please check your query" in content.lower():
-                err_message = (
-                    f"API request failed. URL: '{URL}' "
-                    f"Status: '{status}', "
-                    f"Content: '{output_string}'\n\n"
-                    "Your request may be missing one or more required "
-                    "parameters. Please adjust your query and try again."
-                )
-            else:
-                err_message = (
-                    f"API request failed. URL: '{URL}' "
-                    f"Status: '{status}', "
-                    f"Content: '{output_string}'"
-                )
-
-            if _ < times - 1:
-                sleep(5 ** (_ + 1))
-            else:
-                raise ValueError(err_message)
-        else:
-            try:
-                json_parsed = loads(content)
-                return json_parsed
-            except JSONDecodeError:
-                if _ < times - 1:
-                    sleep(5 ** (_ + 1))
-                else:
-                    raise ValueError(
-                        f"Content from API could not be parsed as JSON. URL: '{URL}' "
-                        f"Status: '{status}', Content: '{content}'"
-                    )
-
-
-def _load_cached_response(URL):
-    file_name = hashlib.sha256(URL.encode()).hexdigest()
-    file_path = f"tests/responses/{file_name}.json"
-
-    if path.exists(file_path):
-        with open(file_path, "r") as file:
-            data = load(file)
-            return data.get("status_code"), data.get("content")
-    return None, None
-
-
-def _imf_dimensions(database_id, times=3, inputs_only=True):
-    """
-    (Internal) Retrieve the list of codes for dimensions of an individual IMF
-    database.
-
-    Args:
-        database_id (str): The ID of the IMF database.
-        times (int, optional): The number of times to retry the request in case
-        of failure. Defaults to 3.
-        inputs_only (bool, optional): If True, only include input parameters.
-        Defaults to True.
-
-    Returns:
-        pandas.DataFrame: A DataFrame containing the parameter names and their
-        corresponding codes and descriptions.
-    """
-    URL = (
-        f"http://dataservices.imf.org/REST/SDMX_JSON.svc/DataStructure/"
-        f"{database_id}"
-    )
-    raw_dl = _download_parse(URL, times)
-
-    code = []
-    for item in raw_dl["Structure"]["CodeLists"]["CodeList"]:
-        code.append(item["@id"])
-    description = []
-    for item in raw_dl["Structure"]["CodeLists"]["CodeList"]:
-        description.append(item["Name"]["#text"])
-    codelist_df = DataFrame({"code": code, "description": description})
-
-    params = [
-        dim["@conceptRef"].lower()
-        for dim in (
-            raw_dl["Structure"]["KeyFamilies"]["KeyFamily"]["Components"]["Dimension"]
-        )
-    ]
-    codes = [
-        dim["@codelist"]
-        for dim in (
-            raw_dl["Structure"]["KeyFamilies"]["KeyFamily"]["Components"]["Dimension"]
-        )
-    ]
-    param_code_df = DataFrame({"parameter": params, "code": codes})
-
-    if inputs_only:
-        result_df = param_code_df.merge(codelist_df, on="code", how="left")
-    else:
-        result_df = param_code_df.merge(codelist_df, on="code", how="outer")
-
-    return result_df
-
-
-def _imf_metadata(URL, times=3):
-    """
-    (Internal) Access metadata for a dataset.
-
-    Args:
-        URL (str): The URL used to request metadata.
-        times (int, optional): Maximum number of requests to attempt. Defaults
-        to 3.
-
-    Returns:
-        dict: A dictionary containing the metadata information.
-
-    Raises:
-        ValueError: If the URL is not provided.
-
-    Examples:
-        # Find Primary Commodity Price System database metadata
-        metadata = (
-            imf_metadata("http://dataservices.imf.org/REST/SDMX_JSON.svc/"
-            "GenericMetadata/PCPS/A..?start_year=2020")
-        )
-    """
-
-    if not URL:
-        raise ValueError("Must supply URL.")
-
-    URL = URL.replace("CompactData", "GenericMetadata")
-    raw_dl = _download_parse(URL, times=times)
-
-    output = {
-        "XMLschema": raw_dl["GenericMetadata"]["@xmlns:xsd"],
-        "message": raw_dl["GenericMetadata"]["@xsi:schemaLocation"],
-        "language": (
-            raw_dl["GenericMetadata"]["Header"]["Sender"]["Name"]["@xml:lang"]
-        ),
-        "timestamp": raw_dl["GenericMetadata"]["Header"]["Prepared"],
-        "custodian": (raw_dl["GenericMetadata"]["Header"]["Sender"]["Name"]["#text"]),
-        "custodian_url": (
-            raw_dl["GenericMetadata"]["Header"]["Sender"]["Contact"]["URI"]
-        ),
-        "custodian_telephone": (
-            raw_dl["GenericMetadata"]["Header"]["Sender"]["Contact"]["Telephone"]
-        ),
-    }
-    return output
+from os import environ, path
+import hashlib
+from time import sleep, perf_counter
+from requests import get
+from json import loads, load, dump, JSONDecodeError
+from pandas import DataFrame
+import re
+
+
+def _min_wait_time_limited(default_wait_time=1.5):
+    def decorator(func):
+        last_called = [0.0]
+
+        def wrapper(*args, **kwargs):
+            min_wait_time = float(environ.get("IMF_WAIT_TIME", default_wait_time))
+            elapsed = perf_counter() - last_called[0]
+            left_to_wait = min_wait_time - elapsed
+            if left_to_wait > 0:
+                sleep(left_to_wait)
+            ret = func(*args, **kwargs)
+            last_called[0] = perf_counter()
+            return ret
+
+        return wrapper
+
+    return decorator
+
+
+@_min_wait_time_limited()
+def _imf_get(url, headers):
+    """
+    A rate-limited wrapper around the requests.get method.
+
+    Args:
+        url (str): The URL to send a GET request to.
+        headers (dict): The headers to use in the API request.
+
+    Returns:
+        requests.Response: The response object returned by requests.get.
+
+    Usage:
+        response = _imf_get(
+                'http://dataservices.imf.org/REST/SDMX_JSON.svc/Dataflow'
+            )
+        print(response.text)
+    """
+    return get(url, headers)
+
+
+_imf_use_cache = False
+_imf_save_response = False
+
+
+def _download_parse(URL, times=3):
+    """
+    (Internal) Download and parse JSON content from a URL with rate limiting
+    and retries.
+
+    This function is rate-limited and will perform a specified number of
+    retries in case of failure.
+
+    Args:
+        URL (str): The URL to download and parse the JSON content from.
+        times (int, optional): The number of times to retry the request in case
+        of failure. Defaults to 3.
+
+    Returns:
+        dict: The parsed JSON content as a Python dictionary.
+
+    Raises:
+        ValueError: If the content cannot be parsed as JSON after the specified
+        number of retries.
+    """
+
+    global _imf_use_cache, _imf_save_response
+    use_cache = _imf_use_cache
+    save_response = _imf_save_response
+
+    app_name = environ.get("IMF_APP_NAME")
+    if app_name:
+        app_name = app_name[:255]
+    else:
+        app_name = "imfp"
+
+    headers = {"Accept": "application/json", "User-Agent": app_name}
+    for _ in range(times):
+        if use_cache:
+            cached_status, cached_content = _load_cached_response(URL)
+            if cached_content is not None:
+                content = cached_content
+                status = cached_status
+        else:
+            response = _imf_get(URL, headers=headers)
+            content = response.text
+            status = response.status_code
+
+        if save_response:
+            file_name = hashlib.sha256(URL.encode()).hexdigest()
+            file_path = f"tests/responses/{file_name}.json"
+            print(f"Saving response to: {file_path}")
+            with open(file_path, "w") as file:
+                dump({"status_code": status, "content": content}, file)
+
+        if status != 200 or ("<" in content and ">" in content):
+            matches = re.search("<[^>]+>(.*?)<\\/[^>]+>", content)
+            inner_text = matches.group(1)
+            output_string = re.sub(" GKey\\s*=\\s*[a-f0-9-]+", "", inner_text)
+
+            if "Rejected" in content or "Bandwidth" in content:
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'\n\n"
+                    "API may be overwhelmed by too many "
+                    "requests. Take a break and try again."
+                )
+            elif "Service" in content:
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'\n\n"
+                    "Your requested dataset may be too large. "
+                    "Try narrowing your request and try again."
+                )
+            elif status == 400:
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'\n\n"
+                    "Too many parameters supplied. "
+                    "Please narrow the request and try again."
+                )
+            elif status == 500 and "please check your query" in content.lower():
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'\n\n"
+                    "Your request may be missing one or more required "
+                    "parameters. Please adjust your query and try again."
+                )
+            else:
+                err_message = (
+                    f"API request failed. URL: '{URL}' "
+                    f"Status: '{status}', "
+                    f"Content: '{output_string}'"
+                )
+
+            if _ < times - 1:
+                sleep(5 ** (_ + 1))
+            else:
+                raise ValueError(err_message)
+        else:
+            try:
+                json_parsed = loads(content)
+                return json_parsed
+            except JSONDecodeError:
+                if _ < times - 1:
+                    sleep(5 ** (_ + 1))
+                else:
+                    raise ValueError(
+                        f"Content from API could not be parsed as JSON. URL: '{URL}' "
+                        f"Status: '{status}', Content: '{content}'"
+                    )
+
+
+def _load_cached_response(URL):
+    file_name = hashlib.sha256(URL.encode()).hexdigest()
+    file_path = f"tests/responses/{file_name}.json"
+
+    if path.exists(file_path):
+        with open(file_path, "r") as file:
+            data = load(file)
+            return data.get("status_code"), data.get("content")
+    return None, None
+
+
+def _imf_dimensions(database_id, times=3, inputs_only=True):
+    """
+    (Internal) Retrieve the list of codes for dimensions of an individual IMF
+    database.
+
+    Args:
+        database_id (str): The ID of the IMF database.
+        times (int, optional): The number of times to retry the request in case
+        of failure. Defaults to 3.
+        inputs_only (bool, optional): If True, only include input parameters.
+        Defaults to True.
+
+    Returns:
+        pandas.DataFrame: A DataFrame containing the parameter names and their
+        corresponding codes and descriptions.
+    """
+    URL = (
+        f"http://dataservices.imf.org/REST/SDMX_JSON.svc/DataStructure/"
+        f"{database_id}"
+    )
+    raw_dl = _download_parse(URL, times)
+
+    code = []
+    for item in raw_dl["Structure"]["CodeLists"]["CodeList"]:
+        code.append(item["@id"])
+    description = []
+    for item in raw_dl["Structure"]["CodeLists"]["CodeList"]:
+        description.append(item["Name"]["#text"])
+    codelist_df = DataFrame({"code": code, "description": description})
+
+    params = [
+        dim["@conceptRef"].lower()
+        for dim in (
+            raw_dl["Structure"]["KeyFamilies"]["KeyFamily"]["Components"]["Dimension"]
+        )
+    ]
+    codes = [
+        dim["@codelist"]
+        for dim in (
+            raw_dl["Structure"]["KeyFamilies"]["KeyFamily"]["Components"]["Dimension"]
+        )
+    ]
+    param_code_df = DataFrame({"parameter": params, "code": codes})
+
+    if inputs_only:
+        result_df = param_code_df.merge(codelist_df, on="code", how="left")
+    else:
+        result_df = param_code_df.merge(codelist_df, on="code", how="outer")
+
+    return result_df
+
+
+def _imf_metadata(URL, times=3):
+    """
+    (Internal) Access metadata for a dataset.
+
+    Args:
+        URL (str): The URL used to request metadata.
+        times (int, optional): Maximum number of requests to attempt. Defaults
+        to 3.
+
+    Returns:
+        dict: A dictionary containing the metadata information.
+
+    Raises:
+        ValueError: If the URL is not provided.
+
+    Examples:
+        # Find Primary Commodity Price System database metadata
+        metadata = (
+            imf_metadata("http://dataservices.imf.org/REST/SDMX_JSON.svc/"
+            "GenericMetadata/PCPS/A..?start_year=2020")
+        )
+    """
+
+    if not URL:
+        raise ValueError("Must supply URL.")
+
+    URL = URL.replace("CompactData", "GenericMetadata")
+    raw_dl = _download_parse(URL, times=times)
+
+    output = {
+        "XMLschema": raw_dl["GenericMetadata"]["@xmlns:xsd"],
+        "message": raw_dl["GenericMetadata"]["@xsi:schemaLocation"],
+        "language": (
+            raw_dl["GenericMetadata"]["Header"]["Sender"]["Name"]["@xml:lang"]
+        ),
+        "timestamp": raw_dl["GenericMetadata"]["Header"]["Prepared"],
+        "custodian": (raw_dl["GenericMetadata"]["Header"]["Sender"]["Name"]["#text"]),
+        "custodian_url": (
+            raw_dl["GenericMetadata"]["Header"]["Sender"]["Contact"]["URI"]
+        ),
+        "custodian_telephone": (
+            raw_dl["GenericMetadata"]["Header"]["Sender"]["Contact"]["Telephone"]
+        ),
+    }
+    return output
```

### Comparing `imfp-1.1.0/LICENSE` & `imfp-1.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `imfp-1.1.0/pyproject.toml` & `imfp-1.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-[tool.poetry]
-name = "imfp"
-version = "1.1.0"
-description = "Python package for downloading economic data from the International Monetary Fund JSON RESTful API endpoint."
-authors = ["Christopher C. Smith <chriscarrollsmith@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/chriscarrollsmith/imfp"
-repository = "https://github.com/chriscarrollsmith/imfp"
-documentation = ""
-keywords = ["economics", "finance", "IMF", "API"]
-classifiers = [
-    "Intended Audience :: Financial and Insurance Industry",
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-packages = [
-  { include = "imfp" },
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-pandas = "^1.5.3"
-requests = "^2.28.2"
-
-[tool.poetry.group.dev.dependencies]
-responses = "^0.23.1"
-pytest = "^7.2.2"
-pytest-runner = "^6.0.0"
-black = "^23.3.0"
-pytest-mock = "^3.10.0"
-
-[build-system]
-requires = ["poetry-core"]
+[tool.poetry]
+name = "imfp"
+version = "1.1.1"
+description = "Python package for downloading economic data from the International Monetary Fund JSON RESTful API endpoint."
+authors = ["Christopher C. Smith <chriscarrollsmith@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/chriscarrollsmith/imfp"
+repository = "https://github.com/chriscarrollsmith/imfp"
+keywords = ["economics", "finance", "IMF", "API"]
+classifiers = [
+    "Intended Audience :: Financial and Insurance Industry",
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+packages = [
+  { include = "imfp" },
+]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+pandas = "^1.5.3"
+requests = "^2.28.2"
+
+[tool.poetry.group.dev.dependencies]
+responses = "^0.23.1"
+pytest = "^7.2.2"
+pytest-runner = "^6.0.0"
+black = "^23.3.0"
+pytest-mock = "^3.10.0"
+
+[build-system]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `imfp-1.1.0/PKG-INFO` & `imfp-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imfp
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python package for downloading economic data from the International Monetary Fund JSON RESTful API endpoint.
 Home-page: https://github.com/chriscarrollsmith/imfp
 License: MIT
 Keywords: economics,finance,IMF,API
 Author: Christopher C. Smith
 Author-email: chriscarrollsmith@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/chriscarrollsmith/imfp
 Description-Content-Type: text/markdown
 
 # imfp
 
@@ -113,20 +113,19 @@
     </tr>
   </tbody>
 </table>
 </div>
 
 
 
-This function returns the IMF’s listing of 259 databases available through the API. (In reality, 7 of the listed databases are defunct and not actually available: FAS_2015, GFS01, FM202010, APDREO202010, AFRREO202010, WHDREO202010, BOPAGG_2020.)
+This function returns the IMF’s listing of 259 databases available through the API. (In reality, 8 of the listed databases are defunct and not actually available: FAS_2015, GFS01, FM202010, APDREO202010, AFRREO202010, WHDREO202010, BOPAGG_2020, DOT_2020Q1.)
 
 To view and explore the database list, it’s possible to explore subsets of the data frame by row number with `databases.loc`:
 
 
-
 ```python
 # View a subset consisting of rows 5 through 9
 databases.loc[5:9]
 ```
 
 
 
@@ -718,11 +717,21 @@
 
 ### Changing the enforced wait time between API calls with `set_imf_wait_time`
 
 By default, `imfp` enforces a mandatory 1.5-second wait time between API calls to prevent repeated or recursive calls from exceeding the API's bandwidth/rate limit. This wait time should be sufficient for most applications. However, if you are running parallel processes using `imfp` (e.g. during cross-platform testing), this wait time may be insufficient to prevent you from running up against the API's rate and bandwidth limits. You can change this wait time by calling the `set_imf_wait_time` function with a numeric value, in seconds. For instance, to enforce a five-second wait time between API calls, use `set_imf_wait_time(10)`.
 
 Also note that by default, `imfp` functions will retry any API call rejected for bandwidth or rate limit reasons. The number of times `imfp` will attempt the call is set by the `times` argument, with a default value of 3. (With this value, requests will be retried twice after an initial failure.) Note that `imfp` enforces an exponentially increasing wait time between function calls, with a base wait time of 5 seconds on the first retry, so it is not recommended to set a high value for `times`.
 
+## Planned features
+
+- Implement automatic build/render of readthedocs documentation with Sphinx
+- Implement automatic build/release/publish of package updates
+- Move response mocking functionality from `_download_parse` to `_imf_get`
+- Investigate and implement different and more appropriate exception types, as we're currently handling too many different cases with `ValueError`
+- More fully investigate the types of metadata available through the API and the most appropriate way to return them when a user calls `include_metadata`
+- Implement optional response caching for `imf_databases` and `imf_parameters`
+- Simplify and modularize some of the code, particularly in `imf_dataset`
+
 ## Contributing
 
-I would love to have your help in improving `imfr`. If you encounter a bug while using the library, please open an issue. Alternatively, fix the bug and open a pull request. Thanks in advance for your help!
+I would love to have your help in improving `imfp`. If you encounter a bug while using the library, please open an issue. Alternatively, fix the bug and open a pull request. Thanks in advance for your help!
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: imfp Version: 1.1.0 Summary: Python package for
+Metadata-Version: 2.1 Name: imfp Version: 1.1.1 Summary: Python package for
 downloading economic data from the International Monetary Fund JSON RESTful API
 endpoint. Home-page: https://github.com/chriscarrollsmith/imfp License: MIT
 Keywords: economics,finance,IMF,API Author: Christopher C. Smith Author-email:
 chriscarrollsmith@gmail.com Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Financial and Insurance Industry Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: requests
 (>=2.28.2,<3.0.0) Project-URL: Repository, https://github.com/
 chriscarrollsmith/imfp Description-Content-Type: text/markdown # imfp [![Tests]
 (https://github.com/chriscarrollsmith/imfp/actions/workflows/actions.yml/
 badge.svg)](https://github.com/chriscarrollsmith/imfp/actions/workflows/
 actions.yml) [![PyPI Version](https://img.shields.io/pypi/v/imfp.svg)](https://
 pypi.python.org/pypi/imfp) [![Code style: black](https://img.shields.io/badge/
@@ -42,19 +42,20 @@
 |_ _|_dd_aa_tt_aa_bb_aa_ss_ee____ii_dd_|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _dd_ee_ss_cc_rr_ii_pp_tt_ii_oo_nn|
 |_00_|_B_O_P___2_0_1_7_M_0_6_|_B_a_l_a_n_c_e_ _o_f_ _P_a_y_m_e_n_t_s_ _(_B_O_P_)_,_ _2_0_1_7_ _M_0_6_ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |_11_|_B_O_P___2_0_2_0_M_3_ _|_B_a_l_a_n_c_e_ _o_f_ _P_a_y_m_e_n_t_s_ _(_B_O_P_)_,_ _2_0_2_0_ _M_0_3_ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |_22_|_B_O_P___2_0_1_7_M_1_1_|_B_a_l_a_n_c_e_ _o_f_ _P_a_y_m_e_n_t_s_ _(_B_O_P_)_,_ _2_0_1_7_ _M_1_1_ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |_33_|_D_O_T___2_0_2_0_Q_1_ _|_D_i_r_e_c_t_i_o_n_ _o_f_ _T_r_a_d_e_ _S_t_a_t_i_s_t_i_c_s_ _(_D_O_T_S_)_,_ _2_0_2_0_ _Q_1_ _ _ _ |
 |_44_|_G_F_S_M_A_B_2_0_1_6_ _|_G_o_v_e_r_n_m_e_n_t_ _F_i_n_a_n_c_e_ _S_t_a_t_i_s_t_i_c_s_ _Y_e_a_r_b_o_o_k_ _(_G_F_S_Y_ _2_._._.|
 This function returns the IMFâs listing of 259 databases available through
-the API. (In reality, 7 of the listed databases are defunct and not actually
+the API. (In reality, 8 of the listed databases are defunct and not actually
 available: FAS_2015, GFS01, FM202010, APDREO202010, AFRREO202010, WHDREO202010,
-BOPAGG_2020.) To view and explore the database list, itâs possible to explore
-subsets of the data frame by row number with `databases.loc`: ```python # View
-a subset consisting of rows 5 through 9 databases.loc[5:9] ```
+BOPAGG_2020, DOT_2020Q1.) To view and explore the database list, itâs
+possible to explore subsets of the data frame by row number with
+`databases.loc`: ```python # View a subset consisting of rows 5 through 9
+databases.loc[5:9] ```
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |_ _|_ _ _dd_aa_tt_aa_bb_aa_ss_ee____ii_dd_|_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _dd_ee_ss_cc_rr_ii_pp_tt_ii_oo_nn|
 |_55_|_B_O_P___2_0_1_9_M_1_2_ _ _|_B_a_l_a_n_c_e_ _o_f_ _P_a_y_m_e_n_t_s_ _(_B_O_P_)_,_ _2_0_1_9_ _M_1_2_ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |_66_|_G_F_S_Y_F_A_L_C_S_2_0_1_4_|_G_o_v_e_r_n_m_e_n_t_ _F_i_n_a_n_c_e_ _S_t_a_t_i_s_t_i_c_s_ _Y_e_a_r_b_o_o_k_ _(_G_F_S_Y_ _2_._._.|
 |_77_|_G_F_S_E_2_0_1_6_ _ _ _ _ _|_G_o_v_e_r_n_m_e_n_t_ _F_i_n_a_n_c_e_ _S_t_a_t_i_s_t_i_c_s_ _Y_e_a_r_b_o_o_k_ _(_G_F_S_Y_ _2_._._.|
 |_88_|_F_M_2_0_1_5_1_0_ _ _ _ _ _|_F_i_s_c_a_l_ _M_o_n_i_t_o_r_ _(_F_M_)_ _O_c_t_o_b_e_r_ _2_0_1_5_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
 |_99_|_G_F_S_I_B_S_2_0_1_6_ _ _ _|_G_o_v_e_r_n_m_e_n_t_ _F_i_n_a_n_c_e_ _S_t_a_t_i_s_t_i_c_s_ _Y_e_a_r_b_o_o_k_ _(_G_F_S_Y_ _2_._._.|
@@ -240,11 +241,20 @@
 enforce a five-second wait time between API calls, use `set_imf_wait_time(10)`.
 Also note that by default, `imfp` functions will retry any API call rejected
 for bandwidth or rate limit reasons. The number of times `imfp` will attempt
 the call is set by the `times` argument, with a default value of 3. (With this
 value, requests will be retried twice after an initial failure.) Note that
 `imfp` enforces an exponentially increasing wait time between function calls,
 with a base wait time of 5 seconds on the first retry, so it is not recommended
-to set a high value for `times`. ## Contributing I would love to have your help
-in improving `imfr`. If you encounter a bug while using the library, please
-open an issue. Alternatively, fix the bug and open a pull request. Thanks in
-advance for your help!
+to set a high value for `times`. ## Planned features - Implement automatic
+build/render of readthedocs documentation with Sphinx - Implement automatic
+build/release/publish of package updates - Move response mocking functionality
+from `_download_parse` to `_imf_get` - Investigate and implement different and
+more appropriate exception types, as we're currently handling too many
+different cases with `ValueError` - More fully investigate the types of
+metadata available through the API and the most appropriate way to return them
+when a user calls `include_metadata` - Implement optional response caching for
+`imf_databases` and `imf_parameters` - Simplify and modularize some of the
+code, particularly in `imf_dataset` ## Contributing I would love to have your
+help in improving `imfp`. If you encounter a bug while using the library,
+please open an issue. Alternatively, fix the bug and open a pull request.
+Thanks in advance for your help!
```

