# Comparing `tmp/fbgemm_gpu_nightly_cpu-2024.4.22-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2024.4.23-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,60 +1,60 @@
-Zip file size: 3105489 bytes, number of entries: 58
--rw-r--r--  2.0 unx      914 b- defN 24-Apr-22 12:57 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx     3079 b- defN 24-Apr-22 12:57 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      789 b- defN 24-Apr-22 12:57 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10703352 b- defN 24-Apr-22 12:57 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5663 b- defN 24-Apr-22 12:57 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2362 b- defN 24-Apr-22 12:57 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2752 b- defN 24-Apr-22 12:57 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7885 b- defN 24-Apr-22 12:57 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4143 b- defN 24-Apr-22 12:57 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     6947 b- defN 24-Apr-22 12:57 fbgemm_gpu/runtime_monitor.py
--rw-r--r--  2.0 unx    20486 b- defN 24-Apr-22 12:57 fbgemm_gpu/sparse_ops.py
--rw-r--r--  2.0 unx     5774 b- defN 24-Apr-22 12:57 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     7058 b- defN 24-Apr-22 12:57 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      540 b- defN 24-Apr-22 12:57 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    26853 b- defN 24-Apr-22 12:57 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2339 b- defN 24-Apr-22 12:57 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3493 b- defN 24-Apr-22 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    66800 b- defN 24-Apr-22 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    98158 b- defN 24-Apr-22 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    40680 b- defN 24-Apr-22 12:57 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      925 b- defN 24-Apr-22 12:57 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx      383 b- defN 24-Apr-22 12:57 fbgemm_gpu/docs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 24-Apr-22 12:57 fbgemm_gpu/docs/common.py
--rw-r--r--  2.0 unx     2377 b- defN 24-Apr-22 12:57 fbgemm_gpu/docs/examples.py
--rw-r--r--  2.0 unx     7381 b- defN 24-Apr-22 12:57 fbgemm_gpu/docs/jagged_tensor_ops.py
--rw-r--r--  2.0 unx     7708 b- defN 24-Apr-22 12:57 fbgemm_gpu/docs/table_batched_embedding_ops.py
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-22 12:57 fbgemm_gpu/docs/version.py
--rw-r--r--  2.0 unx      854 b- defN 24-Apr-22 12:52 fbgemm_gpu/experimental/example/__init__.py
--rwxr-xr-x  2.0 unx    30688 b- defN 24-Apr-22 12:57 fbgemm_gpu/experimental/example/fbgemm_gpu_experimental_example_py.so
--rw-r--r--  2.0 unx      381 b- defN 24-Apr-22 12:52 fbgemm_gpu/experimental/example/utils.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4180 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4180 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
--rw-r--r--  2.0 unx     2147 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
--rw-r--r--  2.0 unx     3144 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     3144 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
--rw-r--r--  2.0 unx     2420 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2420 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
--rw-r--r--  2.0 unx     4512 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     4512 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
--rw-r--r--  2.0 unx     3964 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3964 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
--rw-r--r--  2.0 unx     3762 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     3762 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
--rw-r--r--  2.0 unx      649 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6162 b- defN 24-Apr-22 12:56 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx     2602 b- defN 24-Apr-22 12:58 fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-Apr-22 12:58 fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-22 12:57 fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6344 b- defN 24-Apr-22 12:58 fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/RECORD
-58 files, 11150731 bytes uncompressed, 3094869 bytes compressed:  72.2%
+Zip file size: 3105484 bytes, number of entries: 58
+-rw-r--r--  2.0 unx      914 b- defN 24-Apr-23 12:59 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx     3079 b- defN 24-Apr-23 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      789 b- defN 24-Apr-23 12:59 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10703352 b- defN 24-Apr-23 12:59 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5663 b- defN 24-Apr-23 12:59 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-Apr-23 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-Apr-23 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-Apr-23 12:59 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4143 b- defN 24-Apr-23 12:59 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     6947 b- defN 24-Apr-23 12:59 fbgemm_gpu/runtime_monitor.py
+-rw-r--r--  2.0 unx    20486 b- defN 24-Apr-23 12:59 fbgemm_gpu/sparse_ops.py
+-rw-r--r--  2.0 unx     5774 b- defN 24-Apr-23 12:59 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     7058 b- defN 24-Apr-23 12:59 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      540 b- defN 24-Apr-23 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    26853 b- defN 24-Apr-23 12:59 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-Apr-23 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-Apr-23 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    66800 b- defN 24-Apr-23 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    98158 b- defN 24-Apr-23 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    40680 b- defN 24-Apr-23 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      925 b- defN 24-Apr-23 12:59 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx      383 b- defN 24-Apr-23 12:59 fbgemm_gpu/docs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 24-Apr-23 12:59 fbgemm_gpu/docs/common.py
+-rw-r--r--  2.0 unx     2377 b- defN 24-Apr-23 12:59 fbgemm_gpu/docs/examples.py
+-rw-r--r--  2.0 unx     7381 b- defN 24-Apr-23 12:59 fbgemm_gpu/docs/jagged_tensor_ops.py
+-rw-r--r--  2.0 unx     7708 b- defN 24-Apr-23 12:59 fbgemm_gpu/docs/table_batched_embedding_ops.py
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-23 12:59 fbgemm_gpu/docs/version.py
+-rw-r--r--  2.0 unx      854 b- defN 24-Apr-23 12:54 fbgemm_gpu/experimental/example/__init__.py
+-rwxr-xr-x  2.0 unx    30688 b- defN 24-Apr-23 12:59 fbgemm_gpu/experimental/example/fbgemm_gpu_experimental_example_py.so
+-rw-r--r--  2.0 unx      381 b- defN 24-Apr-23 12:54 fbgemm_gpu/experimental/example/utils.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
+-rw-r--r--  2.0 unx     2147 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
+-rw-r--r--  2.0 unx      649 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6162 b- defN 24-Apr-23 12:57 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     2602 b- defN 24-Apr-23 12:59 fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 24-Apr-23 12:59 fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-23 12:59 fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6344 b- defN 24-Apr-23 12:59 fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/RECORD
+58 files, 11150731 bytes uncompressed, 3094864 bytes compressed:  72.2%
```

## zipnote {}

```diff
@@ -156,20 +156,20 @@
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -1611041,15 +1611041,15 @@
 	call   *%rax
 	test   %al,%al
 	je     8a84dc <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xb0c>
 	call   1b4dd0 <at::detail::getCUDAHooks()@plt>
 	movb   $0x0,-0x634(%rbp)
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0xf0(%rax),%rax
+	mov    0xf8(%rax),%rax
 	cmp    0x1865de(%rip),%rax        
 	je     8a7de1 <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x411>
 	jmp    8a852a <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xb5a>
 	nopl   (%rax)
 	call   *%rax
 	test   %al,%al
 	je     8a84bf <int_nbit_split_embedding_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xaef>
