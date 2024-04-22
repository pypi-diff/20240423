# Comparing `tmp/mqt_core-2.4.0.tar.gz` & `tmp/mqt_core-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt_core-2.4.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "mqt_core-2.4.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `mqt_core-2.4.0.tar` & `mqt_core-2.4.1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 mqt_core-2.4.0/.clang-format
--rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 mqt_core-2.4.0/.clang-tidy
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_core-2.4.0/.cmake-format.yaml
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 mqt_core-2.4.0/.git_archival.txt
--rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_core-2.4.0/.gitattributes
--rw-r--r--   0        0        0     2009 2022-11-09 12:37:21.000000 mqt_core-2.4.0/.gitignore
--rw-r--r--   0        0        0     3529 2022-11-09 12:37:21.000000 mqt_core-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 mqt_core-2.4.0/.readthedocs.yaml
--rwxr-xr-x   0        0        0     2786 2022-11-09 12:37:21.000000 mqt_core-2.4.0/CMakeLists.txt
--rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 mqt_core-2.4.0/LICENSE.md
--rw-r--r--   0        0        0     6778 2022-11-09 12:37:21.000000 mqt_core-2.4.0/README.md
--rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/Cache.cmake
--rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/CompilerOptions.cmake
--rw-r--r--   0        0        0     5318 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/CompilerWarnings.cmake
--rw-r--r--   0        0        0     3231 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/ExternalDependencies.cmake
--rw-r--r--   0        0        0     2844 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/FindGMP.cmake
--rw-r--r--   0        0        0     7877 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/GetVersion.cmake
--rw-r--r--   0        0        0      795 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/PackageAddTest.cmake
--rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/Sanitizers.cmake
--rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/StandardProjectSettings.cmake
--rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 mqt_core-2.4.0/cmake/mqt-core-config.cmake.in
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 mqt_core-2.4.0/eval/CMakeLists.txt
--rw-r--r--   0        0        0     8559 2022-11-09 12:37:21.000000 mqt_core-2.4.0/eval/eval_dd_package.cpp
--rw-r--r--   0        0        0     3162 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/CircuitOptimizer.hpp
--rw-r--r--   0        0        0     3981 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/Definitions.hpp
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/Permutation.hpp
--rw-r--r--   0        0        0    41610 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/QuantumComputation.hpp
--rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/algorithms/BernsteinVazirani.hpp
--rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/algorithms/Entanglement.hpp
--rw-r--r--   0        0        0     1528 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/algorithms/GoogleRandomCircuitSampling.hpp
--rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/algorithms/Grover.hpp
--rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/algorithms/QFT.hpp
--rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/algorithms/QPE.hpp
--rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/algorithms/RandomCliffordCircuit.hpp
--rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/algorithms/WState.hpp
--rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Benchmark.hpp
--rw-r--r--   0        0        0     6105 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/CachedEdge.hpp
--rw-r--r--   0        0        0     4947 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Complex.hpp
--rw-r--r--   0        0        0     4498 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/ComplexNumbers.hpp
--rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/ComplexValue.hpp
--rw-r--r--   0        0        0     3619 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/ComputeTable.hpp
--rw-r--r--   0        0        0     3723 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/DDDefinitions.hpp
--rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/DDpackageConfig.hpp
--rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/DensityNoiseTable.hpp
--rw-r--r--   0        0        0    16220 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Edge.hpp
--rw-r--r--   0        0        0    32823 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Export.hpp
--rw-r--r--   0        0        0     1459 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/FunctionalityConstruction.hpp
--rw-r--r--   0        0        0     6331 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/GateMatrixDefinitions.hpp
--rw-r--r--   0        0        0     6484 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/MemoryManager.hpp
--rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Node.hpp
--rw-r--r--   0        0        0     4421 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/NoiseFunctionality.hpp
--rw-r--r--   0        0        0     9048 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Operations.hpp
--rw-r--r--   0        0        0    93777 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Package.hpp
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Package_fwd.hpp
--rw-r--r--   0        0        0    10422 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/RealNumber.hpp
--rw-r--r--   0        0        0     8768 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/RealNumberUniqueTable.hpp
--rw-r--r--   0        0        0     1672 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/Simulation.hpp
--rw-r--r--   0        0        0     2021 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/StochasticNoiseOperationTable.hpp
--rw-r--r--   0        0        0     1879 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/UnaryComputeTable.hpp
--rw-r--r--   0        0        0    12308 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/UniqueTable.hpp
--rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/statistics/MemoryManagerStatistics.hpp
--rw-r--r--   0        0        0    11654 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/statistics/PackageStatistics.hpp
--rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/statistics/Statistics.hpp
--rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/statistics/TableStatistics.hpp
--rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/dd/statistics/UniqueTableStatistics.hpp
--rw-r--r--   0        0        0     3103 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/ecc/Ecc.hpp
--rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/ecc/Id.hpp
--rw-r--r--   0        0        0     2452 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/ecc/Q18Surface.hpp
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/ecc/Q3Shor.hpp
--rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/ecc/Q5Laflamme.hpp
--rw-r--r--   0        0        0     1000 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/ecc/Q7Steane.hpp
--rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/ecc/Q9Shor.hpp
--rw-r--r--   0        0        0     1800 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/ecc/Q9Surface.hpp
--rw-r--r--   0        0        0     5055 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/ClassicControlledOperation.hpp
--rw-r--r--   0        0        0     5925 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/CompoundOperation.hpp
--rw-r--r--   0        0        0     1993 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/Control.hpp
--rw-r--r--   0        0        0    15630 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/Expression.hpp
--rw-r--r--   0        0        0     3600 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/NonUnitaryOperation.hpp
--rw-r--r--   0        0        0     6345 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/OpType.hpp
--rw-r--r--   0        0        0     6092 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/Operation.hpp
--rw-r--r--   0        0        0     3590 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/StandardOperation.hpp
--rw-r--r--   0        0        0     5717 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/operations/SymbolicOperation.hpp
--rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Exception.hpp
--rw-r--r--   0        0        0     1359 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Gate.hpp
--rw-r--r--   0        0        0     5284 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/InstVisitor.hpp
--rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/NestedEnvironment.hpp
--rw-r--r--   0        0        0     5441 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Parser.hpp
--rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Scanner.hpp
--rw-r--r--   0        0        0    13570 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Statement.hpp
--rw-r--r--   0        0        0     7101 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/StdGates.hpp
--rw-r--r--   0        0        0     9447 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Token.hpp
--rw-r--r--   0        0        0     5987 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Types.hpp
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/passes/CompilerPass.hpp
--rw-r--r--   0        0        0     5047 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/passes/ConstEvalPass.hpp
--rw-r--r--   0        0        0     3982 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/passes/TypeCheckPass.hpp
--rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/python/pybind11.hpp
--rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/python/qiskit/QuantumCircuit.hpp
--rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/zx/FunctionalityConstruction.hpp
--rw-r--r--   0        0        0     5874 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/zx/Rational.hpp
--rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/zx/Rules.hpp
--rw-r--r--   0        0        0     1688 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/zx/Simplify.hpp
--rw-r--r--   0        0        0     4335 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/zx/Utils.hpp
--rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/zx/ZXDefinitions.hpp
--rw-r--r--   0        0        0     5135 2022-11-09 12:37:21.000000 mqt_core-2.4.0/include/mqt-core/zx/ZXDiagram.hpp
--rw-r--r--   0        0        0     3352 2022-11-09 12:37:21.000000 mqt_core-2.4.0/noxfile.py
--rw-r--r--   0        0        0     8282 2022-11-09 12:37:21.000000 mqt_core-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     9262 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/CMakeLists.txt
--rw-r--r--   0        0        0    60140 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/CircuitOptimizer.cpp
--rw-r--r--   0        0        0    35083 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/QuantumComputation.cpp
--rw-r--r--   0        0        0     3263 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/algorithms/BernsteinVazirani.cpp
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/algorithms/Entanglement.cpp
--rw-r--r--   0        0        0     4387 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/algorithms/GoogleRandomCircuitSampling.cpp
--rw-r--r--   0        0        0     3073 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/algorithms/Grover.cpp
--rw-r--r--   0        0        0     2716 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/algorithms/QFT.cpp
--rw-r--r--   0        0        0     4317 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/algorithms/QPE.cpp
--rw-r--r--   0        0        0     5785 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/algorithms/RandomCliffordCircuit.cpp
--rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/algorithms/WState.cpp
--rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/Benchmark.cpp
--rw-r--r--   0        0        0     1204 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/CMakeLists.txt
--rw-r--r--   0        0        0     5653 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/CachedEdge.cpp
--rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/Complex.cpp
--rw-r--r--   0        0        0     1805 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/ComplexNumbers.cpp
--rw-r--r--   0        0        0     8904 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/ComplexValue.cpp
--rw-r--r--   0        0        0    21653 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/Edge.cpp
--rw-r--r--   0        0        0     6592 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/FunctionalityConstruction.cpp
--rw-r--r--   0        0        0     2028 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/MemoryManager.cpp
--rw-r--r--   0        0        0     2437 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/Node.cpp
--rw-r--r--   0        0        0    16109 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/NoiseFunctionality.cpp
--rw-r--r--   0        0        0     4408 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/Operations.cpp
--rw-r--r--   0        0        0     3235 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/RealNumber.cpp
--rw-r--r--   0        0        0     9683 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/RealNumberUniqueTable.cpp
--rw-r--r--   0        0        0    16155 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/Simulation.cpp
--rw-r--r--   0        0        0     2914 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/statistics/MemoryManagerStatistics.cpp
--rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/statistics/Statistics.cpp
--rw-r--r--   0        0        0     1571 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/statistics/TableStatistics.cpp
--rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/dd/statistics/UniqueTableStatistics.cpp
--rw-r--r--   0        0        0      956 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/ecc/CMakeLists.txt
--rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/ecc/Ecc.cpp
--rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/ecc/Q18Surface.cpp
--rw-r--r--   0        0        0     4465 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/ecc/Q3Shor.cpp
--rw-r--r--   0        0        0     5384 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/ecc/Q5Laflamme.cpp
--rw-r--r--   0        0        0     8164 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/ecc/Q7Steane.cpp
--rw-r--r--   0        0        0     6993 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/ecc/Q9Shor.cpp
--rw-r--r--   0        0        0     5996 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/ecc/Q9Surface.cpp
--rw-r--r--   0        0        0      513 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/__init__.py
--rw-r--r--   0        0        0      954 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/__main__.py
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/_compat/__init__.py
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/_compat/typing.py
--rw-r--r--   0        0        0    16637 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/_core/__init__.pyi
--rw-r--r--   0        0        0    11935 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/_core/operations.pyi
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/_core/symbolic.pyi
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/_version.py
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/_version.pyi
--rw-r--r--   0        0        0     1350 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/commands.py
--rw-r--r--   0        0        0    11961 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/evaluation.py
--rw-r--r--   0        0        0     1814 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/io.py
--rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/operations.py
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/plugins/__init__.py
--rw-r--r--   0        0        0    13057 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/plugins/qiskit.py
--rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/py.typed
--rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/mqt/core/symbolic.py
--rw-r--r--   0        0        0      858 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/operations/ClassicControlledOperation.cpp
--rw-r--r--   0        0        0     5699 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/operations/CompoundOperation.cpp
--rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/operations/Expression.cpp
--rw-r--r--   0        0        0     6254 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/operations/NonUnitaryOperation.cpp
--rw-r--r--   0        0        0     4489 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/operations/Operation.cpp
--rw-r--r--   0        0        0    16967 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/operations/StandardOperation.cpp
--rw-r--r--   0        0        0    12020 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/operations/SymbolicOperation.cpp
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/GRCSParser.cpp
--rw-r--r--   0        0        0    31466 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/QASM3Parser.cpp
--rw-r--r--   0        0        0    10467 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/QCParser.cpp
--rw-r--r--   0        0        0     8912 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/RealParser.cpp
--rw-r--r--   0        0        0     8273 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/TFCParser.cpp
--rw-r--r--   0        0        0    26220 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/qasm3_parser/Parser.cpp
--rw-r--r--   0        0        0    13173 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/qasm3_parser/Scanner.cpp
--rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/qasm3_parser/Statement.cpp
--rw-r--r--   0        0        0     1599 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/qasm3_parser/Types.cpp
--rw-r--r--   0        0        0    17353 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/qasm3_parser/passes/ConstEvalPass.cpp
--rw-r--r--   0        0        0    10210 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/parsers/qasm3_parser/passes/TypeCheckPass.cpp
--rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/CMakeLists.txt
--rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/module.cpp
--rw-r--r--   0        0        0     1784 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/operations/register_classic_controlled_operation.cpp
--rw-r--r--   0        0        0     2957 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/operations/register_compound_operation.cpp
--rw-r--r--   0        0        0     1604 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/operations/register_control.cpp
--rw-r--r--   0        0        0     1886 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/operations/register_non_unitary_operation.cpp
--rw-r--r--   0        0        0     3932 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/operations/register_operation.cpp
--rw-r--r--   0        0        0     2172 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/operations/register_optype.cpp
--rw-r--r--   0        0        0     3843 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/operations/register_standard_operation.cpp
--rw-r--r--   0        0        0     4031 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/operations/register_symbolic_operation.cpp
--rw-r--r--   0        0        0    18179 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/qiskit/QuantumCircuit.cpp
--rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/register_operations.cpp
--rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/register_permutation.cpp
--rw-r--r--   0        0        0    25756 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/register_quantum_computation.cpp
--rw-r--r--   0        0        0      319 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/register_symbolic.cpp
--rw-r--r--   0        0        0     4638 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/symbolic/register_expression.cpp
--rw-r--r--   0        0        0     1794 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/symbolic/register_term.cpp
--rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/python/symbolic/register_variable.cpp
--rw-r--r--   0        0        0     3009 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/zx/CMakeLists.txt
--rw-r--r--   0        0        0    25831 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/zx/FunctionalityConstruction.cpp
--rw-r--r--   0        0        0     1809 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/zx/Rational.cpp
--rw-r--r--   0        0        0    10647 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/zx/Rules.cpp
--rw-r--r--   0        0        0     2829 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/zx/Simplify.cpp
--rw-r--r--   0        0        0     4310 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/zx/Utils.cpp
--rw-r--r--   0        0        0    11414 2022-11-09 12:37:21.000000 mqt_core-2.4.0/src/zx/ZXDiagram.cpp
--rw-r--r--   0        0        0    10966 2022-11-09 12:37:21.000000 mqt_core-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 mqt_core-2.4.1/.clang-format
+-rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 mqt_core-2.4.1/.clang-tidy
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_core-2.4.1/.cmake-format.yaml
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 mqt_core-2.4.1/.git_archival.txt
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 mqt_core-2.4.1/.gitattributes
+-rw-r--r--   0        0        0     2019 2022-11-09 12:37:21.000000 mqt_core-2.4.1/.gitignore
+-rw-r--r--   0        0        0     3529 2022-11-09 12:37:21.000000 mqt_core-2.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 mqt_core-2.4.1/.readthedocs.yaml
+-rwxr-xr-x   0        0        0     2786 2022-11-09 12:37:21.000000 mqt_core-2.4.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1125 2022-11-09 12:37:21.000000 mqt_core-2.4.1/LICENSE.md
+-rw-r--r--   0        0        0     5818 2022-11-09 12:37:21.000000 mqt_core-2.4.1/README.md
+-rw-r--r--   0        0        0      841 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/Cache.cmake
+-rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/CompilerOptions.cmake
+-rw-r--r--   0        0        0     5318 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/CompilerWarnings.cmake
+-rw-r--r--   0        0        0     3231 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/ExternalDependencies.cmake
+-rw-r--r--   0        0        0     2844 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/FindGMP.cmake
+-rw-r--r--   0        0        0     7877 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/GetVersion.cmake
+-rw-r--r--   0        0        0      795 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/PackageAddTest.cmake
+-rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0        0        0     1834 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/Sanitizers.cmake
+-rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/StandardProjectSettings.cmake
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0        0        0     1245 2022-11-09 12:37:21.000000 mqt_core-2.4.1/cmake/mqt-core-config.cmake.in
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 mqt_core-2.4.1/eval/CMakeLists.txt
+-rw-r--r--   0        0        0     8559 2022-11-09 12:37:21.000000 mqt_core-2.4.1/eval/eval_dd_package.cpp
+-rw-r--r--   0        0        0     3599 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/CircuitOptimizer.hpp
+-rw-r--r--   0        0        0     3981 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/Definitions.hpp
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/Permutation.hpp
+-rw-r--r--   0        0        0    41610 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/QuantumComputation.hpp
+-rw-r--r--   0        0        0      615 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/algorithms/BernsteinVazirani.hpp
+-rw-r--r--   0        0        0      183 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/algorithms/Entanglement.hpp
+-rw-r--r--   0        0        0     1528 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/algorithms/GoogleRandomCircuitSampling.hpp
+-rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/algorithms/Grover.hpp
+-rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/algorithms/QFT.hpp
+-rw-r--r--   0        0        0      418 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/algorithms/QPE.hpp
+-rw-r--r--   0        0        0      628 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/algorithms/RandomCliffordCircuit.hpp
+-rw-r--r--   0        0        0      165 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/algorithms/WState.hpp
+-rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Benchmark.hpp
+-rw-r--r--   0        0        0     6105 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/CachedEdge.hpp
+-rw-r--r--   0        0        0     4947 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Complex.hpp
+-rw-r--r--   0        0        0     4498 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/ComplexNumbers.hpp
+-rw-r--r--   0        0        0     6377 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/ComplexValue.hpp
+-rw-r--r--   0        0        0     3619 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/ComputeTable.hpp
+-rw-r--r--   0        0        0     3723 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/DDDefinitions.hpp
+-rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/DDpackageConfig.hpp
+-rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/DensityNoiseTable.hpp
+-rw-r--r--   0        0        0    16220 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Edge.hpp
+-rw-r--r--   0        0        0    32823 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Export.hpp
+-rw-r--r--   0        0        0     1459 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/FunctionalityConstruction.hpp
+-rw-r--r--   0        0        0     6331 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/GateMatrixDefinitions.hpp
+-rw-r--r--   0        0        0     6484 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/MemoryManager.hpp
+-rw-r--r--   0        0        0     7562 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Node.hpp
+-rw-r--r--   0        0        0     4421 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/NoiseFunctionality.hpp
+-rw-r--r--   0        0        0     9048 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Operations.hpp
+-rw-r--r--   0        0        0    93777 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Package.hpp
+-rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Package_fwd.hpp
+-rw-r--r--   0        0        0    10422 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/RealNumber.hpp
+-rw-r--r--   0        0        0     8768 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/RealNumberUniqueTable.hpp
+-rw-r--r--   0        0        0     1672 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/Simulation.hpp
+-rw-r--r--   0        0        0     2021 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/StochasticNoiseOperationTable.hpp
+-rw-r--r--   0        0        0     1879 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/UnaryComputeTable.hpp
+-rw-r--r--   0        0        0    12308 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/UniqueTable.hpp
+-rw-r--r--   0        0        0     2247 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/statistics/MemoryManagerStatistics.hpp
+-rw-r--r--   0        0        0    11654 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/statistics/PackageStatistics.hpp
+-rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/statistics/Statistics.hpp
+-rw-r--r--   0        0        0     1989 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/statistics/TableStatistics.hpp
+-rw-r--r--   0        0        0      819 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/dd/statistics/UniqueTableStatistics.hpp
+-rw-r--r--   0        0        0     3103 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/ecc/Ecc.hpp
+-rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/ecc/Id.hpp
+-rw-r--r--   0        0        0     2452 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/ecc/Q18Surface.hpp
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/ecc/Q3Shor.hpp
+-rw-r--r--   0        0        0     1200 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/ecc/Q5Laflamme.hpp
+-rw-r--r--   0        0        0     1000 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/ecc/Q7Steane.hpp
+-rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/ecc/Q9Shor.hpp
+-rw-r--r--   0        0        0     1800 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/ecc/Q9Surface.hpp
+-rw-r--r--   0        0        0     5055 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/ClassicControlledOperation.hpp
+-rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/CompoundOperation.hpp
+-rw-r--r--   0        0        0     2264 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/Control.hpp
+-rw-r--r--   0        0        0    15630 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/Expression.hpp
+-rw-r--r--   0        0        0     3656 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/NonUnitaryOperation.hpp
+-rw-r--r--   0        0        0     6345 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/OpType.hpp
+-rw-r--r--   0        0        0     6053 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/Operation.hpp
+-rw-r--r--   0        0        0     3590 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/StandardOperation.hpp
+-rw-r--r--   0        0        0     5717 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/operations/SymbolicOperation.hpp
+-rw-r--r--   0        0        0     1240 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Exception.hpp
+-rw-r--r--   0        0        0     1359 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Gate.hpp
+-rw-r--r--   0        0        0     5284 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/InstVisitor.hpp
+-rw-r--r--   0        0        0      640 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/NestedEnvironment.hpp
+-rw-r--r--   0        0        0     5441 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Parser.hpp
+-rw-r--r--   0        0        0     1556 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Scanner.hpp
+-rw-r--r--   0        0        0    13570 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Statement.hpp
+-rw-r--r--   0        0        0     7101 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/StdGates.hpp
+-rw-r--r--   0        0        0     9447 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Token.hpp
+-rw-r--r--   0        0        0     5987 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Types.hpp
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/passes/CompilerPass.hpp
+-rw-r--r--   0        0        0     5047 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/passes/ConstEvalPass.hpp
+-rw-r--r--   0        0        0     3982 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/passes/TypeCheckPass.hpp
+-rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/python/pybind11.hpp
+-rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/python/qiskit/QuantumCircuit.hpp
+-rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/zx/FunctionalityConstruction.hpp
+-rw-r--r--   0        0        0     5874 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/zx/Rational.hpp
+-rw-r--r--   0        0        0      839 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/zx/Rules.hpp
+-rw-r--r--   0        0        0     1688 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/zx/Simplify.hpp
+-rw-r--r--   0        0        0     4335 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/zx/Utils.hpp
+-rw-r--r--   0        0        0     1537 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/zx/ZXDefinitions.hpp
+-rw-r--r--   0        0        0     5135 2022-11-09 12:37:21.000000 mqt_core-2.4.1/include/mqt-core/zx/ZXDiagram.hpp
+-rw-r--r--   0        0        0     3858 2022-11-09 12:37:21.000000 mqt_core-2.4.1/noxfile.py
+-rw-r--r--   0        0        0     8291 2022-11-09 12:37:21.000000 mqt_core-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     9262 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/CMakeLists.txt
+-rw-r--r--   0        0        0    62150 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/CircuitOptimizer.cpp
+-rw-r--r--   0        0        0    35051 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/QuantumComputation.cpp
+-rw-r--r--   0        0        0     3263 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/algorithms/BernsteinVazirani.cpp
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/algorithms/Entanglement.cpp
+-rw-r--r--   0        0        0     4387 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/algorithms/GoogleRandomCircuitSampling.cpp
+-rw-r--r--   0        0        0     3073 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/algorithms/Grover.cpp
+-rw-r--r--   0        0        0     2716 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/algorithms/QFT.cpp
+-rw-r--r--   0        0        0     4317 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/algorithms/QPE.cpp
+-rw-r--r--   0        0        0     5785 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/algorithms/RandomCliffordCircuit.cpp
+-rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/algorithms/WState.cpp
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/Benchmark.cpp
+-rw-r--r--   0        0        0     1204 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/CMakeLists.txt
+-rw-r--r--   0        0        0     5653 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/CachedEdge.cpp
+-rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/Complex.cpp
+-rw-r--r--   0        0        0     1805 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/ComplexNumbers.cpp
+-rw-r--r--   0        0        0     8904 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/ComplexValue.cpp
+-rw-r--r--   0        0        0    21653 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/Edge.cpp
+-rw-r--r--   0        0        0     6592 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/FunctionalityConstruction.cpp
+-rw-r--r--   0        0        0     2028 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/MemoryManager.cpp
+-rw-r--r--   0        0        0     2437 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/Node.cpp
+-rw-r--r--   0        0        0    16109 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/NoiseFunctionality.cpp
+-rw-r--r--   0        0        0     4408 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/Operations.cpp
+-rw-r--r--   0        0        0     3235 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/RealNumber.cpp
+-rw-r--r--   0        0        0     9683 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/RealNumberUniqueTable.cpp
+-rw-r--r--   0        0        0    16155 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/Simulation.cpp
+-rw-r--r--   0        0        0     2914 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/statistics/MemoryManagerStatistics.cpp
+-rw-r--r--   0        0        0      245 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/statistics/Statistics.cpp
+-rw-r--r--   0        0        0     1571 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/statistics/TableStatistics.cpp
+-rw-r--r--   0        0        0      686 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/dd/statistics/UniqueTableStatistics.cpp
+-rw-r--r--   0        0        0      956 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/ecc/CMakeLists.txt
+-rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/ecc/Ecc.cpp
+-rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/ecc/Q18Surface.cpp
+-rw-r--r--   0        0        0     4465 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/ecc/Q3Shor.cpp
+-rw-r--r--   0        0        0     5384 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/ecc/Q5Laflamme.cpp
+-rw-r--r--   0        0        0     8164 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/ecc/Q7Steane.cpp
+-rw-r--r--   0        0        0     6993 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/ecc/Q9Shor.cpp
+-rw-r--r--   0        0        0     5996 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/ecc/Q9Surface.cpp
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/__init__.py
+-rw-r--r--   0        0        0     1392 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/__main__.py
+-rw-r--r--   0        0        0     1625 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/_commands.py
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/_compat/__init__.py
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/_compat/typing.py
+-rw-r--r--   0        0        0    58276 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/_core/__init__.pyi
+-rw-r--r--   0        0        0    25527 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/_core/operations.pyi
+-rw-r--r--   0        0        0     5467 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/_core/symbolic.pyi
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/_version.py
+-rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/_version.pyi
+-rw-r--r--   0        0        0    13040 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/evaluation.py
+-rw-r--r--   0        0        0     1922 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/io.py
+-rw-r--r--   0        0        0      693 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/operations.py
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/plugins/__init__.py
+-rw-r--r--   0        0        0    13166 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/plugins/qiskit.py
+-rw-r--r--   0        0        0       93 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/py.typed
+-rw-r--r--   0        0        0      267 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/mqt/core/symbolic.py
+-rw-r--r--   0        0        0      858 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/operations/ClassicControlledOperation.cpp
+-rw-r--r--   0        0        0     5856 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/operations/CompoundOperation.cpp
+-rw-r--r--   0        0        0      485 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/operations/Expression.cpp
+-rw-r--r--   0        0        0     6373 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/operations/NonUnitaryOperation.cpp
+-rw-r--r--   0        0        0     4669 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/operations/Operation.cpp
+-rw-r--r--   0        0        0    16967 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/operations/StandardOperation.cpp
+-rw-r--r--   0        0        0    12020 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/operations/SymbolicOperation.cpp
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/GRCSParser.cpp
+-rw-r--r--   0        0        0    31466 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/QASM3Parser.cpp
+-rw-r--r--   0        0        0    10369 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/QCParser.cpp
+-rw-r--r--   0        0        0     8912 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/RealParser.cpp
+-rw-r--r--   0        0        0     8273 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/TFCParser.cpp
+-rw-r--r--   0        0        0    26220 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/qasm3_parser/Parser.cpp
+-rw-r--r--   0        0        0    13173 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/qasm3_parser/Scanner.cpp
+-rw-r--r--   0        0        0      688 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/qasm3_parser/Statement.cpp
+-rw-r--r--   0        0        0     1599 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/qasm3_parser/Types.cpp
+-rw-r--r--   0        0        0    17353 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/qasm3_parser/passes/ConstEvalPass.cpp
+-rw-r--r--   0        0        0    10210 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/parsers/qasm3_parser/passes/TypeCheckPass.cpp
+-rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/CMakeLists.txt
+-rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/module.cpp
+-rw-r--r--   0        0        0     1517 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/operations/register_classic_controlled_operation.cpp
+-rw-r--r--   0        0        0     2460 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/operations/register_compound_operation.cpp
+-rw-r--r--   0        0        0     1529 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/operations/register_control.cpp
+-rw-r--r--   0        0        0     1568 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/operations/register_non_unitary_operation.cpp
+-rw-r--r--   0        0        0     2651 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/operations/register_operation.cpp
+-rw-r--r--   0        0        0     2096 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/operations/register_optype.cpp
+-rw-r--r--   0        0        0     2836 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/operations/register_standard_operation.cpp
+-rw-r--r--   0        0        0     2436 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/operations/register_symbolic_operation.cpp
+-rw-r--r--   0        0        0    18179 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/qiskit/QuantumCircuit.cpp
+-rw-r--r--   0        0        0      732 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/register_operations.cpp
+-rw-r--r--   0        0        0     2170 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/register_permutation.cpp
+-rw-r--r--   0        0        0    18425 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/register_quantum_computation.cpp
+-rw-r--r--   0        0        0      319 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/register_symbolic.cpp
+-rw-r--r--   0        0        0     3729 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/symbolic/register_expression.cpp
+-rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/symbolic/register_term.cpp
+-rw-r--r--   0        0        0      588 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/python/symbolic/register_variable.cpp
+-rw-r--r--   0        0        0     3009 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/zx/CMakeLists.txt
+-rw-r--r--   0        0        0    25831 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/zx/FunctionalityConstruction.cpp
+-rw-r--r--   0        0        0     1809 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/zx/Rational.cpp
+-rw-r--r--   0        0        0    10647 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/zx/Rules.cpp
+-rw-r--r--   0        0        0     2829 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/zx/Simplify.cpp
+-rw-r--r--   0        0        0     4310 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/zx/Utils.cpp
+-rw-r--r--   0        0        0    11414 2022-11-09 12:37:21.000000 mqt_core-2.4.1/src/zx/ZXDiagram.cpp
+-rw-r--r--   0        0        0     9968 2022-11-09 12:37:21.000000 mqt_core-2.4.1/PKG-INFO
```

### Comparing `mqt_core-2.4.0/.clang-tidy` & `mqt_core-2.4.1/.clang-tidy`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/.gitignore` & `mqt_core-2.4.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+docs/api/
 
 # PyBuilder
 .pybuilder/
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
```

