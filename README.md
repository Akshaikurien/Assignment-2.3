# Assignment-2.3

Hadoop 1.x Major Components
Hadoop 1.x Major Components are: HDFS and MapReduce.

1.     HDFS: 
The storage mechanism is known as HDFS (Hadoop Distributed File System). It is based on google GFS(Google File System) white paper.
HDFS is a Hadoop Distributed FileSystem, where our BigData is stored using Commodity Hardware. It is designed to work with Large DataSets with default block size is 64MB (We can change it as per our Project requirements).
HDFS component is again divided into two sub-components:
·        Name Node
Name Node is placed in Master Node.it is stored in high end machines.It used to store Meta Data about Data Nodes like “How many blocks are stored in Data Nodes, Which Data Nodes have data, Slave Node Details, Data Nodes locations, timestamps etc” .
·        Data Node
Data Nodes are places in Slave Nodes.It is stored in commodity machines. It is used to store our Application Actual Data. It stores data in Data Slots of size 64MB by default.
 
2.     MapReduce: 
The analytical mechanism is known as Map Reduce and is based on google map reduce white paper
MapReduce is a Distributed Data Processing or Batch Processing Programming Model. Like HDFS, MapReduce component also uses Commodity Hardware to process “High Volume of Variety of Data at High Velocity Rate” in a reliable and fault-tolerant manner.
MapReduce component is again divided into two sub-components:
·        Job Tracker
Job Tracker is used to assign MapReduce Tasks to Task Trackers in the Cluster of Nodes. Sometimes, it reassigns same tasks to other Task Trackers as previous Task Trackers are failed or shutdown scenarios.
Job Tracker maintains all the Task Trackers status like Up/running, Failed, Recovered etc.
·        Task Tracker
Task Tracker executes the Tasks which are assigned by Job Tracker and sends the status of those tasks to Job Tracker.