@@ -1612987,15 +1612987,15 @@
 	call   *%rax
 	test   %al,%al
 	je     8aac54 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xad4>
 	call   1b4dd0 <at::detail::getCUDAHooks()@plt>
 	movb   $0x0,-0x6d0(%rbp)
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0xf0(%rax),%rax
+	mov    0xf8(%rax),%rax
 	cmp    0x183eae(%rip),%rax        
 	je     8aa583 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0x403>
 	jmp    8aaca2 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xb22>
 	nopl   (%rax)
 	call   *%rax
 	test   %al,%al
 	je     8aac37 <int_nbit_split_embedding_nobag_codegen_forward_unweighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, long, long, long)@@Base+0xab7>
@@ -1627827,15 +1627827,15 @@
 	call   *%rax
 	test   %al,%al
 	je     8bbd64 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x1d84>
 	call   1b4dd0 <at::detail::getCUDAHooks()@plt>
 	movb   $0x0,-0x220(%rbp)
 	mov    %rax,%rdi
 	mov    (%rax),%rax
-	mov    0xf0(%rax),%rax
+	mov    0xf8(%rax),%rax
 	cmp    0x172e2e(%rip),%rax        
 	je     8bb21b <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x123b>
 	jmp    8bbdb2 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x1dd2>
 	nopl   (%rax)
 	call   *%rax
 	test   %al,%al
 	je     8bbd47 <int_nbit_split_embedding_codegen_forward_weighted_cpu(at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor, long, at::Tensor, at::Tensor, long, long, at::Tensor, long, long, long)@@Base+0x1d67>
