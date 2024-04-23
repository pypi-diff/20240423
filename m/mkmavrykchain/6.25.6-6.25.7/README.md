# Comparing `tmp/mkmavrykchain-6.25.6-py3-none-any.whl.zip` & `tmp/mkmavrykchain-6.25.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 9478 bytes, number of entries: 9
--rw-r--r--  2.0 unx      498 b- defN 24-Apr-23 09:48 mavrykchain/_version.py
--rw-r--r--  2.0 unx     1916 b- defN 24-Apr-23 09:48 mavrykchain/keys.py
--rw-r--r--  2.0 unx    12375 b- defN 24-Apr-23 09:48 mavrykchain/mkmavrykchain.py
--rw-r--r--  2.0 unx     2580 b- defN 24-Apr-23 09:48 mavrykchain/parameters.yaml
--rw-r--r--  2.0 unx     5164 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      753 b- defN 24-Apr-23 09:48 mkmavrykchain-6.25.6.dist-info/RECORD
-9 files, 23456 bytes uncompressed, 8172 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx      498 b- defN 24-Apr-23 10:10 mavrykchain/_version.py
+-rw-r--r--  2.0 unx     1918 b- defN 24-Apr-23 10:10 mavrykchain/keys.py
+-rw-r--r--  2.0 unx    12385 b- defN 24-Apr-23 10:10 mavrykchain/mkmavrykchain.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-Apr-23 10:10 mavrykchain/parameters.yaml
+-rw-r--r--  2.0 unx     5167 b- defN 24-Apr-23 10:10 mkmavrykchain-6.25.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 10:10 mkmavrykchain-6.25.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-23 10:10 mkmavrykchain-6.25.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-23 10:10 mkmavrykchain-6.25.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      753 b- defN 24-Apr-23 10:10 mkmavrykchain-6.25.7.dist-info/RECORD
+9 files, 23471 bytes uncompressed, 8172 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: mavrykchain/mkmavrykchain.py
 Comment: 
 
 Filename: mavrykchain/parameters.yaml
 Comment: 
 
-Filename: mkmavrykchain-6.25.6.dist-info/METADATA
+Filename: mkmavrykchain-6.25.7.dist-info/METADATA
 Comment: 
 
-Filename: mkmavrykchain-6.25.6.dist-info/WHEEL
+Filename: mkmavrykchain-6.25.7.dist-info/WHEEL
 Comment: 
 
-Filename: mkmavrykchain-6.25.6.dist-info/entry_points.txt
+Filename: mkmavrykchain-6.25.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.6.dist-info/top_level.txt
+Filename: mkmavrykchain-6.25.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mkmavrykchain-6.25.6.dist-info/RECORD
+Filename: mkmavrykchain-6.25.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mavrykchain/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2024-04-23T11:46:17+0200",
+ "date": "2024-04-23T12:05:12+0200",
  "dirty": false,
  "error": null,
- "full-revisionid": "56a783955d53fd40500e5d1c1b618d0859cebed8",
- "version": "6.25.6"
+ "full-revisionid": "2adfd6fb1fb76529e6363c87dba77ca6a559cff4",
+ "version": "6.25.7"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## mavrykchain/keys.py

```diff
@@ -53,14 +53,14 @@
         key = pymavryk.key.generate(export=False)
         return {"public": key.public_key(), "secret": key.secret_key()}
 
     keys = run_docker(
         image,
         "sh",
         "-c",
-        "'/usr/local/bin/octez-client "
+        "'/usr/local/bin/mavkit-client "
         + "--protocol PsDELPH1Kxsx gen keys mykey && "
-        + "/usr/local/bin/octez-client "
+        + "/usr/local/bin/mavkit-client "
         + "--protocol PsDELPH1Kxsx show address mykey -S'",
     ).split(b"\n")
 
     return {"public": extract_key(keys, 1), "secret": extract_key(keys, 2)}
```

## mavrykchain/mkmavrykchain.py

