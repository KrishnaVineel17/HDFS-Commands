# HDFS-Commands
This gives a basic idea on some of the mostly used HDFS commands in Linux Terminal while doing some application on Apache Hadoop.

What is HDFS?
HDFS is a distributed file system that handles large data sets running on commodity hardware. It is used to scale a single Apache Hadoop cluster to hundreds (and even thousands) of nodes. HDFS is one of the major components of Apache Hadoop, the others being MapReduce and YARN. HDFS should not be confused with or replaced by Apache HBase, which is a column-oriented non-relational database management system that sits on top of HDFS and can better support real-time data needs with its in-memory processing engine.

HDFS is a highly scalable and reliable storage system for the Big Data platform, Hadoop. Working closely with Hadoop YARN for data processing and data analytics, it improves the data management layer of the Hadoop cluster making it efficient enough to process big data, concurrently. HDFS also works in close coordination with HBase. 

Some of the useful HDFS commands are mentioned below:
Initially, start all the Apache Hadoop daemnons by using the following command:
**start-all.sh**

Then use the following commands:

1. hdfd dfs -mkdir <directory>         //this command helps in creating a new directory

2. hdfs dfs -ls /directory             //this command displays list of all files present in the directory 

3. hdfs dfs -ls /                      //this command helps in displaying all the directories present in HDFS

4. hdfs dfs -cat /directory/sample.txt //this command helps to display the text data present in the sample.txt file.

5. hdfs dfs -touchz /directory/sample.txt  //this command helps to create a file of zero length/an empty file

6. hdfs dfs -copyFromLocal <source_path> <destination_path> //this command helps in copying a file from local file system to HDFS

7. hdfs dfs -put <source_path> <destination_path> // this command helps in copying a file from local file system to HDFS

8. hdfs dfs -copyToLocal <source_path> <destination_path> //this command helps in copying a file from HDFS to local file system

9. hdfs dfs -get <source_path> <destination_path> //this command helps in copying a file from HDFS to local file system
 
10.hdfs dfs -moveFromLocal <source_path> <destination_path> //this command helps in moving a file from local file system to HDFS

11.hdfs dfs -cp <dir_1> <dir_2>        //this command helps us in copying all files in dir_1 to dir_2 within HDFS

12.hdfs dfs -mv <dir_1> <dir_2>        //this command helps us in moving all files from dir_1 to dir_2 within HDFS

13.hdfs dfs -rmdir <directory>        //this command helps us in deleting a dorectory

14.hdfs dfs -rmr <directory>          //this is a recursive version of delete, which is useful in deleting a non-empty directory

Finally, to stop all the Apache Hadoop daemons use the following command:
**stop-all.sh**
