# PlateAnalyze
It aims to test of usage [Apache Storm](https://github.com/apache/storm), [Cassandra](http://cassandra.apache.org/), [Apache Flux](https://github.com/apache/storm/tree/master/external/flux), [Apache Flume](https://flume.apache.org/) and [Kafka](http://kafka.apache.org/)

This project is maven based java project.

* With initial commit it is constructed static topology configuration. 
* (TODO) But first issue is that this project will be configured with [Apache Flux](https://github.com/apache/storm/tree/master/external/flux) using local.yaml and remote.yaml.
* It accepts streams via tcp socket to spout.
* (TODO) It must accept stream via [Apache Flume](https://flume.apache.org/) and [Kafka Spout](https://github.com/apache/storm/tree/master/external/storm-kafka) rather than tcp.
* It writes results to Cassandra if it detects right sequence of plates.
* (TODO) It must be run without any tcp input, means auto generated. (Kafka Spout generated)
* (TODO) It must use error topic to write error logs.
