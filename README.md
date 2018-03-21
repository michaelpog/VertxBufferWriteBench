# VertxBufferWriteBench
Tests writes to Vertx Buffer with undersized and oversized buffer size

Results:

Benchmark                             (initialCapacity)   Mode   Samples         Mean   Mean error    Units
o.s.MyBenchmark.testOutOfLimitLimit                1024   avgt        15    11166.683      707.722    ns/op
o.s.MyBenchmark.testOutOfLimitLimit                2048   avgt        15    23237.960      571.892    ns/op
o.s.MyBenchmark.testOutOfLimitLimit                4096   avgt        15    44972.959      718.425    ns/op
o.s.MyBenchmark.testOutOfLimitLimit                8192   avgt        15    87296.486     4077.987    ns/op
o.s.MyBenchmark.testOutOfLimitLimit               16384   avgt        15   164924.033     1743.486    ns/op
o.s.MyBenchmark.testWithInLimit                    1024   avgt        15     7313.486      400.628    ns/op
o.s.MyBenchmark.testWithInLimit                    2048   avgt        15    15303.920      385.321    ns/op
o.s.MyBenchmark.testWithInLimit                    4096   avgt        15    30864.934      466.334    ns/op
o.s.MyBenchmark.testWithInLimit                    8192   avgt        15    59420.100     2989.484    ns/op
o.s.MyBenchmark.testWithInLimit                   16384   avgt        15   115228.745     6053.443    ns/op


To run:
mvn clean install
java -jar target/microbenchmarks.jar

