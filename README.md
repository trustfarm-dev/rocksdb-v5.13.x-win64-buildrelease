# rocksdb-2.7-win64-buildrelease

Build on MS Visual Studio 2017 x64 targets.

[[https://github.com/facebook/rocksdb/wiki/Building-on-Windows ||RocksDB Wiki]] how to build on windows is a little bit outdated.
And CMake scripts also not run well on CLI.

Giggs on googling and many other resources helps to build this release.

Final output's included this repository.

All library and executables built on MSVS 2017 v141 build toolkit. regardless of directory names.

rocksdb/
rocksdb/build/release 
```
==== list of zipped files ====

Archive:  release_pack.zip
  Length      Date    Time    Name
---------  ---------- -----   ----
  4910180  2018-04-23 21:58   rocksdb-2.7-win64-release/gflags-2.2.1/target/lib/Debug/gflags_nothreads_static.lib
  4909478  2018-04-23 21:58   rocksdb-2.7-win64-release/gflags-2.2.1/target/lib/Debug/gflags_static.lib
   906434  2018-04-23 21:59   rocksdb-2.7-win64-release/gflags-2.2.1/target/lib/Release/gflags_nothreads_static.lib
   912128  2018-04-23 21:59   rocksdb-2.7-win64-release/gflags-2.2.1/target/lib/Release/gflags_static.lib
    14336  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/datagen.exe
    69632  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/frametest.exe
    66560  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/fullbench.exe
    22528  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/fullbench-dll.exe
    74240  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/fuzzer.exe
    66048  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/liblz4.dll
    12428  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/liblz4.lib
   219526  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/liblz4_static.lib
    94208  2018-04-23 22:40   rocksdb-2.7-win64-release/lz4-1.7.5/visual/VS2010/bin/x64_Release/lz4.exe
  5468672  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/cache_bench.exe
     9084  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/cache_bench.lib
  5622272  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/column_aware_encoding_exp.exe
     9790  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/column_aware_encoding_exp.lib
  6560256  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/db_bench.exe
     8952  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/db_bench.lib
   384000  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/hash_table_bench.exe
    66048  2018-04-23 22:40   rocksdb-2.7-win64-release/rocksdb/build/Release/liblz4.dll
  5639168  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/memtablerep_bench.exe
     9430  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/memtablerep_bench.lib
184105568  2018-04-23 23:02   rocksdb-2.7-win64-release/rocksdb/build/Release/rocksdb.lib
  7840768  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/rocksdb-shared.dll
   144686  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/rocksdb-shared.lib
   335360  2018-04-23 22:11   rocksdb-2.7-win64-release/rocksdb/build/Release/snappy64.dll
  5559296  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/table_reader_bench.exe
     9476  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/Release/table_reader_bench.lib
   114176  2018-04-23 22:29   rocksdb-2.7-win64-release/rocksdb/build/Release/zlibwapi.dll
   121038  2018-04-23 22:53   rocksdb-2.7-win64-release/rocksdb/build/testharness.dir/Release/testharness.lib
  4014776  2018-04-23 22:53   rocksdb-2.7-win64-release/rocksdb/build/third-party/gtest-1.7.0/fused-src/gtest/Release/gtest.lib
  5293056  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/db_repl_stress.exe
     9296  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/db_repl_stress.lib
  5042176  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/db_sanity_test.exe
     9296  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/db_sanity_test.lib
  5454336  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/db_stress.exe
     8996  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/db_stress.lib
  5833728  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/ldb.exe
     8732  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/ldb.lib
    66048  2018-04-23 22:40   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/liblz4.dll
  5223936  2018-04-23 23:05   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/rocksdb_dump.exe
     9206  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/rocksdb_dump.lib
  5223936  2018-04-23 23:05   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/rocksdb_undump.exe
     9296  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/rocksdb_undump.lib
   335360  2018-04-23 22:11   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/snappy64.dll
  5817856  2018-04-23 23:05   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/sst_dump.exe
     8952  2018-04-23 23:05   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/sst_dump.lib
  5159424  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/write_stress.exe
     9206  2018-04-23 23:04   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/write_stress.lib
   114176  2018-04-23 22:29   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/zlibwapi.dll
    26192  2018-04-23 22:29   rocksdb-2.7-win64-release/rocksdb/build/tools/Release/zlibwapi.lib
    80896  2018-04-23 22:11   rocksdb-2.7-win64-release/snappy-visual-cpp/x64/Release/packagetest.exe
    10752  2018-04-23 22:11   rocksdb-2.7-win64-release/snappy-visual-cpp/x64/Release/runtests.exe
    32768  2018-04-23 22:11   rocksdb-2.7-win64-release/snappy-visual-cpp/x64/Release/singlefiletest.exe
   335360  2018-04-23 22:11   rocksdb-2.7-win64-release/snappy-visual-cpp/x64/Release/snappy64.dll
     6998  2018-04-23 22:11   rocksdb-2.7-win64-release/snappy-visual-cpp/x64/Release/snappy64.lib
    16384  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/MiniUnzipRelease/miniunz.exe
    13824  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/Release/minizip.exe
    12288  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/TestZlibDllRelease/testzlibdll.exe
    67072  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/TestZlibRelease/testzlib.exe
   114176  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/ZlibDllRelease/zlibwapi.dll
    26192  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/ZlibDllRelease/zlibwapi.lib
   760748  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/ZlibStatRelease/zlibstat.lib
   114176  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/ZlibStatRelease/zlibwapi.dll
    26192  2018-04-23 22:29   rocksdb-2.7-win64-release/zlib-1.2.11/contrib/vstudio/vc14/x64/ZlibStatRelease/zlibwapi.lib
---------                     -------
283581572                     66 files
```
