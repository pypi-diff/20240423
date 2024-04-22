# Comparing `tmp/pyield-0.7.4.tar.gz` & `tmp/pyield-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyield-0.7.4.tar", last modified: Sun Apr 21 13:58:29 2024, max compression
+gzip compressed data, was "pyield-0.7.5.tar", last modified: Mon Apr 22 23:52:21 2024, max compression
```

## Comparing `pyield-0.7.4.tar` & `pyield-0.7.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.4/LICENSE
--rw-r--r--   0        0        0     5177 2024-04-19 11:12:40.008362 pyield-0.7.4/README.md
--rw-r--r--   0        0        0       22 2024-04-20 10:57:56.123762 pyield-0.7.4/pyield/__about__.py
--rw-r--r--   0        0        0      422 2024-04-20 13:36:59.541311 pyield-0.7.4/pyield/__init__.py
--rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.4/pyield/bday.py
--rw-r--r--   0        0        0     6073 2024-04-21 13:45:50.722682 pyield-0.7.4/pyield/data_access.py
--rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.4/pyield/data_analysis.py
--rw-r--r--   0        0        0      333 2024-04-21 13:45:50.722682 pyield-0.7.4/pyield/futures/__init__.py
--rw-r--r--   0        0        0     7534 2024-04-21 13:44:00.419409 pyield-0.7.4/pyield/futures/common.py
--rw-r--r--   0        0        0     5817 2024-04-21 13:45:50.732682 pyield-0.7.4/pyield/futures/ddi.py
--rw-r--r--   0        0        0     7159 2024-04-21 13:45:25.305158 pyield-0.7.4/pyield/futures/di.py
--rw-r--r--   0        0        0    11499 2024-04-19 11:12:40.009362 pyield-0.7.4/pyield/futures/di_xml.py
--rw-r--r--   0        0        0     2990 2024-04-21 13:54:31.947419 pyield-0.7.4/pyield/futures/frc.py
--rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.4/pyield/holidays/__init__.py
--rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.4/pyield/holidays/br_holidays_new.txt
--rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.4/pyield/holidays/br_holidays_old.txt
--rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.4/pyield/holidays/core.py
--rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.4/pyield/indicators.py
--rw-r--r--   0        0        0     3395 2024-04-21 10:47:45.706989 pyield-0.7.4/pyield/projections.py
--rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.4/pyield/py.typed
--rw-r--r--   0        0        0     6617 2024-04-21 13:41:53.731824 pyield-0.7.4/pyield/treasuries.py
--rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.4/pyield/utils.py
--rw-r--r--   0        0        0     1195 2024-04-21 13:58:29.781319 pyield-0.7.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.4/tests/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.4/tests/test_bday.py
--rw-r--r--   0        0        0     2566 2024-04-21 13:41:53.732824 pyield-0.7.4/tests/test_futures.py
--rw-r--r--   0        0        0     7232 1970-01-01 00:00:00.000000 pyield-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-12-14 08:54:49.496702 pyield-0.7.5/LICENSE
+-rw-r--r--   0        0        0     6467 2024-04-21 17:20:40.545037 pyield-0.7.5/README.md
+-rw-r--r--   0        0        0       22 2024-04-22 23:36:47.721480 pyield-0.7.5/pyield/__about__.py
+-rw-r--r--   0        0        0      422 2024-04-20 13:36:59.541311 pyield-0.7.5/pyield/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-13 12:39:44.026704 pyield-0.7.5/pyield/bday.py
+-rw-r--r--   0        0        0     6073 2024-04-21 13:45:50.722682 pyield-0.7.5/pyield/data_access.py
+-rw-r--r--   0        0        0     1276 2024-04-17 08:50:12.086620 pyield-0.7.5/pyield/data_analysis.py
+-rw-r--r--   0        0        0      333 2024-04-21 13:45:50.722682 pyield-0.7.5/pyield/futures/__init__.py
+-rw-r--r--   0        0        0     7564 2024-04-22 23:37:56.705516 pyield-0.7.5/pyield/futures/common.py
+-rw-r--r--   0        0        0     4852 2024-04-21 16:42:03.532009 pyield-0.7.5/pyield/futures/ddi.py
+-rw-r--r--   0        0        0     6954 2024-04-22 23:43:30.630534 pyield-0.7.5/pyield/futures/di.py
+-rw-r--r--   0        0        0    11499 2024-04-19 11:12:40.009362 pyield-0.7.5/pyield/futures/di_xml.py
+-rw-r--r--   0        0        0     3190 2024-04-21 16:43:54.862383 pyield-0.7.5/pyield/futures/frc.py
+-rw-r--r--   0        0        0       55 2024-04-06 05:23:30.068485 pyield-0.7.5/pyield/holidays/__init__.py
+-rw-r--r--   0        0        0    14278 2024-01-16 09:33:28.571746 pyield-0.7.5/pyield/holidays/br_holidays_new.txt
+-rw-r--r--   0        0        0    14314 2023-12-28 23:26:42.737321 pyield-0.7.5/pyield/holidays/br_holidays_old.txt
+-rw-r--r--   0        0        0     2192 2024-04-07 10:57:52.523509 pyield-0.7.5/pyield/holidays/core.py
+-rw-r--r--   0        0        0     4268 2024-04-21 10:44:43.260419 pyield-0.7.5/pyield/indicators.py
+-rw-r--r--   0        0        0     3395 2024-04-21 10:47:45.706989 pyield-0.7.5/pyield/projections.py
+-rw-r--r--   0        0        0        0 2024-03-24 19:54:34.284748 pyield-0.7.5/pyield/py.typed
+-rw-r--r--   0        0        0     6617 2024-04-21 13:41:53.731824 pyield-0.7.5/pyield/treasuries.py
+-rw-r--r--   0        0        0     2190 2024-04-20 08:17:03.148377 pyield-0.7.5/pyield/utils.py
+-rw-r--r--   0        0        0     1195 2024-04-22 23:52:21.970537 pyield-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-14 18:12:36.515393 pyield-0.7.5/tests/__init__.py
+-rw-r--r--   0        0        0     1114 2024-04-16 12:01:55.676922 pyield-0.7.5/tests/test_bday.py
+-rw-r--r--   0        0        0     2585 2024-04-22 23:45:59.541771 pyield-0.7.5/tests/test_futures.py
+-rw-r--r--   0        0        0     8522 1970-01-01 00:00:00.000000 pyield-0.7.5/PKG-INFO
```

### Comparing `pyield-0.7.4/LICENSE` & `pyield-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/README.md` & `pyield-0.7.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![PyPI version](https://img.shields.io/pypi/v/pyield.svg)](https://pypi.python.org/pypi/pyield)
 [![Made with Python](https://img.shields.io/badge/Python->=3.11-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 
-# PYield: Fixed Income Toolbox for Brazilian Markets
+# PYield: Brazilian Fixed Income Toolkit
 
 ## Introduction
 
 Welcome to PYield, a Python library designed for the analysis of fixed income instruments in Brazil. This library is tailored for financial analysts, researchers, and enthusiasts interested in the Brazilian fixed income market. Leveraging the power of popular Python libraries like Pandas and Requests, PYield simplifies the process of obtaining and processing data from key sources such as ANBIMA, BCB, IBGE and B3.
 
 ## Features
 
@@ -52,57 +52,67 @@
 1   2024-01-02
 2   2024-01-03
 dtype: datetime64[ns]
 ```
 
 ### Futures Data
 ```python
-# Fetch a DataFrame with the DI Futures data from B3
->>> yd.fetch_asset(asset_code="DI1", reference_date='2024-03-08')
+# Fetch current DI Futures data from B3 (15 minutes delay)
+>>> yd.fetch_asset(asset_code="DI1")
+TradeTimestamp      TickerSymbol ExpirationDate BDaysToExp ... MaxRate LastAskRate LastBidRate LastRate
+2024-04-21 13:37:39       DI1K24     2024-05-02          7 ... 0.10660     0.10652     0.10660  0.10660
+2024-04-21 13:37:39       DI1M24     2024-06-03         28 ... 0.10518     0.10510     0.10516  0.10518
+2024-04-21 13:37:39       DI1N24     2024-07-01         48 ... 0.10480     0.10456     0.10462  0.10460
+                ...          ...            ...        ... ...     ...         ...         ...      ...
+2024-04-21 13:37:39       DI1F37     2037-01-02       3183 ...    <NA>        <NA>     0.11600     <NA>
+2024-04-21 13:37:39       DI1F38     2038-01-04       3432 ...    <NA>        <NA>     0.11600     <NA>
+2024-04-21 13:37:39       DI1F39     2039-01-03       3683 ...    <NA>        <NA>        <NA>     <NA>
 
+# Fetch historical DI Futures data from B3
+>>> yd.fetch_asset(asset_code="DI1", reference_date='2024-03-08')
 TradeDate  TickerSymbol ExpirationDate BDaysToExp ... LastRate LastAskRate LastBidRate SettlementRate
-2024-03-08 DI1J24            2024-04-01     15                ... 10.952   10.952      10.956      10.956
-2024-03-08 DI1K24            2024-05-02     37                ... 10.776   10.774      10.780      10.777
-2024-03-08 DI1M24            2024-06-03     58                ... 10.604   10.602      10.604      10.608
-...        ...            ...            ...               ... ...      ...         ...         ...
-2024-03-08 DI1F37            2037-01-02     3213              ... <NA>     <NA>        <NA>        10.859
-2024-03-08 DI1F38            2038-01-04     3462              ... <NA>     <NA>        <NA>        10.859
-2024-03-08 DI1F39            2039-01-03     3713              ... <NA>     <NA>        <NA>        10.85
+2024-03-08       DI1J24     2024-04-01         15 ...   10.952      10.952      10.956         10.956
+2024-03-08       DI1K24     2024-05-02         37 ...   10.776      10.774      10.780         10.777
+2024-03-08       DI1M24     2024-06-03         58 ...   10.604      10.602      10.604         10.608
+       ...          ...            ...        ... ...      ...         ...         ...            ...
+2024-03-08       DI1F37     2037-01-02       3213 ...     <NA>        <NA>        <NA>         10.859
+2024-03-08       DI1F38     2038-01-04       3462 ...     <NA>        <NA>        <NA>         10.859
+2024-03-08       DI1F39     2039-01-03       3713 ...     <NA>        <NA>        <NA>         10.85
 ```
 
 ### Treasury Bonds Data
 ```python
 # Fetch a DataFrame with the NTN-B data from ANBIMA
 # Anbima data is available for the last 5 working days
 # Obs: Anbima members have access to the full history
 >>> yd.fetch_asset(asset_code="NTN-B", reference_date='2024-04-12')
 
-BondType ReferenceDate MaturityDate BidRate AskRate IndicativeRate Price
-NTN-B    2024-04-12    2024-08-15   0.07540 0.07504 0.07523        4,271.43565
-NTN-B    2024-04-12    2025-05-15   0.05945 0.05913 0.05930        4,361.34391
-NTN-B    2024-04-12    2026-08-15   0.05927 0.05897 0.05910        4,301.40082
-...      ...           ...          ...     ...     ...            ...
-NTN-B    2024-04-12    2050-08-15   0.06039 0.06006 0.06023        4,299.28233
-NTN-B    2024-04-12    2055-05-15   0.06035 0.05998 0.06017        4,367.13360
-NTN-B    2024-04-12    2060-08-15   0.06057 0.06016 0.06036        4,292.26323
+BondType ReferenceDate MaturityDate BidRate AskRate IndicativeRate       Price
+   NTN-B    2024-04-12   2024-08-15 0.07540 0.07504        0.07523 4,271.43565
+   NTN-B    2024-04-12   2025-05-15 0.05945 0.05913        0.05930 4,361.34391
+   NTN-B    2024-04-12   2026-08-15 0.05927 0.05897        0.05910 4,301.40082
+     ...           ...          ...     ...     ...            ...         ...
+   NTN-B    2024-04-12   2050-08-15 0.06039 0.06006        0.06023 4,299.28233
+   NTN-B    2024-04-12   2055-05-15 0.06035 0.05998        0.06017 4,367.13360
+   NTN-B    2024-04-12   2060-08-15 0.06057 0.06016        0.06036 4,292.26323
 ```
 
 ### Spreads Calculation
 ```python
 # Calculate the spread between two DI Futures contracts and the pre-fix bonds
 >>> yd.calculate_spreads(spread_type="di_vs_pre", reference_date="2024-4-11")
 
 BondType ReferenceDate MaturityDate  DISpread
-LTN      2024-04-11    2024-07-01    -20.28000
-LTN      2024-04-11    2024-10-01    -10.19000
-LTN      2024-04-11    2025-01-01    -15.05000
-...      ...           ...           ...
-NTN-F    2024-04-11    2031-01-01    -0.66000
-NTN-F    2024-04-11    2033-01-01    -5.69000
-NTN-F    2024-04-11    2035-01-01    -1.27000
+     LTN    2024-04-11   2024-07-01    -20.28
+     LTN    2024-04-11   2024-10-01    -10.19
+     LTN    2024-04-11   2025-01-01    -15.05
+   ...      ...           ...           ...
+   NTN-F    2024-04-11   2031-01-01     -0.66
+   NTN-F    2024-04-11   2033-01-01     -5.69
+   NTN-F    2024-04-11   2035-01-01     -1.27
 ```
 
 ### Indicators Data
 ```python
 # Fetch the SELIC target rate from the Central Bank of Brazil
 >>> yd.fetch_indicator(indicator_code="SELIC", reference_date='2024-04-12')
 10.75
@@ -111,7 +121,23 @@
 >>> yd.fetch_indicator(indicator_code="IPCA", reference_date='2024-03-18')
 0.16
 
 # If no data is yet available for the indicator, the function returns None
 >>> yd.fetch_indicator(indicator_code="IPCA", reference_date='2024-04-10')
 None
 ```
+
+### Projections Data
+```python
+# Fetch current month projection for IPCA from IBGE API
+>>> ipca = yd.fetch_projection(projection_code="IPCA_CM")
+>>> print(ipca)
+IndicatorProjection(
+    last_updated=Timestamp('2024-04-19 18:55:00'),
+    reference_month_ts=Timestamp('2024-04-01 00:00:00'),
+    reference_month_br='ABR/2024',
+    projected_value=0.0035
+)
+>>> ipca.projected_value
+0.0035
+```
+
```

### Comparing `pyield-0.7.4/pyield/bday.py` & `pyield-0.7.5/pyield/bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/data_access.py` & `pyield-0.7.5/pyield/data_access.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/data_analysis.py` & `pyield-0.7.5/pyield/data_analysis.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/futures/common.py` & `pyield-0.7.5/pyield/futures/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,30 +129,31 @@
 
     except (KeyError, ValueError):
         return pd.NaT  # type: ignore
 
 
 def fetch_past_raw_df(asset_code: str, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
-    Fetch the historical futures data from B3 for a specific trade date.
+    Fetch the historical futures data from B3 for a specific trade date. If the data is
+    not available, an empty DataFrame is returned.
 
     Args:
         trade_date (pd.Timestamp): The trade date for which the data should be fetched.
 
     Returns:
         pd.DataFrame: Raw DI data as a Pandas pd.DataFrame.
     """
     url_date = trade_date.strftime("%d/%m/%Y")
     # url example: https://www2.bmf.com.br/pages/portal/bmfbovespa/boletim1/SistemaPregao_excel1.asp?Data=05/10/2023&Mercadoria=DI1
     url = f"https://www2.bmf.com.br/pages/portal/bmfbovespa/boletim1/SistemaPregao_excel1.asp?Data={url_date}&Mercadoria={asset_code}&XLS=false"
     r = requests.get(url)
 
     text = r.text
     if "AJUSTE" not in text:
-        raise ValueError(f"Could not fetch data for {url_date}.")
+        return pd.DataFrame()
 
     df = pd.read_html(
         io.StringIO(text),
         match="AJUSTE",
         header=1,
         thousands=".",
         decimal=",",
```

### Comparing `pyield-0.7.4/pyield/futures/ddi.py` & `pyield-0.7.5/pyield/futures/di.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,80 @@
 import pandas as pd
 
+from .. import bday
 from . import common
 
 
-def _convert_prices_to_rates(prices: pd.Series, n_days: pd.Series) -> pd.Series:
+def _convert_prices_to_rates(prices: pd.Series, bd: pd.Series) -> pd.Series:
     """
-    Internal function to convert DDI futures prices to rates.
+    Internal function to convert DI futures prices to rates.
 
     Args:
-        prices (pd.Series): A pd.Series containing DDI futures prices.
-        bd (pd.Series): A serie containing the number of days to expiration.
+        prices (pd.Series): A pd.Series containing DI futures prices.
+        bd (pd.Series): A serie containing the number of business days to expiration.
 
     Returns:
-        pd.Series: A pd.Series containing DDI futures rates.
+        pd.Series: A pd.Series containing DI futures rates.
     """
-    rates = (100_000 / prices - 1) * (360 / n_days)
+    rates = (100_000 / prices) ** (252 / bd) - 1
 
     # Return rates as percentage
     return 100 * rates
 
 
 def _convert_prices_in_older_contracts(df: pd.DataFrame) -> pd.DataFrame:
     # Prior to 01/01/2002, prices were not converted to rates
     convert_cols = [
         "FirstRate",
         "MinRate",
         "MaxRate",
         "AvgRate",
-        "LastRate",
-        "LastBidRate",
-        "LastAskRate",
+        "CloseRate",
+        "CloseBidRate",
+        "CloseAskRate",
     ]
     for col in convert_cols:
-        df[col] = _convert_prices_to_rates(df[col], df["DaysToExpiration"])
+        df[col] = _convert_prices_to_rates(df[col], df["BDaysToExp"])
 
     # Invert low and high prices
     df["MinRate"], df["MaxRate"] = df["MaxRate"], df["MinRate"]
 
     return df
 
 
-def _process_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
+def _process_past_raw_df(df: pd.DataFrame, trade_date: pd.Timestamp) -> pd.DataFrame:
     """
     Internal function to process and transform raw DI futures data.
 
     Args:
         df (pd.DataFrame): the raw DI DataFrame.
         trade_date: a datetime-like object representing the trade date.
 
     Returns:
         pd.DataFrame: Processed and transformed data as a Pandas pd.DataFrame.
     """
-    # Check if the pd.DataFrame is empty
-    if df.empty:
-        return df
-
     rename_dict = {
         "VENCTO": "ExpirationCode",
         "CONTR. ABERT.(1)": "OpenContracts",  # At the start of the day
         "CONTR. FECH.(2)": "OpenContractsEndSession",  # At the end of the day
         "NÚM. NEGOC.": "TradeCount",
         "CONTR. NEGOC.": "TradeVolume",
         "VOL.": "FinancialVolume",
         "AJUSTE": "SettlementPrice",
         "AJUSTE ANTER. (3)": "PrevSettlementRate",
         "AJUSTE CORRIG. (4)": "AdjSettlementRate",
         "PREÇO MÍN.": "MinRate",
         "PREÇO MÉD.": "AvgRate",
         "PREÇO MÁX.": "MaxRate",
         "PREÇO ABERTU.": "FirstRate",
-        "ÚLT. PREÇO": "LastRate",
+        "ÚLT. PREÇO": "CloseRate",
         "VAR. PTOS.": "PointsVariation",
         # Attention: bid/ask rates are inverted
-        "ÚLT.OF. COMPRA": "LastAskRate",
-        "ÚLT.OF. VENDA": "LastBidRate",
+        "ÚLT.OF. COMPRA": "CloseAskRate",
+        "ÚLT.OF. VENDA": "CloseBidRate",
     }
 
     df = df.rename(columns=rename_dict)
 
     df["TradeDate"] = trade_date
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradeDate"] = df["TradeDate"].astype("datetime64[ns]")
@@ -86,93 +83,129 @@
     if trade_date < pd.Timestamp("2006-05-22"):
         df["ExpirationDate"] = df["ExpirationCode"].apply(
             common.get_old_expiration_date, args=(trade_date,)
         )
     else:
         df["ExpirationDate"] = df["ExpirationCode"].apply(common.get_expiration_date)
 
-    df["DaysToExpiration"] = (df["ExpirationDate"] - trade_date).dt.days
-    # Convert to nullable integer, since other columns use this data type
-    df["DaysToExpiration"] = df["DaysToExpiration"].astype(pd.Int64Dtype())
+    df["BDaysToExp"] = bday.count_bdays(trade_date, df["ExpirationDate"])
     # Remove expired contracts
-    df.query("DaysToExpiration > 0", inplace=True)
-
-    # Columns where 0 means NaN
-    cols_with_nan = [
-        "SettlementPrice",
-        "FirstRate",
-        "MinRate",
-        "MaxRate",
-        "AvgRate",
-        "LastRate",
-        "LastBidRate",
-        "LastAskRate",
-    ]
-    for col in cols_with_nan:
-        df[col] = df[col].replace(0, pd.NA)
+    df.query("BDaysToExp > 0", inplace=True)
 
     # Prior to 17/01/2002 (incluive), prices were not converted to rates
     if trade_date <= pd.Timestamp("2002-01-17"):
         df = _convert_prices_in_older_contracts(df)
 
     df["SettlementRate"] = _convert_prices_to_rates(
-        df["SettlementPrice"], df["DaysToExpiration"]
+        df["SettlementPrice"], df["BDaysToExp"]
     )
 
-    # Remove percentage in all rate columns and round to 5 decimal places since it's the
-    # precision used by B3. Obs: 5 decimal places = 3 decimal places in percentage
     rate_cols = [col for col in df.columns if "Rate" in col]
-    for col in rate_cols:
-        df[col] = (df[col] / 100).round(5)
+    cols_with_nan = rate_cols + ["SettlementPrice"]
+    # Columns where 0 means NaN
+    df[cols_with_nan] = df[cols_with_nan].replace(0, pd.NA)
+    # Remove % and round to 5 dec. places (3 in %) since it is the contract's precision
+    df[rate_cols] = df[rate_cols].div(100).round(5)
+
+    df["TickerSymbol"] = "DI1" + df["ExpirationCode"]
 
     # Filter and order columns
     ordered_cols = [
         "TradeDate",
-        "ExpirationCode",
+        "TickerSymbol",
+        # "ExpirationCode",
         "ExpirationDate",
-        "DaysToExpiration",
+        "BDaysToExp",
         "OpenContracts",
         # "OpenContractsEndSession" since there is no OpenContracts at the end of the
         # day in XML data, it will be removed to avoid confusion with XML data
         "TradeCount",
         "TradeVolume",
         "FinancialVolume",
         "SettlementPrice",
+        "SettlementRate",
+        "FirstRate",
         "MinRate",
         "AvgRate",
         "MaxRate",
-        "FirstRate",
-        "LastRate",
-        "LastAskRate",
-        "LastBidRate",
-        "SettlementRate",
+        "CloseAskRate",
+        "CloseBidRate",
+        "CloseRate",
     ]
     return df[ordered_cols]
 
 
-def fetch_past_ddi(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+def _process_last_raw_di_df(raw_df: pd.DataFrame) -> pd.DataFrame:
+    df = raw_df.copy()
+
+    # Columns to be renamed
+    rename_columns = {
+        "TradeTimestamp": "TradeTimestamp",
+        "symb": "TickerSymbol",
+        "mtrtyCode": "ExpirationDate",
+        "BDaysToExp": "BDaysToExp",
+        "opnCtrcts": "OpenContracts",
+        "tradQty": "TradeCount",
+        "traddCtrctsQty": "TradeVolume",
+        "grssAmt": "FinancialVolume",
+        "prvsDayAdjstmntPric": "PrevSettlementRate",
+        "bottomLmtPric": "MinLimitRate",
+        "topLmtPric": "MaxLimitRate",
+        "opngPric": "OpenRate",
+        "minPric": "MinRate",
+        "avrgPric": "AvgRate",
+        "maxPric": "MaxRate",
+        "buyOffer.price": "LastAskRate",
+        "sellOffer.price": "LastBidRate",
+        "curPrc": "LastRate",
+    }
+    # Rename columns
+    df = df.rename(columns=rename_columns)
+
+    df["BDaysToExp"] = bday.count_bdays(df["TradeTimestamp"], df["ExpirationDate"])
+
+    # Remove percentage in all rate columns
+    rate_cols = [col for col in df.columns if "Rate" in col]
+    df[rate_cols] = df[rate_cols] / 100
+
+    # Reorder columns based on the order of the dictionary
+    return df[rename_columns.values()]
+
+
+def fetch_last_di() -> pd.DataFrame:
     """
-    Fetchs the DDI futures data for a given date from B3.
+    Fetch the latest DI futures data from B3.
+
+    Returns:
+        pd.DataFrame: A Pandas pd.DataFrame containing the latest DI futures data.
+    """
+    raw_df = common.fetch_last_raw_df(future_code="DI1")
+    return _process_last_raw_di_df(raw_df)
+
+
+def fetch_past_di(trade_date: pd.Timestamp, return_raw: bool = False) -> pd.DataFrame:
+    """
+    Fetchs the DI futures data for a given date from B3.
 
     This function fetches and processes the DI futures data from B3 for a specific
-    trade date. It's the primary external interface for accessing DI data.
+    trade date. It's the primary external interface for accessing DI data. If the data
+    is not available, an empty DataFrame is returned.
 
     Args:
         trade_date (pd.Timestamp): The trade date to fetch the DI futures data.
-        raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
+        return_raw (bool): If True, returns the raw data as a Pandas pd.DataFrame.
             Defaults to False.
 
     Returns:
         pd.DataFrame: A Pandas pd.DataFrame containing processed DI futures data.
 
-    Examples:
-        >>> from pyield.futures import di
-        >>> di.fetch_ddi(pd.Timestamp("2021-01-04"))
-
     Notes:
-        - DaysToExpiration: number of business days to ExpirationDate.
+        - BDaysToExp: number of business days to ExpirationDate.
         - OpenContracts: number of open contracts at the start of the trading day.
     """
-    df_raw = common.fetch_past_raw_df(asset_code="DDI", trade_date=trade_date)
+    df_raw = common.fetch_past_raw_df(asset_code="DI1", trade_date=trade_date)
     if return_raw:
         return df_raw
-    return _process_raw_df(df_raw, trade_date)
+    if df_raw.empty:
+        return pd.DataFrame()
+    else:
+        return _process_past_raw_df(df_raw, trade_date)
```

### Comparing `pyield-0.7.4/pyield/futures/di_xml.py` & `pyield-0.7.5/pyield/futures/di_xml.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/futures/frc.py` & `pyield-0.7.5/pyield/futures/frc.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,22 +37,26 @@
 
     df = df.rename(columns=rename_dict)
 
     df["TradeDate"] = trade_date
     # Convert to datetime64[ns] since it is pandas default type for timestamps
     df["TradeDate"] = df["TradeDate"].astype("datetime64[ns]")
 
-    df["ExpirationDate"] = df["ExpirationCode"].apply(common.get_expiration_date)
+    # Contract code format was changed in 22/05/2006
+    if trade_date < pd.Timestamp("2006-05-22"):
+        df["ExpirationDate"] = df["ExpirationCode"].apply(
+            common.get_old_expiration_date, args=(trade_date,)
+        )
+    else:
+        df["ExpirationDate"] = df["ExpirationCode"].apply(common.get_expiration_date)
 
     # Replace 0 values in rate columns with pd.NA and remove percentage
     rate_cols = [col for col in df.columns if "Rate" in col]
-    for col in rate_cols:
-        df[col] = df[col].replace(0, pd.NA)
-        # Round to 5 decimal places (3 in %) since it is the contract's precision
-        df[col] = (df[col] / 100).round(5)
+    # Round to 5 decimal places (3 in %) since it is the contract's precision
+    df[rate_cols] = df[rate_cols].replace(0, pd.NA).div(100).round(5)
 
     df["TickerSymbol"] = "FRC" + df["ExpirationCode"]
 
     # Filter and order columns
     ordered_cols = [
         "TradeDate",
         "TickerSymbol",
```

### Comparing `pyield-0.7.4/pyield/holidays/br_holidays_new.txt` & `pyield-0.7.5/pyield/holidays/br_holidays_new.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/holidays/br_holidays_old.txt` & `pyield-0.7.5/pyield/holidays/br_holidays_old.txt`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/holidays/core.py` & `pyield-0.7.5/pyield/holidays/core.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/indicators.py` & `pyield-0.7.5/pyield/indicators.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/projections.py` & `pyield-0.7.5/pyield/projections.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/treasuries.py` & `pyield-0.7.5/pyield/treasuries.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyield/utils.py` & `pyield-0.7.5/pyield/utils.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/pyproject.toml` & `pyield-0.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "numpy",
     "beautifulsoup4",
     "html5lib",
     "lxml",
     "python-calamine>=0.2.0",
 ]
 dynamic = []
-version = "0.7.4"
+version = "0.7.5"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Source = "https://github.com/crdcj/PYield"
```

### Comparing `pyield-0.7.4/tests/test_bday.py` & `pyield-0.7.5/tests/test_bday.py`

 * *Files identical despite different names*

### Comparing `pyield-0.7.4/tests/test_futures.py` & `pyield-0.7.5/tests/test_futures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pandas as pd
-import pytest
 
 from pyield import futures as ft
 
 
 def test_valid_old_contract_code1():
     expiration_code = "JAN3"  # Valid contract code
     trade_date = pd.Timestamp("2001-05-21")
@@ -72,9 +71,10 @@
     tickers = list(settlement_rates.keys())  # noqa: F841
     results = df.query("TickerSymbol in @tickers")["SettlementRate"].to_list()
     assert results == list(settlement_rates.values())
 
 
 def test_non_business_day():
     non_business_day = pd.Timestamp("2023-12-24")
-    with pytest.raises(ValueError):
-        ft.fetch_past_di(trade_date=non_business_day)
+    # Test if it an empty DataFrame is returned
+    df = ft.fetch_past_di(trade_date=non_business_day)
+    assert df.empty
```

### Comparing `pyield-0.7.4/PKG-INFO` & `pyield-0.7.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PYield
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Python library for analysis of fixed income instruments in Brazil
 Keywords: fixed-income, brazil, finance, analysis, bonds
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Carlos Carvalho
         
@@ -41,15 +41,15 @@
 Requires-Dist: python-calamine>=0.2.0
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/pyield.svg)](https://pypi.python.org/pypi/pyield)
 [![Made with Python](https://img.shields.io/badge/Python->=3.11-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/badge/License-MIT-blue)](#license)
 
-# PYield: Fixed Income Toolbox for Brazilian Markets
+# PYield: Brazilian Fixed Income Toolkit
 
 ## Introduction
 
 Welcome to PYield, a Python library designed for the analysis of fixed income instruments in Brazil. This library is tailored for financial analysts, researchers, and enthusiasts interested in the Brazilian fixed income market. Leveraging the power of popular Python libraries like Pandas and Requests, PYield simplifies the process of obtaining and processing data from key sources such as ANBIMA, BCB, IBGE and B3.
 
 ## Features
 
@@ -95,57 +95,67 @@
 1   2024-01-02
 2   2024-01-03
 dtype: datetime64[ns]
 ```
 
 ### Futures Data
 ```python
-# Fetch a DataFrame with the DI Futures data from B3
->>> yd.fetch_asset(asset_code="DI1", reference_date='2024-03-08')
+# Fetch current DI Futures data from B3 (15 minutes delay)
+>>> yd.fetch_asset(asset_code="DI1")
+TradeTimestamp      TickerSymbol ExpirationDate BDaysToExp ... MaxRate LastAskRate LastBidRate LastRate
+2024-04-21 13:37:39       DI1K24     2024-05-02          7 ... 0.10660     0.10652     0.10660  0.10660
+2024-04-21 13:37:39       DI1M24     2024-06-03         28 ... 0.10518     0.10510     0.10516  0.10518
+2024-04-21 13:37:39       DI1N24     2024-07-01         48 ... 0.10480     0.10456     0.10462  0.10460
+                ...          ...            ...        ... ...     ...         ...         ...      ...
+2024-04-21 13:37:39       DI1F37     2037-01-02       3183 ...    <NA>        <NA>     0.11600     <NA>
+2024-04-21 13:37:39       DI1F38     2038-01-04       3432 ...    <NA>        <NA>     0.11600     <NA>
+2024-04-21 13:37:39       DI1F39     2039-01-03       3683 ...    <NA>        <NA>        <NA>     <NA>
 
+# Fetch historical DI Futures data from B3
+>>> yd.fetch_asset(asset_code="DI1", reference_date='2024-03-08')
 TradeDate  TickerSymbol ExpirationDate BDaysToExp ... LastRate LastAskRate LastBidRate SettlementRate
-2024-03-08 DI1J24            2024-04-01     15                ... 10.952   10.952      10.956      10.956
-2024-03-08 DI1K24            2024-05-02     37                ... 10.776   10.774      10.780      10.777
-2024-03-08 DI1M24            2024-06-03     58                ... 10.604   10.602      10.604      10.608
-...        ...            ...            ...               ... ...      ...         ...         ...
-2024-03-08 DI1F37            2037-01-02     3213              ... <NA>     <NA>        <NA>        10.859
-2024-03-08 DI1F38            2038-01-04     3462              ... <NA>     <NA>        <NA>        10.859
-2024-03-08 DI1F39            2039-01-03     3713              ... <NA>     <NA>        <NA>        10.85
+2024-03-08       DI1J24     2024-04-01         15 ...   10.952      10.952      10.956         10.956
+2024-03-08       DI1K24     2024-05-02         37 ...   10.776      10.774      10.780         10.777
+2024-03-08       DI1M24     2024-06-03         58 ...   10.604      10.602      10.604         10.608
+       ...          ...            ...        ... ...      ...         ...         ...            ...
+2024-03-08       DI1F37     2037-01-02       3213 ...     <NA>        <NA>        <NA>         10.859
+2024-03-08       DI1F38     2038-01-04       3462 ...     <NA>        <NA>        <NA>         10.859
+2024-03-08       DI1F39     2039-01-03       3713 ...     <NA>        <NA>        <NA>         10.85
 ```
 
 ### Treasury Bonds Data
 ```python
 # Fetch a DataFrame with the NTN-B data from ANBIMA
 # Anbima data is available for the last 5 working days
 # Obs: Anbima members have access to the full history
 >>> yd.fetch_asset(asset_code="NTN-B", reference_date='2024-04-12')
 
-BondType ReferenceDate MaturityDate BidRate AskRate IndicativeRate Price
-NTN-B    2024-04-12    2024-08-15   0.07540 0.07504 0.07523        4,271.43565
-NTN-B    2024-04-12    2025-05-15   0.05945 0.05913 0.05930        4,361.34391
-NTN-B    2024-04-12    2026-08-15   0.05927 0.05897 0.05910        4,301.40082
-...      ...           ...          ...     ...     ...            ...
-NTN-B    2024-04-12    2050-08-15   0.06039 0.06006 0.06023        4,299.28233
-NTN-B    2024-04-12    2055-05-15   0.06035 0.05998 0.06017        4,367.13360
-NTN-B    2024-04-12    2060-08-15   0.06057 0.06016 0.06036        4,292.26323
+BondType ReferenceDate MaturityDate BidRate AskRate IndicativeRate       Price
+   NTN-B    2024-04-12   2024-08-15 0.07540 0.07504        0.07523 4,271.43565
+   NTN-B    2024-04-12   2025-05-15 0.05945 0.05913        0.05930 4,361.34391
+   NTN-B    2024-04-12   2026-08-15 0.05927 0.05897        0.05910 4,301.40082
+     ...           ...          ...     ...     ...            ...         ...
+   NTN-B    2024-04-12   2050-08-15 0.06039 0.06006        0.06023 4,299.28233
+   NTN-B    2024-04-12   2055-05-15 0.06035 0.05998        0.06017 4,367.13360
+   NTN-B    2024-04-12   2060-08-15 0.06057 0.06016        0.06036 4,292.26323
 ```
 
 ### Spreads Calculation
 ```python
 # Calculate the spread between two DI Futures contracts and the pre-fix bonds
 >>> yd.calculate_spreads(spread_type="di_vs_pre", reference_date="2024-4-11")
 
 BondType ReferenceDate MaturityDate  DISpread
-LTN      2024-04-11    2024-07-01    -20.28000
-LTN      2024-04-11    2024-10-01    -10.19000
-LTN      2024-04-11    2025-01-01    -15.05000
-...      ...           ...           ...
-NTN-F    2024-04-11    2031-01-01    -0.66000
-NTN-F    2024-04-11    2033-01-01    -5.69000
-NTN-F    2024-04-11    2035-01-01    -1.27000
+     LTN    2024-04-11   2024-07-01    -20.28
+     LTN    2024-04-11   2024-10-01    -10.19
+     LTN    2024-04-11   2025-01-01    -15.05
+   ...      ...           ...           ...
+   NTN-F    2024-04-11   2031-01-01     -0.66
+   NTN-F    2024-04-11   2033-01-01     -5.69
+   NTN-F    2024-04-11   2035-01-01     -1.27
 ```
 
 ### Indicators Data
 ```python
 # Fetch the SELIC target rate from the Central Bank of Brazil
 >>> yd.fetch_indicator(indicator_code="SELIC", reference_date='2024-04-12')
 10.75
@@ -154,7 +164,23 @@
 >>> yd.fetch_indicator(indicator_code="IPCA", reference_date='2024-03-18')
 0.16
 
 # If no data is yet available for the indicator, the function returns None
 >>> yd.fetch_indicator(indicator_code="IPCA", reference_date='2024-04-10')
 None
 ```
+
+### Projections Data
+```python
+# Fetch current month projection for IPCA from IBGE API
+>>> ipca = yd.fetch_projection(projection_code="IPCA_CM")
+>>> print(ipca)
+IndicatorProjection(
+    last_updated=Timestamp('2024-04-19 18:55:00'),
+    reference_month_ts=Timestamp('2024-04-01 00:00:00'),
+    reference_month_br='ABR/2024',
+    projected_value=0.0035
+)
+>>> ipca.projected_value
+0.0035
+```
+
```

