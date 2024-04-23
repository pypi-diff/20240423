# Comparing `tmp/gimme-aws-creds-2.8.0.tar.gz` & `tmp/gimme_aws_creds-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimme-aws-creds-2.8.0.tar", last modified: Mon Feb 12 20:10:16 2024, max compression
+gzip compressed data, was "gimme_aws_creds-2.8.1.tar", last modified: Tue Apr 23 14:09:04 2024, max compression
```

## Comparing `gimme-aws-creds-2.8.0.tar` & `gimme_aws_creds-2.8.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:10:16.928643 gimme-aws-creds-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/LONG_DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-12 20:10:16.928643 gimme-aws-creds-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20282 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:10:16.920643 gimme-aws-creds-2.8.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      753 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/bin/gimme-aws-creds
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/bin/gimme-aws-creds-autocomplete.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/bin/gimme-aws-creds.cmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:10:16.924643 gimme-aws-creds-2.8.0/gimme_aws_creds/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    31340 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/duo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/duo_universal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    38614 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    49044 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/okta_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/okta_identity_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/registered_authenticators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/gimme_aws_creds/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:10:16.928643 gimme-aws-creds-2.8.0/gimme_aws_creds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-12 20:10:16.000000 gimme-aws-creds-2.8.0/gimme_aws_creds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-12 20:10:16.000000 gimme-aws-creds-2.8.0/gimme_aws_creds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 20:10:16.000000 gimme-aws-creds-2.8.0/gimme_aws_creds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-12 20:10:16.000000 gimme-aws-creds-2.8.0/gimme_aws_creds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-12 20:10:16.000000 gimme-aws-creds-2.8.0/gimme_aws_creds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-12 20:10:16.928643 gimme-aws-creds-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 20:10:16.928643 gimme-aws-creds-2.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/tests/test_aws_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/tests/test_duo_universal_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    61157 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/tests/test_okta_classic_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    70663 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/tests/test_okta_identity_engine_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-02-12 20:09:50.000000 gimme-aws-creds-2.8.0/tests/test_registered_authenticators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/LONG_DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20414 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.253857 gimme_aws_creds-2.8.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      753 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/bin/gimme-aws-creds
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/bin/gimme-aws-creds-autocomplete.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/bin/gimme-aws-creds.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/gimme_aws_creds/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31632 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/duo_universal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38953 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50285 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/okta_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/okta_identity_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/registered_authenticators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_aws_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_duo_universal_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61157 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_okta_classic_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70663 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_okta_identity_engine_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_registered_authenticators.py
```

### Comparing `gimme-aws-creds-2.8.0/LICENSE` & `gimme_aws_creds-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/LONG_DESCRIPTION.md` & `gimme_aws_creds-2.8.1/LONG_DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/NOTICE` & `gimme_aws_creds-2.8.1/NOTICE`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/PKG-INFO` & `gimme_aws_creds-2.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gimme-aws-creds
-Version: 2.8.0
+Name: gimme_aws_creds
+Version: 2.8.1
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `gimme-aws-creds-2.8.0/README.md` & `gimme_aws_creds-2.8.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -224,14 +224,18 @@
   - token:hardware - OTP using hardware like Yubikey
   - call - OTP via Voice call
   - sms - OTP via SMS message
   - email - OTP via email
   - web - DUO uses localhost webbrowser to support push|call|passcode
   - passcode - DUO uses `OKTA_MFA_CODE` or `--mfa-code` if set, or prompts user for passcode(OTP).
   - claims_provider - DUO Universal Prompt
+- preferred_mfa_provider - (optional) automatically select a particular provider when prompted for MFA:
+  - GOOGLE
+  - OKTA
+  - DUO
 - duo_universal_factor - (optional) Configure which type of factor to use with Duo Universal Prompt. Must be one of (case-sensitive):
   - `Duo Push` (default)
   - `Passcode`
   - `Phone Call`
 - resolve_aws_alias - y or n. If yes, gimme-aws-creds will try to resolve AWS account ids with respective alias names (default: n). This option can also be set interactively in the command line using `-r` or `--resolve` parameter
 - include_path - (optional) Includes full role path to the role name in AWS credential profile name. (default: n).  If `y`: `<acct>-/some/path/administrator`. If `n`: `<acct>-administrator`
 - remember_device - y or n. If yes, the MFA device will be remembered by Okta service for a limited time. This option can also be set interactively in the command line using `-m` or `--remember-device`
