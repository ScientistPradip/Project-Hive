# Apache Hive  Project
This project focuses on working with Apache Hive to create databases and tables, load data stored in HDFS, define appropriate data types, and query structured data using HiveQL.

The project demonstrates how Hive can be used as a data warehouse tool on top of Hadoop and HDFS. The main goal is to understand how data stored in HDFS can be organized into tables and accessed using SQL-like queries.

### Technologies Used
- Apache Hive
- Hadoop HDFS
- HiveQL
- Docker
- Linux Terminal
- CSV / Text 
- Files

### Project Objectives
- Start and work with the Hadoop and Hive environment.
- Create and manage Hive databases.
- Create tables using different Hive data types.
- Use external tables with HDFS data.
- Define row format and field delimiters.
- Load and access data stored in HDFS.
- View table structures and column data types.
- Query data using HiveQL.
- Understand the relationship between Hive and HDFS.

### Step 1: Start Hive Console 
Here, if you are logging into your docer desktop trying to enter hive console for very first time then you have to run restartHive else just run Hive only. As restart hive is used to restart all the hive services. 
In case you have already existed hive console then just use hive command instead of restarthive
 ![Step_1](Screenshots/Step1_starting_hive_in_docker.png)

 ### Step 2: Check data in HDFS
 After this open external terminal. Now, we'll be using Hadoop where we'll be creating one empty file.
 We're going to create 'customer.txt and we'll paste 4 lines of already created/ready data in that
 ![Step_2](Screenshots/Step2.png)

### Step 3: Creating Database in Hive Console
Creating database named xyz. Here instead of default data base storage now we'll be using that xyz database to store our data. 
And viewing the data we stored in that database
![Step_3](Screenshots/Step3.png)

### Step 4: Creating external table in hive console and checking if we drop that external table metadata along with data will drop or not
External table created with column name and datatype 

![Step_4](Screenshots/Step4.png)

Now Checking it in default HDFS Storage where the data we created stores in default storage location ie /data/hive/warehouse/xyz.db
that is the db we created its empty.
It means that if we drop external table even metadata is dropped data is still there as HDFS is the original owner of data. 

![Step_4](Screenshots/Step4_partII_dataisStillThereInHDFSWeJustDeletedInHIVE.png)
