# Comparing `tmp/streamsync-0.5.0rc1.tar.gz` & `tmp/streamsync-0.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamsync-0.5.0rc1.tar", max compression
+gzip compressed data, was "streamsync-0.5.0rc2.tar", max compression
```

## Comparing `streamsync-0.5.0rc1.tar` & `streamsync-0.5.0rc2.tar`

### file list

```diff
@@ -1,128 +1,144 @@
--rw-r--r--   0        0        0    11323 2024-04-23 13:12:22.240741 streamsync-0.5.0rc1/LICENSE.txt
--rw-r--r--   0        0        0     3981 2024-04-23 13:12:22.240741 streamsync-0.5.0rc1/README.md
--rw-r--r--   0        0        0     2196 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2637 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/__init__.py
--rw-r--r--   0        0        0    29942 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/app_runner.py
--rw-r--r--   0        0        0     4426 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/command_line.py
--rw-r--r--   0        0        0    48728 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/core.py
--rw-r--r--   0        0        0    10268 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/core_ui.py
--rw-r--r--   0        0        0       30 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/mypy.ini
--rw-r--r--   0        0        0        0 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/py.typed
--rw-r--r--   0        0        0    17872 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/serve.py
--rw-r--r--   0        0        0     3587 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/ss_types.py
--rw-r--r--   0        0        0     8966 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/Arrow.dom-C52_vrWm.js
--rw-r--r--   0        0        0  3287258 2024-04-23 13:14:35.556069 streamsync-0.5.0rc1/src/streamsync/static/assets/BuilderApp-Co-xyrd-.js
--rw-r--r--   0        0        0   283124 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/BuilderApp-Fzhw8njh.css
--rw-r--r--   0        0        0    14964 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/ComponentRenderer-DCaUmBUC.css
--rw-r--r--   0        0        0     7749 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/ComponentRenderer-DR8XBO3z.js
--rw-r--r--   0        0        0    98868 2024-04-23 13:14:35.228071 streamsync-0.5.0rc1/src/streamsync/static/assets/Inter-Regular-CKDp9E3C.woff2
--rw-r--r--   0        0        0   309828 2024-04-23 13:14:35.228071 streamsync-0.5.0rc1/src/streamsync/static/assets/Inter-Regular-CKX1N0ak.ttf
--rw-r--r--   0        0        0    14409 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/abap-D8nrxEjS.js
--rw-r--r--   0        0        0     4198 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/apex-BrXDlLUW.js
--rw-r--r--   0        0        0     1094 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/azcli-CElzELwZ.js
--rw-r--r--   0        0        0     2091 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/bat-CUsyEhik.js
--rw-r--r--   0        0        0     2782 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/bicep-BtxyJn6H.js
--rw-r--r--   0        0        0     2431 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/cameligo-ClBCoF8h.js
--rw-r--r--   0        0        0     9889 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/clojure-B9TqLHAk.js
--rw-r--r--   0        0        0    79568 2024-04-23 13:14:35.228071 streamsync-0.5.0rc1/src/streamsync/static/assets/codicon-BA2IlpFX.ttf
--rw-r--r--   0        0        0     3836 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/coffee-DYsfeylR.js
--rw-r--r--   0        0        0     5680 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/cpp-VVGvvgir.js
--rw-r--r--   0        0        0     4770 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/csharp-Z6z2stHy.js
--rw-r--r--   0        0        0     1665 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/csp-DgZoLDI1.js
--rw-r--r--   0        0        0     4756 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/css-KqQ96-gC.js
--rw-r--r--   0        0        0   984347 2024-04-23 13:14:35.512069 streamsync-0.5.0rc1/src/streamsync/static/assets/css.worker-DvNUQFd1.js
--rw-r--r--   0        0        0    33713 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/cssMode-DtVHD6mi.js
--rw-r--r--   0        0        0     3631 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/cypher-CYoSlgTu.js
--rw-r--r--   0        0        0     4496 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/dart-BGDl7St1.js
--rw-r--r--   0        0        0     2115 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/dockerfile-CuCtxA7T.js
--rw-r--r--   0        0        0     5588 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/ecl-BCTFAUpS.js
--rw-r--r--   0        0        0   210242 2024-04-23 13:14:35.480069 streamsync-0.5.0rc1/src/streamsync/static/assets/editor.worker-BVwmgLrR.js
--rw-r--r--   0        0        0    10503 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/elixir-C7hRTYZ9.js
--rw-r--r--   0        0        0     2056 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/flow9-Bi_qi707.js
--rw-r--r--   0        0        0    16478 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/freemarker2-DUEoEr62.js
--rw-r--r--   0        0        0     3229 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/fsharp-CxaaEKKi.js
--rw-r--r--   0        0        0     2903 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/go-DUImKuGY.js
--rw-r--r--   0        0        0     2506 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/graphql-D5sGVkLV.js
--rw-r--r--   0        0        0     7156 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/handlebars-IQKTbmUg.js
--rw-r--r--   0        0        0     3836 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/hcl-zD_CCkZ1.js
--rw-r--r--   0        0        0     5396 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/html-ByZsrVkz.js
--rw-r--r--   0        0        0   648041 2024-04-23 13:14:35.508069 streamsync-0.5.0rc1/src/streamsync/static/assets/html.worker-BJMlcbMU.js
--rw-r--r--   0        0        0    34264 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/htmlMode-x26Bv8eO.js
--rw-r--r--   0        0        0   309095 2024-04-23 13:14:35.472070 streamsync-0.5.0rc1/src/streamsync/static/assets/index-CK0qFcoM.js
--rw-r--r--   0        0        0  1798721 2024-04-23 13:14:35.528069 streamsync-0.5.0rc1/src/streamsync/static/assets/index-DJ0okGb-.js
--rw-r--r--   0        0        0     5725 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/index-DMFOqlrb.js
--rw-r--r--   0        0        0   201777 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/index-DaNZqg5r.js
--rw-r--r--   0        0        0   358136 2024-04-23 13:14:35.228071 streamsync-0.5.0rc1/src/streamsync/static/assets/index-Kfy6W749.css
--rw-r--r--   0        0        0     1347 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/ini-8kKHd4ZL.js
--rw-r--r--   0        0        0     3467 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/java-De1axCfe.js
--rw-r--r--   0        0        0     1292 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/javascript-TK_dEQGI.js
--rw-r--r--   0        0        0   339023 2024-04-23 13:14:35.484069 streamsync-0.5.0rc1/src/streamsync/static/assets/json.worker-BwvX8PuZ.js
--rw-r--r--   0        0        0    39790 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/jsonMode-CcIaVIWF.js
--rw-r--r--   0        0        0     7395 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/julia-D3ApGBxz.js
--rw-r--r--   0        0        0     3685 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/kotlin-GbSrCElU.js
--rw-r--r--   0        0        0     4144 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/less-DNUaDNdz.js
--rw-r--r--   0        0        0     2683 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/lexon-Bg9QKxBu.js
--rw-r--r--   0        0        0     4342 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/liquid-CWE4cS-c.js
--rw-r--r--   0        0        0     2369 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/lua-Crkvc3mc.js
--rw-r--r--   0        0        0     3063 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/m3-DsrzVyM1.js
--rw-r--r--   0        0        0  1289773 2024-04-23 13:14:35.520069 streamsync-0.5.0rc1/src/streamsync/static/assets/mapbox-gl-BgoVqks1.js
--rw-r--r--   0        0        0     4034 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/markdown-CY5IOZuu.js
--rw-r--r--   0        0        0    35703 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/marked.esm-273vDTCT.js
--rw-r--r--   0        0        0     5247 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/mdx-BCqw-Sgx.js
--rw-r--r--   0        0        0     2825 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/mips-BE8RsGBA.js
--rw-r--r--   0        0        0     5158 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/msdax-N5ajIiFQ.js
--rw-r--r--   0        0        0    11520 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/mysql-DRxbB97D.js
--rw-r--r--   0        0        0     2648 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/objective-c-BHUZy23s.js
--rw-r--r--   0        0        0     3241 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/pascal-BemVzBTY.js
--rw-r--r--   0        0        0     2246 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/pascaligo-BACCcnx_.js
--rw-r--r--   0        0        0     8501 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/perl-CuU66Ptk.js
--rw-r--r--   0        0        0    13710 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/pgsql-CQ6TMH2r.js
--rw-r--r--   0        0        0     8273 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/php-BvyzZa65.js
--rw-r--r--   0        0        0     1929 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/pla-DrIuu9u1.js
--rw-r--r--   0        0        0  3704067 2024-04-23 13:14:35.564069 streamsync-0.5.0rc1/src/streamsync/static/assets/plotly.min-ETB9zM8E.js
--rw-r--r--   0        0        0     8102 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/postiats-BR_hrfni.js
--rw-r--r--   0        0        0    17185 2024-04-23 13:14:35.460070 streamsync-0.5.0rc1/src/streamsync/static/assets/powerquery-CKDUeRmd.js
--rw-r--r--   0        0        0     3515 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/powershell-Dsa4rhA_.js
--rw-r--r--   0        0        0     9292 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/protobuf-CGsvhooB.js
--rw-r--r--   0        0        0     5074 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/pug-D2p3uOX2.js
--rw-r--r--   0        0        0     4006 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/python-DeglcX7v.js
--rw-r--r--   0        0        0     3181 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/qsharp-B7F3HtPF.js
--rw-r--r--   0        0        0     3377 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/r-3aLoi2fs.js
--rw-r--r--   0        0        0     9160 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/razor-C0ubHCZJ.js
--rw-r--r--   0        0        0     3802 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/redis-jqFeRM5s.js
--rw-r--r--   0        0        0    12046 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/redshift-BriwQgXR.js
--rw-r--r--   0        0        0   163200 2024-04-23 13:14:35.228071 streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-BVOYbT3K.woff2
--rw-r--r--   0        0        0   525572 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-D9ZyeRwQ.ttf
--rw-r--r--   0        0        0   525744 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-DUK49BtM.eot
--rw-r--r--   0        0        0   224116 2024-04-23 13:14:35.228071 streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-DfzPQSMi.woff
--rw-r--r--   0        0        0  2460531 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-ncU_JTfY.svg
--rw-r--r--   0        0        0     4139 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/restructuredtext-hbBFZ0w9.js
--rw-r--r--   0        0        0     8750 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/ruby-ByThyB2Q.js
--rw-r--r--   0        0        0     4406 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/rust-DIEZMp5R.js
--rw-r--r--   0        0        0     2075 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/sb-C6Gjjw_x.js
--rw-r--r--   0        0        0     7564 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/scala-DZNw3jJB.js
--rw-r--r--   0        0        0     2013 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/scheme-55eqh71t.js
--rw-r--r--   0        0        0     6655 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/scss-D-OVkc4F.js
--rw-r--r--   0        0        0   202255 2024-04-23 13:14:35.464070 streamsync-0.5.0rc1/src/streamsync/static/assets/serialization-DDqLB4lR.js
--rw-r--r--   0        0        0     3319 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/shell-DSpi8_qN.js
--rw-r--r--   0        0        0    18843 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/solidity-BHddiNFS.js
--rw-r--r--   0        0        0     3010 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/sophia-D6taVZFb.js
--rw-r--r--   0        0        0     2798 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/sparql-LA0C7mUc.js
--rw-r--r--   0        0        0    10543 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/sql-C3-3IcFM.js
--rw-r--r--   0        0        0     7645 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/st-C4g7059C.js
--rw-r--r--   0        0        0     5417 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/swift-DNI1vH3h.js
--rw-r--r--   0        0        0     7849 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/systemverilog-DL_FVbcQ.js
--rw-r--r--   0        0        0     3817 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/tcl-DVJXmIwd.js
--rw-r--r--   0        0        0  4847810 2024-04-23 13:14:35.568069 streamsync-0.5.0rc1/src/streamsync/static/assets/ts.worker-CwG1rUES.js
--rw-r--r--   0        0        0    22645 2024-04-23 13:14:35.472070 streamsync-0.5.0rc1/src/streamsync/static/assets/tsMode-nAaFVZJ4.js
--rw-r--r--   0        0        0     6219 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/twig-BVWDLtw5.js
--rw-r--r--   0        0        0     5789 2024-04-23 13:14:35.232071 streamsync-0.5.0rc1/src/streamsync/static/assets/typescript-B1RkFep_.js
--rw-r--r--   0        0        0     6037 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/vb-Btz91-7U.js
--rw-r--r--   0        0        0   839306 2024-04-23 13:14:35.496070 streamsync-0.5.0rc1/src/streamsync/static/assets/vega-embed.module-3YlK5-kl.js
--rw-r--r--   0        0        0     7592 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/wgsl-D8V_buCG.js
--rw-r--r--   0        0        0     2790 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/xml-CDaxQGEH.js
--rw-r--r--   0        0        0     4397 2024-04-23 13:14:35.236071 streamsync-0.5.0rc1/src/streamsync/static/assets/yaml-CYFjN4Gg.js
--rw-r--r--   0        0        0     3780 2024-04-23 13:14:32.404085 streamsync-0.5.0rc1/src/streamsync/static/favicon.png
--rw-r--r--   0        0        0     1864 2024-04-23 13:14:35.488069 streamsync-0.5.0rc1/src/streamsync/static/index.html
--rw-r--r--   0        0        0     7748 2024-04-23 13:12:22.356740 streamsync-0.5.0rc1/src/streamsync/ui_manager.py
--rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 streamsync-0.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11323 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/LICENSE.txt
+-rw-r--r--   0        0        0     3981 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/README.md
+-rw-r--r--   0        0        0     2267 2024-04-23 14:51:41.684885 streamsync-0.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2637 2024-04-23 14:51:41.684885 streamsync-0.5.0rc2/src/streamsync/__init__.py
+-rw-r--r--   0        0        0    29942 2024-04-23 14:51:41.684885 streamsync-0.5.0rc2/src/streamsync/app_runner.py
+-rw-r--r--   0        0        0     1034 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/default/main.py
+-rw-r--r--   0        0        0      416 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/default/static/README.md
+-rw-r--r--   0        0        0     3780 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/default/static/favicon.png
+-rw-r--r--   0        0        0     4848 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/default/ui.json
+-rw-r--r--   0        0        0      482 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/Dockerfile
+-rw-r--r--   0        0        0     1250 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/assets/main_df.csv
+-rw-r--r--   0        0        0     2818 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/assets/story.txt
+-rw-r--r--   0        0        0     7818 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/main.py
+-rw-r--r--   0        0        0        0 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/requirements.txt
+-rw-r--r--   0        0        0      628 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/static/README.md
+-rw-r--r--   0        0        0     3780 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/static/favicon.png
+-rw-r--r--   0        0        0   249778 2024-04-23 14:51:41.572884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/static/neon_feathers.pdf
+-rw-r--r--   0        0        0   179279 2024-04-23 14:51:41.576884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/static/pigeon1.jpg
+-rw-r--r--   0        0        0     1494 2024-04-23 14:51:41.576884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/test_app.py
+-rw-r--r--   0        0        0    44329 2024-04-23 14:51:41.576884 streamsync-0.5.0rc2/src/streamsync/app_templates/hello/ui.json
+-rw-r--r--   0        0        0     4426 2024-04-23 14:51:41.684885 streamsync-0.5.0rc2/src/streamsync/command_line.py
+-rw-r--r--   0        0        0    48728 2024-04-23 14:51:41.684885 streamsync-0.5.0rc2/src/streamsync/core.py
+-rw-r--r--   0        0        0    10268 2024-04-23 14:51:41.688886 streamsync-0.5.0rc2/src/streamsync/core_ui.py
+-rw-r--r--   0        0        0       30 2024-04-23 14:51:41.688886 streamsync-0.5.0rc2/src/streamsync/mypy.ini
+-rw-r--r--   0        0        0        0 2024-04-23 14:51:41.688886 streamsync-0.5.0rc2/src/streamsync/py.typed
+-rw-r--r--   0        0        0    17872 2024-04-23 14:51:41.688886 streamsync-0.5.0rc2/src/streamsync/serve.py
+-rw-r--r--   0        0        0     3587 2024-04-23 14:51:41.688886 streamsync-0.5.0rc2/src/streamsync/ss_types.py
+-rw-r--r--   0        0        0     8966 2024-04-23 14:53:51.574686 streamsync-0.5.0rc2/src/streamsync/static/assets/Arrow.dom-C52_vrWm.js
+-rw-r--r--   0        0        0  3287258 2024-04-23 14:53:51.582687 streamsync-0.5.0rc2/src/streamsync/static/assets/BuilderApp-Co-xyrd-.js
+-rw-r--r--   0        0        0   283124 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/BuilderApp-Fzhw8njh.css
+-rw-r--r--   0        0        0    14964 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/ComponentRenderer-DCaUmBUC.css
+-rw-r--r--   0        0        0     7749 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/ComponentRenderer-DR8XBO3z.js
+-rw-r--r--   0        0        0    98868 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/Inter-Regular-CKDp9E3C.woff2
+-rw-r--r--   0        0        0   309828 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/Inter-Regular-CKX1N0ak.ttf
+-rw-r--r--   0        0        0    14409 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/abap-D8nrxEjS.js
+-rw-r--r--   0        0        0     4198 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/apex-BrXDlLUW.js
+-rw-r--r--   0        0        0     1094 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/azcli-CElzELwZ.js
+-rw-r--r--   0        0        0     2091 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/bat-CUsyEhik.js
+-rw-r--r--   0        0        0     2782 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/bicep-BtxyJn6H.js
+-rw-r--r--   0        0        0     2431 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/cameligo-ClBCoF8h.js
+-rw-r--r--   0        0        0     9889 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/clojure-B9TqLHAk.js
+-rw-r--r--   0        0        0    79568 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/codicon-BA2IlpFX.ttf
+-rw-r--r--   0        0        0     3836 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/coffee-DYsfeylR.js
+-rw-r--r--   0        0        0     5680 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/cpp-VVGvvgir.js
+-rw-r--r--   0        0        0     4770 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/csharp-Z6z2stHy.js
+-rw-r--r--   0        0        0     1665 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/csp-DgZoLDI1.js
+-rw-r--r--   0        0        0     4756 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/css-KqQ96-gC.js
+-rw-r--r--   0        0        0   984347 2024-04-23 14:53:51.578686 streamsync-0.5.0rc2/src/streamsync/static/assets/css.worker-DvNUQFd1.js
+-rw-r--r--   0        0        0    33713 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/cssMode-DtVHD6mi.js
+-rw-r--r--   0        0        0     3631 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/cypher-CYoSlgTu.js
+-rw-r--r--   0        0        0     4496 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/dart-BGDl7St1.js
+-rw-r--r--   0        0        0     2115 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/dockerfile-CuCtxA7T.js
+-rw-r--r--   0        0        0     5588 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/ecl-BCTFAUpS.js
+-rw-r--r--   0        0        0   210242 2024-04-23 14:53:51.574686 streamsync-0.5.0rc2/src/streamsync/static/assets/editor.worker-BVwmgLrR.js
+-rw-r--r--   0        0        0    10503 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/elixir-C7hRTYZ9.js
+-rw-r--r--   0        0        0     2056 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/flow9-Bi_qi707.js
+-rw-r--r--   0        0        0    16478 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/freemarker2-DUEoEr62.js
+-rw-r--r--   0        0        0     3229 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/fsharp-CxaaEKKi.js
+-rw-r--r--   0        0        0     2903 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/go-DUImKuGY.js
+-rw-r--r--   0        0        0     2506 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/graphql-D5sGVkLV.js
+-rw-r--r--   0        0        0     7156 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/handlebars-IQKTbmUg.js
+-rw-r--r--   0        0        0     3836 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/hcl-zD_CCkZ1.js
+-rw-r--r--   0        0        0     5396 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/html-ByZsrVkz.js
+-rw-r--r--   0        0        0   648041 2024-04-23 14:53:51.578686 streamsync-0.5.0rc2/src/streamsync/static/assets/html.worker-BJMlcbMU.js
+-rw-r--r--   0        0        0    34264 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/htmlMode-x26Bv8eO.js
+-rw-r--r--   0        0        0   309095 2024-04-23 14:53:51.574686 streamsync-0.5.0rc2/src/streamsync/static/assets/index-CK0qFcoM.js
+-rw-r--r--   0        0        0  1798721 2024-04-23 14:53:51.578686 streamsync-0.5.0rc2/src/streamsync/static/assets/index-DJ0okGb-.js
+-rw-r--r--   0        0        0     5725 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/index-DMFOqlrb.js
+-rw-r--r--   0        0        0   201777 2024-04-23 14:53:51.574686 streamsync-0.5.0rc2/src/streamsync/static/assets/index-DaNZqg5r.js
+-rw-r--r--   0        0        0   358136 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/index-Kfy6W749.css
+-rw-r--r--   0        0        0     1347 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/ini-8kKHd4ZL.js
+-rw-r--r--   0        0        0     3467 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/java-De1axCfe.js
+-rw-r--r--   0        0        0     1292 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/javascript-TK_dEQGI.js
+-rw-r--r--   0        0        0   339023 2024-04-23 14:53:51.574686 streamsync-0.5.0rc2/src/streamsync/static/assets/json.worker-BwvX8PuZ.js
+-rw-r--r--   0        0        0    39790 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/jsonMode-CcIaVIWF.js
+-rw-r--r--   0        0        0     7395 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/julia-D3ApGBxz.js
+-rw-r--r--   0        0        0     3685 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/kotlin-GbSrCElU.js
+-rw-r--r--   0        0        0     4144 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/less-DNUaDNdz.js
+-rw-r--r--   0        0        0     2683 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/lexon-Bg9QKxBu.js
+-rw-r--r--   0        0        0     4342 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/liquid-CWE4cS-c.js
+-rw-r--r--   0        0        0     2369 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/lua-Crkvc3mc.js
+-rw-r--r--   0        0        0     3063 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/m3-DsrzVyM1.js
+-rw-r--r--   0        0        0  1289773 2024-04-23 14:53:51.578686 streamsync-0.5.0rc2/src/streamsync/static/assets/mapbox-gl-BgoVqks1.js
+-rw-r--r--   0        0        0     4034 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/markdown-CY5IOZuu.js
+-rw-r--r--   0        0        0    35703 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/marked.esm-273vDTCT.js
+-rw-r--r--   0        0        0     5247 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/mdx-BCqw-Sgx.js
+-rw-r--r--   0        0        0     2825 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/mips-BE8RsGBA.js
+-rw-r--r--   0        0        0     5158 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/msdax-N5ajIiFQ.js
+-rw-r--r--   0        0        0    11520 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/mysql-DRxbB97D.js
+-rw-r--r--   0        0        0     2648 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/objective-c-BHUZy23s.js
+-rw-r--r--   0        0        0     3241 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/pascal-BemVzBTY.js
+-rw-r--r--   0        0        0     2246 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/pascaligo-BACCcnx_.js
+-rw-r--r--   0        0        0     8501 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/perl-CuU66Ptk.js
+-rw-r--r--   0        0        0    13710 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/pgsql-CQ6TMH2r.js
+-rw-r--r--   0        0        0     8273 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/php-BvyzZa65.js
+-rw-r--r--   0        0        0     1929 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/pla-DrIuu9u1.js
+-rw-r--r--   0        0        0  3704067 2024-04-23 14:53:51.582687 streamsync-0.5.0rc2/src/streamsync/static/assets/plotly.min-ETB9zM8E.js
+-rw-r--r--   0        0        0     8102 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/postiats-BR_hrfni.js
+-rw-r--r--   0        0        0    17185 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/powerquery-CKDUeRmd.js
+-rw-r--r--   0        0        0     3515 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/powershell-Dsa4rhA_.js
+-rw-r--r--   0        0        0     9292 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/protobuf-CGsvhooB.js
+-rw-r--r--   0        0        0     5074 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/pug-D2p3uOX2.js
+-rw-r--r--   0        0        0     4006 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/python-DeglcX7v.js
+-rw-r--r--   0        0        0     3181 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/qsharp-B7F3HtPF.js
+-rw-r--r--   0        0        0     3377 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/r-3aLoi2fs.js
+-rw-r--r--   0        0        0     9160 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/razor-C0ubHCZJ.js
+-rw-r--r--   0        0        0     3802 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/redis-jqFeRM5s.js
+-rw-r--r--   0        0        0    12046 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/redshift-BriwQgXR.js
+-rw-r--r--   0        0        0   163200 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-BVOYbT3K.woff2
+-rw-r--r--   0        0        0   525572 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-D9ZyeRwQ.ttf
+-rw-r--r--   0        0        0   525744 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-DUK49BtM.eot
+-rw-r--r--   0        0        0   224116 2024-04-23 14:53:51.510686 streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-DfzPQSMi.woff
+-rw-r--r--   0        0        0  2460531 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-ncU_JTfY.svg
+-rw-r--r--   0        0        0     4139 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/restructuredtext-hbBFZ0w9.js
+-rw-r--r--   0        0        0     8750 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/ruby-ByThyB2Q.js
+-rw-r--r--   0        0        0     4406 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/rust-DIEZMp5R.js
+-rw-r--r--   0        0        0     2075 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/sb-C6Gjjw_x.js
+-rw-r--r--   0        0        0     7564 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/scala-DZNw3jJB.js
+-rw-r--r--   0        0        0     2013 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/scheme-55eqh71t.js
+-rw-r--r--   0        0        0     6655 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/scss-D-OVkc4F.js
+-rw-r--r--   0        0        0   202255 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/serialization-DDqLB4lR.js
+-rw-r--r--   0        0        0     3319 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/shell-DSpi8_qN.js
+-rw-r--r--   0        0        0    18843 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/solidity-BHddiNFS.js
+-rw-r--r--   0        0        0     3010 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/sophia-D6taVZFb.js
+-rw-r--r--   0        0        0     2798 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/sparql-LA0C7mUc.js
+-rw-r--r--   0        0        0    10543 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/sql-C3-3IcFM.js
+-rw-r--r--   0        0        0     7645 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/st-C4g7059C.js
+-rw-r--r--   0        0        0     5417 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/swift-DNI1vH3h.js
+-rw-r--r--   0        0        0     7849 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/systemverilog-DL_FVbcQ.js
+-rw-r--r--   0        0        0     3817 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/tcl-DVJXmIwd.js
+-rw-r--r--   0        0        0  4847810 2024-04-23 14:53:51.582687 streamsync-0.5.0rc2/src/streamsync/static/assets/ts.worker-CwG1rUES.js
+-rw-r--r--   0        0        0    22645 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/tsMode-nAaFVZJ4.js
+-rw-r--r--   0        0        0     6219 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/twig-BVWDLtw5.js
+-rw-r--r--   0        0        0     5789 2024-04-23 14:53:51.574686 streamsync-0.5.0rc2/src/streamsync/static/assets/typescript-B1RkFep_.js
+-rw-r--r--   0        0        0     6037 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/vb-Btz91-7U.js
+-rw-r--r--   0        0        0   839306 2024-04-23 14:53:51.578686 streamsync-0.5.0rc2/src/streamsync/static/assets/vega-embed.module-3YlK5-kl.js
+-rw-r--r--   0        0        0     7592 2024-04-23 14:53:51.518686 streamsync-0.5.0rc2/src/streamsync/static/assets/wgsl-D8V_buCG.js
+-rw-r--r--   0        0        0     2790 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/xml-CDaxQGEH.js
+-rw-r--r--   0        0        0     4397 2024-04-23 14:53:51.514685 streamsync-0.5.0rc2/src/streamsync/static/assets/yaml-CYFjN4Gg.js
+-rw-r--r--   0        0        0     3780 2024-04-23 14:53:48.602645 streamsync-0.5.0rc2/src/streamsync/static/favicon.png
+-rw-r--r--   0        0        0     1864 2024-04-23 14:53:51.574686 streamsync-0.5.0rc2/src/streamsync/static/index.html
+-rw-r--r--   0        0        0    59287 2024-04-23 14:52:36.713641 streamsync-0.5.0rc2/src/streamsync/ui.py
+-rw-r--r--   0        0        0     7748 2024-04-23 14:51:41.688886 streamsync-0.5.0rc2/src/streamsync/ui_manager.py
+-rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 streamsync-0.5.0rc2/PKG-INFO
```

### Comparing `streamsync-0.5.0rc1/LICENSE.txt` & `streamsync-0.5.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/README.md` & `streamsync-0.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/pyproject.toml` & `streamsync-0.5.0rc2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "streamsync"
-version = "0.5.0rc1"
+version = "0.5.0rc2"
 description = "Streamsync helps you create performant data apps, via Python code and its built-in visual UI editor."
 authors = ["Ramiro Medina <ramiro.a.medina@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://www.streamsync.cloud"
 repository = "https://www.github.com/streamsync-cloud/streamsync"
 documentation = "https://www.streamsync.cloud/getting-started.html"
@@ -20,15 +20,17 @@
     "Programming Language :: Python :: 3.12",
     "Development Status :: 4 - Beta"
 ]
 packages = [
     { include = "streamsync", from = "src" }
 ]
 include = [
-	"src/streamsync/static/**/*"
+    "src/streamsync/*.py",
+    "src/streamsync/static/**/*",
+    "src/streamsync/app_templates/**/*"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9.2, <4.0"
 pydantic = ">= 2.6.0, < 3"
 fastapi = ">= 0.89.1, < 1"
 websockets = ">= 12, < 13"
```

### Comparing `streamsync-0.5.0rc1/src/streamsync/__init__.py` & `streamsync-0.5.0rc2/src/streamsync/__init__.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/app_runner.py` & `streamsync-0.5.0rc2/src/streamsync/app_runner.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/command_line.py` & `streamsync-0.5.0rc2/src/streamsync/command_line.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/core.py` & `streamsync-0.5.0rc2/src/streamsync/core.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/core_ui.py` & `streamsync-0.5.0rc2/src/streamsync/core_ui.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/serve.py` & `streamsync-0.5.0rc2/src/streamsync/serve.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/ss_types.py` & `streamsync-0.5.0rc2/src/streamsync/ss_types.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/Arrow.dom-C52_vrWm.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/Arrow.dom-C52_vrWm.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/BuilderApp-Co-xyrd-.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/BuilderApp-Co-xyrd-.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/BuilderApp-Fzhw8njh.css` & `streamsync-0.5.0rc2/src/streamsync/static/assets/BuilderApp-Fzhw8njh.css`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/ComponentRenderer-DCaUmBUC.css` & `streamsync-0.5.0rc2/src/streamsync/static/assets/ComponentRenderer-DCaUmBUC.css`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/ComponentRenderer-DR8XBO3z.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/ComponentRenderer-DR8XBO3z.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/Inter-Regular-CKDp9E3C.woff2` & `streamsync-0.5.0rc2/src/streamsync/static/assets/Inter-Regular-CKDp9E3C.woff2`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/Inter-Regular-CKX1N0ak.ttf` & `streamsync-0.5.0rc2/src/streamsync/static/assets/Inter-Regular-CKX1N0ak.ttf`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/abap-D8nrxEjS.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/abap-D8nrxEjS.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/apex-BrXDlLUW.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/apex-BrXDlLUW.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/azcli-CElzELwZ.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/azcli-CElzELwZ.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/bat-CUsyEhik.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/bat-CUsyEhik.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/bicep-BtxyJn6H.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/bicep-BtxyJn6H.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/cameligo-ClBCoF8h.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/cameligo-ClBCoF8h.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/clojure-B9TqLHAk.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/clojure-B9TqLHAk.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/codicon-BA2IlpFX.ttf` & `streamsync-0.5.0rc2/src/streamsync/static/assets/codicon-BA2IlpFX.ttf`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/coffee-DYsfeylR.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/coffee-DYsfeylR.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/cpp-VVGvvgir.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/cpp-VVGvvgir.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/csharp-Z6z2stHy.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/csharp-Z6z2stHy.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/csp-DgZoLDI1.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/csp-DgZoLDI1.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/css-KqQ96-gC.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/css-KqQ96-gC.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/css.worker-DvNUQFd1.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/css.worker-DvNUQFd1.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/cssMode-DtVHD6mi.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/cssMode-DtVHD6mi.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/cypher-CYoSlgTu.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/cypher-CYoSlgTu.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/dart-BGDl7St1.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/dart-BGDl7St1.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/dockerfile-CuCtxA7T.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/dockerfile-CuCtxA7T.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/ecl-BCTFAUpS.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/ecl-BCTFAUpS.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/editor.worker-BVwmgLrR.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/editor.worker-BVwmgLrR.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/elixir-C7hRTYZ9.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/elixir-C7hRTYZ9.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/flow9-Bi_qi707.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/flow9-Bi_qi707.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/freemarker2-DUEoEr62.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/freemarker2-DUEoEr62.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/fsharp-CxaaEKKi.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/fsharp-CxaaEKKi.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/go-DUImKuGY.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/go-DUImKuGY.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/graphql-D5sGVkLV.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/graphql-D5sGVkLV.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/handlebars-IQKTbmUg.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/handlebars-IQKTbmUg.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/hcl-zD_CCkZ1.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/hcl-zD_CCkZ1.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/html-ByZsrVkz.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/html-ByZsrVkz.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/html.worker-BJMlcbMU.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/html.worker-BJMlcbMU.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/htmlMode-x26Bv8eO.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/htmlMode-x26Bv8eO.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/index-CK0qFcoM.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/index-CK0qFcoM.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/index-DJ0okGb-.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/index-DJ0okGb-.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/index-DMFOqlrb.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/index-DMFOqlrb.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/index-DaNZqg5r.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/index-DaNZqg5r.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/index-Kfy6W749.css` & `streamsync-0.5.0rc2/src/streamsync/static/assets/index-Kfy6W749.css`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/ini-8kKHd4ZL.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/ini-8kKHd4ZL.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/java-De1axCfe.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/java-De1axCfe.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/javascript-TK_dEQGI.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/javascript-TK_dEQGI.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/json.worker-BwvX8PuZ.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/json.worker-BwvX8PuZ.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/jsonMode-CcIaVIWF.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/jsonMode-CcIaVIWF.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/julia-D3ApGBxz.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/julia-D3ApGBxz.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/kotlin-GbSrCElU.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/kotlin-GbSrCElU.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/less-DNUaDNdz.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/less-DNUaDNdz.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/lexon-Bg9QKxBu.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/lexon-Bg9QKxBu.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/liquid-CWE4cS-c.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/liquid-CWE4cS-c.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/lua-Crkvc3mc.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/lua-Crkvc3mc.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/m3-DsrzVyM1.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/m3-DsrzVyM1.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/mapbox-gl-BgoVqks1.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/mapbox-gl-BgoVqks1.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/markdown-CY5IOZuu.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/markdown-CY5IOZuu.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/marked.esm-273vDTCT.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/marked.esm-273vDTCT.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/mdx-BCqw-Sgx.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/mdx-BCqw-Sgx.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/mips-BE8RsGBA.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/mips-BE8RsGBA.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/msdax-N5ajIiFQ.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/msdax-N5ajIiFQ.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/mysql-DRxbB97D.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/mysql-DRxbB97D.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/objective-c-BHUZy23s.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/objective-c-BHUZy23s.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/pascal-BemVzBTY.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/pascal-BemVzBTY.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/pascaligo-BACCcnx_.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/pascaligo-BACCcnx_.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/perl-CuU66Ptk.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/perl-CuU66Ptk.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/pgsql-CQ6TMH2r.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/pgsql-CQ6TMH2r.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/php-BvyzZa65.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/php-BvyzZa65.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/pla-DrIuu9u1.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/pla-DrIuu9u1.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/plotly.min-ETB9zM8E.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/plotly.min-ETB9zM8E.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/postiats-BR_hrfni.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/postiats-BR_hrfni.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/powerquery-CKDUeRmd.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/powerquery-CKDUeRmd.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/powershell-Dsa4rhA_.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/powershell-Dsa4rhA_.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/protobuf-CGsvhooB.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/protobuf-CGsvhooB.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/pug-D2p3uOX2.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/pug-D2p3uOX2.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/python-DeglcX7v.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/python-DeglcX7v.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/qsharp-B7F3HtPF.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/qsharp-B7F3HtPF.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/r-3aLoi2fs.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/r-3aLoi2fs.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/razor-C0ubHCZJ.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/razor-C0ubHCZJ.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/redis-jqFeRM5s.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/redis-jqFeRM5s.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/redshift-BriwQgXR.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/redshift-BriwQgXR.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-BVOYbT3K.woff2` & `streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-BVOYbT3K.woff2`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-D9ZyeRwQ.ttf` & `streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-D9ZyeRwQ.ttf`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-DUK49BtM.eot` & `streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-DUK49BtM.eot`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-DfzPQSMi.woff` & `streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-DfzPQSMi.woff`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/remixicon-ncU_JTfY.svg` & `streamsync-0.5.0rc2/src/streamsync/static/assets/remixicon-ncU_JTfY.svg`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/restructuredtext-hbBFZ0w9.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/restructuredtext-hbBFZ0w9.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/ruby-ByThyB2Q.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/ruby-ByThyB2Q.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/rust-DIEZMp5R.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/rust-DIEZMp5R.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/sb-C6Gjjw_x.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/sb-C6Gjjw_x.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/scala-DZNw3jJB.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/scala-DZNw3jJB.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/scheme-55eqh71t.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/scheme-55eqh71t.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/scss-D-OVkc4F.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/scss-D-OVkc4F.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/serialization-DDqLB4lR.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/serialization-DDqLB4lR.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/shell-DSpi8_qN.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/shell-DSpi8_qN.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/solidity-BHddiNFS.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/solidity-BHddiNFS.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/sophia-D6taVZFb.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/sophia-D6taVZFb.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/sparql-LA0C7mUc.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/sparql-LA0C7mUc.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/sql-C3-3IcFM.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/sql-C3-3IcFM.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/st-C4g7059C.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/st-C4g7059C.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/swift-DNI1vH3h.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/swift-DNI1vH3h.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/systemverilog-DL_FVbcQ.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/systemverilog-DL_FVbcQ.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/tcl-DVJXmIwd.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/tcl-DVJXmIwd.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/ts.worker-CwG1rUES.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/ts.worker-CwG1rUES.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/tsMode-nAaFVZJ4.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/tsMode-nAaFVZJ4.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/twig-BVWDLtw5.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/twig-BVWDLtw5.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/typescript-B1RkFep_.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/typescript-B1RkFep_.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/vb-Btz91-7U.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/vb-Btz91-7U.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/vega-embed.module-3YlK5-kl.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/vega-embed.module-3YlK5-kl.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/wgsl-D8V_buCG.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/wgsl-D8V_buCG.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/xml-CDaxQGEH.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/xml-CDaxQGEH.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/assets/yaml-CYFjN4Gg.js` & `streamsync-0.5.0rc2/src/streamsync/static/assets/yaml-CYFjN4Gg.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/favicon.png` & `streamsync-0.5.0rc2/src/streamsync/app_templates/default/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/static/index.html` & `streamsync-0.5.0rc2/src/streamsync/static/index.html`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/src/streamsync/ui_manager.py` & `streamsync-0.5.0rc2/src/streamsync/ui_manager.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.5.0rc1/PKG-INFO` & `streamsync-0.5.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamsync
-Version: 0.5.0rc1
+Version: 0.5.0rc2
 Summary: Streamsync helps you create performant data apps, via Python code and its built-in visual UI editor.
 Home-page: https://www.streamsync.cloud
 License: Apache 2.0
 Keywords: data apps,gui,ui
 Author: Ramiro Medina
 Author-email: ramiro.a.medina@gmail.com
 Requires-Python: >=3.9.2,<4.0
```

