# Comparing `tmp/telegram_wallet_pay-0.3.2.tar.gz` & `tmp/telegram_wallet_pay-0.4.0.tar.gz`

## Comparing `telegram_wallet_pay-0.3.2.tar` & `telegram_wallet_pay-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,41 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/.editorconfig
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/Makefile
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/codecov.yaml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/examples/00_create_order.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/examples/01_get_order_preview.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/errors.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/tools.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/create_order_request.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/create_order_response.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/get_order_preview_response.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_amount_response.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/webhook_message.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/tests/test_client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/tests/test_schemas.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/tests/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/.gitignore
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/README.md
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/.editorconfig
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/Makefile
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/codecov.yaml
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/examples/00_create_order.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/examples/01_get_order_preview.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/examples/02_bot_example.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/examples/03_webhook_handler_example.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/tools/__init__.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/tools/fastapi.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/tools/signature.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/telegram_wallet_pay/tools/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/tests/samples.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/tests/test_client.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/tests/test_schemas.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/tests/test_tools/test_fastapi.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/tests/test_tools/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/.gitignore
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/README.md
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.4.0/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.3.2/examples/00_create_order.py` & `telegram_wallet_pay-0.4.0/examples/00_create_order.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.4.0/telegram_wallet_pay/client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/telegram_wallet_pay/tools.py` & `telegram_wallet_pay-0.4.0/telegram_wallet_pay/tools/signature.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,35 +2,26 @@
 import hmac
 from base64 import b64encode
 from typing import Union
 
 ENCODING = "utf-8"
 
 
-def from_snake_to_pascal(snake_str: str) -> str:
-    """Convert snake_case to PascalCase."""
-    return "".join(x.capitalize() for x in snake_str.lower().split("_"))
-
-
-def from_snake_to_camel(snake_str: str) -> str:
-    """Convert snake_case to camelCase."""
-    if "_" not in snake_str:
-        return snake_str
-    camel_string = from_snake_to_pascal(snake_str)
-    return snake_str[0].lower() + camel_string[1:]
-
-
 def compute_signature(
     store_api_key: str,
     http_method: str,
     uri_path: str,
     timestamp: str,
     body: Union[str, bytes],
 ) -> str:
     """Compute signature."""
+    if not store_api_key:
+        msg = f"Argument 'store_api_key' should not be empty. Passed {store_api_key=}"
+        raise ValueError(msg)
+
     if isinstance(body, str):
         body = bytes(body, ENCODING)
 
     body_base64 = b64encode(body).decode(ENCODING)
     payload = f"{http_method}.{uri_path}.{timestamp}.{body_base64}"
 
     signature_bytes = hmac.new(
```

### Comparing `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/__init__.py` & `telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/create_order_request.py` & `telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/order_reconciliation_item.py` & `telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/order_reconciliation_item.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/webhook_message.py` & `telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.4.0/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/tests/test_client.py` & `telegram_wallet_pay-0.4.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/tests/test_schemas.py` & `telegram_wallet_pay-0.4.0/tests/test_schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     amount_net=money_amount,
     exchange_rate="",
 )
 webhook_payload = WebhookPayload(
     id=1,
     number="",
     external_id="",
-    status="PAID",
     order_amount=money_amount,
     selected_payment_option=payment_option,
     order_completed_datetime=datetime.now(),
 )
 webhook_message = WebhookMessage(
     event_datetime=datetime.now(),
     event_id=1,
```

### Comparing `telegram_wallet_pay-0.3.2/tests/test_signature.py` & `telegram_wallet_pay-0.4.0/tests/test_tools/test_signature.py`

 * *Files 15% similar despite different names*

```diff
@@ -40,7 +40,22 @@
         http_method="POST",
         uri_path="/webhook/",
         timestamp="168824905680291",
         body=body,
     )
 
     assert signature == "MGfJzeEprADZbihhRcGcCY5pYTI/IEJ91ejyA+XOWAs="
