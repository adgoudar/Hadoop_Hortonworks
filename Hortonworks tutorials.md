
## Introduction

The Sandbox is a straightforward, pre-configured, learning environment that contains the latest developments from Apache Hadoop, specifically the Hortonworks Data Platform (HDP). 

HDF - is used to handle Data in Motion
HDP - is used to handle Data at Rest
But HDP contains storm (real time message processing) and Kafka ( distributed messaging system ).

## __Case of Hadoop__

## Data Trends
Hadoop was specifically designed to work with Big Data. The term big Data comes from the computational sciences.

### 3 V's of Data
* Variety - Types of data being generated. (Structured data in tradional databases, semi-structured data like XML, JSOn, Unstructured text documents, email etc)
* Velocity -The rate at which new data is generated.
* Volume - The amount of data being generated (Transaction, unstructured data streaming, Incresing amounts of sensor and machine-to-machine data)


### Apache Hadoop
It is a scalable, fault tolerant, open source framework for the distributed storing and processing of large sets of data on commity hardware.

* Scalable - Hadoop clusters can range from as few as one machine to thousands of machines/
* Fault tolerant - Hadoop services become fault tolerant through redundancy. E.g. : HDPF automatically replicated data blocks to 3 separate machines, assuming that your cluster has 3 machines in it. Hadoop services are replicated to avoid any single points of failure.
* Distributed - Large datasets are automatically split into smaller chunks called blocks and distributed across the cluster machines. Each machine processes its local block of data. This means that processing is distributed too.
* Commidity - All of the above occurs on commidity hardware which reduces the purchase price and support cost.


```
Hadoop Core = Storage + Compute
```
Compute via YARN (Yet another resource Negotiator)
Store via HDFS

YARN supports multiple, heterogenous data access engines that analyze one shared big data set with batch processing, interactive query serarch, analysis of streaming data or iterative machine learning. All these can run simultaneously, centrally managed by YARN. 

### Popular Use cases for Hadoop
* Data discovery - Uncover new insights of the data.
* Single View - Use Hadoop to unify all the scattered data and paint a single view of their (Company's) business
* Predictive Analytics - Predict the future outcomes with far more certainity. E.g. for proactive repairs to equipment, recommend next product to buy etc.

### Characteristics of Data Discovery Use Cases
* Variety of sources - Combine data from any and all new sources with more variable structures.
* Fragmentation - Data scattered across different groups and databases.
* Short retention Horizons - too expensive to keep data for very long.

### Characteristics of Single View Use cases
* Storage Fragmentation - Data scattered across many platforms.
* Customer Blind spots - subsection of customer interactions.
* Incomplete Failure Analysis = Difficult to identify root causes acoss multiple business touch points.
* Imperfect Collaboration - Routinely ask other groups for data.

### Characteristics of Predictive Analytics Use Cases
* Poor confidence - Predictions with high uncertainity.
* Preventative Maintenance - Fix or Replace equipment before it breaks.
* Insufficient Capacity - Make subset of the predictions you need.
* Recommendation Engines - Automatically suggest the next product to buy.
* Familiar Surprisese - Aware of problems that will happen, but surprised and unprepared when they do.

## __The Hadoop Ecosystem__

### Data Management Frameworks

There are two data management frameworks
* HDFS : A java-based, distributed file system that provides scalable, reliable, high-throughput access to application data stored across commodity servers.
* YARN : A framework for cluster resource management and job scheduling. It enables multiple data processing engines such as interactive SQL, real-time streaming, and batch processing to co-exist on a single cluster.

### Operations Framwork
* Apache Ambari : A web based, open operational framework for provisioning, managing and monitoring Hadoop clusters. It includes an intuitive collection of operator tools and set of RESTful APIs that masks the complexity of Hadoop.
* Apache ZooKeeper : A high-performance coordination service for distributed applications.
* Cloudbreak : A cloud agnostic tool for provisioning and managing Hadoop clusters in the cloud. It automates the launching of elastic Hadoop clusters with policy-based autoscaling on the major cloud infrastructure platforms including Azure, AWS, OpenStack and Docker containers.
* Oozie : A server-based workflow engine used to execute Hadoop jobs. It enables Hadoop users to build and schedule complex data transformations by combining Mapreduce, Hive, Pig and Sqoop jobs into a single, logical unit of work.

### Data Access Frameworks

Pig : For extracting, transforming or analyzing large datasets
Hive : A data warehouse infrastructure that supports ad hoc SQL queries.
HCatalog : A table information, schema and metadata management layer supporting Hive, Pig, MapReduce and Tez Processing.
Cascading : An application development framework for builing data applications, abstracting the details of complex MapReduce programming.
HBase : 






### Steps for Environment Setup
1. Determine Network Adapter of the Sandbox:

###Network Address Translation(NAT)
By default, the VM attaches to Network Address Translation (NAT) network mode.
The guest’s IP address by default translates over to the host’s IP address.
NAT allows for the guest system to connect to external devices on external networks, but external devices cannot access the guest system.

2. Bridged Networking
