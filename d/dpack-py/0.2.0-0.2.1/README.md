# Comparing `tmp/dpack_py-0.2.0.tar.gz` & `tmp/dpack_py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpack_py-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dpack_py-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dpack_py-0.2.0.tar` & `dpack_py-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       27 2024-04-22 18:27:21.236302 dpack_py-0.2.0/.gitignore
--rw-r--r--   0        0        0      100 2024-04-22 18:30:45.593747 dpack_py-0.2.0/Makefile
--rw-r--r--   0        0        0     7397 2024-04-22 18:26:09.899181 dpack_py-0.2.0/examples/uniswap-v3.dpack.json
--rw-r--r--   0        0        0     2156 2024-04-22 18:08:54.448859 dpack_py-0.2.0/examples/uniswap.py
--rw-r--r--   0        0        0      555 2024-04-22 22:21:45.543441 dpack_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4636 2024-04-22 22:21:26.863611 dpack_py-0.2.0/readme.md
--rw-r--r--   0        0        0       55 2024-04-22 16:49:07.422511 dpack_py-0.2.0/src/dpack/__init__.py
--rw-r--r--   0        0        0     1198 2024-04-22 22:09:39.235312 dpack_py-0.2.0/src/dpack/ape.py
--rw-r--r--   0        0        0     2885 2024-04-22 19:07:37.069606 dpack_py-0.2.0/src/dpack/dpack.py
--rw-r--r--   0        0        0     2407 2024-04-22 16:52:36.990501 dpack_py-0.2.0/tests/test_dpack.py
--rw-r--r--   0        0        0    10293 2024-04-22 10:38:52.852458 dpack_py-0.2.0/tests/weth-ropsten-artifact.json
--rw-r--r--   0        0        0      723 2024-04-21 07:13:55.705183 dpack_py-0.2.0/tests/weth_ropsten.dpack.json
--rw-r--r--   0        0        0     5206 1970-01-01 00:00:00.000000 dpack_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-04-22 18:27:21.236302 dpack_py-0.2.1/.gitignore
+-rw-r--r--   0        0        0      100 2024-04-22 18:30:45.593747 dpack_py-0.2.1/Makefile
+-rw-r--r--   0        0        0     7398 2024-04-23 13:10:17.896775 dpack_py-0.2.1/examples/uniswap-v3.dpack.json
+-rw-r--r--   0        0        0     2555 2024-04-23 13:10:09.129746 dpack_py-0.2.1/examples/uniswap.py
+-rw-r--r--   0        0        0      555 2024-04-23 13:15:40.662308 dpack_py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4636 2024-04-22 22:21:26.863611 dpack_py-0.2.1/readme.md
+-rw-r--r--   0        0        0       55 2024-04-22 16:49:07.422511 dpack_py-0.2.1/src/dpack/__init__.py
+-rw-r--r--   0        0        0     1198 2024-04-22 22:09:39.235312 dpack_py-0.2.1/src/dpack/ape.py
+-rw-r--r--   0        0        0     3006 2024-04-23 13:15:23.502221 dpack_py-0.2.1/src/dpack/dpack.py
+-rw-r--r--   0        0        0     2452 2024-04-23 13:15:18.878780 dpack_py-0.2.1/tests/test_dpack.py
+-rw-r--r--   0        0        0    10293 2024-04-22 10:38:52.852458 dpack_py-0.2.1/tests/weth-ropsten-artifact.json
+-rw-r--r--   0        0        0      723 2024-04-21 07:13:55.705183 dpack_py-0.2.1/tests/weth_ropsten.dpack.json
+-rw-r--r--   0        0        0     5206 1970-01-01 00:00:00.000000 dpack_py-0.2.1/PKG-INFO
```

### Comparing `dpack_py-0.2.0/examples/uniswap-v3.dpack.json` & `dpack_py-0.2.1/examples/uniswap-v3.dpack.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.86328125%*

 * *Differences: {"'network'": "'ethereum'",*

 * * "'objects'": "{'factory': {'artifact': {'/': "*

 * *              "'bafkreiecs7ltlmc2sg5rvlovum5t7hcf5bxuwhvpujdcd4vx2obnk25jhm'}}, 'multicall': "*

 * *              "{'artifact': {'/': 'bafkreibvnxd7qhm5ppxsc45r3gfp2ggp3wgx7nrz223rg5pglacwgufnve'}}, "*

 * *              "'multicall2': {'artifact': {'/': "*

 * *              "'bafkreif5hugwwzhqaayfjujum2yj6aaj7bv6fyzpv5apdb4ndwwlyfraji'}}, 'proxy_admin': "*

 * *              "{'artifact': {'/': 'bafkreift2anfyw3xo2rpyqfpo4565jdp5tuizjknvcaukgupvf7wy22kr […]*

```diff
@@ -1,240 +1,240 @@
 {
     "format": "dpack-1",
-    "network": "mainnet",
+    "network": "ethereum",
     "objects": {
         "factory": {
             "address": "0x1F98431c8aD98523631AE4a59f267346ea31F984",
             "artifact": {
-                "/": "bafkreicfd2yml7evjxgssrqgzkb2qkyobvmonp5us2w3xqtr2zuuqzl4ku"
+                "/": "bafkreiecs7ltlmc2sg5rvlovum5t7hcf5bxuwhvpujdcd4vx2obnk25jhm"
             },
             "objectname": "factory",
             "typename": "UniswapV3Factory"
         },
         "multicall": {
             "address": "0x1F98415757620B543A52E61c46B32eB19261F984",
             "artifact": {
-                "/": "bafkreicd25dxfrtvn2oavbipzsp237dvbkbhsjeqr6ouuo23s5xhhj377e"
+                "/": "bafkreibvnxd7qhm5ppxsc45r3gfp2ggp3wgx7nrz223rg5pglacwgufnve"
             },
             "objectname": "multicall",
             "typename": "UniswapInterfaceMulticall"
         },
         "multicall2": {
             "address": "0x5BA1e12693Dc8F9c48aAD8770482f4739bEeD696",
             "artifact": {
-                "/": "bafkreifdsw4uxxzq4e7judcpdhlh4nwush33kkxbjna5lkxy2d5mbfqmja"
+                "/": "bafkreif5hugwwzhqaayfjujum2yj6aaj7bv6fyzpv5apdb4ndwwlyfraji"
             },
             "objectname": "multicall2",
             "typename": "Multicall2"
         },
         "nft_descriptor": {
             "address": "0x42B24A95702b9986e82d421cC3568932790A48Ec",
             "artifact": {
-                "/": "bafkreid4545gqtrx4hptvotnb5osdy7ofewzzxifxhumvvrqkr4e773ace"
+                "/": "bafkreicwyd57wsz7b5a6lz3i24mgh2xldsdcyjc45chmzyzkrwtbhzogdu"
             },
             "objectname": "nft_descriptor",
             "typename": "NFTDescriptor"
         },
         "nonfungible_position_manager": {
             "address": "0xC36442b4a4522E871399CD717aBDD847Ab11FE88",
             "artifact": {
-                "/": "bafkreic2gyd3oj5iyxrv6rdcidc22bqvbc6ypous6xv4klvptsscsgbpx4"
+                "/": "bafkreihu2zyfq4lh7tpughmajmgo5uu27kjspn55jo7zmkqhgzxqt64fdu"
             },
             "objectname": "nonfungible_position_manager",
             "typename": "NonfungiblePositionManager"
         },
         "nonfungible_token_position_descriptor": {
             "address": "0x91ae842A5Ffd8d12023116943e72A606179294f3",
             "artifact": {
-                "/": "bafkreic2doioye74gf34crxggv4bso36xsamq5vsbsaktqluo5mnr4vv3q"
+                "/": "bafkreieo6gqe5nbvvichcl7rr7yyzp4gc2vji427xyfv2e7cacjr2nojnq"
             },
             "objectname": "nonfungible_token_position_descriptor",
             "typename": "NonfungibleTokenPositionDescriptor"
         },
         "permit_2": {
             "address": "0x000000000022D473030F116dDEE9F6B43aC78BA3",
             "artifact": {
-                "/": "bafkreicttw522lrgona4yv2h43fy6b3q4jmm526k2tmm2azreh4fz4apl4"
+                "/": "bafkreihkpy5ns73mfk3tolcorppq7uncohykehk4y6yc5yneuripguycwy"
             },
             "objectname": "permit_2",
             "typename": "Permit2"
         },
         "pool": {
             "address": "0x8f8EF111B67C04Eb1641f5ff19EE54Cda062f163",
             "artifact": {
-                "/": "bafkreicll4d3mtce2szttnqqhrypw7dae74ic2ga5u66gxukz6mznnfkvy"
+                "/": "bafkreiaoslqt7asr3gxfddko2sbf45f5ad53xqh5otdzc36vfgwzhwhyv4"
             },
             "objectname": "pool",
             "typename": "UniswapV3Pool"
         },
         "proxy_admin": {
             "address": "0xB753548F6E010e7e680BA186F9Ca1BdAB2E90cf2",
             "artifact": {
-                "/": "bafkreifdxty7rkvyivxglvjmj5lb5a6gk5u4sbsnt3moflww6bipybbeyi"
+                "/": "bafkreift2anfyw3xo2rpyqfpo4565jdp5tuizjknvcaukgupvf7wy22kry"
             },
             "objectname": "proxy_admin",
             "typename": "ProxyAdmin"
         },
         "quoter": {
             "address": "0x61fFE014bA17989E743c5F6cB21bF9697530B21e",
             "artifact": {
-                "/": "bafkreidg3a3cs7ozqelzc2vv65s3hxojwxfxck3dvp374kyidlsfssjgiq"
+                "/": "bafkreieuydcmbrep3fynrn64vbv3b3qhwqrb773ctb44hbcvmyzyd4uc6e"
             },
             "objectname": "quoter",
             "typename": "QuoterV2"
         },
         "staker": {
             "address": "0xe34139463bA50bD61336E0c446Bd8C0867c6fE65",
             "artifact": {
-                "/": "bafkreiej6mvcyhtkg3apj7jexpy5y64zmse4lnds53o5b5skbdmm2jpevy"
+                "/": "bafkreigkgixpwv5ehyxaye44hlt2smsv6rx6gfvjnmc7qm6jukmtshfgla"
             },
             "objectname": "staker",
             "typename": "UniswapV3Staker"
         },
         "swap_router": {
             "address": "0x68b3465833fb72A70ecDF485E0e4C7bD8665Fc45",
             "artifact": {
-                "/": "bafkreibcmumnft2hsal4lvtckatbnggq44pf5sawmo3ul232qxludtqs7a"
+                "/": "bafkreierdwmfuxsh5kd5olxztorx5ml2hb4of62po3uoy54mgyhh4nb2iu"
             },
             "objectname": "swap_router",
             "typename": "SwapRouter02"
         },
         "tick_lens": {
             "address": "0xbfd8137f7d1516D3ea5cA83523914859ec47F573",
             "artifact": {
-                "/": "bafkreigwm4evjtkju5qtp7bezp4bqerozjgn2eww54oxgfejpwplgsuz4e"
+                "/": "bafkreiao2uqriqw74ynntzti5k2llv6td3tik3mwgp6dvsbrbgjldd5z4y"
             },
             "objectname": "tick_lens",
             "typename": "TickLens"
         },
         "transparent_upgradeable_proxy": {
             "address": "0xEe6A57eC80ea46401049E92587E52f5Ec1c24785",
             "artifact": {
-                "/": "bafkreic2doioye74gf34crxggv4bso36xsamq5vsbsaktqluo5mnr4vv3q"
+                "/": "bafkreieo6gqe5nbvvichcl7rr7yyzp4gc2vji427xyfv2e7cacjr2nojnq"
             },
             "objectname": "transparent_upgradeable_proxy",
             "typename": "NonfungibleTokenPositionDescriptor"
         },
         "uni": {
             "address": "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984",
             "artifact": {
-                "/": "bafkreicvgwk45gdmt56fiwhyvw4tqijq6la73zr27gz2s47d3knbjhuvsm"
+                "/": "bafkreifocfyjpxvkajsriea3333s3kjsqmkxpsdaeqyzuel52wwcyepbru"
             },
             "objectname": "uni",
             "typename": "Uni"
         },
         "universal_router": {
             "address": "0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD",
             "artifact": {
-                "/": "bafkreiae266w7plknc5got2zdn6anb3umvkadigsc4vxsaktv4767it6qa"
+                "/": "bafkreigprw4ahsfs4prrdtfjifjlvewc4oiffdhtljcxtqcnhmnqyijvfa"
             },
             "objectname": "universal_router",
             "typename": "UniversalRouter"
         },
         "v3_migrator": {
             "address": "0xA5644E29708357803b5A882D272c41cC0dF92B34",
             "artifact": {
-                "/": "bafkreib7rzq2sqqqhtgv77aojigzaisfimqsfngz6dahqxamgkwl5jnvae"
+                "/": "bafkreicl6vspjx5232txdogq6dflt27w4pexadbmku4wtaanztjuw7ompi"
             },
             "objectname": "v3_migrator",
             "typename": "V3Migrator"
         }
     },
     "types": {
         "Multicall2": {
             "artifact": {
-                "/": "bafkreifdsw4uxxzq4e7judcpdhlh4nwush33kkxbjna5lkxy2d5mbfqmja"
+                "/": "bafkreif5hugwwzhqaayfjujum2yj6aaj7bv6fyzpv5apdb4ndwwlyfraji"
             },
             "typename": "Multicall2"
         },
         "NFTDescriptor": {
             "artifact": {
-                "/": "bafkreid4545gqtrx4hptvotnb5osdy7ofewzzxifxhumvvrqkr4e773ace"
+                "/": "bafkreicwyd57wsz7b5a6lz3i24mgh2xldsdcyjc45chmzyzkrwtbhzogdu"
             },
             "typename": "NFTDescriptor"
         },
         "NonfungiblePositionManager": {
             "artifact": {
-                "/": "bafkreic2gyd3oj5iyxrv6rdcidc22bqvbc6ypous6xv4klvptsscsgbpx4"
+                "/": "bafkreihu2zyfq4lh7tpughmajmgo5uu27kjspn55jo7zmkqhgzxqt64fdu"
             },
             "typename": "NonfungiblePositionManager"
         },
         "NonfungibleTokenPositionDescriptor": {
             "artifact": {
-                "/": "bafkreic2doioye74gf34crxggv4bso36xsamq5vsbsaktqluo5mnr4vv3q"
+                "/": "bafkreieo6gqe5nbvvichcl7rr7yyzp4gc2vji427xyfv2e7cacjr2nojnq"
             },
             "typename": "NonfungibleTokenPositionDescriptor"
         },
         "Permit2": {
             "artifact": {
-                "/": "bafkreicttw522lrgona4yv2h43fy6b3q4jmm526k2tmm2azreh4fz4apl4"
+                "/": "bafkreihkpy5ns73mfk3tolcorppq7uncohykehk4y6yc5yneuripguycwy"
             },
             "typename": "Permit2"
         },
         "ProxyAdmin": {
             "artifact": {
-                "/": "bafkreifdxty7rkvyivxglvjmj5lb5a6gk5u4sbsnt3moflww6bipybbeyi"
+                "/": "bafkreift2anfyw3xo2rpyqfpo4565jdp5tuizjknvcaukgupvf7wy22kry"
             },
             "typename": "ProxyAdmin"
         },
         "QuoterV2": {
             "artifact": {
-                "/": "bafkreidg3a3cs7ozqelzc2vv65s3hxojwxfxck3dvp374kyidlsfssjgiq"
+                "/": "bafkreieuydcmbrep3fynrn64vbv3b3qhwqrb773ctb44hbcvmyzyd4uc6e"
             },
             "typename": "QuoterV2"
         },
         "SwapRouter02": {
             "artifact": {
-                "/": "bafkreibcmumnft2hsal4lvtckatbnggq44pf5sawmo3ul232qxludtqs7a"
+                "/": "bafkreierdwmfuxsh5kd5olxztorx5ml2hb4of62po3uoy54mgyhh4nb2iu"
             },
             "typename": "SwapRouter02"
         },
         "TickLens": {
             "artifact": {
-                "/": "bafkreigwm4evjtkju5qtp7bezp4bqerozjgn2eww54oxgfejpwplgsuz4e"
+                "/": "bafkreiao2uqriqw74ynntzti5k2llv6td3tik3mwgp6dvsbrbgjldd5z4y"
             },
             "typename": "TickLens"
         },
         "Uni": {
             "artifact": {
-                "/": "bafkreicvgwk45gdmt56fiwhyvw4tqijq6la73zr27gz2s47d3knbjhuvsm"
+                "/": "bafkreifocfyjpxvkajsriea3333s3kjsqmkxpsdaeqyzuel52wwcyepbru"
             },
             "typename": "Uni"
         },
         "UniswapInterfaceMulticall": {
             "artifact": {
-                "/": "bafkreicd25dxfrtvn2oavbipzsp237dvbkbhsjeqr6ouuo23s5xhhj377e"
+                "/": "bafkreibvnxd7qhm5ppxsc45r3gfp2ggp3wgx7nrz223rg5pglacwgufnve"
             },
             "typename": "UniswapInterfaceMulticall"
         },
         "UniswapV3Factory": {
             "artifact": {
-                "/": "bafkreicfd2yml7evjxgssrqgzkb2qkyobvmonp5us2w3xqtr2zuuqzl4ku"
+                "/": "bafkreiecs7ltlmc2sg5rvlovum5t7hcf5bxuwhvpujdcd4vx2obnk25jhm"
             },
             "typename": "UniswapV3Factory"
         },
         "UniswapV3Pool": {
             "artifact": {
-                "/": "bafkreicll4d3mtce2szttnqqhrypw7dae74ic2ga5u66gxukz6mznnfkvy"
+                "/": "bafkreiaoslqt7asr3gxfddko2sbf45f5ad53xqh5otdzc36vfgwzhwhyv4"
             },
             "typename": "UniswapV3Pool"
         },
         "UniswapV3Staker": {
             "artifact": {
-                "/": "bafkreiej6mvcyhtkg3apj7jexpy5y64zmse4lnds53o5b5skbdmm2jpevy"
+                "/": "bafkreigkgixpwv5ehyxaye44hlt2smsv6rx6gfvjnmc7qm6jukmtshfgla"
             },
             "typename": "UniswapV3Staker"
         },
         "UniversalRouter": {
             "artifact": {
-                "/": "bafkreiae266w7plknc5got2zdn6anb3umvkadigsc4vxsaktv4767it6qa"
+                "/": "bafkreigprw4ahsfs4prrdtfjifjlvewc4oiffdhtljcxtqcnhmnqyijvfa"
             },
             "typename": "UniversalRouter"
         },
         "V3Migrator": {
             "artifact": {
-                "/": "bafkreib7rzq2sqqqhtgv77aojigzaisfimqsfngz6dahqxamgkwl5jnvae"
+                "/": "bafkreicl6vspjx5232txdogq6dflt27w4pexadbmku4wtaanztjuw7ompi"
             },
             "typename": "V3Migrator"
         }
     }
 }
```

### Comparing `dpack_py-0.2.0/examples/uniswap.py` & `dpack_py-0.2.1/examples/uniswap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import dpack
-from ape import Contract, networks
+import json
 import tempfile
 from pathlib import Path
+
+import dpack
+from ape import Contract, networks
 from rich import print
 
 # https://docs.uniswap.org/contracts/v3/reference/deployments/ethereum-deployments
 uniswap_v3_deployment = {
     "factory": "0x1F98431c8aD98523631AE4a59f267346ea31F984",
     "multicall": "0x1F98415757620B543A52E61c46B32eB19261F984",
     "multicall2": "0x5BA1e12693Dc8F9c48aAD8770482f4739bEeD696",
@@ -23,23 +25,28 @@
     "staker": "0xe34139463bA50bD61336E0c446Bd8C0867c6fE65",
     "uni": "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984",
     "pool": "0x8f8EF111B67C04Eb1641f5ff19EE54Cda062f163",
 }
 
 
 def main():
-    pack = dpack.Dpack(network="mainnet")
+    # NOTE https://github.com/ricobank/dpack/blob/830ce46cc2cf6cc65888b6c9625e86d8cc9859d4/src/builder.ts#L19
+    pack = dpack.Dpack(network="ethereum")
     with tempfile.TemporaryDirectory() as artifacts:
         artifacts = Path(artifacts)
         for objectname, address in uniswap_v3_deployment.items():
             print(objectname, address)
             contract = Contract(address)
             type = contract.contract_type
             path = artifacts / f"{type.name}.json"
-            path.write_text(type.model_dump_json(include={"name", "abi"}))
+            artifact = type.model_dump(include={"name", "abi"})
+            # NOTE this is initcode. the spec says it's optional but a null doesn't work with it,
+            # so we cheat a little. this bytecode is meant for deploying new contracts from type.
+            artifact["bytecode"] = "0x"
+            path.write_text(json.dumps(artifact))
             pack.pack_object(path, typename=type.name, objectname=objectname, address=address)
 
     print(pack)
     save_path = Path("examples/uniswap-v3.dpack.json")
     pack.save(save_path)
     print(f"saved to {save_path}")
```

### Comparing `dpack_py-0.2.0/pyproject.toml` & `dpack_py-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "dpack-py"
 authors = [{ name = "banteg" }]
 classifiers = ["License :: OSI Approved :: MIT License"]
-version = "0.2.0"
+version = "0.2.1"
 readme = "readme.md"
 description = "dpack is an evm artifact package format"
 requires-python = ">=3.9"
 dependencies = ["pydantic >=2", "httpx", "ethpm-types"]
 
 [tool.flit.module]
 name = "dpack"
```

### Comparing `dpack_py-0.2.0/readme.md` & `dpack_py-0.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.0/src/dpack/ape.py` & `dpack_py-0.2.1/src/dpack/ape.py`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.0/src/dpack/dpack.py` & `dpack_py-0.2.1/src/dpack/dpack.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 class DpackArtifact(BaseModel):
     artifact: dict[Literal["/"], IpfsCid]
 
     @property
     def contract_type(self):
         payload = fetch_artifact(self.artifact["/"])
         payload.setdefault("contractName", self.typename)
+        if initcode := payload.pop("bytecode", None):
+            payload["deploymentBytecode"] = {"bytecode": initcode}
         return ContractType.model_validate(payload)
 
     @classmethod
     def from_path(cls, path: Path, **fields):
         cid = upload_artifact(path)
         return cls.model_validate(dict(artifact={"/": cid}, **fields))
```

### Comparing `dpack_py-0.2.0/tests/test_dpack.py` & `dpack_py-0.2.1/tests/test_dpack.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         "deposit()",
         "allowance(address,address)",
         "Approval(address,address,uint256)",
         "Transfer(address,address,uint256)",
         "Deposit(address,uint256)",
         "Withdrawal(address,uint256)",
     }
+    assert contract_type.deployment_bytecode
 
 
 def test_instance(pack):
     instance = pack.objects["weth"].contract_instance
     print(instance)
     assert instance.contract_type == "WETH9"
```

### Comparing `dpack_py-0.2.0/tests/weth-ropsten-artifact.json` & `dpack_py-0.2.1/tests/weth-ropsten-artifact.json`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.0/tests/weth_ropsten.dpack.json` & `dpack_py-0.2.1/tests/weth_ropsten.dpack.json`

 * *Files identical despite different names*

### Comparing `dpack_py-0.2.0/PKG-INFO` & `dpack_py-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpack-py
-Version: 0.2.0
+Version: 0.2.1
 Summary: dpack is an evm artifact package format
 Author: banteg
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic >=2
 Requires-Dist: httpx
```