+
+
+def test_empty_key(body: Union[str, bytes]) -> None:
+    """Test signature provided by docs."""
+    with pytest.raises(
+        expected_exception=ValueError,
+        match="Argument 'store_api_key' should not be empty.*",
+    ):
+        compute_signature(
+            store_api_key="",
+            http_method="POST",
+            uri_path="/webhook/",
+            timestamp="168824905680291",
+            body=body,
+        )
```

### Comparing `telegram_wallet_pay-0.3.2/.gitignore` & `telegram_wallet_pay-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.2/README.md` & `telegram_wallet_pay-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Telegram Wallet Pay
 
 Python async client for [Telegram Wallet Pay API](https://pay.wallet.tg) made of `aiohttp` and `pydantic`
 
+**Also contains:**
+ - `pydantic` models for every schema, even for incoming webhooks
+ - signature validation tool, including ready-made `Depends` for `FastAPI`
+
 [![Python](https://img.shields.io/pypi/pyversions/telegram-wallet-pay.svg)](https://pypi.org/project/telegram-wallet-pay/)
 [![pypi](https://img.shields.io/pypi/v/telegram-wallet-pay?label=pypi%20package)](https://pypi.org/project/telegram-wallet-pay/)
 [![Tests](https://github.com/Olegt0rr/TelegramWalletPay/actions/workflows/tests.yml/badge.svg)](https://github.com/Olegt0rr/YaTracker/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/Olegt0rr/TelegramWalletPay)](https://app.codecov.io/gh/Olegt0rr/TelegramWalletPay)
 [![Code linter: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 ---
@@ -86,7 +90,17 @@
     await wallet.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
+
+
+## Other examples
+
+* [Telegram bot example (aiogram)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/02_bot_example.py)
+* [Webhook handler example (FastAPI)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/03_webhook_handler_example.py)
+
+Also, feel free to open the
+[folder with examples](https://github.com/Olegt0rr/TelegramWalletPay/tree/main/examples),
+and if there is something missing there, describe your needs in [issue](https://github.com/Olegt0rr/TelegramWalletPay/issues/new/choose).
```

### Comparing `telegram_wallet_pay-0.3.2/pyproject.toml` & `telegram_wallet_pay-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -48,29 +48,35 @@
     "aiohttp>=3.8,<4",
     "pydantic>=2.4,<3",
     "certifi>=2023",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "ruff>=0",
-    "mypy>=1",
-    "pre-commit>=3",
+    "ruff>=0,<1",
+    "mypy>=1,<2",
+    "pre-commit>=3,<4",
+    "fastapi>=0.110,<1",
+    "uvicorn>=0.29,<1",
+    "httpx>=0.27,<1",
 ]
 test = [
-    "coverage>=7",
-    "pytest>=8",
-    "pytest-asyncio>=0",
-    "pytest-cov>=5",
-    "aresponses>=3",
+    "coverage>=7,<8",
+    "pytest>=8,<9",
+    "pytest-asyncio>=0,<1",
+    "pytest-cov>=5,<6",
+    "aresponses>=3,<4",
+    "fastapi>=0.110,<1",
+    "httpx>=0.27,<1",
 ]
 
 
 [project.urls]
 Repository = "https://github.com/Olegt0rr/TelegramWalletPay"
+Documentation = "https://docs.wallet.tg/pay/"
 
 [tool.hatch.version]
 path = "telegram_wallet_pay/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
     "/.github",
@@ -184,9 +190,9 @@
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.ruff.lint.flake8-type-checking]
 runtime-evaluated-base-classes = ["pydantic.BaseModel", "telegram_wallet_pay.schemas._default.DefaultModel"]
 
 [tool.ruff.lint.per-file-ignores]
-"tests/*" = ["S101", "INP001"]
+"tests/*" = ["S101", "INP001", "D"]
 "examples/*" = ["INP001", "T201"]
```

### Comparing `telegram_wallet_pay-0.3.2/PKG-INFO` & `telegram_wallet_pay-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.3.2
+Version: 0.4.0
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
+Project-URL: Documentation, https://docs.wallet.tg/pay/
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Pydantic
@@ -27,29 +28,38 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: aiohttp<4,>=3.8
 Requires-Dist: certifi>=2023
 Requires-Dist: pydantic<3,>=2.4
 Provides-Extra: dev
-Requires-Dist: mypy>=1; extra == 'dev'
-Requires-Dist: pre-commit>=3; extra == 'dev'
-Requires-Dist: ruff>=0; extra == 'dev'
+Requires-Dist: fastapi<1,>=0.110; extra == 'dev'
+Requires-Dist: httpx<1,>=0.27; extra == 'dev'
+Requires-Dist: mypy<2,>=1; extra == 'dev'
+Requires-Dist: pre-commit<4,>=3; extra == 'dev'
+Requires-Dist: ruff<1,>=0; extra == 'dev'
+Requires-Dist: uvicorn<1,>=0.29; extra == 'dev'
 Provides-Extra: test
-Requires-Dist: aresponses>=3; extra == 'test'
-Requires-Dist: coverage>=7; extra == 'test'
-Requires-Dist: pytest-asyncio>=0; extra == 'test'
-Requires-Dist: pytest-cov>=5; extra == 'test'
-Requires-Dist: pytest>=8; extra == 'test'
+Requires-Dist: aresponses<4,>=3; extra == 'test'
+Requires-Dist: coverage<8,>=7; extra == 'test'
+Requires-Dist: fastapi<1,>=0.110; extra == 'test'
+Requires-Dist: httpx<1,>=0.27; extra == 'test'
+Requires-Dist: pytest-asyncio<1,>=0; extra == 'test'
+Requires-Dist: pytest-cov<6,>=5; extra == 'test'
+Requires-Dist: pytest<9,>=8; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Telegram Wallet Pay
 
 Python async client for [Telegram Wallet Pay API](https://pay.wallet.tg) made of `aiohttp` and `pydantic`
 
+**Also contains:**
+ - `pydantic` models for every schema, even for incoming webhooks
+ - signature validation tool, including ready-made `Depends` for `FastAPI`
+
 [![Python](https://img.shields.io/pypi/pyversions/telegram-wallet-pay.svg)](https://pypi.org/project/telegram-wallet-pay/)
 [![pypi](https://img.shields.io/pypi/v/telegram-wallet-pay?label=pypi%20package)](https://pypi.org/project/telegram-wallet-pay/)
 [![Tests](https://github.com/Olegt0rr/TelegramWalletPay/actions/workflows/tests.yml/badge.svg)](https://github.com/Olegt0rr/YaTracker/actions/workflows/tests.yml)
 [![Coverage](https://img.shields.io/codecov/c/github/Olegt0rr/TelegramWalletPay)](https://app.codecov.io/gh/Olegt0rr/TelegramWalletPay)
 [![Code linter: ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](https://mypy-lang.org/)
 ---
@@ -130,7 +140,17 @@
     await wallet.close()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
+
+
+## Other examples
+
+* [Telegram bot example (aiogram)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/02_bot_example.py)
+* [Webhook handler example (FastAPI)](https://github.com/Olegt0rr/TelegramWalletPay/blob/main/examples/03_webhook_handler_example.py)
+
+Also, feel free to open the
+[folder with examples](https://github.com/Olegt0rr/TelegramWalletPay/tree/main/examples),
+and if there is something missing there, describe your needs in [issue](https://github.com/Olegt0rr/TelegramWalletPay/issues/new/choose).
```