```

### Comparing `gimme-aws-creds-2.8.0/bin/gimme-aws-creds` & `gimme_aws_creds-2.8.1/bin/gimme-aws-creds`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/bin/gimme-aws-creds-autocomplete.sh` & `gimme_aws_creds-2.8.1/bin/gimme-aws-creds-autocomplete.sh`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/bin/gimme-aws-creds.cmd` & `gimme_aws_creds-2.8.1/bin/gimme-aws-creds.cmd`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/aws.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/aws.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/common.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/common.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/config.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,14 +197,18 @@
     def _handle_config(self, config, profile_config, include_inherits = True):
         # Convert True/False strings to booleans
         for key in profile_config:
             if profile_config[key] == 'True':
                 profile_config[key] = True
             elif profile_config[key] == 'False':
                 profile_config[key] = False
+        
+        # Empty string in force_classic should be handled as True - this makes sure that migrating from Classic to OIE is seamless
+        if profile_config.get('force_classic') == '' or profile_config.get('force_classic') is None:
+            profile_config['force_classic'] = True
 
         if "inherits" in profile_config.keys() and include_inherits:
             self.ui.message("Using inherited config: " + profile_config["inherits"])
             if profile_config["inherits"] not in config:
                 raise errors.GimmeAWSCredsError(self.conf_profile + " inherits from " + profile_config["inherits"] + ", but could not find " + profile_config["inherits"])
             combined_config = {
                 **self._handle_config(config, dict(config[profile_config["inherits"]])),
```

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/default.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/default.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/duo.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/duo.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/duo_universal.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/duo_universal.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/errors.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/errors.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/main.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         self.ui = ui
         self.FILE_ROOT = self.ui.HOME
         self.AWS_CONFIG = self.ui.environ.get(
             'AWS_SHARED_CREDENTIALS_FILE',
             os.path.join(self.FILE_ROOT, '.aws', 'credentials')
         )
         self._cache = {}
+        self.skip_DT = False
 
     #  this is modified code from https://github.com/nimbusscale/okta_aws_login
     def _write_aws_creds(self, profile, access_key, secret_key, token, expiration, aws_config=None):
         """ Writes the AWS STS token into the AWS credential file"""
         # Check to see if the aws creds path exists, if not create it
         aws_config = aws_config or self.AWS_CONFIG
         creds_dir = os.path.dirname(aws_config)
@@ -501,20 +502,14 @@
         self._cache['okta_platform'] = okta_platform
 
     @property
     def okta_platform(self):
         if 'okta_platform' in self._cache:
             return self._cache['okta_platform']
 
