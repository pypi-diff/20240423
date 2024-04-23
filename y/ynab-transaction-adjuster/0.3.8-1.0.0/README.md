# Comparing `tmp/ynab_transaction_adjuster-0.3.8.tar.gz` & `tmp/ynab_transaction_adjuster-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_transaction_adjuster-0.3.8.tar", max compression
+gzip compressed data, was "ynab_transaction_adjuster-1.0.0.tar", max compression
```

## Comparing `ynab_transaction_adjuster-0.3.8.tar` & `ynab_transaction_adjuster-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0    35148 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/LICENSE
--rw-r--r--   0        0        0     3462 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/README.md
--rw-r--r--   0        0        0      680 2024-04-08 08:57:18.496879 ynab_transaction_adjuster-0.3.8/pyproject.toml
--rw-r--r--   0        0        0       84 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/__init__.py
--rw-r--r--   0        0        0     1942 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/adjuster.py
--rw-r--r--   0        0        0     2481 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/client.py
--rw-r--r--   0        0        0      903 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/exceptions.py
--rw-r--r--   0        0        0      358 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/__init__.py
--rw-r--r--   0        0        0      246 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/category.py
--rw-r--r--   0        0        0      621 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/categorygroup.py
--rw-r--r--   0        0        0     3209 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/modifiedtransaction.py
--rw-r--r--   0        0        0      602 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/originalsubtransaction.py
--rw-r--r--   0        0        0     2865 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/originaltransaction.py
--rw-r--r--   0        0        0      586 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/payee.py
--rw-r--r--   0        0        0     1244 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/subtransaction.py
--rw-r--r--   0        0        0     1860 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/transactionmodifier.py
--rw-r--r--   0        0        0       72 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/__init__.py
--rw-r--r--   0        0        0     1918 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/categoryrepo.py
--rw-r--r--   0        0        0     1723 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/payeerepo.py
--rw-r--r--   0        0        0     4357 2024-04-08 08:56:59.384784 ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/ynabtransactionadjuster.py
--rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3588 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/README.md
+-rw-r--r--   0        0        0      673 2024-04-23 05:43:58.176581 ynab_transaction_adjuster-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      291 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/__init__.py
+-rw-r--r--   0        0        0     5018 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/adjuster.py
+-rw-r--r--   0        0        0     2686 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/client.py
+-rw-r--r--   0        0        0     1003 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/exceptions.py
+-rw-r--r--   0        0        0      357 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/__init__.py
+-rw-r--r--   0        0        0      246 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/category.py
+-rw-r--r--   0        0        0      621 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/categorygroup.py
+-rw-r--r--   0        0        0      263 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/credentials.py
+-rw-r--r--   0        0        0     2920 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifiedtransaction.py
+-rw-r--r--   0        0        0     1718 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifier.py
+-rw-r--r--   0        0        0     1252 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifiersubtransaction.py
+-rw-r--r--   0        0        0      586 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/payee.py
+-rw-r--r--   0        0        0      594 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/subtransaction.py
+-rw-r--r--   0        0        0     2905 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/transaction.py
+-rw-r--r--   0        0        0       72 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/__init__.py
+-rw-r--r--   0        0        0     1980 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/categoryrepo.py
+-rw-r--r--   0        0        0     1771 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/payeerepo.py
+-rw-r--r--   0        0        0     2848 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/serializer.py
+-rw-r--r--   0        0        0     1283 2024-04-23 05:43:39.000562 ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/signaturechecker.py
+-rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 ynab_transaction_adjuster-1.0.0/PKG-INFO
```

### Comparing `ynab_transaction_adjuster-0.3.8/LICENSE` & `ynab_transaction_adjuster-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.8/README.md` & `ynab_transaction_adjuster-1.0.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # ynab-transaction-adjuster
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-transaction-adjuster?style=flat)]() 
-[![Github Release](https://img.shields.io/maintenance/yes/2100)]()
+[![Maintained](https://img.shields.io/maintenance/yes/2100)]()
+[![Monthly downloads](https://img.shields.io/pypi/dm/ynab-transaction-adjuster)]()
 
 [!["Buy Me A Coffee"](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/dnbasta)
 
 This library helps you to automatically adjust transactions in YNAB based on your logic. It allows you to implement 
 your adjustments in a simple factory class which you can run against your existing transactions and update relevant 
 fields like date, payee, category, memo and flags. It also allows you to split transactions.
 
@@ -23,54 +24,57 @@
 
 ## Usage
 A detailed documentation is available at https://ynab-transaction-adjuster.readthedocs.io
 
 # Basic Usage
 
 ### Create an Adjuster
-Create a child class of `YnabTransactionAdjuster`.
-This class needs to implement a `filter()` and an `adjust()` method which contain the intended logic. The `filter()`
-method receives a list of `OriginalTransaction` objects which can be filtered before 
-adjustement. The `adjust()` method receives a singular `OriginalTransaction` and a 
-`TransactionModifier`. The latter is prefilled with values from the original transaction. 
-Its attributes can be modified, and it needs to be returned at the end of the function. 
-Please check the [detailed usage](https://ynab-transaction-adjuster.readthedocs.io/en/latest/detailed_usage/) section for explanations how to change different attributes.
+Create a child class of `Adjuster`. This class needs to implement a `filter()` and an `adjust()` method which contain 
+the intended logic. The `filter()` method receives a list of `Transaction` objects which can be filtered before 
+adjustement. The `adjust()` method receives a single `Transaction` and a `Modifier`.The latter is prefilled with values 
+from the original transaction and can be altered. The modifier needs to be returned at the end of the function. 
+Please check the [detailed usage](https://ynab-transaction-adjuster.readthedocs.io/en/latest/detailed_usage/) section 
+for explanations how to change different attributes.
+
 ```py
-from ynabtransactionadjuster import YnabTransactionAdjuster
-from ynabtransactionadjuster.models import OriginalTransaction, TransactionModifier
+from ynabtransactionadjuster import Adjuster, Transaction, Modifier
+
+
+class MyAdjuster(Adjuster):
 
+	def filter(self, transactions: List[Transaction]) -> List[Transaction]:
+		# your implementation
 
-class MyAdjuster(YnabTransactionAdjuster):
-    
-    def filter(self, transactions: List[OriginalTransaction]) -> List[OriginalTransaction]:
-        # your implementation
-        
-        # return the filtered list of transactions
-        return transactions
-        
-    def adjust(self, original: OriginalTransaction, modifier: TransactionModifier) -> TransactionModifier:
-        # your implementation
+		# return the filtered list of transactions
+		return transactions
+
+	def adjust(self, transaction: Transaction, modifier: Modifier) -> Modifier:
+		# your implementation
 
 		# return the altered modifier
 		return modifier
 ```
 
 ### Initialize
-Initalize the adjuster with `token`, `budget` and `account` from YNAB
+Create a [`Credentials`][models.Credentials] object and initialize Adjuster class with it
 ```py
-my_adjuster = MyAdjuster(token='<token>', budget='<budget>', account='<account>')
+from ynabtransactionadjuster import Credentials
+
+my_credentials = Credentials(token='<token>', budget='<budget>', account='<account>')
+my_adjuster = MyAdjuster.from_credentials(credentials=my_credentials)
 ```
 
 ### Test
-Test the adjuster on records fetched via the `test()`method. The method fetches and executes the 
-adjustments but doesn't write the results back to YNAB. Instead it returns a list of 
-the changed transactions which can be inspected for the changed properties.
+Test the adjuster on records fetched via the `dry_run()` method. It executes the adjustments but doesn't write the 
+results back to YNAB. Instead it returns a list of the changed transactions which can be inspected for the changed 
+properties. It takes an optional parameter `pretty_print` which, if set to `True`, prints modifications in an easy 
+readable string representation to the console.
 
 ```py
-mod_transactions = my_adjuster.test()
+mod_transactions = my_adjuster.dry_run()
 ```
 
 ### Run
 If you are satisfied with the functionality you can execute the adjuster with the `run()` method. This will run the 
 adjustments and will update the changed transactions in YNAB. The method returns an integer with the number of 
 successfully updated records.
 ```py
```

### Comparing `ynab_transaction_adjuster-0.3.8/pyproject.toml` & `ynab_transaction_adjuster-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "ynab-transaction-adjuster"
-version = "0.3.8"
+version = "1.0.0"
 description = "Library to adjust transactions in YNAB based on custom patterns"
 authors = ["Daniel Basta <ynab@basta.info>"]
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabtransactionadjuster'}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = '>=3.8,<4.0'
-requests = '>=2.28.0'
-pydantic = "^2.6.4"
+python = '^3.8'
+requests = '^2.28.0'
+pydantic = '^2.7.0'
 pytest = "^8.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/client.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import List
 
 import requests
 from requests import HTTPError
 
 from ynabtransactionadjuster.models import CategoryGroup, ModifiedTransaction
-from ynabtransactionadjuster.models import OriginalTransaction
+from ynabtransactionadjuster.models import Transaction
 from ynabtransactionadjuster.models import Payee
-
+from ynabtransactionadjuster.models.credentials import Credentials
 
 YNAB_BASE_URL = 'https://api.ynab.com/v1'
 
 
 class Client:
 	"""Client for reading from and writing to YNAB
 
@@ -20,14 +20,18 @@
 	"""
 
 	def __init__(self, token: str, budget: str, account: str):
 		self._header = {'Authorization': f'Bearer {token}'}
 		self._budget = budget
 		self._account = account
 
+	@classmethod
+	def from_credentials(cls, credentials: Credentials):
+		return cls(token=credentials.token, budget=credentials.budget, account=credentials.account)
+
 	def fetch_categories(self) -> List[CategoryGroup]:
 		"""Fetches categories from YNAB"""
 		r = requests.get(f'{YNAB_BASE_URL}/budgets/{self._budget}/categories', headers=self._header)
 		r.raise_for_status()
 
 		data = r.json()['data']['category_groups']
 		categories = [CategoryGroup.from_dict(cg) for cg in data if cg['deleted'] is False]
@@ -38,22 +42,22 @@
 		r = requests.get(f'{YNAB_BASE_URL}/budgets/{self._budget}/payees', headers=self._header)
 		r.raise_for_status()
 
 		data = r.json()['data']['payees']
 		payees = [Payee.from_dict(p) for p in data if p['deleted'] is False]
 		return payees
 
-	def fetch_transactions(self) -> List[OriginalTransaction]:
+	def fetch_transactions(self) -> List[Transaction]:
 		"""Fetches transactions from YNAB"""
 		r = requests.get(f'{YNAB_BASE_URL}/budgets/{self._budget}/accounts/{self._account}/transactions', headers=self._header)
 		r.raise_for_status()
 
 		data = r.json()['data']['transactions']
 		transaction_dicts = [t for t in data if t['deleted'] is False]
-		transactions = [OriginalTransaction.from_dict(t) for t in transaction_dicts]
+		transactions = [Transaction.from_dict(t) for t in transaction_dicts]
 		return transactions
 
 	def update_transactions(self, transactions: List[ModifiedTransaction]) -> int:
 		"""Updates transactions in YNAB. The updates are done in bulk.
 
 		:param transactions: list of modified transactions to be updated
 		:raises HTTPError: if bulk update call is not successful. Error can be related to any item in the passed list
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/exceptions.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,7 +21,11 @@
 	pass
 
 
 class AdjustError(Exception):
 	"""Raised when an error occurs while running the factory on a transaction or during validation of the returned
 	results of the run"""
 	pass
+
+
+class SignatureError(Exception):
+	""" Raised when function is not defined with right signature"""
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/categorygroup.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/categorygroup.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/modifiedtransaction.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/serializer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,75 +1,74 @@
-from datetime import datetime
+import inspect
+from typing import List, Optional, Callable
 
-from pydantic import BaseModel, model_validator
-
-from ynabtransactionadjuster.models.originaltransaction import OriginalTransaction
-from ynabtransactionadjuster.models.transactionmodifier import TransactionModifier
-
-
-class ModifiedTransaction(BaseModel):
-	original_transaction: OriginalTransaction
-	transaction_modifier: TransactionModifier
-
-	def is_changed(self) -> bool:
-		"""Helper function to determine if transaction has been altered as compared to original one
-
-		:returns: True if values from original transaction have been altered, False otherwise
-		"""
-		if self.changed_attributes():
-			return True
-		return False
-
-	def as_dict(self) -> dict:
-		"""Returns a dictionary representation of the transaction which is used for the update call to YNAB"""
-		t_dict = dict(id=self.original_transaction.id,
-					payee_name=self.transaction_modifier.payee.name,
-					payee_id=self.transaction_modifier.payee.id,
-					date=datetime.strftime(self.transaction_modifier.transaction_date, '%Y-%m-%d'),
-					approved=self.transaction_modifier.approved,
-					cleared=self.transaction_modifier.cleared)
-		if len(self.transaction_modifier.subtransactions) > 0:
-			t_dict['subtransactions'] = [s.as_dict() for s in self.transaction_modifier.subtransactions]
-		if self.transaction_modifier.category:
-			t_dict['category_id'] = self.transaction_modifier.category.id
-		if self.transaction_modifier.flag_color:
-			t_dict['flag_color'] = self.transaction_modifier.flag_color
-		if self.transaction_modifier.memo:
-			t_dict['memo'] = self.transaction_modifier.memo
-
-		return t_dict
-
-	def changed_attributes(self) -> dict:
-		"""Returns a dictionary representation of the modified values and the original transaction"""
-		changed_attributes = dict()
-
-		for a in ('payee', 'category', 'flag_color', 'memo', 'approved', 'cleared'):
-			if self._attribute_changed(a):
-				changed_attributes[a] = self._create_changed_dict(a)
-
-		if (self.transaction_modifier.transaction_date.isocalendar() !=
-				self.original_transaction.transaction_date.isocalendar()):
-			changed_attributes['transaction_date'] = self._create_changed_dict('transaction_date')
-
-		if len(self.transaction_modifier.subtransactions) > 0:
-			changed_attributes['subtransactions'] = self._create_changed_dict('subtransactions')
-
-		return changed_attributes
-
-	def _attribute_changed(self, attribute: str) -> bool:
-		o = self.original_transaction.__getattribute__(attribute)
-		m = self.transaction_modifier.__getattribute__(attribute)
-		if o != m:
-			return True
-
-	def _create_changed_dict(self, attribute: str) -> dict:
-		return dict(original=self.original_transaction.__getattribute__(attribute),
-											  changed=self.transaction_modifier.__getattribute__(attribute))
-
-	@model_validator(mode='after')
-	def check_values(self):
-		if len(self.transaction_modifier.subtransactions) > 1:
-			if len(self.original_transaction.subtransactions) > 1:
-				raise ValueError(f"Existing Subtransactions can not be updated")
-			if sum(a.amount for a in self.transaction_modifier.subtransactions) != self.original_transaction.amount:
-				raise ValueError('Amount of subtransactions needs to be equal to amount of original transaction')
-		return self
+from ynabtransactionadjuster.repos import CategoryRepo
+from ynabtransactionadjuster.exceptions import AdjustError
+from ynabtransactionadjuster.models import Transaction, ModifiedTransaction, Modifier, Category
+
+
+class Serializer:
+
+	def __init__(self, transactions: List[Transaction], categories: CategoryRepo, adjust_func: Callable):
+		self._transactions = transactions
+		self._adjust_func = adjust_func
+		self._categories = categories
+
+	def run(self) -> List[ModifiedTransaction]:
+		modified_transactions = [self.adjust_single(transaction=t)
+								 for t in self._transactions]
+		filtered_transactions = [t for t in modified_transactions if t.is_changed()]
+		return filtered_transactions
+
+	def adjust_single(self, transaction: Transaction) -> ModifiedTransaction:
+		modifier = Modifier.from_transaction(transaction=transaction)
+		transaction_field, modifier_field = self.find_field_names()
+		modifier_return = self._adjust_func(**{transaction_field: transaction, modifier_field: modifier})
+		try:
+			self.validate_instance(modifier_return)
+			self.validate_attributes(modifier_return)
+			self.validate_category(modifier_return.category)
+			modified_transaction = ModifiedTransaction(transaction=transaction,
+													   modifier=modifier_return)
+			return modified_transaction
+		except Exception as e:
+			raise AdjustError(f"Error while adjusting {transaction.as_dict()}") from e
+
+	def validate_category(self, category: Category):
+		if category:
+			self._categories.fetch_by_id(category.id)
+
+	@staticmethod
+	def validate_attributes(modifier: Modifier):
+		Modifier.model_validate(modifier.__dict__)
+
+	@staticmethod
+	def validate_instance(modifier: Optional[Modifier]):
+		if not isinstance(modifier, Modifier):
+			raise AdjustError(f"Adjust function doesn't return TransactionModifier object")
+
+	def find_field_names(self) -> (str, str):
+		args_dict = inspect.signature(self._adjust_func).parameters
+
+		# Find transaction field by annotation
+		try:
+			transaction_field = next(k for k, v in args_dict.items() if v.annotation == Transaction)
+		except StopIteration:
+			transaction_field = None
+
+		# Find modifier field by annotation
+		try:
+			modifier_field = next(k for k, v in args_dict.items() if v.annotation == Modifier)
+		except StopIteration:
+			modifier_field = None
+
+		if transaction_field and modifier_field:
+			pass
+		elif transaction_field and not modifier_field:
+			modifier_field = next(k for k, _ in iter(args_dict.items()) if k != transaction_field)
+		elif modifier_field and not transaction_field:
+			transaction_field = next(k for k, _ in iter(args_dict.items()) if k != modifier_field)
+		else:
+			field_iterator = iter(args_dict.keys())
+			transaction_field = next(field_iterator)
+			modifier_field = next(field_iterator)
+		return transaction_field, modifier_field
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/originalsubtransaction.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/subtransaction.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 from ynabtransactionadjuster.models.category import Category
 from ynabtransactionadjuster.models.payee import Payee
 
 
 @dataclass(frozen=True)
-class OriginalSubTransaction:
+class SubTransaction:
 	"""Represents an YNAB Subtransaction as part of an existing split transaction
 
 	:ivar payee: The payee of the subtransaction
 	:ivar category: The category of the subtransaction
 	:ivar amount: The amount of the subtransaction in milliunits
 	:ivar memo: The memo of the subtransaction
 	"""
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/originaltransaction.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/transaction.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass, asdict
 from datetime import date, datetime
 from typing import Literal, Optional, Tuple
 
 from ynabtransactionadjuster.models.category import Category
 from ynabtransactionadjuster.models.payee import Payee
-from ynabtransactionadjuster.models.originalsubtransaction import OriginalSubTransaction
+from ynabtransactionadjuster.models.subtransaction import SubTransaction
 
 
 @dataclass(frozen=True, eq=True)
-class OriginalTransaction:
+class Transaction:
 	"""Represents original transaction from YNAB
 
 	:ivar id: The original transaction id
 	:ivar amount: The transaction amount in milliunits format
 	:ivar category: The category of the original transaction
 	:ivar transaction_date: The date of the original transaction
 	:ivar memo: The memo of the original transaction
@@ -28,43 +28,46 @@
 	category: Optional[Category]
 	amount: int
 	memo: Optional[str]
 	payee: Payee
 	flag_color: Optional[Literal['red', 'green', 'blue', 'orange', 'purple', 'yellow']]
 	import_payee_name_original: Optional[str]
 	import_payee_name: Optional[str]
-	subtransactions: Tuple[OriginalSubTransaction, ...]
+	subtransactions: Tuple[SubTransaction, ...]
 	cleared: Literal['uncleared', 'cleared', 'reconciled']
 	approved: bool
 
 	@classmethod
-	def from_dict(cls, t_dict: dict) -> 'OriginalTransaction':
+	def from_dict(cls, t_dict: dict) -> 'Transaction':
 
 		def build_category(t_dict: dict) -> Optional[Category]:
 			if not t_dict['category_name'] in ('Uncategorized', 'Split'):
 				return Category(id=t_dict['category_id'], name=t_dict['category_name'])
 
 		def build_payee(t_dict: dict) -> Payee:
 			return Payee(id=t_dict['payee_id'], name=t_dict['payee_name'],
 						 transfer_account_id=t_dict['transfer_account_id'])
 
-		def build_subtransaction(s_dict: dict) -> OriginalSubTransaction:
-			return OriginalSubTransaction(payee=build_payee(s_dict),
-										  category=build_category(s_dict),
-										  amount=s_dict['amount'],
-										  memo=s_dict['memo'])
-
-		return OriginalTransaction(id=t_dict['id'],
-								   transaction_date=datetime.strptime(t_dict['date'], '%Y-%m-%d').date(),
-								   category=build_category(t_dict),
-								   memo=t_dict['memo'],
-								   import_payee_name_original=t_dict['import_payee_name_original'],
-								   import_payee_name=t_dict['import_payee_name'],
-								   flag_color=t_dict['flag_color'],
-								   payee=build_payee(t_dict),
-								   subtransactions=tuple([build_subtransaction(st) for st in t_dict['subtransactions']]),
-								   amount=t_dict['amount'],
-								   approved=t_dict['approved'],
-								   cleared=t_dict['cleared'])
+		def build_subtransaction(s_dict: dict) -> SubTransaction:
+			return SubTransaction(payee=build_payee(s_dict),
+								  category=build_category(s_dict),
+								  amount=s_dict['amount'],
+								  memo=s_dict['memo'])
+
+		return Transaction(id=t_dict['id'],
+						   transaction_date=datetime.strptime(t_dict['date'], '%Y-%m-%d').date(),
+						   category=build_category(t_dict),
+						   memo=t_dict['memo'],
+						   import_payee_name_original=t_dict['import_payee_name_original'],
+						   import_payee_name=t_dict['import_payee_name'],
+						   flag_color=t_dict['flag_color'],
+						   payee=build_payee(t_dict),
+						   subtransactions=tuple([build_subtransaction(st) for st in t_dict['subtransactions']]),
+						   amount=t_dict['amount'],
+						   approved=t_dict['approved'],
+						   cleared=t_dict['cleared'])
 
 	def as_dict(self) -> dict:
 		return asdict(self)
+
+	def __str__(self) -> str:
+		return f"{self.transaction_date} | {self.payee.name} | {float(self.amount) / 1000:.2f} | {self.memo}"
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/payee.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/payee.py`

 * *Files identical despite different names*

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/models/subtransaction.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/models/modifiersubtransaction.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pydantic import BaseModel, model_validator
 
 from ynabtransactionadjuster.models.category import Category
 from ynabtransactionadjuster.models.payee import Payee
 
 
-class SubTransaction(BaseModel):
+class ModifierSubTransaction(BaseModel):
 	"""YNAB Subtransaction object for creating split transactions. To be used as element in subtransaction attribute of
 	Transaction class
 
 	:ivar amount: The amount of the subtransaction in milliunits
 	:ivar category: The category of the subtransaction
 	:ivar payee: The payee of the subtransaction
 	:ivar memo: The memo of the subtransaction
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/categoryrepo.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/categoryrepo.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 from ynabtransactionadjuster.exceptions import NoMatchingCategoryError, MultipleMatchingCategoriesError
 from ynabtransactionadjuster.models import CategoryGroup
 from ynabtransactionadjuster.models import Category
 
 
 class CategoryRepo:
-	"""Repository which holds all categories from your YNAB budget"""
+	"""Repository which holds all categories from your YNAB budget
+
+	:ivar _categories: List of Category Groups in YNAB budget
+	"""
 	def __init__(self, categories: List[CategoryGroup]):
 		self._categories = categories
 
 	def fetch_by_name(self, category_name: str, group_name: str = None) -> Category:
 		"""Fetches a YNAB category by its name
 
 		:param category_name: Name of the category to fetch
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/repos/payeerepo.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/repos/payeerepo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import List
 
 from ynabtransactionadjuster.exceptions import NoMatchingPayeeError
 from ynabtransactionadjuster.models import Payee
 
 
 class PayeeRepo:
-	"""Repository which holds all payees from your YNAB budget"""
+	"""Repository which holds all payees from your YNAB budget
 
+	:ivar _payees: List of payees in YNAB budget
+	"""
 	def __init__(self, payees: List[Payee]):
 		self._payees = payees
 
 	def fetch_by_name(self, payee_name: str) -> Payee:
 		"""Fetches a payee by its name
 
 		:param payee_name: Name of the payee to fetch
```

### Comparing `ynab_transaction_adjuster-0.3.8/ynabtransactionadjuster/ynabtransactionadjuster.py` & `ynab_transaction_adjuster-1.0.0/ynabtransactionadjuster/adjuster.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,107 @@
-from abc import abstractmethod
+from abc import abstractmethod, ABCMeta
+from dataclasses import dataclass
 from typing import List
 
-from ynabtransactionadjuster.adjuster import Adjuster
+from ynabtransactionadjuster.models import ModifiedTransaction
+from ynabtransactionadjuster.models.credentials import Credentials
 from ynabtransactionadjuster.client import Client
-from ynabtransactionadjuster.models import OriginalTransaction
-from ynabtransactionadjuster.models import TransactionModifier
+from ynabtransactionadjuster.models import Transaction
+from ynabtransactionadjuster.models import Modifier
 from ynabtransactionadjuster.repos import CategoryRepo
 from ynabtransactionadjuster.repos import PayeeRepo
+from ynabtransactionadjuster.serializer import Serializer
+from ynabtransactionadjuster.signaturechecker import SignatureChecker
 
 
-class YnabTransactionAdjuster:
+@dataclass
+class Adjuster(metaclass=ABCMeta):
 	"""Abstract class which modifies transactions according to concrete implementation. You need to create your own
 	child class and implement the `filter()`and `adjust()` method in it according to your needs. It has attributes
 	which allow you to lookup categories and payees from your budget.
 
-	:param budget: The YNAB budget id to use
-	:param account: The YNAB account id to use
-	:param token: The YNAB token to use
-
 	:ivar categories: Collection of current categories in YNAB budget
 	:ivar payees: Collection of current payees in YNAB budget
+	:ivar transactions: Transactions from YNAB Account
+	:ivar credentials: Credentials for YNAB API
 	"""
-	def __init__(self, budget: str, account: str, token: str) -> None:
-		self._budget = budget
-		self._account = account
-		self._client = Client(token=token, budget=budget, account=account)
-		self.categories: CategoryRepo = CategoryRepo(self._client.fetch_categories())
-		self.payees: PayeeRepo = PayeeRepo(self._client.fetch_payees())
-
-	def run(self) -> int:
-		"""Run the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
-		implementation of the two methods and push the updated transactions back to YNAB
-
-		:return: count of adjusted transactions which have been updated in YNAB
-		:raises AdjustError: if there is any error during the adjust process
-		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
-		"""
-		transactions = self._client.fetch_transactions()
-		filtered_transactions = self.filter(transactions)
-		adjuster = Adjuster(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
-		modified_transactions = adjuster.run()
-		if modified_transactions:
-			updated = self._client.update_transactions(modified_transactions)
-			return updated
-		return 0
-
-	def test(self) -> List[dict]:
-		"""Tests the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
-		implementation of the two methods. This function doesn't update records in YNAB but returns the modified
-		transactions so that they can be inspected. `#! select * from source`
-
-		The returned dicts have the following structure:
+	credentials: Credentials
+	categories: CategoryRepo
+	payees: PayeeRepo
+	transactions: List[Transaction]
+
+	@classmethod
+	def from_credentials(cls, credentials: Credentials):
+		"""Instantiate a Adjuster class from a Credentials object
 
-			{
-				"original": "<OriginalTransaction>",
-			 	"changes": {
-			 		"<Attribute>": {
-			 			"original": "<Original Value>",
-			 			"changed": "<Changed Value>"
-			 			}
-					}
-				}
-
-		:return: List of modified transactions in the format
-		:raises AdjustError: if there is any error during the adjust process
-		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
+		:param credentials: Credentials to use for YNAB API
 		"""
-		transactions = self._client.fetch_transactions()
-		filtered_transactions = self.filter(transactions)
-		sa = Adjuster(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
-		modified_transactions = [{'original': mt.original_transaction, 'changes': mt.changed_attributes()} for mt in sa.run()]
-		return modified_transactions
+		client = Client.from_credentials(credentials=credentials)
+		categories = CategoryRepo(client.fetch_categories())
+		payees = PayeeRepo(client.fetch_payees())
+		transactions = client.fetch_transactions()
+		return cls(categories=categories, payees=payees, transactions=transactions, credentials=credentials)
 
 	@abstractmethod
-	def filter(self, transactions: List[OriginalTransaction]) -> List[OriginalTransaction]:
+	def filter(self, transactions: List[Transaction]) -> List[Transaction]:
 		"""Function which implements filtering for the list of transactions from YNAB account. It receives a list of
 		the original transactions which can be filtered. Must return the filtered list or just the list if no filtering
 		is intended.
 
 		:param transactions: List of original transactions from YNAB
 		:return: Method needs to return a list of filtered transactions"""
 		pass
 
 	@abstractmethod
-	def adjust(self, original: OriginalTransaction, modifier: TransactionModifier) -> TransactionModifier:
+	def adjust(self, transaction: Transaction, modifier: Modifier) -> Modifier:
 		"""Function which implements the actual modification of a transaction. It receives the original transaction from
 		YNAB and a prefilled modifier. The modifier can be altered and must be returned.
 
-		:param original: Original transaction
+		:param transaction: Original transaction
 		:param modifier: Transaction modifier prefilled with values from original transaction. All attributes can be
 		changed and will modify the transaction
 		:returns: Method needs to return the transaction modifier after modification
 		"""
 		pass
+
+	def dry_run(self, pretty_print: bool = False) -> List[ModifiedTransaction]:
+		"""Tests the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
+		implementation of the two methods. This function doesn't update records in YNAB but returns the modified
+		transactions so that they can be inspected.
+
+		:param pretty_print: if set to True will print modified transactions as strings in console
+
+		:return: List of modified transactions
+		:raises SignatureError: if signature of implemented adjuster functions is not compatible
+		:raises AdjustError: if there is any error during the adjust process
+		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
+		"""
+		self.check_signatures()
+		filtered_transactions = self.filter(self.transactions)
+		s = Serializer(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
+		modified_transactions = s.run()
+		if pretty_print:
+			print('\n'.join(map(str, modified_transactions)))
+		return modified_transactions
+
+	def run(self) -> int:
+		"""Run the adjuster. It will fetch transactions from the YNAB account, filter & adjust them as per
+		implementation of the two methods and push the updated transactions back to YNAB
+
+		:return: count of adjusted transactions which have been updated in YNAB
+		:raises SignatureError: if signature of implemented adjuster functions is not compatible
+		:raises AdjustError: if there is any error during the adjust process
+		:raises HTTPError: if there is any error with the YNAB API (e.g. wrong credentials)
+		"""
+		self.check_signatures()
+		filtered_transactions = self.filter(self.transactions)
+		s = Serializer(transactions=filtered_transactions, adjust_func=self.adjust, categories=self.categories)
+		modified_transactions = s.run()
+		if modified_transactions:
+			client = Client.from_credentials(credentials=self.credentials)
+			updated = client.update_transactions(modified_transactions)
+			return updated
+		return 0
+
+	def check_signatures(self):
+		SignatureChecker(func=self.filter, parent_func=Adjuster.filter).check()
+		SignatureChecker(func=self.adjust, parent_func=Adjuster.adjust).check()
```

### Comparing `ynab_transaction_adjuster-0.3.8/PKG-INFO` & `ynab_transaction_adjuster-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: ynab-transaction-adjuster
-Version: 0.3.8
+Version: 1.0.0
 Summary: Library to adjust transactions in YNAB based on custom patterns
 License: MIT
 Author: Daniel Basta
 Author-email: ynab@basta.info
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
-Requires-Dist: requests (>=2.28.0)
+Requires-Dist: requests (>=2.28.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # ynab-transaction-adjuster
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-transaction-adjuster?style=flat)]() 
-[![Github Release](https://img.shields.io/maintenance/yes/2100)]()
+[![Maintained](https://img.shields.io/maintenance/yes/2100)]()
+[![Monthly downloads](https://img.shields.io/pypi/dm/ynab-transaction-adjuster)]()
 
 [!["Buy Me A Coffee"](https://img.shields.io/badge/Buy_Me_A_Coffee-FFDD00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black)](https://www.buymeacoffee.com/dnbasta)
 
 This library helps you to automatically adjust transactions in YNAB based on your logic. It allows you to implement 
 your adjustments in a simple factory class which you can run against your existing transactions and update relevant 
 fields like date, payee, category, memo and flags. It also allows you to split transactions.
 
@@ -44,54 +45,57 @@
 
 ## Usage
 A detailed documentation is available at https://ynab-transaction-adjuster.readthedocs.io
 
 # Basic Usage
 
 ### Create an Adjuster
-Create a child class of `YnabTransactionAdjuster`.
-This class needs to implement a `filter()` and an `adjust()` method which contain the intended logic. The `filter()`
-method receives a list of `OriginalTransaction` objects which can be filtered before 
-adjustement. The `adjust()` method receives a singular `OriginalTransaction` and a 
-`TransactionModifier`. The latter is prefilled with values from the original transaction. 
-Its attributes can be modified, and it needs to be returned at the end of the function. 
-Please check the [detailed usage](https://ynab-transaction-adjuster.readthedocs.io/en/latest/detailed_usage/) section for explanations how to change different attributes.
+Create a child class of `Adjuster`. This class needs to implement a `filter()` and an `adjust()` method which contain 
+the intended logic. The `filter()` method receives a list of `Transaction` objects which can be filtered before 
+adjustement. The `adjust()` method receives a single `Transaction` and a `Modifier`.The latter is prefilled with values 
+from the original transaction and can be altered. The modifier needs to be returned at the end of the function. 
+Please check the [detailed usage](https://ynab-transaction-adjuster.readthedocs.io/en/latest/detailed_usage/) section 
+for explanations how to change different attributes.
+
 ```py
-from ynabtransactionadjuster import YnabTransactionAdjuster
-from ynabtransactionadjuster.models import OriginalTransaction, TransactionModifier
+from ynabtransactionadjuster import Adjuster, Transaction, Modifier
+
+
+class MyAdjuster(Adjuster):
 
+	def filter(self, transactions: List[Transaction]) -> List[Transaction]:
+		# your implementation
 
-class MyAdjuster(YnabTransactionAdjuster):
-    
-    def filter(self, transactions: List[OriginalTransaction]) -> List[OriginalTransaction]:
-        # your implementation
-        
-        # return the filtered list of transactions
-        return transactions
-        
-    def adjust(self, original: OriginalTransaction, modifier: TransactionModifier) -> TransactionModifier:
-        # your implementation
+		# return the filtered list of transactions
+		return transactions
+
+	def adjust(self, transaction: Transaction, modifier: Modifier) -> Modifier:
+		# your implementation
 
 		# return the altered modifier
 		return modifier
 ```
 
 ### Initialize
-Initalize the adjuster with `token`, `budget` and `account` from YNAB
+Create a [`Credentials`][models.Credentials] object and initialize Adjuster class with it
 ```py
-my_adjuster = MyAdjuster(token='<token>', budget='<budget>', account='<account>')
+from ynabtransactionadjuster import Credentials
+
+my_credentials = Credentials(token='<token>', budget='<budget>', account='<account>')
+my_adjuster = MyAdjuster.from_credentials(credentials=my_credentials)
 ```
 
 ### Test
-Test the adjuster on records fetched via the `test()`method. The method fetches and executes the 
-adjustments but doesn't write the results back to YNAB. Instead it returns a list of 
-the changed transactions which can be inspected for the changed properties.
+Test the adjuster on records fetched via the `dry_run()` method. It executes the adjustments but doesn't write the 
+results back to YNAB. Instead it returns a list of the changed transactions which can be inspected for the changed 
+properties. It takes an optional parameter `pretty_print` which, if set to `True`, prints modifications in an easy 
+readable string representation to the console.
 
 ```py
-mod_transactions = my_adjuster.test()
+mod_transactions = my_adjuster.dry_run()
 ```
 
 ### Run
 If you are satisfied with the functionality you can execute the adjuster with the `run()` method. This will run the 
 adjustments and will update the changed transactions in YNAB. The method returns an integer with the number of 
 successfully updated records.
 ```py
```

