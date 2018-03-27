# VertxBufferWriteBench
Tests writes to Vertx Buffer with undersized and oversized buffer size

Results:
```
Benchmark                             (initialCapacity)   Mode   Samples         Mean   Mean error    Units
Benchmark                             (initialCapacity)   Mode   Samples         Mean   Mean error    Units
o.s.MyBenchmark.testOutOfLimitLimit                1024   avgt        15     6215.471      205.501    ns/op
o.s.MyBenchmark.testOutOfLimitLimit                2048   avgt        15    12388.545      209.285    ns/op
o.s.MyBenchmark.testOutOfLimitLimit                4096   avgt        15    24305.648     1335.379    ns/op
o.s.MyBenchmark.testOutOfLimitLimit                8192   avgt        15    41826.354     7310.396    ns/op
o.s.MyBenchmark.testOutOfLimitLimit               16384   avgt        15    61848.759     2031.296    ns/op
o.s.MyBenchmark.testWithInLimit                    1024   avgt        15     4151.396      104.554    ns/op
o.s.MyBenchmark.testWithInLimit                    2048   avgt        15     8453.334      244.082    ns/op
o.s.MyBenchmark.testWithInLimit                    4096   avgt        15    16318.144      333.417    ns/op
o.s.MyBenchmark.testWithInLimit                    8192   avgt        15    32161.362     1604.270    ns/op
o.s.MyBenchmark.testWithInLimit                   16384   avgt        15    58428.859      516.533    ns/op
```

To run:
mvn clean install
java -jar target/microbenchmarks.jar