```diff
@@ -36,15 +36,15 @@
 ROLLING_REGULAR_NODE_NAME = "rolling-node"
 
 
 cli_args = {
     "should_generate_unsafe_deterministic_data": {
         "help": (
             "Should mavryk-k8s generate deterministic account keys and genesis"
-            " block hash instead of mkmavrykchain using octez-client to generate"
+            " block hash instead of mkmavrykchain using mavkit-client to generate"
             " random ones. This option is helpful for testing purposes."
         ),
         "action": "store_true",
         "default": False,
     },
     "number_of_nodes": {
         "help": "number of peers in the cluster",
@@ -64,17 +64,17 @@
         "type": int,
     },
     "bootstrap_peers": {
         "help": "Bootstrap addresses to connect to. Can specify multiple.",
         "action": "extend",
         "nargs": "+",
     },
-    "octez_docker_image": {
-        "help": "Version of the Octez docker image",
-        "default": "mavrykdynamics/mavryk:v17.3",
+    "mavkit_docker_image": {
+        "help": "Version of the Mavkit docker image",
+        "default": "mavrykdynamics/mavryk:v19.3",
     },
     "use_docker": {
         "action": "store_true",
         "default": None,
     },
     "no_use_docker": {
         "dest": "use_docker",
@@ -168,15 +168,15 @@
     args = get_args()
 
     validate_args(args)
     set_use_docker(args.use_docker)
 
     base_constants = {
         "images": {
-            "octez": args.octez_docker_image,
+            "mavkit": args.mavkit_docker_image,
         },
         "node_config_network": {"chain_name": args.chain_name},
         "zerotier_config": {
             "zerotier_network": args.zerotier_network,
             "zerotier_token": args.zerotier_token,
         },
         # Custom chains should not pull snapshots or tarballs
@@ -242,29 +242,29 @@
             accounts["public"] = old_invite_values["accounts"]
     elif not args.should_generate_unsafe_deterministic_data:
         baking_accounts = {
             f"{ARCHIVE_BAKER_NODE_NAME}-{n}": {} for n in range(args.number_of_bakers)
         }
         for account in [*baking_accounts, "authorized-key-0"]:
             print(f"Generating keys for account {account}")
-            keys = gen_key(args.octez_docker_image)
+            keys = gen_key(args.mavkit_docker_image)
             for key_type in keys:
                 accounts[key_type][account] = {
                     "key": keys[key_type],
                     "is_bootstrap_baker_account": (
                         False if account == "authorized-key-0" else True
                     ),
                     "bootstrap_balance": "4000000000000",
                 }
 
     # First 2 bakers are acting as bootstrap nodes for the others, and run in
     # archive mode. Any other bakers will be in rolling mode.
     creation_nodes = {
         ARCHIVE_BAKER_NODE_NAME: {
-            "runs": ["octez_node", "baker"],
+            "runs": ["mavkit_node", "baker"],
             "storage_size": "15Gi",
             "instances": [
                 node_config(ARCHIVE_BAKER_NODE_NAME, n, is_baker=True)
                 for n in range(args.number_of_bakers)
             ],
         },
         ROLLING_REGULAR_NODE_NAME: None,
@@ -274,15 +274,15 @@
             "storage_size": "15Gi",
             "instances": [
                 node_config(ROLLING_REGULAR_NODE_NAME, n, is_baker=False)
                 for n in range(args.number_of_nodes)
             ],
         }
 
-    octezSigners = {
+    mavkitSigners = {
         "mavryk-signer-0": {
             "accounts": [
                 f"{ARCHIVE_BAKER_NODE_NAME}-{n}" for n in range(args.number_of_bakers)
             ],
             "authorized_keys": ["authorized-key-0"],
         }
     }
@@ -308,15 +308,15 @@
     creation_constants = {
         "is_invitation": False,
         "should_generate_unsafe_deterministic_data": args.should_generate_unsafe_deterministic_data,
         "expected_proof_of_work": args.expected_proof_of_work,
         **base_constants,
         "bootstrap_peers": bootstrap_peers,
         "accounts": accounts["secret"],
-        "octezSigners": octezSigners,
+        "mavkitSigners": mavkitSigners,
         "nodes": creation_nodes,
         **activation,
     }
 
     with open(f"{files_path}_values.yaml", "w") as yaml_file:
         yaml.dump(
             creation_constants,
```

## Comparing `mkmavrykchain-6.25.6.dist-info/METADATA` & `mkmavrykchain-6.25.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkmavrykchain
-Version: 6.25.6
+Version: 6.25.7
 Summary: A utility to generate k8s configs for a Mavryk blockchain
 Home-page: https://github.com/mavryk-network/mavryk-k8s
 Author: MavrykDynamics
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -102,15 +102,15 @@
 | -------------------------------- | ------------------------ | -------------------------------------------------------------- | ----------------------- |
 |                                  | -h                       | mkmavrykchain help message                                           |                         |
 |                                  | -v                       | mkmavrykchain version                                                |                         |
 |                                  | --number-of-bakers       | Number of baking nodes in the cluster                          | 1                       |
 |                                  | --number-of-nodes        | Number of non-baking nodes in the cluster                      | 0                       |
 | bootstrap_peers                  | --bootstrap-peers        | Peer ips to connect to                                         | []                      |
 | expected_proof_of_work           | --expected-proof-of-work | Node identity generation difficulty                            | 0                       |
-| images.octez                     | --octez-docker-image     | Version of the Octez docker image to run                       | mavrykdynamics/mavryk:v17.3 |
+| images.mavkit                     | --mavkit-docker-image     | Version of the Mavkit docker image to run                       | mavrykdynamics/mavryk:v19.3 |
 |                                  | --use-docker (--no...)   | Use (or don't use) docker to generate keys rather than pymavryk | autodetect              |
 | zerotier_config.zerotier_network | --zerotier-network       | Zerotier network id for external chain access                  |                         |
 | zerotier_config.zerotier_token   | --zerotier-token         | Zerotier token for external chain access                       |                         |
 
 ## Create Mavryk Chain
 
 Make sure you have the Mavryk Helm chart repo:
```