### Comparing `mqt_core-2.4.0/.pre-commit-config.yaml` & `mqt_core-2.4.1/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   # Python linting using ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
         types_or: [python, pyi, jupyter]
       - id: ruff-format
         types_or: [python, pyi, jupyter]
```

### Comparing `mqt_core-2.4.0/.readthedocs.yaml` & `mqt_core-2.4.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/CMakeLists.txt` & `mqt_core-2.4.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/LICENSE.md` & `mqt_core-2.4.1/LICENSE.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Chair for Design Automation, Technical University of Munich, Germany
+Copyright (c) 2024 Chair for Design Automation, Technical University of Munich, Germany
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
```

### Comparing `mqt_core-2.4.0/README.md` & `mqt_core-2.4.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,47 +3,41 @@
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-core/ci.yml?branch=main&style=flat-square&logo=github&label=ci)](https://github.com/cda-tum/mqt-core/actions/workflows/ci.yml)
 [![CD](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-core/cd.yml?style=flat-square&logo=github&label=cd)](https://github.com/cda-tum/mqt-core/actions/workflows/cd.yml)
 [![Documentation](https://img.shields.io/readthedocs/mqt-core?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/core)
 [![codecov](https://img.shields.io/codecov/c/github/cda-tum/mqt-core?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/mqt-core)
 
 <p align="center">
- <picture>
-   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/mqt_light.png" width="60%">
-   <img src="https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/mqt_dark.png" width="60%">
- </picture>
+  <a href="https://mqt.readthedocs.io">
+   <picture>
+     <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/mqt_light.png" width="60%">
+     <img src="https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/mqt_dark.png" width="60%">
+   </picture>
+  </a>
 </p>
 
 # MQT Core - The Backbone of the Munich Quantum Toolkit (MQT)
 
-The MQT Core library forms the backbone of the quantum software tools developed as part of the _Munich Quantum Toolkit_ (_MQT_) by the [Chair for Design Automation](https://www.cda.cit.tum.de/) at the [Technical University of Munich](https://www.tum.de/). This includes the following tools:
-
-- [MQT DDSIM](https://github.com/cda-tum/mqt-ddsim): A Tool for Classical Quantum Circuit Simulation based on Decision Diagrams.
-- [MQT QMAP](https://github.com/cda-tum/mqt-qmap): A Tool for Quantum Circuit Mapping.
-- [MQT QCEC](https://github.com/cda-tum/mqt-qcec): A Tool for Quantum Circuit Equivalence Checking.
-- [MQT QECC](https://github.com/cda-tum/mqt-qecc): A Tool for Quantum Error Correcting Codes.
-- [MQT DDVis](https://github.com/cda-tum/mqt-ddvis): A Web-Application visualizing Decision Diagrams for Quantum Computing.
-- [MQT SyReC](https://github.com/cda-tum/mqt-syrec): A Tool for Synthesis of Reversible Circuits/Quantum Computing Oracles.
-
-For a full list of tools and libraries, please visit the [MQT website](https://mqt.readthedocs.io/).
+MQT Core is an open-source C++17 and Python library for quantum computing that forms the backbone of the quantum software tools developed as part of the [_Munich Quantum Toolkit_ (_MQT_)](https://mqt.readthedocs.io) by the [Chair for Design Automation](https://www.cda.cit.tum.de/) at the [Technical University of Munich](https://www.tum.de/).
+To this end, it consists of multiple components that are used throughout the MQT, including a fully fledged intermediate representation (IR) for quantum computations, a state-of-the-art decision diagram (DD) package for quantum computing, and a dedicated ZX-diagram package for working with the ZX-calculus.
 
 <p align="center">
   <a href="https://mqt.readthedocs.io/projects/core">
   <img width=30% src="https://img.shields.io/badge/documentation-blue?style=for-the-badge&logo=read%20the%20docs" alt="Documentation" />
   </a>
 </p>
 
 If you have any questions, feel free to create a [discussion](https://github.com/cda-tum/mqt-core/discussions) or an [issue](https://github.com/cda-tum/mqt-core/issues) on [GitHub](https://github.com/cda-tum/mqt-core).
 
 ## Getting Started
 
 `mqt.core` is available via [PyPI](https://pypi.org/project/mqt.core/) for all major operating systems and supports Python 3.8 to 3.12.
 
 ```console
-(venv) $ pip install mqt.core
+(.venv) $ pip install mqt.core
 ```
 
 The following code gives an example on the usage:
 
 ```python3
 from mqt.core import QuantumComputation
 
@@ -53,28 +47,14 @@
 qc.measure(range(2), range(2))
 
 print(qc)
 ```
 
 **Detailed documentation and examples are available at [ReadTheDocs](https://mqt.readthedocs.io/projects/core).**
 
-## Library Overview
-
-<!-- SPHINX-START -->
-
-MQT Core encompasses:
-
-- `MQT::Core`: An intermediate representation (IR) for quantum computations including means to import and export circuits in various formats.
-- `MQT::CoreDD`: A fully-fledged decision diagram (DD) library for quantum computing.
-- `MQT::CoreZX`: A library for working with ZX-diagrams and the ZX-calculus.
-- `MQT::CoreECC`: A library for working with error correcting codes (ECCs) for quantum computing.
-- `MQT::CorePython`: A Python interface for the MQT Core library (e.g., facilitating the import of Qiskit QuantumCircuits).
-
-<!-- SPHINX-END -->
-
 ## System Requirements
 
 Building (and running) is continuously tested under Linux, MacOS, and Windows using the [latest available system versions for GitHub Actions](https://github.com/actions/runner-images).
 However, the implementation should be compatible with any current C++ compiler supporting C++17 and a minimum CMake version of 3.19.
 
 MQT Core relies on some external dependencies:
```

#### html2text {}

```diff
@@ -8,73 +8,61 @@
 workflows/ci.yml) [![CD](https://img.shields.io/github/actions/workflow/status/
 cda-tum/mqt-core/cd.yml?style=flat-square&logo=github&label=cd)](https://
 github.com/cda-tum/mqt-core/actions/workflows/cd.yml) [![Documentation](https:/
 /img.shields.io/readthedocs/mqt-core?logo=readthedocs&style=flat-square)]
 (https://mqt.readthedocs.io/projects/core) [![codecov](https://img.shields.io/
 codecov/c/github/cda-tum/mqt-core?style=flat-square&logo=codecov)](https://
 codecov.io/gh/cda-tum/mqt-core)
-    [https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/
-                                 mqt_dark.png]
-# MQT Core - The Backbone of the Munich Quantum Toolkit (MQT) The MQT Core
-library forms the backbone of the quantum software tools developed as part of
-the _Munich Quantum Toolkit_ (_MQT_) by the [Chair for Design Automation]
-(https://www.cda.cit.tum.de/) at the [Technical University of Munich](https://
-www.tum.de/). This includes the following tools: - [MQT DDSIM](https://
-github.com/cda-tum/mqt-ddsim): A Tool for Classical Quantum Circuit Simulation
-based on Decision Diagrams. - [MQT QMAP](https://github.com/cda-tum/mqt-qmap):
-A Tool for Quantum Circuit Mapping. - [MQT QCEC](https://github.com/cda-tum/
-mqt-qcec): A Tool for Quantum Circuit Equivalence Checking. - [MQT QECC](https:
-//github.com/cda-tum/mqt-qecc): A Tool for Quantum Error Correcting Codes. -
-[MQT DDVis](https://github.com/cda-tum/mqt-ddvis): A Web-Application
-visualizing Decision Diagrams for Quantum Computing. - [MQT SyReC](https://
-github.com/cda-tum/mqt-syrec): A Tool for Synthesis of Reversible Circuits/
-Quantum Computing Oracles. For a full list of tools and libraries, please visit
-the [MQT website](https://mqt.readthedocs.io/).
+    _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_c_d_a_-_t_u_m_/_m_q_t_-_c_o_r_e_/_m_a_i_n_/_d_o_c_s_/___s_t_a_t_i_c_/
+                                 _m_q_t___d_a_r_k_._p_n_g_]
+# MQT Core - The Backbone of the Munich Quantum Toolkit (MQT) MQT Core is an
+open-source C++17 and Python library for quantum computing that forms the
+backbone of the quantum software tools developed as part of the [_Munich
+Quantum Toolkit_ (_MQT_)](https://mqt.readthedocs.io) by the [Chair for Design
+Automation](https://www.cda.cit.tum.de/) at the [Technical University of
+Munich](https://www.tum.de/). To this end, it consists of multiple components
+that are used throughout the MQT, including a fully fledged intermediate
+representation (IR) for quantum computations, a state-of-the-art decision
+diagram (DD) package for quantum computing, and a dedicated ZX-diagram package
+for working with the ZX-calculus.
                                 _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
 If you have any questions, feel free to create a [discussion](https://
 github.com/cda-tum/mqt-core/discussions) or an [issue](https://github.com/cda-
 tum/mqt-core/issues) on [GitHub](https://github.com/cda-tum/mqt-core). ##
 Getting Started `mqt.core` is available via [PyPI](https://pypi.org/project/
 mqt.core/) for all major operating systems and supports Python 3.8 to 3.12.
-```console (venv) $ pip install mqt.core ``` The following code gives an
+```console (.venv) $ pip install mqt.core ``` The following code gives an
 example on the usage: ```python3 from mqt.core import QuantumComputation qc =
 QuantumComputation(2, 2) qc.h(0) qc.cx(0, 1) qc.measure(range(2), range(2))
 print(qc) ``` **Detailed documentation and examples are available at
-[ReadTheDocs](https://mqt.readthedocs.io/projects/core).** ## Library Overview
-MQT Core encompasses: - `MQT::Core`: An intermediate representation (IR) for
-quantum computations including means to import and export circuits in various
-formats. - `MQT::CoreDD`: A fully-fledged decision diagram (DD) library for
-quantum computing. - `MQT::CoreZX`: A library for working with ZX-diagrams and
-the ZX-calculus. - `MQT::CoreECC`: A library for working with error correcting
-codes (ECCs) for quantum computing. - `MQT::CorePython`: A Python interface for
-the MQT Core library (e.g., facilitating the import of Qiskit QuantumCircuits).
-## System Requirements Building (and running) is continuously tested under
-Linux, MacOS, and Windows using the [latest available system versions for
-GitHub Actions](https://github.com/actions/runner-images). However, the
-implementation should be compatible with any current C++ compiler supporting
-C++17 and a minimum CMake version of 3.19. MQT Core relies on some external
-dependencies: - [nlohmann/json](https://github.com/nlohmann/json): A JSON
-library for modern C++. - [boost/multiprecision](https://github.com/boostorg/
-multiprecision): A library for multiprecision arithmetic (used in the ZX
-package). - [google/googletest](https://github.com/google/googletest): A
-testing framework for C++ (only used in tests). - [pybind/pybind11_json](https:
-//github.com/pybind/pybind11_json): Using nlohmann::json with pybind11 (only
-used for creating the Python bindings). CMake will automatically look for
-installed versions of these libraries. If it does not find them, they will be
-fetched automatically at configure time via the [FetchContent](https://
-cmake.org/cmake/help/latest/module/FetchContent.html) module (check out the
-documentation for more information on how to customize this behavior). It is
-recommended (although not required) to have [GraphViz](https://
-www.graphviz.org) installed for visualization purposes. If you want to use the
-ZX library, it is recommended (although not strictly necessary) to have [GMP]
-(https://gmplib.org/) installed in your system. --- ## Acknowledgements The
-Munich Quantum Toolkit has been supported by the European Research Council
-(ERC) under the European Union's Horizon 2020 research and innovation program
-(grant agreement No. 101001318), the Bavarian State Ministry for Science and
-Arts through the Distinguished Professorship Program, as well as the Munich
-Quantum Valley, which is supported by the Bavarian state government with funds
-from the Hightech Agenda Bayern Plus.
+[ReadTheDocs](https://mqt.readthedocs.io/projects/core).** ## System
+Requirements Building (and running) is continuously tested under Linux, MacOS,
+and Windows using the [latest available system versions for GitHub Actions]
+(https://github.com/actions/runner-images). However, the implementation should
+be compatible with any current C++ compiler supporting C++17 and a minimum
+CMake version of 3.19. MQT Core relies on some external dependencies: -
+[nlohmann/json](https://github.com/nlohmann/json): A JSON library for modern
+C++. - [boost/multiprecision](https://github.com/boostorg/multiprecision): A
+library for multiprecision arithmetic (used in the ZX package). - [google/
+googletest](https://github.com/google/googletest): A testing framework for C++
+(only used in tests). - [pybind/pybind11_json](https://github.com/pybind/
+pybind11_json): Using nlohmann::json with pybind11 (only used for creating the
+Python bindings). CMake will automatically look for installed versions of these
+libraries. If it does not find them, they will be fetched automatically at
+configure time via the [FetchContent](https://cmake.org/cmake/help/latest/
+module/FetchContent.html) module (check out the documentation for more
+information on how to customize this behavior). It is recommended (although not
+required) to have [GraphViz](https://www.graphviz.org) installed for
+visualization purposes. If you want to use the ZX library, it is recommended
+(although not strictly necessary) to have [GMP](https://gmplib.org/) installed
+in your system. --- ## Acknowledgements The Munich Quantum Toolkit has been
+supported by the European Research Council (ERC) under the European Union's
+Horizon 2020 research and innovation program (grant agreement No. 101001318),
+the Bavarian State Ministry for Science and Arts through the Distinguished
+Professorship Program, as well as the Munich Quantum Valley, which is supported
+by the Bavarian state government with funds from the Hightech Agenda Bayern
+Plus.
     [https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/
  tum_light.svg][https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/
  _static/logo-bavaria.svg][https://raw.githubusercontent.com/cda-tum/mqt-core/
 main/docs/_static/erc_light.svg][https://raw.githubusercontent.com/cda-tum/mqt-
                      core/main/docs/_static/logo-mqv.svg]
```

### Comparing `mqt_core-2.4.0/cmake/Cache.cmake` & `mqt_core-2.4.1/cmake/Cache.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/CompilerOptions.cmake` & `mqt_core-2.4.1/cmake/CompilerOptions.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/CompilerWarnings.cmake` & `mqt_core-2.4.1/cmake/CompilerWarnings.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/ExternalDependencies.cmake` & `mqt_core-2.4.1/cmake/ExternalDependencies.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/FindGMP.cmake` & `mqt_core-2.4.1/cmake/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/GetVersion.cmake` & `mqt_core-2.4.1/cmake/GetVersion.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/PackageAddTest.cmake` & `mqt_core-2.4.1/cmake/PackageAddTest.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/PreventInSourceBuilds.cmake` & `mqt_core-2.4.1/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/Sanitizers.cmake` & `mqt_core-2.4.1/cmake/Sanitizers.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/StandardProjectSettings.cmake` & `mqt_core-2.4.1/cmake/StandardProjectSettings.cmake`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/cmake_uninstall.cmake.in` & `mqt_core-2.4.1/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/cmake/mqt-core-config.cmake.in` & `mqt_core-2.4.1/cmake/mqt-core-config.cmake.in`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/eval/eval_dd_package.cpp` & `mqt_core-2.4.1/eval/eval_dd_package.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/CircuitOptimizer.hpp` & `mqt_core-2.4.1/include/mqt-core/CircuitOptimizer.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -81,9 +81,19 @@
    * they were collected. Each block is realized as a compound operation.
    * Light optimizations are applied to the blocks, such as removing identity
    * gates and fusing single-qubit gates.
    * @param qc the quantum circuit
    * @param maxBlockSize the maximum size of a block
    */
   static void collectBlocks(QuantumComputation& qc, std::size_t maxBlockSize);
+
+  /**
+   * @brief Elide permutations by propagating them through the circuit.
+   * @details The circuit is traversed and any SWAP gate is eliminated by
+   * propagating the permutation through the circuit. The final layout of the
+   * circuit is updated accordingly. This pass works well together with the
+   * `swapReconstruction` pass.
+   * @param qc the quantum circuit
+   */
+  static void elidePermutations(QuantumComputation& qc);
 };
 } // namespace qc
```

### Comparing `mqt_core-2.4.0/include/mqt-core/Definitions.hpp` & `mqt_core-2.4.1/include/mqt-core/Definitions.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/QuantumComputation.hpp` & `mqt_core-2.4.1/include/mqt-core/QuantumComputation.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/algorithms/BernsteinVazirani.hpp` & `mqt_core-2.4.1/include/mqt-core/algorithms/BernsteinVazirani.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/algorithms/GoogleRandomCircuitSampling.hpp` & `mqt_core-2.4.1/include/mqt-core/algorithms/GoogleRandomCircuitSampling.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/algorithms/Grover.hpp` & `mqt_core-2.4.1/include/mqt-core/algorithms/Grover.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/algorithms/RandomCliffordCircuit.hpp` & `mqt_core-2.4.1/include/mqt-core/algorithms/RandomCliffordCircuit.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/Benchmark.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/Benchmark.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/CachedEdge.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/CachedEdge.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/Complex.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/Complex.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/ComplexNumbers.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/ComplexNumbers.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/ComplexValue.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/ComplexValue.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/ComputeTable.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/ComputeTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/DDDefinitions.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/DDDefinitions.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/DDpackageConfig.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/DDpackageConfig.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/DensityNoiseTable.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/DensityNoiseTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/Edge.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/Edge.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/Export.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/Export.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/FunctionalityConstruction.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/FunctionalityConstruction.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/GateMatrixDefinitions.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/GateMatrixDefinitions.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/MemoryManager.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/MemoryManager.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/Node.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/Node.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/NoiseFunctionality.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/NoiseFunctionality.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/Operations.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/Operations.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/Package.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/Package.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/RealNumber.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/RealNumber.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/RealNumberUniqueTable.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/RealNumberUniqueTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/Simulation.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/Simulation.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/StochasticNoiseOperationTable.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/StochasticNoiseOperationTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/UnaryComputeTable.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/UnaryComputeTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/UniqueTable.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/UniqueTable.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/statistics/MemoryManagerStatistics.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/statistics/MemoryManagerStatistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/statistics/PackageStatistics.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/statistics/PackageStatistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/statistics/Statistics.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/statistics/Statistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/statistics/TableStatistics.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/statistics/TableStatistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/dd/statistics/UniqueTableStatistics.hpp` & `mqt_core-2.4.1/include/mqt-core/dd/statistics/UniqueTableStatistics.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/ecc/Ecc.hpp` & `mqt_core-2.4.1/include/mqt-core/ecc/Ecc.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/ecc/Q18Surface.hpp` & `mqt_core-2.4.1/include/mqt-core/ecc/Q18Surface.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/ecc/Q3Shor.hpp` & `mqt_core-2.4.1/include/mqt-core/ecc/Q3Shor.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/ecc/Q5Laflamme.hpp` & `mqt_core-2.4.1/include/mqt-core/ecc/Q5Laflamme.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/ecc/Q7Steane.hpp` & `mqt_core-2.4.1/include/mqt-core/ecc/Q7Steane.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/ecc/Q9Shor.hpp` & `mqt_core-2.4.1/include/mqt-core/ecc/Q9Shor.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/ecc/Q9Surface.hpp` & `mqt_core-2.4.1/include/mqt-core/ecc/Q9Surface.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/ClassicControlledOperation.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/ClassicControlledOperation.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/CompoundOperation.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/CompoundOperation.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 
   std::vector<std::unique_ptr<Operation>>& getOps() { return ops; }
 
   [[nodiscard]] std::set<Qubit> getUsedQubits() const override;
 
   void invert() override;
 
+  void apply(const Permutation& permutation) override;
+
   /**
    * @brief Merge another compound operation into this one.
    * @details This transfers ownership of the operations from the other compound
    * operation to this one. The other compound operation will be empty after
    * this operation.
    * @param op the compound operation to merge into this one
    */
```

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/Control.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/Control.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #pragma once
 
 #include "Definitions.hpp"
 
+#include <cstddef>
+#include <functional>
 #include <set>
 #include <sstream>
+#include <string>
 
 namespace qc {
 struct Control {
   enum class Type : bool { Pos = true, Neg = false };
 
   Qubit qubit{};
   Type type = Type::Pos;
@@ -42,23 +45,23 @@
   return !(lhs == rhs);
 }
 
 // this allows a set of controls to be indexed by a `Qubit`
 struct CompareControl {
   using is_transparent [[maybe_unused]] = void;
 
-  inline bool operator()(const Control& lhs, const Control& rhs) const {
+  bool operator()(const Control& lhs, const Control& rhs) const {
     return lhs < rhs;
   }
 
-  inline bool operator()(Qubit lhs, const Control& rhs) const {
+  bool operator()(Qubit lhs, const Control& rhs) const {
     return lhs < rhs.qubit;
   }
 
-  inline bool operator()(const Control& lhs, Qubit rhs) const {
+  bool operator()(const Control& lhs, Qubit rhs) const {
     return lhs.qubit < rhs;
   }
 };
 using Controls = std::set<Control, CompareControl>;
 
 inline namespace literals {
 // User-defined literals require unsigned long long int
@@ -69,7 +72,16 @@
 // User-defined literals require unsigned long long int
 // NOLINTNEXTLINE(google-runtime-int)
 inline Control operator""_nc(unsigned long long int q) {
   return {static_cast<Qubit>(q), Control::Type::Neg};
 }
 } // namespace literals
 } // namespace qc
+
+namespace std {
+template <> struct hash<qc::Control> {
+  std::size_t operator()(const qc::Control& c) const {
+    return std::hash<qc::Qubit>{}(c.qubit) ^
+           std::hash<qc::Control::Type>{}(c.type);
+  }
+};
+} // namespace std
```

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/Expression.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/Expression.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/NonUnitaryOperation.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/NonUnitaryOperation.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,16 @@
   void dumpOpenQASM(std::ostream& of, const RegisterNames& qreg,
                     const RegisterNames& creg, size_t indent,
                     bool openQASM3) const override;
 
   void invert() override {
     throw QFRException("Inverting a non-unitary operation is not supported.");
   }
+
+  void apply(const Permutation& permutation) override;
 };
 } // namespace qc
 
 namespace std {
 template <> struct hash<qc::NonUnitaryOperation> {
   std::size_t operator()(qc::NonUnitaryOperation const& op) const noexcept {
     std::size_t seed = 0U;
```

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/OpType.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/OpType.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/Operation.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/Operation.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 #include <memory>
 #include <set>
 #include <vector>
 
 namespace qc {
 class Operation {
 protected:
-  Controls controls{};
-  Targets targets{};
-  std::vector<fp> parameter{};
+  Controls controls;
+  Targets targets;
+  std::vector<fp> parameter;
 
   OpType type = None;
-  std::string name{};
+  std::string name;
 
   static bool isWholeQubitRegister(const RegisterNames& reg, std::size_t start,
                                    std::size_t end) {
     return !reg.empty() && reg[start].first == reg[end].first &&
            (start == 0 || reg[start].first != reg[start - 1].first) &&
            (end == reg.size() - 1 || reg[end].first != reg[end + 1].first);
   }
@@ -111,41 +111,33 @@
   virtual void setGate(const OpType g) {
     type = g;
     name = toString(g);
   }
 
   virtual void setParameter(const std::vector<fp>& p) { parameter = p; }
 
-  [[nodiscard]] inline virtual bool isUnitary() const { return true; }
+  virtual void apply(const Permutation& permutation);
 
-  [[nodiscard]] inline virtual bool isStandardOperation() const {
-    return false;
-  }
+  [[nodiscard]] virtual bool isUnitary() const { return true; }
 
-  [[nodiscard]] inline virtual bool isCompoundOperation() const {
-    return false;
-  }
+  [[nodiscard]] virtual bool isStandardOperation() const { return false; }
 
-  [[nodiscard]] inline virtual bool isNonUnitaryOperation() const {
-    return false;
-  }
+  [[nodiscard]] virtual bool isCompoundOperation() const { return false; }
 
-  [[nodiscard]] inline virtual bool isClassicControlledOperation() const {
-    return false;
-  }
+  [[nodiscard]] virtual bool isNonUnitaryOperation() const { return false; }
 
-  [[nodiscard]] inline virtual bool isSymbolicOperation() const {
+  [[nodiscard]] virtual bool isClassicControlledOperation() const {
     return false;
   }
 
-  [[nodiscard]] inline virtual bool isControlled() const {
-    return !controls.empty();
-  }
+  [[nodiscard]] virtual bool isSymbolicOperation() const { return false; }
+
+  [[nodiscard]] virtual bool isControlled() const { return !controls.empty(); }
 
-  [[nodiscard]] inline virtual bool actsOn(const Qubit i) const {
+  [[nodiscard]] virtual bool actsOn(const Qubit i) const {
     for (const auto& t : targets) {
       if (t == i) {
         return true;
       }
     }
     return controls.count(i) > 0;
   }
```

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/StandardOperation.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/StandardOperation.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/operations/SymbolicOperation.hpp` & `mqt_core-2.4.1/include/mqt-core/operations/SymbolicOperation.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Exception.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Exception.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Gate.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Gate.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/InstVisitor.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/InstVisitor.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/NestedEnvironment.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/NestedEnvironment.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Parser.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Parser.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Scanner.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Scanner.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Statement.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Statement.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/StdGates.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/StdGates.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Token.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Token.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/Types.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/Types.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/passes/ConstEvalPass.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/passes/ConstEvalPass.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/parsers/qasm3_parser/passes/TypeCheckPass.hpp` & `mqt_core-2.4.1/include/mqt-core/parsers/qasm3_parser/passes/TypeCheckPass.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/python/qiskit/QuantumCircuit.hpp` & `mqt_core-2.4.1/include/mqt-core/python/qiskit/QuantumCircuit.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/zx/FunctionalityConstruction.hpp` & `mqt_core-2.4.1/include/mqt-core/zx/FunctionalityConstruction.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/zx/Rational.hpp` & `mqt_core-2.4.1/include/mqt-core/zx/Rational.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/zx/Rules.hpp` & `mqt_core-2.4.1/include/mqt-core/zx/Rules.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/zx/Simplify.hpp` & `mqt_core-2.4.1/include/mqt-core/zx/Simplify.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/zx/Utils.hpp` & `mqt_core-2.4.1/include/mqt-core/zx/Utils.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/zx/ZXDefinitions.hpp` & `mqt_core-2.4.1/include/mqt-core/zx/ZXDefinitions.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/include/mqt-core/zx/ZXDiagram.hpp` & `mqt_core-2.4.1/include/mqt-core/zx/ZXDiagram.hpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/noxfile.py` & `mqt_core-2.4.1/noxfile.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,18 +16,24 @@
 nox.needs_version = ">=2024.3.2"
 nox.options.default_venv_backend = "uv|virtualenv"
 
 nox.options.sessions = ["lint", "tests"]
 
 PYTHON_ALL_VERSIONS = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
+# The following lists all the build requirements for building the package.
+# Note that this includes transitive build dependencies of package dependencies,
+# since we use `--no-build-isolation` to install the package in editable mode
+# and get better caching performance. This only concerns dependencies that are
+# not available via wheels on PyPI (i.e., only as source distributions).
 BUILD_REQUIREMENTS = [
     "scikit-build-core[pyproject]>=0.8.1",
     "setuptools_scm>=7",
     "pybind11>=2.12",
+    "wheel>=0.40",  # transitive dependency of pytest on Windows
 ]
 
 if os.environ.get("CI", None):
     nox.options.error_on_missing_interpreters = True
 
 
 @nox.session(reuse_venv=True)
@@ -68,15 +74,15 @@
 
 @nox.session(reuse_venv=True, python=PYTHON_ALL_VERSIONS)
 def tests(session: nox.Session) -> None:
     """Run the test suite."""
     _run_tests(session)
 
 
-@nox.session(reuse_venv=True, venv_backend="uv")
+@nox.session(reuse_venv=True, venv_backend="uv", python=PYTHON_ALL_VERSIONS)
 def minimums(session: nox.Session) -> None:
     """Test the minimum versions of dependencies."""
     _run_tests(
         session,
         install_args=["--resolution=lowest-direct"],
         run_args=["-Wdefault"],
         extras=["qiskit", "evaluation"],
@@ -107,10 +113,10 @@
         f"-b={args.builder}",
         ".",
         f"_build/{args.builder}",
         *posargs,
     )
 
     if serve:
-        session.run("sphinx-autobuild", *shared_args)
+        session.run("sphinx-autobuild", "--ignore", "**jupyter**", *shared_args)
     else:
         session.run("sphinx-build", "--keep-going", *shared_args)
```

### Comparing `mqt_core-2.4.0/pyproject.toml` & `mqt_core-2.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -41,36 +41,35 @@
 evaluation = [
     "pandas[output_formatting]>=2.0; python_version < '3.9'",
     "pandas[output-formatting]>=2.1.2; python_version >= '3.9'",
 ]
 docs = [
     "furo>=2023.08.17",
     "sphinx",
-    "myst_parser>=0.13",
+    "myst_nb>=1.1.0",
     "setuptools-scm>=7",
     "sphinx-copybutton",
     "sphinx_design",
     "sphinxext-opengraph",
     "sphinxcontrib-bibtex>=2.4.2",
+    "sphinxcontrib-svg2pdfconverter",
     "pybtex>=0.24",
     "ipython",
     "ipykernel",
-    "nbsphinx",
-    "sphinx-autodoc-typehints",
     "sphinx-autoapi",
     "qiskit[visualization]",
     "mqt.core[evaluation]"
 ]
 qiskit = [
    "qiskit[qasm3-import]>=1.0.0",
 ]
 dev = ["mqt.core[coverage, docs]",]
 
 [project.scripts]
-compare = "mqt.core.evaluation:main"
+mqt-core-compare = "mqt.core.evaluation:main"
 mqt-core-cli = "mqt.core.__main__:main"
 
 [project.urls]
 Homepage = "https://github.com/cda-tum/mqt-core"
 Documentation = "https://mqt.readthedocs.io/projects/core"
 Issues = "https://github.com/cda-tum/mqt-core/issues"
 Discussions = "https://github.com/cda-tum/mqt-core/discussions"
@@ -238,15 +237,15 @@
 "importlib.resources".msg = "Use scikit_build_core._compat.importlib.resources instead."
 "importlib_resources".msg = "Use scikit_build_core._compat.importlib.resources instead."
 
 [tool.ruff.lint.per-file-ignores]
 "test/python/**" = ["T20", "ANN"]
 "docs/**" = ["T20"]
 "noxfile.py" = ["T20", "TID251"]
-"*.pyi" = ["D"]  # pydocstyle
+"*.pyi" = ["D418", "PYI021"]  # pydocstyle
 "*.ipynb" = [
     "D",    # pydocstyle
     "E402", # Allow imports to appear anywhere in Jupyter notebooks
     "I002", # Allow missing `from __future__ import annotations` import
 ]
 "src/mqt/core/_compat/**.py" = ["TID251"]
 "src/mqt/core/evaluation.py" = ["T201"]
```

### Comparing `mqt_core-2.4.0/src/CMakeLists.txt` & `mqt_core-2.4.1/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/CircuitOptimizer.cpp` & `mqt_core-2.4.1/src/CircuitOptimizer.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 #include "CircuitOptimizer.hpp"
 
+#include "operations/NonUnitaryOperation.hpp"
+
 #include <algorithm>
 #include <cassert>
+#include <unordered_map>
 #include <utility>
 #include <vector>
 
 namespace qc {
 void CircuitOptimizer::removeIdentities(QuantumComputation& qc) {
   // delete the identities from circuit
   auto it = qc.ops.begin();
@@ -923,14 +926,17 @@
             continue;
           }
         }
       }
     }
     ++it;
   }
+  if (qubitsToAddMeasurements.empty()) {
+    return;
+  }
   qc.outputPermutation.clear();
   for (const auto& [qubit, clbit] : qubitsToAddMeasurements) {
     qc.measure(qubit, clbit);
   }
   qc.initializeIOMapping();
 }
 
@@ -1742,8 +1748,69 @@
     if (q == index) {
       dsu.finalizeBlock(q);
     }
   }
   removeIdentities(qc);
 }
 
+void elidePermutations(std::vector<std::unique_ptr<Operation>>& ops,
+                       Permutation& permutation) {
+  for (auto it = ops.begin(); it != ops.end();) {
+    auto& op = *it;
+    if (auto* compOp = dynamic_cast<CompoundOperation*>(op.get())) {
+      elidePermutations(compOp->getOps(), permutation);
+      if (compOp->empty()) {
+        it = ops.erase(it);
+        continue;
+      }
+      if (compOp->isConvertibleToSingleOperation()) {
+        *it = compOp->collapseToSingleOperation();
+      } else {
+        // also update the tracked controls in the compound operation
+        compOp->getControls() = permutation.apply(compOp->getControls());
+      }
+      ++it;
+      continue;
+    }
+
+    if (op->getType() == SWAP && !op->isControlled()) {
+      const auto& targets = op->getTargets();
+      assert(targets.size() == 2U);
+      assert(permutation.find(targets[0]) != permutation.end());
+      assert(permutation.find(targets[1]) != permutation.end());
+      auto& target0 = permutation[targets[0]];
+      auto& target1 = permutation[targets[1]];
+      std::swap(target0, target1);
+      it = ops.erase(it);
+      continue;
+    }
+
+    op->apply(permutation);
+    ++it;
+  }
+}
+
+void CircuitOptimizer::elidePermutations(QuantumComputation& qc) {
+  if (qc.empty()) {
+    return;
+  }
+
+  auto permutation = qc.initialLayout;
+  ::qc::elidePermutations(qc.ops, permutation);
+
+  // adjust the initial layout
+  Permutation initialLayout{};
+  for (auto& [physical, logical] : qc.initialLayout) {
+    initialLayout[logical] = logical;
+  }
+  qc.initialLayout = initialLayout;
+
+  // adjust the output permutation
+  Permutation outputPermutation{};
+  for (auto& [physical, logical] : qc.outputPermutation) {
+    assert(permutation.find(physical) != permutation.end());
+    outputPermutation[permutation[physical]] = logical;
+  }
+  qc.outputPermutation = outputPermutation;
+}
+
 } // namespace qc
```

### Comparing `mqt_core-2.4.0/src/QuantumComputation.cpp` & `mqt_core-2.4.1/src/QuantumComputation.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -161,16 +161,15 @@
         }
 
         const auto bitidx = *classicIt;
         if (outputPermutationFound) {
           // output permutation was already set before -> permute existing
           // values
           const auto current = outputPermutation.at(qubitidx);
-          if (static_cast<std::size_t>(qubitidx) != bitidx &&
-              static_cast<std::size_t>(current) != bitidx) {
+          if (static_cast<std::size_t>(current) != bitidx) {
             for (auto& p : outputPermutation) {
               if (static_cast<std::size_t>(p.second) == bitidx) {
                 p.second = current;
                 break;
               }
             }
             outputPermutation.at(qubitidx) = static_cast<Qubit>(bitidx);
@@ -498,15 +497,16 @@
     os << std::setw(4) << logical << "\033[0m";
   }
   os << "\n";
 
   size_t i = 0U;
   for (const auto& op : ops) {
     os << std::setw(width) << ++i << ":";
-    op->print(os, {}, static_cast<std::size_t>(width) + 1U, nqubits);
+    op->print(os, initialLayout, static_cast<std::size_t>(width) + 1U,
+              getNqubits());
     os << "\n";
   }
 
   os << std::setw(width + 1) << "o:";
   for (const auto& physicalQubit : initialLayout) {
     auto it = outputPermutation.find(physicalQubit.first);
     if (it == outputPermutation.end()) {
```

### Comparing `mqt_core-2.4.0/src/algorithms/BernsteinVazirani.cpp` & `mqt_core-2.4.1/src/algorithms/BernsteinVazirani.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/algorithms/GoogleRandomCircuitSampling.cpp` & `mqt_core-2.4.1/src/algorithms/GoogleRandomCircuitSampling.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/algorithms/Grover.cpp` & `mqt_core-2.4.1/src/algorithms/Grover.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/algorithms/QFT.cpp` & `mqt_core-2.4.1/src/algorithms/QFT.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/algorithms/QPE.cpp` & `mqt_core-2.4.1/src/algorithms/QPE.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/algorithms/RandomCliffordCircuit.cpp` & `mqt_core-2.4.1/src/algorithms/RandomCliffordCircuit.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/algorithms/WState.cpp` & `mqt_core-2.4.1/src/algorithms/WState.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/Benchmark.cpp` & `mqt_core-2.4.1/src/dd/Benchmark.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/CMakeLists.txt` & `mqt_core-2.4.1/src/dd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/CachedEdge.cpp` & `mqt_core-2.4.1/src/dd/CachedEdge.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/Complex.cpp` & `mqt_core-2.4.1/src/dd/Complex.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/ComplexNumbers.cpp` & `mqt_core-2.4.1/src/dd/ComplexNumbers.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/ComplexValue.cpp` & `mqt_core-2.4.1/src/dd/ComplexValue.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/Edge.cpp` & `mqt_core-2.4.1/src/dd/Edge.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/FunctionalityConstruction.cpp` & `mqt_core-2.4.1/src/dd/FunctionalityConstruction.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/MemoryManager.cpp` & `mqt_core-2.4.1/src/dd/MemoryManager.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/Node.cpp` & `mqt_core-2.4.1/src/dd/Node.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/NoiseFunctionality.cpp` & `mqt_core-2.4.1/src/dd/NoiseFunctionality.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/Operations.cpp` & `mqt_core-2.4.1/src/dd/Operations.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/RealNumber.cpp` & `mqt_core-2.4.1/src/dd/RealNumber.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/RealNumberUniqueTable.cpp` & `mqt_core-2.4.1/src/dd/RealNumberUniqueTable.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/Simulation.cpp` & `mqt_core-2.4.1/src/dd/Simulation.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/statistics/MemoryManagerStatistics.cpp` & `mqt_core-2.4.1/src/dd/statistics/MemoryManagerStatistics.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/statistics/TableStatistics.cpp` & `mqt_core-2.4.1/src/dd/statistics/TableStatistics.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/dd/statistics/UniqueTableStatistics.cpp` & `mqt_core-2.4.1/src/dd/statistics/UniqueTableStatistics.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/ecc/CMakeLists.txt` & `mqt_core-2.4.1/src/ecc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/ecc/Ecc.cpp` & `mqt_core-2.4.1/src/ecc/Ecc.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/ecc/Q18Surface.cpp` & `mqt_core-2.4.1/src/ecc/Q18Surface.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/ecc/Q3Shor.cpp` & `mqt_core-2.4.1/src/ecc/Q3Shor.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/ecc/Q5Laflamme.cpp` & `mqt_core-2.4.1/src/ecc/Q5Laflamme.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/ecc/Q7Steane.cpp` & `mqt_core-2.4.1/src/ecc/Q7Steane.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/ecc/Q9Shor.cpp` & `mqt_core-2.4.1/src/ecc/Q9Shor.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/ecc/Q9Surface.cpp` & `mqt_core-2.4.1/src/ecc/Q9Surface.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/mqt/core/__main__.py` & `mqt_core-2.4.1/src/mqt/core/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 """Command line interface for mqt-core."""
 
 from __future__ import annotations
 
 import argparse
 import sys
 
+from ._commands import cmake_dir, include_dir
 from ._version import version as __version__
-from .commands import cmake_dir, include_dir
 
 
 def main() -> None:
-    """Entry point for the mqt-core command line interface."""
+    """Entry point for the mqt-core command line interface.
+
+    This function is called when running the `mqt-core-cli` script.
+
+    .. code-block:: bash
+
+        mqt-core-cli [--version] [--include_dir] [--cmake_dir]
+
+    It provides the following command line options:
+
+    - :code:`--version`: Print the version and exit.
+    - :code:`--include_dir`: Print the path to the mqt-core C++ include directory.
+    - :code:`--cmake_dir`: Print the path to the mqt-core CMake module directory.
+
+    """
     parser = argparse.ArgumentParser()
     parser.add_argument("--version", action="version", version=__version__, help="Print version and exit.")
 
     parser.add_argument(
         "--include_dir", action="store_true", help="Print the path to the mqt-core C++ include directory."
     )
     parser.add_argument(
```

### Comparing `mqt_core-2.4.0/src/mqt/core/commands.py` & `mqt_core-2.4.1/src/mqt/core/_commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,39 @@
 from __future__ import annotations
 
 from importlib.metadata import PackageNotFoundError, distribution
 from pathlib import Path
 
 
 def include_dir() -> Path:
-    """Return the path to the mqt-core include directory."""
+    """Return the path to the mqt-core include directory.
+
+    Raises:
+        FileNotFoundError: If the include directory is not found.
+        ImportError: If mqt-core is not installed.
+    """
     try:
         dist = distribution("mqt-core")
         located_include_dir = Path(dist.locate_file("mqt/core/include/mqt-core"))
         if located_include_dir.exists() and located_include_dir.is_dir():
             return located_include_dir
         msg = "mqt-core include files not found."
         raise FileNotFoundError(msg)
     except PackageNotFoundError:
         msg = "mqt-core not installed, installation required to access the include files."
         raise ImportError(msg) from None
 
 
 def cmake_dir() -> Path:
-    """Return the path to the mqt-core CMake module directory."""
+    """Return the path to the mqt-core CMake module directory.
+
+    Raises:
+        FileNotFoundError: If the CMake module directory is not found.
+        ImportError: If mqt-core is not installed.
+    """
     try:
         dist = distribution("mqt-core")
         located_cmake_dir = Path(dist.locate_file("mqt/core/share/cmake"))
         if located_cmake_dir.exists() and located_cmake_dir.is_dir():
             return located_cmake_dir
         msg = "mqt-core CMake files not found."
         raise FileNotFoundError(msg)
```

### Comparing `mqt_core-2.4.0/src/mqt/core/evaluation.py` & `mqt_core-2.4.1/src/mqt/core/evaluation.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     from os import PathLike
 
 # Avoid output truncation
 pd.set_option("display.max_colwidth", None)
 pd.set_option("display.max_rows", None)
 pd.set_option("display.width", None)
 
-sort_options = ["ratio", "algorithm"]
-higher_better_metrics = ["hits", "hit_ratio"]
+__sort_options = ["ratio", "algorithm"]
+__higher_better_metrics = ["hits", "hit_ratio"]
 
 
-class Bcolors:
+class _BColors:
     """Class for colored output in the terminal."""
 
     OKGREEN = "\033[92m"
     FAIL = "\033[91m"
     ENDC = "\033[0m"
 
 
@@ -38,28 +38,28 @@
         if isinstance(value, dict):
             items.update(__flatten_dict(value, new_key, sep=sep))
         else:
             items[new_key] = value
     return items
 
 
-class BenchmarkDict(TypedDict, total=False):
+class _BenchmarkDict(TypedDict, total=False):
     """A dictionary containing the data of one particular benchmark."""
 
     algo: str
     task: str
     n: int
     component: str
     metric: str
 
 
-def __post_processing(key: str) -> BenchmarkDict:
+def __post_processing(key: str) -> _BenchmarkDict:
     """Postprocess the key of a flattened dictionary to get the metrics for the DataFrame columns."""
     metrics_divided = key.split(".")
-    result_metrics = BenchmarkDict()
+    result_metrics = _BenchmarkDict()
     if len(metrics_divided) < 4:
         raise ValueError("Benchmark " + key + " is missing algorithm, task, number of qubits or metric!")
     result_metrics["algo"] = metrics_divided.pop(0)
     result_metrics["task"] = metrics_divided.pop(0)
     result_metrics["n"] = int(metrics_divided.pop(0))
     num_remaining_benchmarks = len(metrics_divided)
     if num_remaining_benchmarks == 1:
@@ -85,15 +85,15 @@
             if component.startswith("dd_"):
                 component = component[3:]
             result_metrics["component"] = component
 
     return result_metrics
 
 
-class DataDict(TypedDict):
+class _DataDict(TypedDict):
     """A dictionary containing the data for one entry in the DataFrame."""
 
     before: float
     after: float
     ratio: float
     algo: str
     task: str
@@ -139,25 +139,25 @@
         before = v[0]
         after = v[1]
         if math.isnan(before) or math.isnan(after):
             ratio = float("nan")
         else:
             ratio = after / before if before != 0 else 1 if after == 0 else math.inf
         key = k
-        if k.endswith(tuple(higher_better_metrics)):
+        if k.endswith(tuple(__higher_better_metrics)):
             ratio = 1 / ratio
             key += "*"
         before = round(before, 3) if isinstance(before, float) else before
         after = round(after, 3) if isinstance(after, float) else after
         ratio = round(ratio, 3)
         # postprocessing
         result_metrics = __post_processing(key)
 
         df_all_entries.append(
-            DataDict(
+            _DataDict(
                 before=before,
                 after=after,
                 ratio=ratio,
                 algo=result_metrics["algo"],
                 task=result_metrics["task"],
                 n=result_metrics["n"],
                 component=result_metrics["component"],
@@ -184,18 +184,18 @@
 
     if no_split:
         if only_changed:
             print(df[m1 | m2].sort_values(by=sort_indices).to_markdown(index=False, stralign="right"))
         print(df.sort_values(by=sort_indices).to_markdown(index=False, stralign="right"))
         return
 
-    print(f"\n{Bcolors.OKGREEN}Benchmarks that have improved:{Bcolors.ENDC}\n")
+    print(f"\n{_BColors.OKGREEN}Benchmarks that have improved:{_BColors.ENDC}\n")
     print(df[m1].sort_values(by=sort_indices).to_markdown(index=False, stralign="right"))
 
-    print(f"\n{Bcolors.FAIL}Benchmarks that have worsened:{Bcolors.ENDC}\n")
+    print(f"\n{_BColors.FAIL}Benchmarks that have worsened:{_BColors.ENDC}\n")
     print(df[m2].sort_values(by=sort_indices, ascending=False).to_markdown(index=False, stralign="right"))
 
     if only_changed:
         return
 
     print("\nBenchmarks that have stayed the same:\n")
     print(df[m3].sort_values(by=sort_indices).to_markdown(index=False, stralign="right"))
@@ -215,31 +215,31 @@
 ) -> None:
     """Compare the results of two benchmarking runs from the generated json file.
 
     Args:
         baseline_filepath: Path to the baseline json file.
         feature_filepath: Path to the feature json file.
         factor: How much a result has to change to be considered significant.
-        sort: Sort the table by this column. Valid options are "ratio" and "experiment".
+        sort: Sort the table by this column. Valid options are "ratio" and "algorithm".
         dd: Whether to show the detailed DD benchmark results.
         only_changed: Whether to only show results that changed significantly.
         no_split: Whether to merge all results together in one table or to separate the results into benchmarks that improved, stayed the same, or worsened.
         algorithm: Only show results for this algorithm.
         task: Only show results for this task.
         num_qubits: Only show results for this number of qubits. Can only be used if algorithm is also specified.
 
     Raises:
         ValueError: If factor is negative or sort is invalid or if num_qubits is specified while algorithm is not.
         FileNotFoundError: If the baseline_filepath argument or the feature_filepath argument does not point to a valid file.
-        JSONDecodeError: If the baseline_filepath argument or the feature_filepath argument points to a file that is not a valid JSON file.
+        json.JSONDecodeError: If the baseline_filepath argument or the feature_filepath argument points to a file that is not a valid JSON file.
     """
     if factor < 0:
         msg = "Factor must be positive!"
         raise ValueError(msg)
-    if sort not in sort_options:
+    if sort not in __sort_options:
         msg = "Invalid sort option! Valid options are 'ratio' and 'algorithm'."
         raise ValueError(msg)
     if algorithm is None and num_qubits is not None:
         msg = "num_qubits can only be specified if algorithm is also specified!"
         raise ValueError(msg)
 
     df_all = __aggregate(baseline_filepath, feature_filepath)
@@ -263,15 +263,33 @@
     print("\nDD Package details:")
     df_dd = df_all[df_all["metric"] != "runtime"]
     sort_indices = ["ratio"] if sort == "ratio" else ["algo", "task", "n", "component", "metric"]
     __print_results(df_dd, sort_indices, factor, no_split, only_changed)
 
 
 def main() -> None:
-    """Main function for the command line interface."""
+    """Main function for the command line interface.
+
+    This function is called when running the `mqt-core-compare` CLI command.
+
+    .. code-block:: bash
+
+        mqt-core-compare baseline.json feature.json [options]
+
+    In addition to the mandatory filepath arguments, it provides the following optional command line options:
+
+    - :code:`--factor <float>`: How much a result has to change to be considered significant.
+    - :code:`--sort`: Sort the table by this column. Valid options are 'ratio' and 'algorithm'.
+    - :code:`--dd`: Whether to show the detailed DD benchmark results.
+    - :code:`--only_changed`: Whether to only show results that changed significantly.
+    - :code:`--no_split`: Whether to merge all results together in one table or to separate the results into benchmarks that improved, stayed the same, or worsened.
+    - :code:`--algorithm <str>`: Only show results for this algorithm.
+    - :code:`--task <str>`: Only show results for this task.
+    - :code:`--num_qubits <int>`: Only show results for this number of qubits. Can only be used if algorithm is also specified.
+    """
     parser = argparse.ArgumentParser(
         description="Compare the results of two benchmarking runs from the generated json files."
     )
     parser.add_argument("baseline_filepath", type=str, help="Path to the baseline json file.")
     parser.add_argument("feature_filepath", type=str, help="Path to the feature json file.")
     parser.add_argument(
         "--factor", type=float, default=0.1, help="How much a result has to change to be considered significant."
```

### Comparing `mqt_core-2.4.0/src/mqt/core/io.py` & `mqt_core-2.4.1/src/mqt/core/io.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from . import QuantumComputation
 
 if TYPE_CHECKING:
     from qiskit.circuit import QuantumCircuit
 
 
 def load(input_circuit: QuantumComputation | str | PathLike[str] | QuantumCircuit) -> QuantumComputation:
-    """Load a quantum circuit from any supported format as a ``QuantumComputation``.
+    """Load a quantum circuit from any supported format as a :class:`~mqt.core.QuantumComputation`.
 
     Args:
-        input_circuit: The input circuit to translate to a ``QuantumComputation``. This can be a `QuantumComputation` itself, a file name to any of the supported file formats, an OpenQASM (2.0 or 3.0) string, or a Qiskit `QuantumCircuit`.
+        input_circuit: The input circuit to translate to a :class:`~mqt.core.QuantumComputation`. This can be a :class:`~mqt.core.QuantumComputation` itself, a file name to any of the supported file formats, an OpenQASM (2.0 or 3.0) string, or a Qiskit :class:`~qiskit.circuit.QuantumCircuit`.
 
     Returns:
-        The ``QuantumComputation``.
+        The :class:`~mqt.core.QuantumComputation`.
 
     Raises:
-        ValueError: If the input circuit is a Qiskit `QuantumCircuit` but the `qiskit` extra is not installed.
+        ValueError: If the input circuit is a Qiskit :class:`~qiskit.circuit.QuantumCircuit` but the `qiskit` extra is not installed.
         FileNotFoundError: If the input circuit is a file name and the file does not exist.
     """
     if isinstance(input_circuit, QuantumComputation):
         return input_circuit
 
     if isinstance(input_circuit, (str, PathLike)):
         if not Path(input_circuit).is_file():
```

### Comparing `mqt_core-2.4.0/src/mqt/core/operations.py` & `mqt_core-2.4.1/src/mqt/core/operations.py`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/mqt/core/plugins/qiskit.py` & `mqt_core-2.4.1/src/mqt/core/plugins/qiskit.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 if TYPE_CHECKING:
     from collections.abc import Mapping, Sequence
 
     from qiskit.circuit import QuantumCircuit
 
 
 def qiskit_to_mqt(circ: QuantumCircuit) -> QuantumComputation:
-    """Convert a Qiskit `QuantumCircuit` to a `QuantumComputation` object.
+    """Convert a Qiskit :class:`~qiskit.circuit.QuantumCircuit` to a :class:`~mqt.core.QuantumComputation` object.
 
     Args:
         circ: The Qiskit circuit to convert.
 
     Returns:
         The converted circuit.
     """
@@ -355,17 +355,15 @@
         qc.append(SymbolicOperation(controls, target1, target2, type_, parameters))
     else:
         qc.append(StandardOperation(controls, target1, target2, type_, cast(List[float], parameters)))
     return parameters
 
 
 def _import_layouts(qc: QuantumComputation, circ: QuantumCircuit) -> None:
-    # qiskit-terra 0.24.0 added a (public) `layout` attribute
-    layout = circ.layout if hasattr(circ, "layout") else circ._layout  # noqa: SLF001
-
+    layout = circ.layout
     initial_layout = layout.initial_layout
 
     # The following creates a map of virtual qubits in the layout to an integer index.
     # Using the `get_virtual_bits()` method of the layout guarantees that the order
     # of the qubits is the same as in the original circuit. In contrast, the
     # `get_registers()` method does not guarantee this as it returns a set that
     # reorders the qubits.
@@ -382,22 +380,23 @@
         for qubit in reversed(register):
             qc.set_circuit_qubit_ancillary(qubit_to_idx[qubit])
 
     # create initial layout (and assume identical output permutation)
     for device_qubit, circuit_qubit in initial_layout.get_physical_bits().items():
         idx = qubit_to_idx[circuit_qubit]
         qc.initial_layout[device_qubit] = idx
-        qc.output_permutation[device_qubit] = idx
 
-    if not hasattr(layout, "final_layout"):
+    if layout.final_layout is None:
+        qc.output_permutation = qc.initial_layout
         return
 
-    final_layout = layout.final_layout
-    if final_layout is None:
-        return
+    # final_index_layout creates a list of final positions for input circuit qubits
+    final_index_layout = layout.final_index_layout(filter_ancillas=False)
+    for idx, value in enumerate(final_index_layout):
+        qc.output_permutation[value] = idx
 
 
 def _import_definition(
     qc: QuantumComputation | CompoundOperation,
     circ: QuantumCircuit,
     qargs: Sequence[Qubit],
     cargs: Sequence[Clbit],
@@ -416,7 +415,10 @@
         mapped_cargs = [carg_map[carg] for carg in c_args]
         instruction_params = instruction.params
         new_params = _emplace_operation(
             comp_op, instruction, mapped_qargs, mapped_cargs, instruction_params, qubit_map, clbit_map
         )
         params.extend(new_params)
     return params
+
+
+__all__ = ["qiskit_to_mqt"]
```

### Comparing `mqt_core-2.4.0/src/operations/ClassicControlledOperation.cpp` & `mqt_core-2.4.1/src/operations/ClassicControlledOperation.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/operations/CompoundOperation.cpp` & `mqt_core-2.4.1/src/operations/CompoundOperation.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,21 @@
 void CompoundOperation::invert() {
   for (auto& op : ops) {
     op->invert();
   }
   std::reverse(ops.begin(), ops.end());
 }
 
+void CompoundOperation::apply(const Permutation& permutation) {
+  Operation::apply(permutation);
+  for (auto& op : ops) {
+    op->apply(permutation);
+  }
+}
+
 void CompoundOperation::merge(CompoundOperation& op) {
   ops.reserve(ops.size() + op.size());
   ops.insert(ops.end(), std::make_move_iterator(op.begin()),
              std::make_move_iterator(op.end()));
   op.clear();
 }
```

### Comparing `mqt_core-2.4.0/src/operations/NonUnitaryOperation.cpp` & `mqt_core-2.4.1/src/operations/NonUnitaryOperation.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -188,8 +188,12 @@
 
 void NonUnitaryOperation::addDepthContribution(
     std::vector<std::size_t>& depths) const {
   for (const auto& target : getTargets()) {
     depths[target] += 1;
   }
 }
+
+void NonUnitaryOperation::apply(const Permutation& permutation) {
+  getTargets() = permutation.apply(getTargets());
+}
 } // namespace qc
```

### Comparing `mqt_core-2.4.0/src/operations/Operation.cpp` & `mqt_core-2.4.1/src/operations/Operation.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include "operations/Operation.hpp"
 
 #include <algorithm>
+#include <cassert>
 
 namespace qc {
 
 std::ostream& Operation::printParameters(std::ostream& os) const {
   if (isClassicControlledOperation()) {
     os << "  c[" << parameter[0];
     if (parameter[1] != 1) {
@@ -171,8 +172,13 @@
     depths[target] = maxDepth;
   }
   for (const auto& control : getControls()) {
     depths[control.qubit] = maxDepth;
   }
 }
 
+void Operation::apply(const Permutation& permutation) {
+  getTargets() = permutation.apply(getTargets());
+  getControls() = permutation.apply(getControls());
+}
+
 } // namespace qc
```

### Comparing `mqt_core-2.4.0/src/operations/StandardOperation.cpp` & `mqt_core-2.4.1/src/operations/StandardOperation.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/operations/SymbolicOperation.cpp` & `mqt_core-2.4.1/src/operations/SymbolicOperation.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/GRCSParser.cpp` & `mqt_core-2.4.1/src/parsers/GRCSParser.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/QASM3Parser.cpp` & `mqt_core-2.4.1/src/parsers/QASM3Parser.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/QCParser.cpp` & `mqt_core-2.4.1/src/parsers/QCParser.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -132,16 +132,15 @@
       varMap.insert({var, qidx++});
     } else {
       if (!constants.empty()) {
         if (constants.at(constidx - inputs.size()) == "0" ||
             constants.at(constidx - inputs.size()) == "1") {
           // add X operation in case of initial value 1
           if (constants.at(constidx - inputs.size()) == "1") {
-            emplace_back<StandardOperation>(nqubits + nancillae,
-                                            static_cast<Qubit>(constidx), X);
+            x(static_cast<Qubit>(constidx));
           }
           varMap.insert({var, static_cast<Qubit>(constidx++)});
         } else {
           throw QFRException("[qc parser] l:" + std::to_string(line) +
                              " msg: Non-binary constant specified: " + cmd);
         }
       } else {
```

### Comparing `mqt_core-2.4.0/src/parsers/RealParser.cpp` & `mqt_core-2.4.1/src/parsers/RealParser.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/TFCParser.cpp` & `mqt_core-2.4.1/src/parsers/TFCParser.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/qasm3_parser/Parser.cpp` & `mqt_core-2.4.1/src/parsers/qasm3_parser/Parser.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/qasm3_parser/Scanner.cpp` & `mqt_core-2.4.1/src/parsers/qasm3_parser/Scanner.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/qasm3_parser/Statement.cpp` & `mqt_core-2.4.1/src/parsers/qasm3_parser/Statement.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/qasm3_parser/Types.cpp` & `mqt_core-2.4.1/src/parsers/qasm3_parser/Types.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/qasm3_parser/passes/ConstEvalPass.cpp` & `mqt_core-2.4.1/src/parsers/qasm3_parser/passes/ConstEvalPass.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/parsers/qasm3_parser/passes/TypeCheckPass.cpp` & `mqt_core-2.4.1/src/parsers/qasm3_parser/passes/TypeCheckPass.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/python/CMakeLists.txt` & `mqt_core-2.4.1/src/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/python/module.cpp` & `mqt_core-2.4.1/src/python/module.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/python/operations/register_classic_controlled_operation.cpp` & `mqt_core-2.4.1/src/python/operations/register_classic_controlled_operation.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 #include "operations/ClassicControlledOperation.hpp"
 #include "python/pybind11.hpp"
 
 namespace mqt {
 
 void registerClassicControlledOperation(py::module& m) {
   auto ccop = py::class_<qc::ClassicControlledOperation, qc::Operation>(
-      m, "ClassicControlledOperation",
-      "Quantum operation controlled by classical results.");
+      m, "ClassicControlledOperation");
 
   ccop.def(
       py::init([](qc::Operation* operation, qc::ClassicalRegister controlReg,
                   std::uint64_t expectedVal) {
         auto op = operation->clone();
         return std::make_unique<qc::ClassicControlledOperation>(op, controlReg,
                                                                 expectedVal);
       }),
-      "operation"_a, "control_register"_a, "expected_value"_a = 1U,
-      "Applies operation if the control register has the expected value.");
+      "operation"_a, "control_register"_a, "expected_value"_a = 1U);
+  ccop.def_property_readonly("operation",
+                             &qc::ClassicControlledOperation::getOperation,
+                             py::return_value_policy::reference_internal);
   ccop.def_property_readonly(
-      "operation", &qc::ClassicControlledOperation::getOperation,
-      "Returns the operation controlled by the classical register.",
-      py::return_value_policy::reference_internal);
-  ccop.def_property_readonly(
-      "control_register", &qc::ClassicControlledOperation::getControlRegister,
-      "Returns the classical register controlling the operation.");
-  ccop.def_property_readonly(
-      "expected_value", &qc::ClassicControlledOperation::getExpectedValue,
-      "Returns the expected value of the classical register.");
+      "control_register", &qc::ClassicControlledOperation::getControlRegister);
+  ccop.def_property_readonly("expected_value",
+                             &qc::ClassicControlledOperation::getExpectedValue);
   ccop.def("__repr__", [](const qc::ClassicControlledOperation& op) {
     std::stringstream ss;
     const auto& controlReg = op.getControlRegister();
     ss << "ClassicControlledOperation(<...op...>, " << "control_register=("
        << controlReg.first << ", " << controlReg.second << "), "
        << "expected_value=" << op.getExpectedValue() << ")";
     return ss.str();
```

### Comparing `mqt_core-2.4.0/src/python/operations/register_compound_operation.cpp` & `mqt_core-2.4.1/src/python/operations/register_compound_operation.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -13,38 +13,33 @@
     }
     if (i < 0 || static_cast<SizeType>(i) >= size) {
       throw py::index_error();
     }
     return i;
   };
 
-  py::class_<qc::CompoundOperation, qc::Operation>(
-      m, "CompoundOperation",
-      "Quantum operation comprised of multiple sub-operations.")
-      .def(py::init<>(), "Create an empty compound operation.")
+  py::class_<qc::CompoundOperation, qc::Operation>(m, "CompoundOperation")
+      .def(py::init<>())
       .def(py::init([](std::vector<qc::Operation*>& ops) {
              std::vector<std::unique_ptr<qc::Operation>> uniqueOps;
              uniqueOps.reserve(ops.size());
              for (auto& op : ops) {
                uniqueOps.emplace_back(op->clone());
              }
              return qc::CompoundOperation(std::move(uniqueOps));
            }),
-           "ops"_a, "Create a compound operation from a list of operations.")
-      .def("__len__", &qc::CompoundOperation::size,
-           "Return number of sub-operations.")
+           "ops"_a)
+      .def("__len__", &qc::CompoundOperation::size)
       .def(
           "__getitem__",
           [&wrap](const qc::CompoundOperation& op, DiffType i) {
             i = wrap(i, op.size());
             return op.at(static_cast<SizeType>(i)).get();
           },
-          py::return_value_policy::reference_internal, "i"_a,
-          "Return i-th sub-operation. Beware: this gives write access to the "
-          "sub-operation.")
+          py::return_value_policy::reference_internal, "i"_a)
       .def(
           "__getitem__",
           [](qc::CompoundOperation& op, const py::slice& slice) {
             std::size_t start{};
             std::size_t stop{};
             std::size_t step{};
             std::size_t sliceLength{};
@@ -54,23 +49,21 @@
             auto ops = std::vector<qc::Operation*>();
             ops.reserve(sliceLength);
             for (std::size_t i = start; i < stop; i += step) {
               ops.emplace_back(op.at(i).get());
             }
             return ops;
           },
-          py::return_value_policy::reference_internal, "slice"_a,
-          "Return a slice of the compound operation. Beware: this gives write "
-          "access to the sub-operations.")
+          py::return_value_policy::reference_internal, "slice"_a)
       .def(
           "append",
           [](qc::CompoundOperation& compOp, const qc::Operation& op) {
             compOp.emplace_back(op.clone());
           },
-          "op"_a, "Append operation op to the `CompoundOperation`.")
+          "op"_a)
       .def("empty", &qc::CompoundOperation::empty)
       .def("__repr__", [](const qc::CompoundOperation& op) {
         std::stringstream ss;
         ss << "CompoundOperation([..." << op.size() << " ops...])";
         return ss.str();
       });
 }
```

### Comparing `mqt_core-2.4.0/src/python/operations/register_control.cpp` & `mqt_core-2.4.1/src/python/operations/register_control.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #include "operations/Control.hpp"
+#include "pybind11/operators.h"
 #include "python/pybind11.hpp"
 
 namespace mqt {
 
 void registerControl(py::module& m) {
 
   auto control = py::class_<qc::Control>(m, "Control");
@@ -24,20 +25,19 @@
   controlType.def("__bool__", [](const qc::Control::Type& type) {
     return type == qc::Control::Type::Pos;
   });
   py::implicitly_convertible<py::bool_, qc::Control::Type>();
   py::implicitly_convertible<py::str, qc::Control::Type>();
 
   control.def(py::init<qc::Qubit, qc::Control::Type>(), "qubit"_a,
-              "type_"_a = qc::Control::Type::Pos,
-              "Create a control qubit of the specified control type.");
-  control.def_readwrite(
-      "type_", &qc::Control::type,
-      "The type of the control qubit. Can be positive or negative.");
-  control.def_readwrite("qubit", &qc::Control::qubit,
-                        "The qubit index of the control qubit.");
+              "type_"_a = qc::Control::Type::Pos);
+  control.def_readwrite("type_", &qc::Control::type);
+  control.def_readwrite("qubit", &qc::Control::qubit);
   control.def("__str__", [](const qc::Control& c) { return c.toString(); });
   control.def("__repr__", [](const qc::Control& c) { return c.toString(); });
+  control.def(py::self == py::self);
+  control.def(py::self != py::self);
+  control.def(hash(py::self));
   py::implicitly_convertible<py::int_, qc::Control>();
 }
 
 } // namespace mqt
```

### Comparing `mqt_core-2.4.0/src/python/operations/register_non_unitary_operation.cpp` & `mqt_core-2.4.1/src/python/operations/register_non_unitary_operation.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,22 @@
 #include "operations/NonUnitaryOperation.hpp"
 #include "python/pybind11.hpp"
 
 namespace mqt {
 
 void registerNonUnitaryOperation(py::module& m) {
-  py::class_<qc::NonUnitaryOperation, qc::Operation>(
-      m, "NonUnitaryOperation",
-      "Non-unitary operations such as measurements and resets.")
+  py::class_<qc::NonUnitaryOperation, qc::Operation>(m, "NonUnitaryOperation")
       .def(py::init<std::vector<qc::Qubit>, std::vector<qc::Bit>>(),
-           "targets"_a, "classics"_a,
-           "Create a multi-qubit measurement operation.")
-      .def(py::init<qc::Qubit, qc::Bit>(), "target"_a, "classic"_a,
-           "Create a measurement operation that measures `target` into "
-           "`classic`.")
+           "targets"_a, "classics"_a)
+      .def(py::init<qc::Qubit, qc::Bit>(), "target"_a, "classic"_a)
       .def(py::init<std::vector<qc::Qubit>, qc::OpType>(), "targets"_a,
-           "op_type"_a = qc::OpType::Reset,
-           "Create a multi-qubit reset operation.")
+           "op_type"_a = qc::OpType::Reset)
       .def_property_readonly(
-          "classics",
-          py::overload_cast<>(&qc::NonUnitaryOperation::getClassics,
-                              py::const_),
-          "Return the classical bits.")
+          "classics", py::overload_cast<>(&qc::NonUnitaryOperation::getClassics,
+                                          py::const_))
       .def("__repr__", [](const qc::NonUnitaryOperation& op) {
         std::stringstream ss;
         ss << "NonUnitaryOperation(";
         const auto& targets = op.getTargets();
         if (targets.size() == 1U) {
           ss << "target=" << targets[0];
         } else {
```

### Comparing `mqt_core-2.4.0/src/python/operations/register_optype.cpp` & `mqt_core-2.4.1/src/python/operations/register_optype.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #include "operations/OpType.hpp"
 #include "python/pybind11.hpp"
 
 namespace mqt {
 
 void registerOptype(py::module& m) {
-  py::enum_<qc::OpType>(
-      m, "OpType",
-      "Enum class for representing the type of quantum operations.")
+  py::enum_<qc::OpType>(m, "OpType")
       .value("none", qc::OpType::None)
       .value("gphase", qc::OpType::GPhase)
       .value("i", qc::OpType::I)
       .value("h", qc::OpType::H)
       .value("x", qc::OpType::X)
       .value("y", qc::OpType::Y)
       .value("z", qc::OpType::Z)
```

### Comparing `mqt_core-2.4.0/src/python/qiskit/QuantumCircuit.cpp` & `mqt_core-2.4.1/src/python/qiskit/QuantumCircuit.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/python/register_operations.cpp` & `mqt_core-2.4.1/src/python/register_operations.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/python/register_permutation.cpp` & `mqt_core-2.4.1/src/python/register_permutation.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 #include "Permutation.hpp"
+#include "pybind11/operators.h"
 #include "python/pybind11.hpp"
 
 namespace mqt {
 
 void registerPermutation(py::module& m) {
-  py::class_<qc::Permutation>(m, "Permutation",
-                              "Class representing a permutation of qubits.")
+  py::class_<qc::Permutation>(m, "Permutation")
       .def(py::init([](const py::dict& p) {
              qc::Permutation perm;
              for (const auto& [key, value] : p) {
                perm[key.cast<qc::Qubit>()] = value.cast<qc::Qubit>();
              }
              return perm;
            }),
            "perm"_a, "Create a permutation from a dictionary.")
       .def("apply",
            py::overload_cast<const qc::Controls&>(&qc::Permutation::apply,
                                                   py::const_),
-           "controls"_a,
-           "Apply the permutation to a set of controls and return the permuted "
-           "controls.")
+           "controls"_a)
       .def("apply",
            py::overload_cast<const qc::Targets&>(&qc::Permutation::apply,
                                                  py::const_),
-           "targets"_a,
-           "Apply the permutation to a set of targets and return the permuted "
-           "targets.")
+           "targets"_a)
       .def("__getitem__",
            [](const qc::Permutation& p, const qc::Qubit q) { return p.at(q); })
       .def("__setitem__", [](qc::Permutation& p, const qc::Qubit q,
                              const qc::Qubit r) { p.at(q) = r; })
       .def("__delitem__",
            [](qc::Permutation& p, const qc::Qubit q) { p.erase(q); })
       .def("__len__", &qc::Permutation::size)
       .def(
           "__iter__",
           [](const qc::Permutation& p) {
             return py::make_iterator(p.begin(), p.end());
           },
           py::keep_alive<0, 1>())
+      .def(py::self == py::self)
+      .def(py::self != py::self)
+      .def(hash(py::self))
       .def("__str__",
            [](const qc::Permutation& p) {
              std::stringstream ss;
              ss << "{";
              for (const auto& [k, v] : p) {
                ss << k << ": " << v << ", ";
              }
@@ -54,10 +53,11 @@
         ss << "Permutation({";
         for (const auto& [k, v] : p) {
           ss << k << ": " << v << ", ";
         }
         ss << "})";
         return ss.str();
       });
+  py::implicitly_convertible<py::dict, qc::Permutation>();
 }
 
 } // namespace mqt
```

### Comparing `mqt_core-2.4.0/src/zx/CMakeLists.txt` & `mqt_core-2.4.1/src/zx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/zx/FunctionalityConstruction.cpp` & `mqt_core-2.4.1/src/zx/FunctionalityConstruction.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/zx/Rational.cpp` & `mqt_core-2.4.1/src/zx/Rational.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/zx/Rules.cpp` & `mqt_core-2.4.1/src/zx/Rules.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/zx/Simplify.cpp` & `mqt_core-2.4.1/src/zx/Simplify.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/zx/Utils.cpp` & `mqt_core-2.4.1/src/zx/Utils.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/src/zx/ZXDiagram.cpp` & `mqt_core-2.4.1/src/zx/ZXDiagram.cpp`

 * *Files identical despite different names*

### Comparing `mqt_core-2.4.0/PKG-INFO` & `mqt_core-2.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mqt-core
-Version: 2.4.0
+Version: 2.4.1
 Summary: The Backbone of the Munich Quantum Toolkit
-Keywords: MQT quantum-computing design-automation decision-diagrams zx-calculus
+Keywords: MQT,quantum-computing,design-automation,decision-diagrams,zx-calculus
 Author-Email: Lukas Burgholzer <burgholzer@me.com>
 License: MIT License
         
-        Copyright (c) 2023 Chair for Design Automation, Technical University of Munich, Germany
+        Copyright (c) 2024 Chair for Design Automation, Technical University of Munich, Germany
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use,
         copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all
         copies or substantial portions of the Software.
         
@@ -55,25 +55,24 @@
 Requires-Dist: mqt.core[evaluation,qiskit]; extra == "test"
 Requires-Dist: mqt.core[test]; extra == "coverage"
 Requires-Dist: pytest-cov>=4; extra == "coverage"
 Requires-Dist: pandas[output_formatting]>=2.0; python_version < "3.9" and extra == "evaluation"
 Requires-Dist: pandas[output-formatting]>=2.1.2; python_version >= "3.9" and extra == "evaluation"
 Requires-Dist: furo>=2023.08.17; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: myst_parser>=0.13; extra == "docs"
+Requires-Dist: myst_nb>=1.1.0; extra == "docs"
 Requires-Dist: setuptools-scm>=7; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx_design; extra == "docs"
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex>=2.4.2; extra == "docs"
+Requires-Dist: sphinxcontrib-svg2pdfconverter; extra == "docs"
 Requires-Dist: pybtex>=0.24; extra == "docs"
 Requires-Dist: ipython; extra == "docs"
 Requires-Dist: ipykernel; extra == "docs"
-Requires-Dist: nbsphinx; extra == "docs"
-Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-autoapi; extra == "docs"
 Requires-Dist: qiskit[visualization]; extra == "docs"
 Requires-Dist: mqt.core[evaluation]; extra == "docs"
 Requires-Dist: qiskit[qasm3-import]>=1.0.0; extra == "qiskit"
 Requires-Dist: mqt.core[coverage,docs]; extra == "dev"
 Description-Content-Type: text/markdown
 
@@ -82,47 +81,41 @@
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 [![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-core/ci.yml?branch=main&style=flat-square&logo=github&label=ci)](https://github.com/cda-tum/mqt-core/actions/workflows/ci.yml)
 [![CD](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-core/cd.yml?style=flat-square&logo=github&label=cd)](https://github.com/cda-tum/mqt-core/actions/workflows/cd.yml)
 [![Documentation](https://img.shields.io/readthedocs/mqt-core?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/core)
 [![codecov](https://img.shields.io/codecov/c/github/cda-tum/mqt-core?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/mqt-core)
 
 <p align="center">
- <picture>
-   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/mqt_light.png" width="60%">
-   <img src="https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/mqt_dark.png" width="60%">
- </picture>
+  <a href="https://mqt.readthedocs.io">
+   <picture>
+     <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/mqt_light.png" width="60%">
+     <img src="https://raw.githubusercontent.com/cda-tum/mqt-core/main/docs/_static/mqt_dark.png" width="60%">
+   </picture>
+  </a>
 </p>
 
 # MQT Core - The Backbone of the Munich Quantum Toolkit (MQT)
 
-The MQT Core library forms the backbone of the quantum software tools developed as part of the _Munich Quantum Toolkit_ (_MQT_) by the [Chair for Design Automation](https://www.cda.cit.tum.de/) at the [Technical University of Munich](https://www.tum.de/). This includes the following tools:
-
-- [MQT DDSIM](https://github.com/cda-tum/mqt-ddsim): A Tool for Classical Quantum Circuit Simulation based on Decision Diagrams.
-- [MQT QMAP](https://github.com/cda-tum/mqt-qmap): A Tool for Quantum Circuit Mapping.
-- [MQT QCEC](https://github.com/cda-tum/mqt-qcec): A Tool for Quantum Circuit Equivalence Checking.
-- [MQT QECC](https://github.com/cda-tum/mqt-qecc): A Tool for Quantum Error Correcting Codes.
-- [MQT DDVis](https://github.com/cda-tum/mqt-ddvis): A Web-Application visualizing Decision Diagrams for Quantum Computing.
-- [MQT SyReC](https://github.com/cda-tum/mqt-syrec): A Tool for Synthesis of Reversible Circuits/Quantum Computing Oracles.
-
-For a full list of tools and libraries, please visit the [MQT website](https://mqt.readthedocs.io/).
+MQT Core is an open-source C++17 and Python library for quantum computing that forms the backbone of the quantum software tools developed as part of the [_Munich Quantum Toolkit_ (_MQT_)](https://mqt.readthedocs.io) by the [Chair for Design Automation](https://www.cda.cit.tum.de/) at the [Technical University of Munich](https://www.tum.de/).
+To this end, it consists of multiple components that are used throughout the MQT, including a fully fledged intermediate representation (IR) for quantum computations, a state-of-the-art decision diagram (DD) package for quantum computing, and a dedicated ZX-diagram package for working with the ZX-calculus.
 
 <p align="center">
   <a href="https://mqt.readthedocs.io/projects/core">
   <img width=30% src="https://img.shields.io/badge/documentation-blue?style=for-the-badge&logo=read%20the%20docs" alt="Documentation" />
   </a>
 </p>
 
 If you have any questions, feel free to create a [discussion](https://github.com/cda-tum/mqt-core/discussions) or an [issue](https://github.com/cda-tum/mqt-core/issues) on [GitHub](https://github.com/cda-tum/mqt-core).
 
 ## Getting Started
 
 `mqt.core` is available via [PyPI](https://pypi.org/project/mqt.core/) for all major operating systems and supports Python 3.8 to 3.12.
 
 ```console
-(venv) $ pip install mqt.core
+(.venv) $ pip install mqt.core
 ```
 
 The following code gives an example on the usage:
 
 ```python3
 from mqt.core import QuantumComputation
 
@@ -132,28 +125,14 @@
 qc.measure(range(2), range(2))
 
 print(qc)
 ```
 
 **Detailed documentation and examples are available at [ReadTheDocs](https://mqt.readthedocs.io/projects/core).**
 
-## Library Overview
-
-<!-- SPHINX-START -->
-
-MQT Core encompasses:
-
-- `MQT::Core`: An intermediate representation (IR) for quantum computations including means to import and export circuits in various formats.
-- `MQT::CoreDD`: A fully-fledged decision diagram (DD) library for quantum computing.
-- `MQT::CoreZX`: A library for working with ZX-diagrams and the ZX-calculus.
-- `MQT::CoreECC`: A library for working with error correcting codes (ECCs) for quantum computing.
-- `MQT::CorePython`: A Python interface for the MQT Core library (e.g., facilitating the import of Qiskit QuantumCircuits).
-
-<!-- SPHINX-END -->
-
 ## System Requirements
 
 Building (and running) is continuously tested under Linux, MacOS, and Windows using the [latest available system versions for GitHub Actions](https://github.com/actions/runner-images).
 However, the implementation should be compatible with any current C++ compiler supporting C++17 and a minimum CMake version of 3.19.
 
 MQT Core relies on some external dependencies:
```

