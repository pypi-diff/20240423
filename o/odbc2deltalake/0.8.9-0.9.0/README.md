# Comparing `tmp/odbc2deltalake-0.8.9.tar.gz` & `tmp/odbc2deltalake-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odbc2deltalake-0.8.9.tar", max compression
+gzip compressed data, was "odbc2deltalake-0.9.0.tar", max compression
```

## Comparing `odbc2deltalake-0.8.9.tar` & `odbc2deltalake-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1081 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/LICENSE
--rw-r--r--   0        0        0     3563 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/README.md
--rw-r--r--   0        0        0      571 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/__init__.py
--rw-r--r--   0        0        0    36444 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/db_to_delta.py
--rw-r--r--   0        0        0     4371 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/delta_logger.py
--rw-r--r--   0        0        0       38 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/destination/__init__.py
--rw-r--r--   0        0        0     2554 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/destination/azure.py
--rw-r--r--   0        0        0     2923 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/destination/azure_utils.py
--rw-r--r--   0        0        0     2541 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/destination/databricks.py
--rw-r--r--   0        0        0     1196 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/destination/destination.py
--rw-r--r--   0        0        0     1592 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/destination/file_system.py
--rw-r--r--   0        0        0     5458 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/metadata.py
--rw-r--r--   0        0        0     1221 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/odbc_utils.py
--rw-r--r--   0        0        0     1851 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/query.py
--rw-r--r--   0        0        0       38 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/reader/__init__.py
--rw-r--r--   0        0        0     7295 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/reader/odbc_reader.py
--rw-r--r--   0        0        0     1961 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/reader/reader.py
--rw-r--r--   0        0        0     4932 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/reader/spark_reader.py
--rw-r--r--   0        0        0     1976 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/sql_glot_utils.py
--rw-r--r--   0        0        0     1211 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/sql_schema.py
--rw-r--r--   0        0        0      249 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/utils.py
--rw-r--r--   0        0        0     7525 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/write_init.py
--rw-r--r--   0        0        0        0 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/write_utils/__init__.py
--rw-r--r--   0        0        0     6810 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/odbc2deltalake/write_utils/restore_pk.py
--rw-r--r--   0        0        0     1392 2024-04-22 11:36:48.490805 odbc2deltalake-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 odbc2deltalake-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-23 12:52:12.356009 odbc2deltalake-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3563 2024-04-23 12:52:12.356009 odbc2deltalake-0.9.0/README.md
+-rw-r--r--   0        0        0      571 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/__init__.py
+-rw-r--r--   0        0        0    37607 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/db_to_delta.py
+-rw-r--r--   0        0        0     4371 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/delta_logger.py
+-rw-r--r--   0        0        0       38 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/__init__.py
+-rw-r--r--   0        0        0     2554 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/azure.py
+-rw-r--r--   0        0        0     2923 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/azure_utils.py
+-rw-r--r--   0        0        0     2541 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/databricks.py
+-rw-r--r--   0        0        0     1196 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/destination.py
+-rw-r--r--   0        0        0     1592 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/destination/file_system.py
+-rw-r--r--   0        0        0     5458 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/metadata.py
+-rw-r--r--   0        0        0     1221 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/odbc_utils.py
+-rw-r--r--   0        0        0     1851 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/query.py
+-rw-r--r--   0        0        0       38 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/reader/__init__.py
+-rw-r--r--   0        0        0     7295 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/reader/odbc_reader.py
+-rw-r--r--   0        0        0     1961 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/reader/reader.py
+-rw-r--r--   0        0        0     4932 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/reader/spark_reader.py
+-rw-r--r--   0        0        0     1976 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/sql_glot_utils.py
+-rw-r--r--   0        0        0     1211 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/sql_schema.py
+-rw-r--r--   0        0        0      249 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/utils.py
+-rw-r--r--   0        0        0     7829 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/write_init.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/write_utils/__init__.py
+-rw-r--r--   0        0        0     6810 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/odbc2deltalake/write_utils/restore_pk.py
+-rw-r--r--   0        0        0     1393 2024-04-23 12:52:12.360010 odbc2deltalake-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 odbc2deltalake-0.9.0/PKG-INFO
```

### Comparing `odbc2deltalake-0.8.9/LICENSE` & `odbc2deltalake-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/README.md` & `odbc2deltalake-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/__init__.py` & `odbc2deltalake-0.9.0/odbc2deltalake/__init__.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/db_to_delta.py` & `odbc2deltalake-0.9.0/odbc2deltalake/db_to_delta.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,15 +186,17 @@
                 do_full_load(
                     infos=infos,
                     mode="append",
                 )
             else:
                 do_delta_load(
                     infos=infos,
-                    simple=write_config.load_mode == "simple_delta",
+                    simple=write_config.load_mode in ["simple_delta", "simple_delta_check"],
+                    simple_check=write_config.load_mode == "simple_delta_check"
+
                 )
         lock_file_path.remove()
         _vacuum(
             source, destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION
         )
         _vacuum(source, destination / "delta_load" / DBDeltaPathConfigs.DELTA_1_NAME)
         _vacuum(source, destination / "delta_load" / DBDeltaPathConfigs.DELTA_2_NAME)
