# Comparing `tmp/motion-learning-toolbox-1.0.5.tar.gz` & `tmp/motion_learning_toolbox-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion-learning-toolbox-1.0.5.tar", last modified: Wed Jan 31 12:23:28 2024, max compression
+gzip compressed data, was "motion_learning_toolbox-1.0.6.tar", last modified: Tue Apr 23 08:51:14 2024, max compression
```

## Comparing `motion-learning-toolbox-1.0.5.tar` & `motion_learning_toolbox-1.0.6.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 cs        (1000) cs        (1000)        0 2024-01-31 12:23:28.935004 motion-learning-toolbox-1.0.5/
--rw-rw-r--   0 cs        (1000) cs        (1000)      335 2023-09-15 13:17:03.000000 motion-learning-toolbox-1.0.5/License.md
--rw-r--r--   0 cs        (1000) cs        (1000)     7633 2024-01-31 12:23:28.935004 motion-learning-toolbox-1.0.5/PKG-INFO
--rw-rw-r--   0 cs        (1000) cs        (1000)     6490 2024-01-31 09:29:52.000000 motion-learning-toolbox-1.0.5/Readme.md
-drwxrwxr-x   0 cs        (1000) cs        (1000)        0 2024-01-31 12:23:28.931004 motion-learning-toolbox-1.0.5/motion_learning_toolbox/
--rw-rw-r--   0 cs        (1000) cs        (1000)      335 2023-09-15 13:17:03.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox/__init__.py
--rw-rw-r--   0 cs        (1000) cs        (1000)     1751 2023-09-15 13:17:03.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox/canonicalize_quaternions.py
--rw-rw-r--   0 cs        (1000) cs        (1000)     2571 2023-09-18 11:20:31.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox/fix_controller_mapping.py
--rw-rw-r--   0 cs        (1000) cs        (1000)     2369 2024-01-29 11:28:13.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox/resample.py
--rw-rw-r--   0 cs        (1000) cs        (1000)      573 2023-09-21 09:32:43.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox/to_acceleration.py
--rw-rw-r--   0 cs        (1000) cs        (1000)     5003 2024-01-31 11:55:18.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox/to_body_relative.py
--rw-rw-r--   0 cs        (1000) cs        (1000)     3343 2024-01-31 12:00:00.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox/to_velocity.py
-drwxrwxr-x   0 cs        (1000) cs        (1000)        0 2024-01-31 12:23:28.935004 motion-learning-toolbox-1.0.5/motion_learning_toolbox.egg-info/
--rw-r--r--   0 cs        (1000) cs        (1000)     7633 2024-01-31 12:23:28.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 cs        (1000) cs        (1000)      721 2024-01-31 12:23:28.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 cs        (1000) cs        (1000)        1 2024-01-31 12:23:28.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 cs        (1000) cs        (1000)       68 2024-01-31 12:23:28.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox.egg-info/requires.txt
--rw-rw-r--   0 cs        (1000) cs        (1000)       24 2024-01-31 12:23:28.000000 motion-learning-toolbox-1.0.5/motion_learning_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 cs        (1000) cs        (1000)      907 2024-01-31 12:23:22.000000 motion-learning-toolbox-1.0.5/pyproject.toml
--rw-rw-r--   0 cs        (1000) cs        (1000)       38 2024-01-31 12:23:28.935004 motion-learning-toolbox-1.0.5/setup.cfg
-drwxrwxr-x   0 cs        (1000) cs        (1000)        0 2024-01-31 12:23:28.935004 motion-learning-toolbox-1.0.5/tests/
--rw-rw-r--   0 cs        (1000) cs        (1000)     1105 2023-09-15 13:17:03.000000 motion-learning-toolbox-1.0.5/tests/test_canonicalize_quaternions.py
--rw-rw-r--   0 cs        (1000) cs        (1000)     2025 2023-09-18 11:22:06.000000 motion-learning-toolbox-1.0.5/tests/test_controller_mapping.py
--rw-rw-r--   0 cs        (1000) cs        (1000)      680 2023-09-15 13:17:03.000000 motion-learning-toolbox-1.0.5/tests/test_resample.py
--rw-rw-r--   0 cs        (1000) cs        (1000)     3222 2024-01-31 11:55:18.000000 motion-learning-toolbox-1.0.5/tests/test_to_body_relative.py
--rw-rw-r--   0 cs        (1000) cs        (1000)     3246 2024-01-31 12:07:04.000000 motion-learning-toolbox-1.0.5/tests/test_to_velocity.py
+drwxrwxr-x   0 cs        (1000) cs        (1000)        0 2024-04-23 08:51:14.836844 motion_learning_toolbox-1.0.6/
+-rw-rw-r--   0 cs        (1000) cs        (1000)      335 2023-09-15 13:17:03.000000 motion_learning_toolbox-1.0.6/License.md
+-rw-r--r--   0 cs        (1000) cs        (1000)     7700 2024-04-23 08:51:14.836844 motion_learning_toolbox-1.0.6/PKG-INFO
+-rw-rw-r--   0 cs        (1000) cs        (1000)     6557 2024-01-31 12:36:59.000000 motion_learning_toolbox-1.0.6/Readme.md
+drwxrwxr-x   0 cs        (1000) cs        (1000)        0 2024-04-23 08:51:14.832844 motion_learning_toolbox-1.0.6/motion_learning_toolbox/
+-rw-rw-r--   0 cs        (1000) cs        (1000)      335 2023-09-15 13:17:03.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox/__init__.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     1751 2023-09-15 13:17:03.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox/canonicalize_quaternions.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     2571 2023-09-18 11:20:31.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox/fix_controller_mapping.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     2369 2024-01-29 11:28:13.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox/resample.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)      573 2023-09-21 09:32:43.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox/to_acceleration.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     3710 2024-04-22 10:46:24.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox/to_body_relative.foo.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     5216 2024-04-23 08:47:42.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox/to_body_relative.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     3321 2024-04-23 08:49:35.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox/to_velocity.py
+drwxrwxr-x   0 cs        (1000) cs        (1000)        0 2024-04-23 08:51:14.832844 motion_learning_toolbox-1.0.6/motion_learning_toolbox.egg-info/
+-rw-r--r--   0 cs        (1000) cs        (1000)     7700 2024-04-23 08:51:14.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 cs        (1000) cs        (1000)      769 2024-04-23 08:51:14.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 cs        (1000) cs        (1000)        1 2024-04-23 08:51:14.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 cs        (1000) cs        (1000)       68 2024-04-23 08:51:14.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 cs        (1000) cs        (1000)       24 2024-04-23 08:51:14.000000 motion_learning_toolbox-1.0.6/motion_learning_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 cs        (1000) cs        (1000)      907 2024-04-23 08:50:40.000000 motion_learning_toolbox-1.0.6/pyproject.toml
+-rw-rw-r--   0 cs        (1000) cs        (1000)       38 2024-04-23 08:51:14.836844 motion_learning_toolbox-1.0.6/setup.cfg
+drwxrwxr-x   0 cs        (1000) cs        (1000)        0 2024-04-23 08:51:14.832844 motion_learning_toolbox-1.0.6/tests/
+-rw-rw-r--   0 cs        (1000) cs        (1000)     1105 2023-09-15 13:17:03.000000 motion_learning_toolbox-1.0.6/tests/test_canonicalize_quaternions.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     2025 2023-09-18 11:22:06.000000 motion_learning_toolbox-1.0.6/tests/test_controller_mapping.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)      680 2023-09-15 13:17:03.000000 motion_learning_toolbox-1.0.6/tests/test_resample.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     5684 2024-04-23 08:48:33.000000 motion_learning_toolbox-1.0.6/tests/test_to_body_relative.py
+-rw-rw-r--   0 cs        (1000) cs        (1000)     3650 2024-04-23 08:46:09.000000 motion_learning_toolbox-1.0.6/tests/test_to_velocity.py
```

### Comparing `motion-learning-toolbox-1.0.5/PKG-INFO` & `motion_learning_toolbox-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-learning-toolbox
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library for preprocessing of XR motion tracking data for machine learning applications.
 Author-email: Christian Rack <mail@chrisrack.de>, Lukas Schach <mail.lukas@schach.one>
 License: This work by Christian Rack, Lukas Schach and Marc E. Latoschik is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
 Project-URL: GitHub Repository, https://github.com/cschell/Motion-Learning-Toolbox
 Keywords: motion_data,preprocessing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 The library is still in active development and we continue to add and update functionality. Therefore, any feedback and contributions are very welcome!
 
 ## Origins
 
 The methods and techniques in this library have been developed, analysed and applied in our papers:
 
 1. ["Comparison of Data Encodings and Machine Learning Architectures for User Identification on Arbitrary Motion Sequences"](https://ieeexplore.ieee.org/document/10024474), 2022, C. Rack, A. Hotho and M. E. Latoschik, IEEE AIVR
-2. ["Who Is Alyx? A new Behavioral Biometric Dataset for User Identification in XR"](https://arxiv.org/abs/2308.03788), 2023, C. Rack, T.  Fernando, M. Yalcin, A. Hotho, and M. E. Latoschik, *arXiv e-prints*
+2. ["Who Is Alyx? A new Behavioral Biometric Dataset for User Identification in XR"](https://www.frontiersin.org/articles/10.3389/frvir.2023.1272234/full), 2023, C. Rack, T.  Fernando, M. Yalcin, A. Hotho, and M. E. Latoschik, Frontiers in Virtual Reality
 3. ["Extensible Motion-based Identification of XR Users using Non-Specific Motion Data"](https://arxiv.org/abs/2302.07517), 2023, C. Rack, K. Kobs, T. Fernando, A. Hotho, M. E. Latoschik, *arXiv e-prints*
 
 ## Importance of Data Encoding
 The core features of this library target the encoding of tracking data. Identifying users based on their motions usually starts with a raw stream of positional and rotational data, which we term scene-relative (SR) data. While SR data is informative, it includes information that can distort the learning objectives of identification models.  For instance, SR data includes not just user-specific characteristics but also information about the user's arbitrary position in the VR scene—features that don't contribute to user identity. To alleviate this, Motion Learning Toolbox offers additional encodings, such as:
 
 - **Body-Relative (BR) Data**: Transforms the coordinate system to a frame of reference attached to the user's head, thereby filtering out some of the scene-specific noise.
   
@@ -90,16 +90,16 @@
 
 We welcome any discussion, ideas and feedback around this library. Feel free to either open an issue on GitHub or directly contact Christian Rack or Lukas Schach.
 
 ## Development
 
 ### Build and publish library
 
-1. Bump versions in setup.py and pyproject.toml
-2. Build with `python setup.py build` and `python setup.py sdist`
+1. Bump version in pyproject.toml
+2. Build with `python -m build` (make sure `build` is installed, otherwise do `pip install build`)
 3. Upload to pypi with `twine upload -r pypi dist/* --skip-existing`
    - username: __token__
    - password: <api-token: pypi-...> 
 ## License Information
 
 <p xmlns:cc="http://creativecommons.org/ns#">
   This work by <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://hci.uni-wuerzburg.de">Christian Rack, Lukas Schach and Marc E. Latoschik</a> is
```

### Comparing `motion-learning-toolbox-1.0.5/Readme.md` & `motion_learning_toolbox-1.0.6/Readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 The library is still in active development and we continue to add and update functionality. Therefore, any feedback and contributions are very welcome!
 
 ## Origins
 
 The methods and techniques in this library have been developed, analysed and applied in our papers:
 
 1. ["Comparison of Data Encodings and Machine Learning Architectures for User Identification on Arbitrary Motion Sequences"](https://ieeexplore.ieee.org/document/10024474), 2022, C. Rack, A. Hotho and M. E. Latoschik, IEEE AIVR
-2. ["Who Is Alyx? A new Behavioral Biometric Dataset for User Identification in XR"](https://arxiv.org/abs/2308.03788), 2023, C. Rack, T.  Fernando, M. Yalcin, A. Hotho, and M. E. Latoschik, *arXiv e-prints*
+2. ["Who Is Alyx? A new Behavioral Biometric Dataset for User Identification in XR"](https://www.frontiersin.org/articles/10.3389/frvir.2023.1272234/full), 2023, C. Rack, T.  Fernando, M. Yalcin, A. Hotho, and M. E. Latoschik, Frontiers in Virtual Reality
 3. ["Extensible Motion-based Identification of XR Users using Non-Specific Motion Data"](https://arxiv.org/abs/2302.07517), 2023, C. Rack, K. Kobs, T. Fernando, A. Hotho, M. E. Latoschik, *arXiv e-prints*
 
 ## Importance of Data Encoding
 The core features of this library target the encoding of tracking data. Identifying users based on their motions usually starts with a raw stream of positional and rotational data, which we term scene-relative (SR) data. While SR data is informative, it includes information that can distort the learning objectives of identification models.  For instance, SR data includes not just user-specific characteristics but also information about the user's arbitrary position in the VR scene—features that don't contribute to user identity. To alleviate this, Motion Learning Toolbox offers additional encodings, such as:
 
 - **Body-Relative (BR) Data**: Transforms the coordinate system to a frame of reference attached to the user's head, thereby filtering out some of the scene-specific noise.
   
@@ -68,16 +68,16 @@
 
 We welcome any discussion, ideas and feedback around this library. Feel free to either open an issue on GitHub or directly contact Christian Rack or Lukas Schach.
 
 ## Development
 
 ### Build and publish library
 
-1. Bump versions in setup.py and pyproject.toml
-2. Build with `python setup.py build` and `python setup.py sdist`
+1. Bump version in pyproject.toml
+2. Build with `python -m build` (make sure `build` is installed, otherwise do `pip install build`)
 3. Upload to pypi with `twine upload -r pypi dist/* --skip-existing`
    - username: __token__
    - password: <api-token: pypi-...> 
 ## License Information
 
 <p xmlns:cc="http://creativecommons.org/ns#">
   This work by <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://hci.uni-wuerzburg.de">Christian Rack, Lukas Schach and Marc E. Latoschik</a> is
```

### Comparing `motion-learning-toolbox-1.0.5/motion_learning_toolbox/canonicalize_quaternions.py` & `motion_learning_toolbox-1.0.6/motion_learning_toolbox/canonicalize_quaternions.py`

 * *Files identical despite different names*

### Comparing `motion-learning-toolbox-1.0.5/motion_learning_toolbox/fix_controller_mapping.py` & `motion_learning_toolbox-1.0.6/motion_learning_toolbox/fix_controller_mapping.py`

 * *Files identical despite different names*

### Comparing `motion-learning-toolbox-1.0.5/motion_learning_toolbox/resample.py` & `motion_learning_toolbox-1.0.6/motion_learning_toolbox/resample.py`

 * *Files identical despite different names*

### Comparing `motion-learning-toolbox-1.0.5/motion_learning_toolbox/to_acceleration.py` & `motion_learning_toolbox-1.0.6/motion_learning_toolbox/to_acceleration.py`

 * *Files identical despite different names*

### Comparing `motion-learning-toolbox-1.0.5/motion_learning_toolbox/to_body_relative.py` & `motion_learning_toolbox-1.0.6/motion_learning_toolbox/to_body_relative.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, List
 import quaternionic
 import numpy as np
 import pandas as pd
 
+from .canonicalize_quaternions import canonicalize_quaternions
 
 def quaternion_composition(quaternion_array1, quaternion_array2):
     w1, x1, y1, z1 = (
         quaternion_array1[:, 0],
         quaternion_array1[:, 1],
         quaternion_array1[:, 2],
         quaternion_array1[:, 3],
@@ -99,9 +100,11 @@
         sr_rotations = quaternionic.array(frames[joint_rotation_names]).astype(target_dtype)
         br_rotations = quaternion_composition(correction_rotations.ndarray, sr_rotations.ndarray)
 
         relative_positions_and_rotations[joint_rotation_names] = br_rotations.normalized.astype(target_dtype).ndarray
 
     # add horizontal rotations of reference joint
     relative_positions_and_rotations[reference_rotation_names] = (correction_rotations * reference_rotations).normalized.astype(target_dtype).ndarray
+    
+    relative_positions_and_rotations = canonicalize_quaternions(relative_positions_and_rotations, joint_names=[reference_joint, *target_joints])
 
     return relative_positions_and_rotations
```

### Comparing `motion-learning-toolbox-1.0.5/motion_learning_toolbox/to_velocity.py` & `motion_learning_toolbox-1.0.6/motion_learning_toolbox/to_velocity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import numpy as np
 import pandas as pd
 from scipy.spatial.transform import Rotation
 
+from .canonicalize_quaternions import canonicalize_quaternions
 
 def compute_velocities_simple(data: pd.DataFrame, inplace=False) -> pd.DataFrame:
     """
     Calculates velocities from position data using a simple differencing method.
 
     :param data: A DataFrame containing position data.
     :param inplace: If True, the velocities are calculated in-place.
     :return: A DataFrame containing the calculated velocities with "delta_" prefix.
     """
     position_columns = [c for c in data.columns if "_pos_" in c]
     velocities = data if inplace else data.copy()
 
     velocities[position_columns] = velocities[position_columns].diff().fillna(np.nan)
-    velocities = velocities.rename(columns={column: f"delta_{column}" for column in position_columns if column in velocities.columns})
+    velocities.rename(columns={column: f"delta_{column}" for column in position_columns if column in velocities.columns}, inplace=True)
     return velocities[[f"delta_{column}" for column in position_columns]]
 
 
 def compute_velocities_quats(data: pd.DataFrame, inplace=False) -> pd.DataFrame:
     """
     Calculates velocities from rotation data using a simple differencing method.
 
@@ -28,40 +29,39 @@
     :return: A DataFrame containing the calculated velocities with "delta_" prefix.
     """
     velocities = data if inplace else data.copy()
 
     step_size = 1
 
     rotation_columns = [c for c in data.columns if "_rot_" in c]
-    # assert np.all(rotation_columns == data.columns), "rotation columns are wrong"
 
     joint_names = set([c[: -len("_rot_x")] for c in rotation_columns])
 
     for joint_name in joint_names:
         joint_rotation_names = [f"{joint_name}_rot_{c}" for c in "xyzw"]
         rotation_data = data[joint_rotation_names]
 
         # while computing acceleration values, we have to select the nan frames
         # (i.e., frames dismissed during the previous velocity value computation) and
         # exclude these
         nan_idxs = np.arange(len(rotation_data))[rotation_data.isna().any(axis=1)]
         rot = Rotation.from_quat(data[joint_rotation_names].fillna(0.25))
         delta_rot = rot[:-step_size].inv() * rot[step_size:]
         velocities.iloc[step_size:, velocities.columns.get_indexer(joint_rotation_names)] = delta_rot.as_quat()
-        # velocities.loc[step_size:, joint_rotation_names] = delta_rot.as_quat()  # old
 
     invalid_frames = np.concatenate(
         [
             nan_idxs,
             nan_idxs + step_size,
         ]
     )
 
     velocities[rotation_columns].values[invalid_frames, :] = np.nan
-    velocities = velocities.rename(columns={column: f"delta_{column}" for column in rotation_columns if column in velocities.columns})
+    canonicalize_quaternions(velocities, joint_names=joint_names, inplace=True)
+    velocities.rename(columns={column: f"delta_{column}" for column in rotation_columns if column in velocities.columns}, inplace=True)
 
     return velocities[[f"delta_{column}" for column in rotation_columns]]
 
 
 def to_velocity(data: pd.DataFrame, inplace=False) -> pd.DataFrame:
     """
     Calculates velocities from position and/or rotation data.
@@ -70,8 +70,9 @@
     :param inplace: If True, the velocities are calculated in-place (default is False).
     :return: A DataFrame containing the calculated velocities.
     """
     velocities = data if inplace else data.copy()
 
     positions = compute_velocities_simple(velocities, inplace)
     rotations = compute_velocities_quats(velocities, inplace)
+    
     return pd.concat([positions, rotations], axis=1)
```

### Comparing `motion-learning-toolbox-1.0.5/motion_learning_toolbox.egg-info/PKG-INFO` & `motion_learning_toolbox-1.0.6/motion_learning_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-learning-toolbox
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python library for preprocessing of XR motion tracking data for machine learning applications.
 Author-email: Christian Rack <mail@chrisrack.de>, Lukas Schach <mail.lukas@schach.one>
 License: This work by Christian Rack, Lukas Schach and Marc E. Latoschik is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/ or send a letter to Creative Commons, PO Box 1866, Mountain View, CA 94042, USA.
 Project-URL: GitHub Repository, https://github.com/cschell/Motion-Learning-Toolbox
 Keywords: motion_data,preprocessing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -27,15 +27,15 @@
 The library is still in active development and we continue to add and update functionality. Therefore, any feedback and contributions are very welcome!
 
 ## Origins
 
 The methods and techniques in this library have been developed, analysed and applied in our papers:
 
 1. ["Comparison of Data Encodings and Machine Learning Architectures for User Identification on Arbitrary Motion Sequences"](https://ieeexplore.ieee.org/document/10024474), 2022, C. Rack, A. Hotho and M. E. Latoschik, IEEE AIVR
-2. ["Who Is Alyx? A new Behavioral Biometric Dataset for User Identification in XR"](https://arxiv.org/abs/2308.03788), 2023, C. Rack, T.  Fernando, M. Yalcin, A. Hotho, and M. E. Latoschik, *arXiv e-prints*
+2. ["Who Is Alyx? A new Behavioral Biometric Dataset for User Identification in XR"](https://www.frontiersin.org/articles/10.3389/frvir.2023.1272234/full), 2023, C. Rack, T.  Fernando, M. Yalcin, A. Hotho, and M. E. Latoschik, Frontiers in Virtual Reality
 3. ["Extensible Motion-based Identification of XR Users using Non-Specific Motion Data"](https://arxiv.org/abs/2302.07517), 2023, C. Rack, K. Kobs, T. Fernando, A. Hotho, M. E. Latoschik, *arXiv e-prints*
 
 ## Importance of Data Encoding
 The core features of this library target the encoding of tracking data. Identifying users based on their motions usually starts with a raw stream of positional and rotational data, which we term scene-relative (SR) data. While SR data is informative, it includes information that can distort the learning objectives of identification models.  For instance, SR data includes not just user-specific characteristics but also information about the user's arbitrary position in the VR scene—features that don't contribute to user identity. To alleviate this, Motion Learning Toolbox offers additional encodings, such as:
 
 - **Body-Relative (BR) Data**: Transforms the coordinate system to a frame of reference attached to the user's head, thereby filtering out some of the scene-specific noise.
   
@@ -90,16 +90,16 @@
 
 We welcome any discussion, ideas and feedback around this library. Feel free to either open an issue on GitHub or directly contact Christian Rack or Lukas Schach.
 
 ## Development
 
 ### Build and publish library
 
-1. Bump versions in setup.py and pyproject.toml
-2. Build with `python setup.py build` and `python setup.py sdist`
+1. Bump version in pyproject.toml
+2. Build with `python -m build` (make sure `build` is installed, otherwise do `pip install build`)
 3. Upload to pypi with `twine upload -r pypi dist/* --skip-existing`
    - username: __token__
    - password: <api-token: pypi-...> 
 ## License Information
 
 <p xmlns:cc="http://creativecommons.org/ns#">
   This work by <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://hci.uni-wuerzburg.de">Christian Rack, Lukas Schach and Marc E. Latoschik</a> is
```

### Comparing `motion-learning-toolbox-1.0.5/motion_learning_toolbox.egg-info/SOURCES.txt` & `motion_learning_toolbox-1.0.6/motion_learning_toolbox.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Readme.md
 pyproject.toml
 motion_learning_toolbox/__init__.py
 motion_learning_toolbox/canonicalize_quaternions.py
 motion_learning_toolbox/fix_controller_mapping.py
 motion_learning_toolbox/resample.py
 motion_learning_toolbox/to_acceleration.py
+motion_learning_toolbox/to_body_relative.foo.py
 motion_learning_toolbox/to_body_relative.py
 motion_learning_toolbox/to_velocity.py
 motion_learning_toolbox.egg-info/PKG-INFO
 motion_learning_toolbox.egg-info/SOURCES.txt
 motion_learning_toolbox.egg-info/dependency_links.txt
 motion_learning_toolbox.egg-info/requires.txt
 motion_learning_toolbox.egg-info/top_level.txt
```

### Comparing `motion-learning-toolbox-1.0.5/pyproject.toml` & `motion_learning_toolbox-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion-learning-toolbox"
-version = "1.0.5"
+version = "1.0.6"
 description = "Python library for preprocessing of XR motion tracking data for machine learning applications."
 readme = "Readme.md"
 authors = [{ name = "Christian Rack", email = "mail@chrisrack.de" }, {name = "Lukas Schach", email="mail.lukas@schach.one" }]
 license = { file = "License.md" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3"
```

### Comparing `motion-learning-toolbox-1.0.5/tests/test_canonicalize_quaternions.py` & `motion_learning_toolbox-1.0.6/tests/test_canonicalize_quaternions.py`

 * *Files identical despite different names*

### Comparing `motion-learning-toolbox-1.0.5/tests/test_controller_mapping.py` & `motion_learning_toolbox-1.0.6/tests/test_controller_mapping.py`

 * *Files identical despite different names*

### Comparing `motion-learning-toolbox-1.0.5/tests/test_resample.py` & `motion_learning_toolbox-1.0.6/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `motion-learning-toolbox-1.0.5/tests/test_to_velocity.py` & `motion_learning_toolbox-1.0.6/tests/test_to_velocity.py`

 * *Files 25% similar despite different names*

```diff
@@ -46,25 +46,42 @@
     # Assumption 4: Rotating a frame by the following ang. velocity should yield the following frame's routation
     expected_rotations = (R.from_quat(test_df[:-1]) * R.from_quat(velocities_df[1:])).as_quat()
     actual_rotations = R.from_quat(test_df.iloc[1:]).as_quat()
 
     assert np.allclose(expected_rotations, actual_rotations)
 
 
+def test_compute_velocities_canonicalized_quats():
+    # Load test data
+    test_df1 = pd.read_csv("test_data.csv")[["hmd_rot_x", "hmd_rot_y", "hmd_rot_z", "hmd_rot_w"]]
+
+    test_df2 = test_df1.copy()
+    test_df2 *= -1
+
+    vel1 = to_velocity(test_df1)
+    vel2 = to_velocity(test_df2)
+
+    pd.testing.assert_frame_equal(vel1, vel2)
+
+
 def test_compute_velocities():
     # Load test data
-    test_df = pd.read_csv("test_data.csv")[["hmd_rot_x", "hmd_rot_y", "hmd_rot_z", "hmd_rot_w", "hmd_pos_x", "hmd_pos_y", "hmd_pos_z"]]
+    test_df = pd.read_csv("test_data.csv")[["hmd_rot_x", "hmd_rot_y", "hmd_rot_z", "hmd_rot_w", "hmd_pos_x", "hmd_pos_y", "hmd_pos_z"]].astype(float)
     velocities_df2 = test_df.copy()
 
     to_velocity(velocities_df2, inplace=True)
     velocities_df = to_velocity(test_df)
 
-    # Assumption 1: Output DataFrame has the same number of rows as input
     assert len(test_df) == len(velocities_df) == len(velocities_df2)
 
+    pd.testing.assert_frame_equal(
+        velocities_df2.sort_index(axis=1),
+        velocities_df.sort_index(axis=1),
+    )
+
 
 def test_compute_acceleration():
     # Load test data
     test_df = pd.read_csv("test_data.csv")[["hmd_rot_x", "hmd_rot_y", "hmd_rot_z", "hmd_rot_w", "hmd_pos_x", "hmd_pos_y", "hmd_pos_z"]]
 
     velocities_df = to_velocity(test_df)
     acceleration_df = to_acceleration(test_df)
```

