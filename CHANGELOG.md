# Changelog

## 0.12.0 (upcoming)

* Pending changelog


## 0.11.0 (upcoming)

* Docker updated with Spark and DC/OS Mesos integration
* Updated Receiver RabbitMQ for Distributed mode
* Batch + Streaming Queries
* Input Sql Sentences
* Slidding Windows in Triggers
* User plugins jars added in policy definition
* Spark configurations added in policy definition
* Bugfix: Kafka Direct
* Bugfix: Ingestion parser
* Bugfix: Date options in dimension time
* Bugfix: Relaunch policies
* Bugfix: Auto fragments creation
* Bugfix: Delete checkpoint when edit one policy
* Bugfix: Api end points return the correct policy with fragments
* Bugfix: Swagger data types

## 0.10.0 (July 2016)

* Added coveralls badge
* Updated to Spark 1.6.2
* Updated Cassandra, ElasticSearch and MongoDb to the latest library version
* Updated Receiver RabbitMQ
* Zookeeper offset path updated in kafka receivers
* Ingestion Parser with Avro Serialization
* Bugfix: Akka dependency
* Bugfix: Actors creation process with not unique identifier
* Bugfix: Policy statuses corrected
* Bugfix: Updated all policies when one fragment is changed
* Bugfix: Policy download in Firefox

## 0.9.5 (April 2016)

* Added remember field in order to run queries that last more than the streaming batch
* Add Timestamp type to selectable output type in DateTime parser
* Bugfix: Removed fragments when downloading the policy
* Bugfix: Geo icon not showing
* Bugfix: Set default checkpoint path as relative
* Bugfix: Fixed measures field wrong behaviour

## 0.9.4 (April 2016)

* Bugfix: Solved problem with hdfs.

## 0.9.3 (April 2016)

* Bugfix: Solved problem with permissions and owners.

## 0.9.2 (April 2016)

* Bugfix: Fixed examples

## 0.9.1 (April 2016)

* Bugfix: Fixed documentation links

## 0.9.0 (April 2016)

* New look & feel and more user friendly user interface
* New policy component: Triggers
* New parser for geolocation
* Renamed Sparkta to Sparta
* Improved performance
* No-time aggregations
* User benchmark
* Kafka output
* JDBC output
* Policy refactor
* Fault tolerance
* Refactor Cluster deployment
* Addition of a new operator: Associative Mean
* Fixes for Count and Sum operators 
* Added flexibility to create policies with no cubes 
* Integration with a SSO 
* Sparta API supports SSL

## 0.8.0 (December 2015)

* Solved issue related to PID folder creation.
* New parser Stratio Ingestion
* Upgrade to Spark 1.5.2
* Possibility to package two Spark versions: 1.4.1 and 1.5.2
* MongoDb output updated to version 0.10.1
* New Solr output
* Migration of doc to confluence: https://stratio.atlassian.net/wiki/display/SPARTA0x8/
* Solved issue when a policy is stopped in the cluster
* Improve performance in associative operators
* Automatic deploy of policies in clusters: Spark Standalone, Mesos and YARN
* Improve Cassandra Output. Possibility to introduce Spark properties
* Solved issue related to stopping Sparta service
* bug corrected in aggregations, Array Index out of bounds

## 0.7.0 (November 2015)

* Bugfix: Front Minors
* Bugfix: Back Minors
* Bugfixes Cassandra
* Bugfixes Elasticsearch
* Package installation permissions fixes
* Bugfix: DateTime field and parser

## 0.6.2 (September 2015)

* Bugfix: DateTime now parses string formats
* Bugfix: Permission issues running Sparta service
* Bugfix: Minor errors in user interface

## 0.6.1 (September 2015)

* Hotfix: User interface was not showing up

## 0.6.0 (September 2015)

* Upgrade Spark version to 1.4.1
* User Interface to help create your cubes
* Automatic deployment in Mesos cluster
* Policy status lifecycle
* New WebSocket input
* Elasticsearch output updated to version 1.7
* New EntityCount and TotalEntityCount operators
* Filters in operators

## 0.5.0 (July 2015)

* Added compatibility with Apache Spark 1.4.x
* Released a specific distribution for Apache Spark 1.3.x
* Support for fragment composition in policies.
* Policy refactor. Improved semantic of the JSON.
* Parquet and CSV outputs.
* Improved Twitter input. Possibility to filter tweets by hashtag.
* Fixed important bug in Elasticsearch output. Fields are mapped according to their type.

## 0.4.0 (May 2015)

* SandBox Stratio Sparta
* Integration with **Spark 1.3.1**
* Auto create time series in outputs if not exist time dimension
* Full integration in Outputs with **Spark DataFrames**
* Auto create "Id" in DataFrames with dimensions
* Save Raw data in **Parquet** files
* Auto detection schema with policies
* Reflexions for native plugins
    * Interactive documentation
    * Client SDK generation and discoverability
    * Compatibility with multiple oputputs
* Output **Cassandra**:
    * Auto tables creation
    * Auto primary key and column families detection
    * Auto index creation
* Output **ElasticSearch**:
    * Options in mapping date types
    * Auto index type with time fields
* Output **Redis**
* Input **Kafka Direct Streaming** integrated in Spark 1.3.0
* Input **RabbitMq**
* Full-Text operator
* Accumulator operator
* Last Value operator