```

## fbgemm_gpu/docs/version.py

```diff
@@ -2,8 +2,8 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-__version__: str = "2024.4.22"
+__version__: str = "2024.4.23"
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2024.4.22
+Version: 2024.4.23
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 fbgemm_gpu/__init__.py,sha256=ZPy0iaSSHb6-eT6lz8MSpr-5Ircj9SLmVpL0o0ejcNQ,914
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=dpxZAueNsadJVuK7Dwo8GbOlho9r67Lfh8kesqRKJNI,3079
 fbgemm_gpu/enums.py,sha256=GVuzF5cFTLzttkvlH1SdcGrxrppMhDSbQj_Vm_4zmEo,789
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=j7aBg-QNPNrJCoIh2x9L-Ich6FtcOMAnIFsBJRgbOis,10703352
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=u6ZX73IGbEtWzUhB2vpTdtOxpZcPg5Nyddc-i5fTjpA,10703352
 fbgemm_gpu/metrics.py,sha256=TsurFLJf0nJvPDN7urWb4LMQlf5RgdWPTTTDO7S4wtI,5663
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=4mHJ2fo3SeG25iSwdm2YsM8q_oWsF1LxRguYmxSnuDI,2362
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=cUrEbRIvLFW_3Zmh07QkN4S1Cfvvge6TYO1VXBFCpz8,2752
 fbgemm_gpu/quantize_comm.py,sha256=UZcVSC2JQ0oSkwsJQnjaZ2k8mm2p3hvVzpyg7X5xFXM,7885
 fbgemm_gpu/quantize_utils.py,sha256=-vwHIEkyStDo1TWoYfwmC5U6DvR6iRMHXyjFc9lO_p8,4143
 fbgemm_gpu/runtime_monitor.py,sha256=tIdxkJIWkJ8705btxs9NqzEXC7QprFh3sA8Q4LpvtJ8,6947
 fbgemm_gpu/sparse_ops.py,sha256=_yq67rG4sabvW5maMiM5IAucMhMWFXM99ABU7es2cm4,20486
@@ -20,15 +20,15 @@
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=S6qWfFzpqNIB8l9N3LAsYfaXSExg53f_b3fl47d1b1U,40680
 fbgemm_gpu/uvm.py,sha256=-cZunsuvnAKUEQptIwdYVar_3hUE99FbQUsyfBVeXPE,925
 fbgemm_gpu/docs/__init__.py,sha256=BbAfYbNZsBhO7L5Am4wyBLet4mTY2aXFucyGTxF9IlI,383
 fbgemm_gpu/docs/common.py,sha256=8ipXTwVb222X-aZ71O6n8fhxHCHPNhJEHMFiO7epcIs,273
 fbgemm_gpu/docs/examples.py,sha256=ZMN_6sL74LH_hrp2bF_hmg8gi29GhcgvwV3kCMjxkoE,2377
 fbgemm_gpu/docs/jagged_tensor_ops.py,sha256=Bsx-ZxvvdMv5CaldSvuw9GPR-HRcLbRR2IEXCOCm9r0,7381
 fbgemm_gpu/docs/table_batched_embedding_ops.py,sha256=h_EQOIMsdVlr-Pygul-fDGxx7JqLRjaBMI_z0PFrGAE,7708
-fbgemm_gpu/docs/version.py,sha256=bX2KXbQgM9nBzyBG3Hxyr7f5rL8hyqi7__uY_wXz5NQ,264
+fbgemm_gpu/docs/version.py,sha256=8rttvYSWTTFYK4wpPJkgUpKRIYi213VwisFiOwj8j4s,264
 fbgemm_gpu/experimental/example/__init__.py,sha256=6lrjWGUE06YBb5He6CHn60zDq8QAgRPSfTohfJ6jms0,854
 fbgemm_gpu/experimental/example/fbgemm_gpu_experimental_example_py.so,sha256=_KcQE1a9Wc3bEtK4MS2iwbQ0aMUOb5dttu6Z_UlCYyo,30688
 fbgemm_gpu/experimental/example/utils.py,sha256=nj4R0e58k3RR-XwMBowveLfC_sSYYYmocrJ2Wuf67uM,381
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=lfob_IDNeAs2FjS2WCldKlw0gm_qUZdp043fngI8sGE,1466
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
@@ -48,11 +48,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py,sha256=Aljkdf4GB0zetL2j5YIhTZaOqiIMIlQ9iTDM421lbiM,4512
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=yiD3_bG5yT5VXLoGw4eeRKQ2Nj087DRq0qKCVPb52SY,649
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=OFw5PM2YDiKvr6T9ZW7BKiq58gB7txcKfuJkBUROxdI,6162
-fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/METADATA,sha256=-k6LiBl0S_Npj4hKM5QwUZZFLTkl0RU4WAf0WDJByo8,2602
-fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
-fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2024.4.22.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/METADATA,sha256=zPWkRBmkEipQVbzlK_VjGcqqcOw46v5bFY8nLMFisN8,2602
+fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
+fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2024.4.23.dist-info/RECORD,,
```

