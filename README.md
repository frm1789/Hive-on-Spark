# The Hadoop Universe
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

## Phases in MapReduce

In a Hadoop MapReduce job, the input data is split into independent chunks that are processed by the mappers in parallel. Next, the results of the map are sorted, which are the input to the reducers. 

The framework is also responsible for managing resources, scheduling, restarting, and monitoring tasks with the Hadoop YARN manager, which has a single Resource Manager and a Node Manager on each cluster node.

- The <b>Map phase</b> is executed in subtasks called <b>mappers</b>. These components are responsible for generating key-value pairs by filtering, grouping, sorting, or transforming the original data. Intermediate data pairs are not stored in HDFS.

- The <b>Shuffle (sort)</b> phase may not be necessary. It is the intermediate step between Map and reduce that helps to collect the data and arrange it in a convenient way for processing. With this phase, it is intended to add the repeated occurrences in each of the mappers.

- The <b>Reduce phase</b> manages the aggregation of the values produced by all the mappers in the system (or by the shuffle phase) of key-value type based on their key. Finally, each reducer generates its output file independently, generally written in HDFS.

### Counting words in Hadoop? Why is this the common example?

The most common example of a MapReduce application is Word Count. It consists of counting the occurrences of each word in a set of documents.

The program is divided into 3 components: the driver (application entry point), the mapper implementation and the reducer implementation.


## Spark on Haddop

Spark is a real-time data analyzer, while Hadoop is a processing engine for very large data sets that don't fit in memory. Hive is a data storage system, like SQL, that is based on Hadoop.

Hadoop can handle large data batching efficiently, while Spark processes real-time data such as Facebook and Twitter feeds. Spark has an interactive mode that allows the user to have more control during the execution of the job.

Spark is the fastest option for ingesting real-time data, including unstructured data streams. Hadoop (with Hive) is optimal for running analytics using SQL.


## Zookeeper - Because coordinating distributed systems is a zoo - 

### Tasks: 
- Coordinate service for distributed applications
- Naming
- Configuration
- Synchronization
- Group management/leader election