-        # Treat this domain as classic, even if it's OIE
-        if self.config.force_classic == True or self.conf_dict.get('force_classic') == "True":
-            self.ui.message('Okta Classic login flow enabled')
-            self.set_okta_platform('classic')
-            return 'classic'
-
         response = requests.get(
             self.okta_org_url + '/.well-known/okta-organization',
             headers={
                 'Accept': 'application/json',
                 'User-Agent': "gimme-aws-creds {}".format(version)
             },
             timeout=30
@@ -523,16 +518,23 @@
         response_data = response.json()
 
         if response.status_code == 200:
             if response_data['pipeline'] == 'v1':
                 ret = 'classic'
             elif response_data['pipeline'] == 'idx':
                 ret = 'identity_engine'
-                if not self.conf_dict.get('client_id'):
-                    raise errors.GimmeAWSCredsError('OAuth Client ID is required for Okta Identity Engine domains.  Try running --config again.')
+                # Force_Classic is set - treat this domain as classic
+                if self.config.force_classic is True or self.conf_dict.get('force_classic') is True:
+                    self.ui.message('Okta Classic login flow enabled')
+                    ret = 'classic'
+                    # Skip Device Token registration
+                    self.skip_DT = True
+                else:
+                    if not self.conf_dict.get('client_id'):
+                        raise errors.GimmeAWSCredsError('OAuth Client ID is required for Okta Identity Engine domains.  Try running --config again.')
             else:
                 raise RuntimeError('Unknown Okta platform type: {}'.format(response_data['pipeline']))
         else:
             response.raise_for_status()
 
         self.set_okta_platform(ret)
         return ret
@@ -579,14 +581,17 @@
 
             if self.conf_dict.get('okta_password'):
                 okta.set_password(self.conf_dict['okta_password'])
 
             if self.conf_dict.get('preferred_mfa_type'):
                 okta.set_preferred_mfa_type(self.conf_dict['preferred_mfa_type'])
 
+            if self.conf_dict.get('preferred_mfa_provider'):
+                okta.set_preferred_mfa_provider(self.conf_dict['preferred_mfa_provider'])
+
             if self.conf_dict.get('duo_universal_factor'):
                 okta.set_duo_universal_factor(self.conf_dict.get('duo_universal_factor'))
 
             if self.config.mfa_code is not None:
                 okta.set_mfa_code(self.config.mfa_code)
             elif self.conf_dict.get('okta_mfa_code'):
                 okta.set_mfa_code(self.conf_dict.get('okta_mfa_code'))
@@ -600,27 +605,27 @@
             return AwsResolver(self.config.verify_ssl_certs)
         elif str(self.conf_dict.get('resolve_aws_alias')) == 'True':
             return AwsResolver(self.config.verify_ssl_certs)
         return self.resolver
 
     @property
     def device_token(self):
-        if self.config.action_register_device is True:
+        if self.config.action_register_device is True or self.skip_DT is True:
             self.conf_dict['device_token'] = None
 
         return self.conf_dict.get('device_token')
 
     def set_auth_session(self, auth_session):
         self._cache['auth_session'] = auth_session
 
     @property
     def auth_session(self):
         if 'auth_session' in self._cache:
             return self._cache['auth_session']
-        if self.config.open_browser is True or self.conf_dict.get('open_browser') == "True":
+        if self.config.open_browser is True or self.conf_dict.get('open_browser') is True:
             open_browser = True
         else:
             open_browser = False
         auth_result = self.okta.auth_session(redirect_uri=self.conf_dict.get('app_url'), open_browser=open_browser)
         self.set_auth_session(auth_result)
 
         return auth_result
@@ -937,15 +942,15 @@
                 self.ui.warning('error parsing json line {}'.format(repr(line)))
                 continue
             self.write_aws_creds_from_data(data)
         raise errors.GimmeAWSCredsExitSuccess()
 
     def handle_action_register_device(self):
         # Capture the Device Token and write it to the config file
-        if self.okta_platform == "classic" and ( not self.device_token or self.config.action_register_device is True ):
+        if self.okta_platform == "classic" and self.skip_DT is False and ( not self.device_token or self.config.action_register_device is True ):
             if not self.config.action_register_device:
                 self.ui.notify('\n*** No device token found in configuration file, it will be created.')
                 self.ui.notify('*** You may be prompted for MFA more than once for this run.\n')
 
             auth_result = self.auth_session
             base_config = self.config.get_config_dict(include_inherits = False)
             base_config['device_token'] = auth_result['device_token']
```

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/okta_classic.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/okta_classic.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
         if verify_ssl_certs is False:
             requests.packages.urllib3.disable_warnings()
 
         self._username = None
         self._password = None
         self._preferred_mfa_type = None
+        self._preferred_mfa_provider = None
         self._duo_universal_factor = 'Duo Push'
         self._mfa_code = None
         self._remember_device = None
 
         self._use_oauth_access_token = False
         self._use_oauth_id_token = False
         self._oauth_access_token = None
@@ -101,14 +102,17 @@
 
     def set_password(self, password):
         self._password = password
 
     def set_preferred_mfa_type(self, preferred_mfa_type):
         self._preferred_mfa_type = preferred_mfa_type
 
+    def set_preferred_mfa_provider(self, preferred_mfa_provider):
+        self._preferred_mfa_provider = preferred_mfa_provider
+
     def set_mfa_code(self, mfa_code):
         self._mfa_code = mfa_code
 
     def set_duo_universal_factor(self, duo_universal_factor):
         self._duo_universal_factor = duo_universal_factor
 
     def set_remember_device(self, remember_device):
@@ -253,14 +257,19 @@
             params=params,
             headers=self._get_headers(),
             verify=self._verify_ssl_certs,
             allow_redirects=False
         )
         response.raise_for_status()
 
+        # If we didn't get a 302 redirect, the MFA factor didn't meet the requirement for the app
+        if 'Location' not in response.headers:
+            raise errors.GimmeAWSCredsError(
+                "LOGIN ERROR: Provided MFA factor does not meet the authentication policies for this application", 2
+            )
         url_parse_results = urlparse(response.headers['Location'])
 
         query_result = parse_qs(url_parse_results.fragment)
 
         tokens = {}
         if 'access_token' in query_result:
             tokens['access_token'] = query_result['access_token'][0]
@@ -833,14 +842,27 @@
         if self._preferred_mfa_type is not None:
             preferred_factors = list(filter(lambda item: item['factorType'] == self._preferred_mfa_type, factors))
             # If the preferred factor isn't in the list of available factors, we'll let the user know before
             # prompting to select another.
             if not preferred_factors:
                 self.ui.notify('Preferred factor type of {} not available.'.format(self._preferred_mfa_type))
 
+        if self._preferred_mfa_provider is not None:
+            preferred_factors_with_preferred_provider = list(
+                filter(lambda item: item['provider'] == self._preferred_mfa_provider, preferred_factors)
+            )
+            # If filtering for the preferred provider yields no results, announce it,
+            # but don't update the list of preferred factors.
+            if preferred_factors and not preferred_factors_with_preferred_provider:
+                self.ui.notify('Preferred factor provider of {} not available. Will use available factors.'.format(
+                    self._preferred_mfa_provider
+                ))
+            else:
+                preferred_factors = preferred_factors_with_preferred_provider
+
         if len(preferred_factors) == 1:
             factor_name = self._build_factor_name(preferred_factors[0])
             self.ui.info(factor_name + ' selected')
             selection = factors.index(preferred_factors[0])
         elif len(factors) == 1:
             factor_name = self._build_factor_name(factors[0])
             print("Using the only authentication factor configured: {}.".format(factor_name))
```

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/okta_identity_engine.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/okta_identity_engine.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/registered_authenticators.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/registered_authenticators.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/u2f.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/u2f.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/ui.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/ui.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds/webauthn.py` & `gimme_aws_creds-2.8.1/gimme_aws_creds/webauthn.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds.egg-info/PKG-INFO` & `gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gimme-aws-creds
-Version: 2.8.0
+Name: gimme_aws_creds
+Version: 2.8.1
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `gimme-aws-creds-2.8.0/gimme_aws_creds.egg-info/SOURCES.txt` & `gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/setup.py` & `gimme_aws_creds-2.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
-    name='gimme-aws-creds',
-    version='2.8.0',
+    name='gimme_aws_creds',
+    version='2.8.1',
     install_requires=requirements,
     author='Eric Pierce',
     author_email='eric.pierce@nike.com',
     description="A CLI to get temporary AWS credentials from Okta",
     url='https://github.com/Nike-Inc/gimme-aws-creds',
     long_description=open("LONG_DESCRIPTION.md").read(),
     python_requires=">=3.7",
```

### Comparing `gimme-aws-creds-2.8.0/tests/test_aws_resolver.py` & `gimme_aws_creds-2.8.1/tests/test_aws_resolver.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/tests/test_config.py` & `gimme_aws_creds-2.8.1/tests/test_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,42 +57,44 @@
             config_file.write("""
 [myprofile]
 client_id = foo
 """)
         config = Config(gac_ui=test_ui, create_config=False)
         config.conf_profile = "myprofile"
         profile_config = config.get_config_dict()
-        self.assertEqual(profile_config, {"client_id": "foo"})
+        self.assertEqual(profile_config, {"client_id": "foo", 'force_classic': True})
 
     def test_read_config_inherited(self):
         """Test to make sure getting config works when inherited"""
         test_ui = MockUserInterface(argv=[
             "--profile",
             "myprofile",
         ])
         with open(test_ui.HOME + "/.okta_aws_login_config", "w") as config_file:
             config_file.write(
                 """
                 [mybase]
                 client_id = bar
                 aws_appname = baz
+                force_classic = True
                 [myprofile]
                 inherits = mybase
                 client_id = foo
                 aws_rolename = myrole
                 """
             )
 
         config = Config(gac_ui=test_ui, create_config=False)
         config.conf_profile = "myprofile"
         profile_config = config.get_config_dict()
         self.assertEqual(profile_config, {
             "client_id": "foo",
             "aws_appname": "baz",
             "aws_rolename": "myrole",
+            'force_classic': True,
         })
 
     def test_read_nested_config_inherited(self):
         """Test to make sure getting config works when inherited"""
         test_ui = MockUserInterface(argv = [
             "--profile",
             "myprofile",
@@ -100,26 +102,28 @@
         with open(test_ui.HOME + "/.okta_aws_login_config", "w") as config_file:
             config_file.write("""
 [mybase-level1]
 client_id = bar
 [mybase-level2]
 inherits = mybase-level1
 aws_appname = baz
+force_classic = 
 [myprofile]
 inherits = mybase-level2
 client_id = foo
 aws_rolename = myrole
 """)
         config = Config(gac_ui=test_ui, create_config=False)
         config.conf_profile = "myprofile"
         profile_config = config.get_config_dict()
         self.assertEqual(profile_config, {
             "client_id": "foo",
             "aws_appname": "baz",
             "aws_rolename": "myrole",
+            "force_classic": True
         })
 
     def test_fail_if_profile_not_found(self):
         """Test to make sure missing Default fails properly"""
         test_ui = MockUserInterface(argv=[])
         with open(test_ui.HOME + "/.okta_aws_login_config", "w") as config_file:
             config_file.write("""
```

### Comparing `gimme-aws-creds-2.8.0/tests/test_duo_universal_client.py` & `gimme_aws_creds-2.8.1/tests/test_duo_universal_client.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/tests/test_main.py` & `gimme_aws_creds-2.8.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/tests/test_okta_classic_client.py` & `gimme_aws_creds-2.8.1/tests/test_okta_classic_client.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/tests/test_okta_identity_engine_client.py` & `gimme_aws_creds-2.8.1/tests/test_okta_identity_engine_client.py`

 * *Files identical despite different names*

### Comparing `gimme-aws-creds-2.8.0/tests/test_registered_authenticators.py` & `gimme_aws_creds-2.8.1/tests/test_registered_authenticators.py`

 * *Files identical despite different names*

