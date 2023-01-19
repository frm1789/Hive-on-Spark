# Hive-on-Spark
Spark is a real-time data analyzer, whereas Hadoop is a processing engine for very large data sets that do not fit in memory. Hive is a data warehouse system, like SQL, that is built on top of Hadoop.

# Apache Hadoop 

## What is Apache Hadoop?
It is a collection of open-source software utilities that facilitates using a network of many computers to solve problems involving massive amounts of data and computation.
It provides massive storage for any type of data, tremendous processing power, and the ability to process virtually unlimited concurrent tasks or jobs.

### Difference vs. RDBMS 

Hadoop is not a database, but rather a distributed file system that can store and process a massive amount of data clusters across computers.
Hadoop is a highly scalable model. A large amount of data is divided into multiple inexpensive machines in a cluster which is processed parallelly.

Unlike traditional relational database systems (RDBMS) that can't scale to process large amounts of data, Hadoop enables businesses to run applications on thousands of nodes involving thousands of terabytes of data

## Hadoop framework 

The main Hadoop framework consists of four modules that work together to make up the Hadoop ecosystem: 

- YARN: This platform manages the computing resources of the clusters and uses them to program the applications of the users. It is responsible for scheduling and allocating the resources of the entire Hadoop system. 

- MapReduce: This programming model allows you to process data on a large scale. It uses parallel and distributed computing algorithms to translate processing logic and make it easy to write applications that transform large data sets into one easy to manage data set. 

The data processing can be divided into two distinct phases or steps: Map and Reduce. These threads associated with the task are executed in a distributed way, in different processing nodes or slaves.
To control and manage its execution, there is a Master or Job Tracker process. It is also in charge of accepting new jobs sent to the system by clients.

- HDFS: It is the main component of the Hadoop ecosystem. HDFS provides the pre-blocking of data that MapReduce needs to run. The processing results can be stored in the same storage system or in an external database or system.

- Hadoop Common – Includes libraries and utilities that are used and shared by other Hadoop modules.
