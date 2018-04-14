# UUID Benchmarks

Benchmarks for UUID generation

## Libraries being compared
* `java.util.UUID`
* `com.eaio.uuid.UUID`

## Pre-requisites
* JDK 8
* Maven 3.x

## How to run

From this directory, run:
```
mvn clean install
java -jar target/uuid-benchmarks.jar
```

If everything runs successfully, you should see output similar to:
```
Benchmark            Mode  Cnt  Score   Error   Units
MyBenchmark.custom  thrpt  100  6.628 ± 0.123  ops/ms
MyBenchmark.name    thrpt  100  1.427 ± 0.030  ops/ms
MyBenchmark.random  thrpt  100  0.514 ± 0.003  ops/ms
MyBenchmark.custom   avgt  100  0.154 ± 0.004   ms/op
MyBenchmark.name     avgt  100  0.715 ± 0.021   ms/op
MyBenchmark.random   avgt  100  1.983 ± 0.030   ms/op

```