@@ -233,28 +235,36 @@
 
 def write_latest_pk(
     reader: DataSourceReader,
     destination: Destination,
     pks: Sequence[InformationSchemaColInfo],
     delta_col: InformationSchemaColInfo,
     write_config: WriteConfig,
+    merge_delta=False,
 ):
     reader.local_register_update_view(
         destination / f"delta_load/{DBDeltaPathConfigs.DELTA_1_NAME}",
         DBDeltaPathConfigs.DELTA_1_NAME,
     )
 
     reader.local_register_update_view(
         destination / f"delta_load/{DBDeltaPathConfigs.DELTA_2_NAME}",
         DBDeltaPathConfigs.DELTA_2_NAME,
     )
-    reader.local_register_update_view(
-        destination / f"delta_load/{DBDeltaPathConfigs.PRIMARY_KEYS_TS}",
-        DBDeltaPathConfigs.PRIMARY_KEYS_TS,
-    )
+    if not merge_delta:
+        reader.local_register_update_view(
+            destination / f"delta_load/{DBDeltaPathConfigs.PRIMARY_KEYS_TS}",
+            "primary_keys_ts_for_write",
+        )
+    else:
+        reader.local_register_update_view(
+            destination / f"delta_load/{DBDeltaPathConfigs.LATEST_PK_VERSION}",
+            "primary_keys_ts_for_write",
+            version=1,
+        )
 
     latest_pk_query = union(
         [
             ex.select(
                 *_get_cols_select(
                     cols=concat_seq(pks, [delta_col]),
                     table_alias="au",
@@ -294,15 +304,15 @@
                     *_get_cols_select(
                         cols=concat_seq(pks, [delta_col]),
                         table_alias="cpk",
                         system="target",
                         get_target_name=write_config.get_target_name,
                     )
                 )
-                .from_(ex.table_(DBDeltaPathConfigs.PRIMARY_KEYS_TS, alias="cpk"))
+                .from_(ex.table_("primary_keys_ts_for_write", alias="cpk"))
                 .join(
                     ex.table_("delta_2", alias="au3"),
                     ex.and_(
                         *[
                             ex.column(
                                 write_config.get_target_name(c), "cpk", quoted=True
                             ).eq(
@@ -341,22 +351,24 @@
         mode="overwrite",
     )
 
 
 def _temp_table(table: table_name_type):
     def _clean(input_str: str):
         return "".join(ch for ch in input_str if ch.isalnum())
+
     if isinstance(table, str):
         return "temp_" + _clean(table)
     return "temp_" + "_".join((_clean(s) for s in table))
 
 
 def do_delta_load(
     infos: WriteConfigAndInfos,
     simple=False,  # a simple delta load assumes that there are no deletes and no additional updates (eg, when soft-delete is implemented in source properly)
+    simple_check = False # does a simple load and checks if the source and target counts match. If not, do a normal delta load on top
 ):
     destination = infos.destination
     logger = infos.logger
     delta_col = infos.delta_col
     write_config = infos.write_config
     assert delta_col is not None, "Must have a delta_col for delta loads"
     reader = infos.source
@@ -404,57 +416,46 @@
             mode="append",
         )
         return
     logger.info(
         f"{table}: Start delta step 1, get primary keys and timestamps. MAX({delta_col.column_name}): {delta_load_value}"
     )
     if not simple:
-        _retrieve_primary_key_data(
-            reader=reader,
-            table=table,
-            delta_col=delta_col,
-            pk_cols=infos.pk_cols,
-            destination=destination,
-            write_config=write_config,
-            logger=infos.logger,
-        )
-
+        _retrieve_primary_key_data(infos=infos)
+    else:
+        source_count = reader.source_sql_to_py(
+            sg.from_(table_from_tuple(table)).select(
+                ex.Count(this=ex.Star()).as_("cnt")
+            )
+        )[0]["cnt"]
     criterion = _source_convert(
         delta_col.column_name,
         delta_col.data_type,
         table_alias="t",
         type_map=write_config.data_type_map,
     ) > ex.convert(delta_load_value)
     logger.info(f"{table}: Start delta step 2, load updates by timestamp")
     upds_sql = _get_update_sql(
         cols=infos.col_infos,
         criterion=criterion,
         table=table,
         write_config=write_config,
     )
-    logger.info("execute sql", load="delta", sub_load="delta_1", sql=upds_sql)
     _load_updates_to_delta(
         logger,
         reader,
         sql=upds_sql,
         delta_path=delta_path,
         delta_name="delta_1",
         write_config=write_config,
     )
     if not simple:
         assert old_pk_version is not None
         _handle_additional_updates(
-            logger,
-            reader=reader,
-            table=table,
-            delta_path=delta_path,
-            pk_cols=infos.pk_cols,
-            delta_col=delta_col,
-            cols=infos.col_infos,
-            write_config=write_config,
+            infos=infos,
             old_pk_version=old_pk_version,
         )
         reader.local_register_update_view(delta_path, _temp_table(table))
 
         logger.info(f"{table}: Start delta step 3.5, write meta for next delta load")
 
         write_latest_pk(
@@ -468,18 +469,40 @@
             cols=infos.col_infos,
             pk_cols=infos.pk_cols,
             old_pk_version=old_pk_version,
             write_config=infos.write_config,
         )
         logger.info(f"{table}: Done delta load")
     else:
-        if (destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION).exists():
-            (destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION).remove(
-                True
-            )
+        _write_delta2(infos, [], mode="overwrite")  # just to create the delta_2 table
+        pk_ts = destination / "delta_load" / DBDeltaPathConfigs.PRIMARY_KEYS_TS
+        if pk_ts.exists():
+            pk_ts.remove()
+        
+        write_latest_pk(
+            reader,
+            destination,
+            infos.pk_cols,
+            delta_col,
+            write_config=write_config,
+            merge_delta=True,
+        )
+        reader.local_register_update_view(
+            destination / "delta_load" / DBDeltaPathConfigs.LATEST_PK_VERSION,
+            DBDeltaPathConfigs.LATEST_PK_VERSION,
+        )
+        target_count = reader.local_execute_sql_to_py(
+            sg.from_(DBDeltaPathConfigs.LATEST_PK_VERSION).select(
+                ex.Count(this=ex.Star()).as_("cnt")
+            )
+        )[0]["cnt"]
+        if source_count != target_count:
+            logger.warning(f"Source and target count do not match. Source: {source_count}, Target: {target_count}. { 'Do a normal delta' if simple_check else ''}")
+            if simple_check:
+                do_delta_load(infos, simple=False)
 
 
 def do_append_inserts_load(infos: WriteConfigAndInfos):
     logger = infos.logger
     write_config = infos.write_config
     assert infos.delta_col is not None, "must have a delta col"
     logger.info(
@@ -634,38 +657,35 @@
             sg.from_("deletes_with_schema").select("*"),
             destination / "delta",
             mode="append",
         )
 
 
 def _retrieve_primary_key_data(
-    reader: DataSourceReader,
-    table: table_name_type,
-    delta_col: InformationSchemaColInfo,
-    pk_cols: Sequence[InformationSchemaColInfo],
-    destination: Destination,
-    write_config: WriteConfig,
-    logger: DeltaLogger,
+    infos: WriteConfigAndInfos,
 ):
+
     pk_ts_col_select = ex.select(
         *_get_cols_select(
             is_full=None,
             is_deleted=None,
-            cols=concat_seq(pk_cols, [delta_col]),
+            cols=concat_seq(
+                infos.pk_cols, [infos.delta_col] if infos.delta_col else []
+            ),
             with_valid_from=False,
-            data_type_map=write_config.data_type_map,
+            data_type_map=infos.write_config.data_type_map,
             system="source",
-            get_target_name=write_config.get_target_name,
+            get_target_name=infos.write_config.get_target_name,
         )
-    ).from_(table_from_tuple(table))
-    pk_ts_reader_sql = pk_ts_col_select.sql(write_config.dialect)
+    ).from_(table_from_tuple(infos.table))
+    pk_ts_reader_sql = pk_ts_col_select.sql(infos.write_config.dialect)
 
-    pk_path = destination / f"delta_load/{DBDeltaPathConfigs.PRIMARY_KEYS_TS}"
-    logger.info("Retrieve all PK/TS", sql=pk_ts_reader_sql)
-    reader.source_write_sql_to_delta(
+    pk_path = infos.destination / f"delta_load/{DBDeltaPathConfigs.PRIMARY_KEYS_TS}"
+    infos.logger.info("Retrieve all PK/TS", sql=pk_ts_reader_sql)
+    infos.source.source_write_sql_to_delta(
         sql=pk_ts_reader_sql, delta_path=pk_path, mode="overwrite"
     )
     return pk_path
 
 
 T = TypeVar("T")
 
@@ -677,27 +697,117 @@
         if len(chunk) >= chunk_size:
             yield chunk
             chunk = list()
     if len(chunk) > 0:
         yield chunk
 
 
+def _write_delta2(
+    infos: WriteConfigAndInfos, data: list[dict], mode: Literal["overwrite", "append"]
+):
+    write_config = infos.write_config
+    from .sql_schema import get_sql_type
+    from .query import sql_quote_value
+
+    def _collate(c: InformationSchemaColInfo):
+        if c.data_type.lower() in [
+            "char",
+            "varchar",
+            "nchar",
+            "nvarchar",
+            "text",
+            "ntext",
+        ]:
+            return "COLLATE Latin1_General_100_BIN "
+        return ""
+
+    delta_2_path = infos.destination / "delta_load" / DBDeltaPathConfigs.DELTA_2_NAME
+
+    def full_sql(js: str):
+        col_defs = ", ".join(
+            [
+                f"p{i} {get_sql_type(p.data_type, p.character_maximum_length)}"
+                for i, p in enumerate(infos.pk_cols)
+            ]
+        )
+
+        selects = list(
+            _get_cols_select(
+                infos.col_infos,
+                is_full=False,
+                is_deleted=False,
+                with_valid_from=True,
+                table_alias="t",
+                data_type_map=write_config.data_type_map,
+                system="source",
+                get_target_name=write_config.get_target_name,
+            )
+        )
+        sql = (
+            ex.select(*selects)
+            .from_(table_from_tuple(infos.table, alias="t"))
+            .sql(write_config.dialect)
+        )
+        pk_map = ", ".join(
+            [
+                "p" + str(i) + " as " + sql_quote_name(write_config.get_target_name(c))
+                for i, c in enumerate(infos.pk_cols)
+            ]
+        )
+        return f"""{sql}
+        inner join (SELECT {pk_map} FROM OPENJSON({sql_quote_value(js)}) with ({col_defs}) ) ttt
+             on {' AND '.join([f't.{sql_quote_name(c.column_name)} {_collate(c)} = ttt.{sql_quote_name(write_config.get_target_name(c))}' for c in infos.pk_cols])}
+        """
+
+    if mode == "overwrite":
+        infos.logger.info(
+            "execute sql",
+            load="delta",
+            sub_load="delta_additional",
+            sql=full_sql(f"[/* {len(data)} entries */]"),
+        )
+    sql = full_sql(json.dumps(data))
+    if (
+        len(sql) > 7000
+    ):  ## oops, spark will not like this (actually the limit is 8000, but spark might use something on it's own)
+        ch_split = len(data) // 2
+        chunk_1 = data[:ch_split]
+        chunk_2 = data[ch_split:]
+        infos.source.source_write_sql_to_delta(
+            full_sql(json.dumps(chunk_1)),
+            delta_2_path,
+            mode=mode,
+        )
+        infos.source.source_write_sql_to_delta(
+            full_sql(json.dumps(chunk_2)),
+            delta_2_path,
+            mode="append",
+        )
+    else:
+        infos.source.source_write_sql_to_delta(
+            sql,
+            delta_2_path,
+            mode=mode,
+        )
+
+
 def _handle_additional_updates(
-    logger: DeltaLogger,
-    reader: DataSourceReader,
-    table: table_name_type,
-    delta_path: Destination,
-    pk_cols: Sequence[InformationSchemaColInfo],
-    delta_col: InformationSchemaColInfo,
-    cols: Sequence[InformationSchemaColInfo],
-    write_config: WriteConfig,
+    infos: WriteConfigAndInfos,
     old_pk_version: int,
 ):
     """Handles updates that are not logical by their timestamp. This can happen on a restore from backup, for example."""
-    folder = delta_path.parent
+    folder = infos.destination
+    table = infos.table
+    delta_col = infos.delta_col
+    pk_cols = infos.pk_cols
+    cols = infos.col_infos
+    reader = infos.source
+    logger = infos.logger
+    write_config = infos.write_config
+    assert delta_col is not None, "Need a delta column"
     pk_ds_cols = concat_seq(pk_cols, [delta_col])
     reader.local_register_update_view(
         folder / f"delta_load/{ DBDeltaPathConfigs.PRIMARY_KEYS_TS}",
         DBDeltaPathConfigs.PRIMARY_KEYS_TS,
     )
     LAST_PK_VERSION = "LAST_PK_VERSION"
     reader.local_register_update_view(
@@ -747,86 +857,31 @@
         ).from_(table_from_tuple("delta_1", alias="d1")),
     )
     reader.local_register_view(sql_query, "real_additional_updates")
     update_count: int = reader.local_execute_sql_to_py(
         sg.from_("real_additional_updates").select(ex.Count(this=ex.Star()).as_("cnt"))
     )[0]["cnt"]
 
-    from .sql_schema import get_sql_type
-    from .query import sql_quote_value
-
     jsd = reader.local_execute_sql_to_py(
         sg.from_("real_additional_updates").select(
             *[
                 ex.column(write_config.get_target_name(c)).as_(
                     "p" + str(i), quoted=False
                 )
                 for i, c in enumerate(pk_cols)
             ]
         )
     )
 
-    def _collate(c: InformationSchemaColInfo):
-        if c.data_type.lower() in [
-            "char",
-            "varchar",
-            "nchar",
-            "nvarchar",
-            "text",
-            "ntext",
-        ]:
-            return "COLLATE Latin1_General_100_BIN "
-        return ""
-
-    delta_2_path = folder / "delta_load/delta_2"
-
-    def full_sql(js: str):
-        col_defs = ", ".join(
-            [
-                f"p{i} {get_sql_type(p.data_type, p.character_maximum_length)}"
-                for i, p in enumerate(pk_cols)
-            ]
-        )
-
-        selects = list(
-            _get_cols_select(
-                cols,
-                is_full=False,
-                is_deleted=False,
-                with_valid_from=True,
-                table_alias="t",
-                data_type_map=write_config.data_type_map,
-                system="source",
-                get_target_name=write_config.get_target_name,
-            )
-        )
-        sql = (
-            ex.select(*selects)
-            .from_(table_from_tuple(table, alias="t"))
-            .sql(write_config.dialect)
-        )
-        pk_map = ", ".join(
-            [
-                "p" + str(i) + " as " + sql_quote_name(write_config.get_target_name(c))
-                for i, c in enumerate(pk_cols)
-            ]
-        )
-        return f"""{sql}
-        inner join (SELECT {pk_map} FROM OPENJSON({sql_quote_value(js)}) with ({col_defs}) ) ttt
-             on {' AND '.join([f't.{sql_quote_name(c.column_name)} {_collate(c)} = ttt.{sql_quote_name(write_config.get_target_name(c))}' for c in pk_cols])}
-        """
-
     if update_count == 0:
-        reader.source_write_sql_to_delta(full_sql("[]"), delta_2_path, mode="overwrite")
+        _write_delta2(infos, [], mode="overwrite")
     elif (
         update_count > 1000
     ) or write_config.no_complex_entries_load:  # many updates. get the smallest timestamp and do "normal" delta, even if there are too many records then
-        reader.source_write_sql_to_delta(
-            full_sql("[]"), delta_2_path, mode="overwrite"
-        )  # still need to create delta_2_path
+        _write_delta2(infos, [], mode="overwrite")  # still need to create delta_2_path
         logger.warning(
             f"{table}: Start delta step 3, load {update_count} strange updates via normal delta load"
         )
         delta_load_value = reader.local_execute_sql_to_py(
             ex.select(
                 ex.func(
                     "MIN",
@@ -847,15 +902,15 @@
         logger.info(
             "execute sql", load="delta", sub_load="delta_1_additional", sql=upds_sql
         )
         _load_updates_to_delta(
             logger,
             reader,
             sql=upds_sql,
-            delta_path=delta_path,
+            delta_path=infos.destination / "delta",
             delta_name="delta_1",
             write_config=write_config,
         )
     else:
         # we don't want to overshoot 8000 chars here because of spark. we estimate how much space in json a record of pk's will take
 
         char_size_pks = sum(
@@ -871,50 +926,25 @@
             ]
         )
         batch_size = max(10, int(7000 / char_size_pks))
 
         logger.warning(
             f"{table}: Start delta step 3, load {update_count} strange updates via batches of size {batch_size}"
         )
-        logger.info(
-            "execute sql",
-            load="delta",
-            sub_load="delta_additional",
-            sql=full_sql("[]"),
-        )
         first = True
         for chunk in _list_to_chunks(jsd, batch_size):
-            sql = full_sql(json.dumps(chunk))
-            if (
-                len(sql) > 7000
-            ):  ## oops, spark will not like this (actually the limit is 8000, but spark might use something on it's own)
-                ch_split = len(chunk) // 2
-                chunk_1 = chunk[:ch_split]
-                chunk_2 = chunk[ch_split:]
-                reader.source_write_sql_to_delta(
-                    full_sql(json.dumps(chunk_1)),
-                    delta_2_path,
-                    mode="overwrite" if first else "append",
-                )
-                reader.source_write_sql_to_delta(
-                    full_sql(json.dumps(chunk_2)),
-                    delta_2_path,
-                    mode="append",
-                )
-            else:
-                reader.source_write_sql_to_delta(
-                    sql,
-                    delta_2_path,
-                    mode="overwrite" if first else "append",
-                )
+            _write_delta2(infos, chunk, mode="overwrite" if first else "append")
             first = False
-        reader.local_register_update_view(delta_2_path, "delta_2")
+        reader.local_register_update_view(
+            infos.destination / "delta_load" / DBDeltaPathConfigs.DELTA_2_NAME,
+            "delta_2",
+        )
         reader.local_execute_sql_to_delta(
             sg.from_("delta_2").select(ex.Star()),
-            delta_path,
+            infos.destination / "delta",
             mode="append",
         )
 
 
 def _get_update_sql(
     cols: Sequence[InformationSchemaColInfo],
     criterion: str | Sequence[str | ex.Expression] | ex.Expression | None,
```

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/delta_logger.py` & `odbc2deltalake-0.9.0/odbc2deltalake/delta_logger.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/destination/azure.py` & `odbc2deltalake-0.9.0/odbc2deltalake/destination/azure.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/destination/azure_utils.py` & `odbc2deltalake-0.9.0/odbc2deltalake/destination/azure_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/destination/databricks.py` & `odbc2deltalake-0.9.0/odbc2deltalake/destination/databricks.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/destination/destination.py` & `odbc2deltalake-0.9.0/odbc2deltalake/destination/destination.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/destination/file_system.py` & `odbc2deltalake-0.9.0/odbc2deltalake/destination/file_system.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/metadata.py` & `odbc2deltalake-0.9.0/odbc2deltalake/metadata.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/odbc_utils.py` & `odbc2deltalake-0.9.0/odbc2deltalake/odbc_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/query.py` & `odbc2deltalake-0.9.0/odbc2deltalake/query.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/reader/odbc_reader.py` & `odbc2deltalake-0.9.0/odbc2deltalake/reader/odbc_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/reader/reader.py` & `odbc2deltalake-0.9.0/odbc2deltalake/reader/reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/reader/spark_reader.py` & `odbc2deltalake-0.9.0/odbc2deltalake/reader/spark_reader.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/sql_glot_utils.py` & `odbc2deltalake-0.9.0/odbc2deltalake/sql_glot_utils.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/sql_schema.py` & `odbc2deltalake-0.9.0/odbc2deltalake/sql_schema.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/write_init.py` & `odbc2deltalake-0.9.0/odbc2deltalake/write_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,19 +82,25 @@
     primary_keys: list[str] | None = None
     """A list of primary keys to use for the delta load. If None, the primary keys will be determined from the source"""
 
     delta_col: str | None = None
     """The column to use for the delta load. If None, the column will be determined from the source. Should be mostly increasing to make load efficient"""
 
     load_mode: Literal[
-        "overwrite", "append", "force_full", "append_inserts", "simple_delta"
+        "overwrite",
+        "append",
+        "force_full",
+        "append_inserts",
+        "simple_delta",
+        "simple_delta_check",
     ] = "append"
     """The load mode to use. Attention: overwrite will not help you build scd2, the history is in the delta table only
         append_inserts is for when you have a delta column which is strictly increasing and you want to append new rows only. No deletes of rows. might be good for logs
         simple_delta is for sources where the delta col is a datetime and you can be sure that there are no deletes or additional updates
+        simple_delta_check is like simple_delta, but checks for deletes if the count does not match. Only use if you do not expect frequent deletes, as it will do simple_delta AND delta if there are deletes, which is slower than delta
     """
 
     data_type_map: Mapping[str, ex.DATA_TYPE] = dataclasses.field(
         default_factory=lambda: _default_type_map.copy()
     )
     """Set this if you want to map stuff like decimal to double before writing to delta. We recommend doing so later in ETL usually"""
```

### Comparing `odbc2deltalake-0.8.9/odbc2deltalake/write_utils/restore_pk.py` & `odbc2deltalake-0.9.0/odbc2deltalake/write_utils/restore_pk.py`

 * *Files identical despite different names*

### Comparing `odbc2deltalake-0.8.9/pyproject.toml` & `odbc2deltalake-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odbc2deltalake"
-version = "0.8.9"
+version = "0.9.0"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -12,15 +12,15 @@
 pyodbc = { version = "^5.1.0", optional = true }
 deltalake2db = { version = ">=0.3.0", optional = true }
 arrow-odbc = { version = "^5.0.0", optional = true }
 deltalake = { version = ">=0.16.1", optional = true }
 duckdb = { version = ">=0.10.1", optional = true }
 azure-identity = { version = "^1.15.0", optional = true }
 adlfs = { version = "^2024.2.0", optional = true }
-sqlglot = "^23.0.5"
+sqlglot = ">=23.0.5"
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.352"
 black = "^24.2.0"
```

### Comparing `odbc2deltalake-0.8.9/PKG-INFO` & `odbc2deltalake-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odbc2deltalake
-Version: 0.8.9
+Version: 0.9.0
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 Requires-Dist: arrow-odbc (>=5.0.0,<6.0.0) ; extra == "local"
 Requires-Dist: azure-identity (>=1.15.0,<2.0.0) ; extra == "local-azure"
 Requires-Dist: deltalake (>=0.16.1) ; extra == "local"
 Requires-Dist: deltalake2db (>=0.3.0) ; extra == "local"
 Requires-Dist: duckdb (>=0.10.1) ; extra == "local"
 Requires-Dist: pydantic (>=1.10.0)
 Requires-Dist: pyodbc (>=5.1.0,<6.0.0) ; extra == "local"
-Requires-Dist: sqlglot (>=23.0.5,<24.0.0)
+Requires-Dist: sqlglot (>=23.0.5)
 Description-Content-Type: text/markdown
 
 # ODBC 2 Deltalake
 
 This is a package that supports reading from ODBC and writing to a scd2 DeltaTable. The delta table will always have the following "system" cols:
 
 - \_\_timestamp : The Date of the Load
```

