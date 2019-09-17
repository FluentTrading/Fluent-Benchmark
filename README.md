# Fluent-Benchmark

#Clean and build the project
mvn clean install

#Shows all command line options
java -jar target/benchmarks.jar -h

#Run a particular benchmark (ABQueueBenchmark)
java -jar target/benchmarks.jar ABQueueBenchmark -bm Throughput -wi 5 -i 5 -f 5 -t 5 -si true -jvmArgs "-Xms2048m -Xmx2048m"


#Run all the benchmarks
java -jar target/benchmarks.jar -bm Throughput -i 5 -wi 5 -f 5 -t 5 -si true -jvmArgs "-Xms2048m -Xmx2048m"
