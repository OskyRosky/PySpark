 ---------------------------------------------

# PySpark
 Everything about PySpark


![py](/ima/ima1.jpeg)

---------------------------------------------
**Repository summary**

1.  **Intro** 🧳

Learn the basics of Apache Spark, its origins, architecture, and how it handles large-scale data processing. Understand the concept of clusters, master and worker nodes, and the MapReduce paradigm. Explore the flexibility and power of PySpark, the Python API for Apache Spark.

2.  **Tech Stack** 🤖

Data Engineering

- **Spark Context and Spark Session**: Understand the roles and functionalities of SparkContext and SparkSession. Learn the similarities and differences between these components, and how to create and use them effectively in your Spark applications.
- **Spark RDD**: Dive into Resilient Distributed Datasets (RDDs), the fundamental data structure of Apache Spark. Learn about RDD characteristics, transformations, actions, and various operations. Understand how to read and write RDDs from/to text files.
- **Spark DataFrame**: Explore DataFrames, a higher-level abstraction compared to RDDs, and their advantages. Learn how to create DataFrames from different data sources and perform complex data manipulations and transformations.
- **Creating DataFrames from Various Data Sources**: Learn to create DataFrames from multiple data sources such as flat files, data warehouses, data lakes, web data, and streaming data sources. Understand different data formats supported by Spark, including CSV, JSON, Parquet, ORC, Avro, Text, XML, and Delta Lake.

3.  **Features** 🤳🏽

**Spark SQL**: Master Spark SQL for structured data processing. Learn to perform SQL-like queries on DataFrames, key features of Spark SQL, and various SQL operations such as selecting, filtering, aggregating, joining, sorting, and pivoting data. Discover how to create and manage temporary views.

**Data Wrangling in Spark DataFrame**: Gain insights into data wrangling processes, including data collection, cleaning, transformation, enrichment, validation, and structuring. Learn specific operations for ingestion, column and row manipulation, general transformations, and working with characters and time series data.

4.  **Process** 👣

Installation Guides: Detailed guides for installing Apache Spark on both Mac and Windows. Instructions include setting up Java, Hadoop, and Spark, and configuring environment variables for seamless operation. Learn how to verify the installation and troubleshoot common issues.

5.  **Learning** 💡

**Other Uses and Applications of PySpark**: Explore the diverse applications of PySpark beyond data engineering. Learn about data analysis, machine learning with Spark's MLlib, graph processing with GraphX, and data visualization. Understand the benefits of using PySpark for advanced analytics and real-time stream processing.

6.  **Improvement** 🔩

**PySpark Applications**: Showcase various applications and projects built using PySpark. Understand practical implementations and real-world use cases to enhance your learning and application of PySpark.

7.  **Running the Project** ⚙️

**Tutorials**: Step-by-step tutorials on how to run and manage your PySpark projects. This includes setting up the environment, writing PySpark scripts, and deploying your applications.

8.  **More** 🙌🏽

**Other PySpark Resources**: Stay updated with the latest developments in PySpark by exploring a curated list of exclusive websites and resources. Access official documentation, community editions, Q&A platforms, GitHub repositories, tutorials, courses, and mailing lists dedicated to PySpark.

**PySpark Tutorials**: Enhance your learning with a collection of YouTube videos that provide practical demonstrations and in-depth tutorials on PySpark. Explore various topics and techniques through these carefully selected video resources.



---------------------------------------------

# :computer: PySpark :computer:

---------------------------------------------
# I. Introduction to PySpark

Apache Spark is a powerful open-source processing engine built around speed, ease of use, and sophisticated analytics. Spark has become a key player in the world of Big Data due to its ability to handle large-scale data processing through distributed computing. Originating from the AMPLab at UC Berkeley, Spark was designed to perform tasks quickly by utilizing in-memory processing and optimizing data distribution across multiple machines. The architecture of Spark revolves around the concept of clusters, where a master node oversees the allocation of tasks to worker nodes. These worker nodes execute tasks in parallel using the MapReduce paradigm, enabling efficient data processing and storage. The flexibility of Spark allows it to be used with multiple programming languages, including Python, through the PySpark framework, making it accessible and versatile for various big data applications.

## Data through Ram memory 

One of core advantages working with data is its ability to load into RAM for fast processing. This allows for quick data manipulation and transformation, significantly reducing the time required compared to traditional disk-based processing. However, when the data size exceeds the available RAM, Spark efficiently manages data overflow by utilizing disk storage. This ensures seamless processing without data loss or significant performance degradation, maintaining high efficiency.

## Apache 

Apache is a community of open-source software projects, of which Apache Spark is a part. The Apache Software Foundation (ASF) provides organizational, legal, and financial support for a broad range of open-source software projects, including Spark. Apache projects are developed and maintained by a community of developers and contributors around the world, fostering collaboration and innovation.

## Apache Spark

Apache Spark is an open-source unified analytics engine designed for large-scale data processing. It provides high-level APIs in Java, Scala, Python, and R, and an optimized engine that supports general execution graphs. Spark is known for its ability to process data in-memory, significantly speeding up data processing tasks. It is capable of handling batch processing, real-time data streaming, machine learning, and graph processing, making it a versatile tool for big data analytics.

## Spark for Big Data

In the realm of big data, Spark stands out for its ability to handle vast amounts of data efficiently. Its in-memory processing and ability to distribute tasks across a cluster of machines make it ideal for big data analytics. Spark's versatility allows it to be used for a variety of big data applications, from ETL processes to complex machine learning algorithms, providing robust tools and capabilities tailored for large-scale data environments.

## Distributed System

In a distributed system, tasks are divided among multiple machines (nodes) to improve efficiency and performance. Spark manages the distribution of data and tasks across nodes, ensuring that processing is done in parallel and resources are utilized optimally. This approach allows Spark to handle large-scale data processing tasks that would be infeasible on a single machine, leveraging the power of distributed computing to achieve remarkable performance.

## The Cluster

A Spark cluster consists of a master node and multiple worker nodes. The master node is responsible for resource management and task scheduling, while worker nodes perform the actual data processing tasks. This cluster-based architecture allows Spark to handle large datasets by distributing the workload across multiple machines, ensuring scalability and high performance. The coordinated effort of these nodes enhances Spark’s ability to process and analyze big data efficiently.

## Map Reduce

MapReduce is a programming model for processing and generating large data sets. It divides the processing into two steps: the "Map" step, where a function is applied to each input data item, and the "Reduce" step, where the results of the map step are aggregated. In Spark, MapReduce is implemented in a more efficient and flexible manner, allowing for iterative algorithms and interactive data analysis. This implementation enhances Spark’s capability to perform complex data processing tasks with high efficiency.


## Python + Spark = PySpark

PySpark is the Python API for Apache Spark, allowing Python developers to leverage the power of Spark for big data processing. It provides an easy-to-use interface for performing a wide range of data processing tasks, from simple data manipulations to complex machine learning algorithms. PySpark combines the simplicity and versatility of Python with the speed and scalability of Spark, making it a popular choice for data scientists and engineers. This synergy enables users to efficiently process and analyze big data using familiar Python constructs.

![py](/ima/ima2.png)

## So...

In summary, Apache Spark is a robust and versatile framework designed for efficient large-scale data processing. Its architecture, which utilizes clusters of machines to distribute tasks and leverage in-memory processing, significantly enhances performance and scalability. The combination of Apache's open-source community support and Spark's ability to handle diverse data processing tasks—from batch processing to real-time streaming—makes it an invaluable tool in the realm of Big Data. Through PySpark, Python developers can harness the power of Spark, enabling seamless integration and advanced analytics capabilities within the Python ecosystem. This synergy between Spark and Python opens up a world of possibilities for data scientists and engineers, driving innovation and efficiency in data processing workflows.

---------------------------------------------
# II. Spark Installation on Mac and Windos

## Detailed Guide for Installing Apache Spark on Mac

**Step 1: Install Homebrew**

Homebrew is a package manager for macOS that simplifies the installation of software. If you don't already have Homebrew installed, follow these steps:

1. Open the Terminal application.
2. Install Homebrew by running the following command:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

3.Follow the on-screen instructions to complete the installation.

**Step 2: Install Java Development Kit (JDK)**

Apache Spark requires Java. You can install the JDK using Homebrew:

1. In the Terminal, run the following command to install the latest version of JDK:

```bash
brew install openjdk
```

2. Once the installation is complete, add the JDK to your PATH by adding the following lines to your ~/.zshrc or ~/.bash_profile file (depending on your shell):

```bash
export PATH="/usr/local/opt/openjdk/bin:$PATH"
export CPPFLAGS="-I/usr/local/opt/openjdk/include"
```

3. Apply the changes by running:

```bash
source ~/.zshrc   # or source ~/.bash_profile
```

4. Verify the installation by running:

```bash
java -version
```

**Step 3: Install Apache Spark**

Now that you have Java installed, you can install Apache Spark using Homebrew:

1. In the Terminal, run the following command to install Apache Spark:

```bash
brew install apache-spark
```

**Step 4: Configure Environment Variables**

To make Spark commands available globally, you need to set up the environment variables.

1. Open your ~/.zshrc or ~/.bash_profile file:

```bash
nano ~/.zshrc   # or nano ~/.bash_profile
```

2. Add the following lines to the file:

```bash
export SPARK_HOME=/usr/local/Cellar/apache-spark/<version>
export PATH=$SPARK_HOME/bin:$PATH
```
Replace <version> with the version number installed by Homebrew (you can find it by looking inside /usr/local/Cellar/apache-spark/).

3. Apply the changes by running:

```bash
source ~/.zshrc   # or source ~/.bash_profile
```

**Step 5: Verify the Installation**

To ensure Spark is installed correctly, you can run the Spark shell:

1. In the Terminal, run:

```bash
spark-shell
```

2. You should see the Spark shell starting, indicating that Spark is correctly installed and configured.

**Step 6: Install PySpark**

If you want to use PySpark, you need to install it via pip:

1. Ensure you have Python installed. If not, install it using Homebrew:

```bash
brew install python
```

2. Install PySpark using pip:

```bash
pip install pyspark
```

3. Verify the installation by running a PySpark shell:

```bash

pyspark
```

**Troubleshooting**
- JAVA_HOME not set: If you encounter issues related to Java, make sure your JAVA_HOME is set correctly. You can set it by adding the following to your ~/.zshrc or ~/.bash_profile:

```bash
export JAVA_HOME=$(/usr/libexec/java_home)
```

Then apply the changes by running:

```bash
source ~/.zshrc   # or source ~/.bash_profile
```

-**Permission issues**: If you encounter permission issues during installation, you might need to prepend the installation commands with *sudo*.

This guide should help you get Apache Spark up and running on your Mac machine.

## Detailed Guide for Installing Apache Spark on Windows

**Step 1: Install Java Development Kit (JDK)**

Apache Spark requires Java. You can install the JDK as follows:

1. Download JDK: Go to the Oracle JDK download page or OpenJDK download page and download the installer for the latest version of JDK.

2. Install JDK: Run the downloaded installer and follow the on-screen instructions to complete the installation.

3. Set JAVA_HOME Environment Variable:

- Open the Start menu, search for "Environment Variables," and select "Edit the system environment variables."
- In the System Properties window, click on the "Environment Variables" button.
- In the Environment Variables window, under System variables, click "New" and add the following:
    1. Variable name: JAVA_HOME
    2. Variable value: C:\Program Files\Java\jdk-<your_version>
- Add Java to the PATH variable:
Find the Path variable in the System variables section, select it, and click "Edit."
Click "New" and add %JAVA_HOME%\bin.

4. Verify the Installation:

- Open Command Prompt and run:

```cmd
java -version
```


- Ensure the version information is displayed correctly.

**Step 2: Install Hadoop (WinUtils.exe)**

Apache Spark needs winutils.exe for Hadoop to run correctly on Windows.

1. Download WinUtils:

- Download winutils.exe from a trusted source, such as the GitHub repository for Hadoop binaries.

2. Set HADOOP_HOME Environment Variable:

- Create a folder, e.g., C:\hadoop\bin, and place winutils.exe inside this folder.

- Open the Environment Variables window as described in Step 1.

- In the System variables section, click "New" and add the following:
   1. Variable name: HADOOP_HOME
   2. Variable value: C:\hadoop

- Add Hadoop to the PATH Variable:

    1. Edit the Path variable in the System variables section.
    2. Click "New" and add %HADOOP_HOME%\bin.

**Step 3: Install Apache Spark**

1. Download Apache Spark:

- Go to the Apache Spark download page.
- Choose a Spark release, and a package type (e.g., pre-built for Hadoop 2.7).
- Download the binary .tgz file.

2. Extract Apache Spark:

- Extract the downloaded .tgz file to a directory, e.g., C:\spark.

3. Set SPARK_HOME Environment Variable:

- Open the Environment Variables window.
- In the System variables section, click "New" and add the following:
    1. Variable name: SPARK_HOME
    2. Variable value: C:\spark\spark-<your_version>
- Add Spark to the PATH variable:
    1. Edit the Path variable in the System variables section.
    2. Click "New" and add %SPARK_HOME%\bin.

**Step 4: Install Python and PySpark**

1. Install Python:

- Download and install Python from the Python website.
- Ensure you check the option "Add Python to PATH" during installation.

2. Install PySpark:

- Open Command Prompt and run:

```cmd
pip install pyspark
```

**Step 5: Verify the Installation**

1. Verify Spark Shell:

- Open Command Prompt and run:
```cmd
spark-shell
```
- You should see the Spark shell starting, indicating that Spark is correctly installed.

2. Verify PySpark:

- Open Command Prompt and run:
```cmd
pyspark
```

- You should see the PySpark shell starting, indicating that PySpark is correctly installed.

**Troubleshooting**

- **JAVA_HOME not set**: If you encounter issues related to Java, ensure your JAVA_HOME environment variable is set correctly.
- **WinUtils.exe not found**: Ensure winutils.exe is placed in the correct directory (C:\hadoop\bin) and that the HADOOP_HOME variable is set correctly.
- **PATH variable issues**: Ensure all required paths (Java, Hadoop, Spark) are correctly added to the PATH variable.

This guide should help you get Apache Spark up and running on your Windows machine

---------------------------------------------

# III. Spark Context and Spark Session

Apache Spark provides two essential components for interacting with the cluster and executing operations: SparkContext and SparkSession. These components serve as the main entry points for Spark functionalities, allowing users to create RDDs, DataFrames, and execute Spark jobs. While SparkContext was the primary entry point in older versions of Spark, SparkSession was introduced in Spark 2.0 to unify the functionalities and simplify the user experience.

## What's SparkContex

SparkContext is the entry point for accessing Spark functionalities. It represents the connection to a Spark cluster and is responsible for managing the distributed environment. SparkContext allows users to create RDDs, broadcast variables, and perform accumulations. It essentially handles the low-level details of the cluster and serves as the core component for distributed computing.

## What's SparkSession

SparkSession is a unified entry point for all the functionalities provided by Spark. Introduced in Spark 2.0, SparkSession consolidates the functionalities of SparkContext, SQLContext, and HiveContext into a single API. It simplifies the user experience by providing a central point for creating DataFrames, executing SQL queries, and accessing catalog functionalities. SparkSession manages the Spark application's lifecycle and configuration.

## Similarities

Both SparkContext and SparkSession provide the means to interact with a Spark cluster and perform data processing tasks. They allow users to create RDDs, DataFrames, and Datasets, and execute transformations and actions on these collections. Both components are essential for managing the distributed nature of Spark applications and ensuring efficient execution of Spark jobs.

## Differences 

- Entry Point: SparkContext was the primary entry point in Spark versions before 2.0, while SparkSession is the primary entry point in Spark 2.0 and later.
  
- Functionality: SparkSession combines the functionalities of SparkContext, SQLContext, and HiveContext, providing a unified API for all Spark operations. SparkContext, on the other hand, focuses primarily on low-level cluster management and RDD creation.
  
- Ease of Use: SparkSession simplifies the user experience by providing a single entry point for all Spark functionalities, making it easier to manage and execute Spark jobs.

## Create an SparkContex

Creating a SparkContext involves initializing it with the necessary configuration settings. Here is an example in Python:

```python
from pyspark import SparkConf, SparkContext

# Create a Spark configuration object
conf = SparkConf().setAppName("MyApp").setMaster("local")

# Initialize SparkContext with the configuration
sc = SparkContext(conf=conf)
```

In this example, SparkConf is used to set the application name and master URL, which specifies where the Spark cluster is running. The SparkContext is then initialized with this configuration.

## Create an SparkSession

Creating a SparkSession is more straightforward, as it combines various contexts into a single entry point. Here is an example in Python:

```python
from pyspark.sql import SparkSession

# Initialize SparkSession
spark = SparkSession.builder \
    .appName("MyApp") \
    .master("local") \
    .getOrCreate()
```

In this example, SparkSession.builder is used to configure the application name and master URL. The getOrCreate method ensures that an existing SparkSession is returned if one already exists, or a new one is created if none exists.

## So...

Understanding SparkContext and SparkSession is crucial for effectively utilizing Apache Spark. While SparkContext provides a foundational entry point for Spark operations, SparkSession simplifies and unifies the user experience by consolidating multiple contexts into a single API. This evolution from SparkContext to SparkSession reflects Spark's continuous efforts to improve usability and functionality for big data processing.

---------------------------------------------

# IV. Spark RDD 

Resilient Distributed Datasets (RDDs) are the fundamental data structure of Apache Spark. They are immutable, distributed collections of objects that can be processed in parallel across a cluster. RDDs provide fault tolerance and lineage information, which helps in recovering lost data. This section covers the basics of RDDs, their characteristics, transformations, actions, and operations.

## What's RDDs (Resilient Distributed Datasets)

RDDs are a core abstraction in Apache Spark, representing a read-only collection of objects distributed across a cluster of machines. RDDs can be created from Hadoop Distributed File System (HDFS) datasets or by transforming existing RDDs. They support two types of operations: transformations and actions.

## RDD Characteristics

1. **Immutable**: Once created, RDDs cannot be modified. This immutability ensures consistency and fault tolerance.
   
2. **Distributed**: RDDs are partitioned across multiple nodes in a cluster, allowing parallel processing.
   
3. **Fault Tolerant**: RDDs are designed to handle node failures by recomputing lost data from the lineage information.
  
4. **Lazy Evaluation**: Transformations on RDDs are not executed immediately. They are evaluated lazily, meaning computation is deferred until an action is performed.
   
5. **In-Memory Computing**: RDDs can cache data in memory, which improves the performance of iterative algorithms.

## RDD Transformations and Actions

RDD operations are divided into two categories: transformations and actions.

Transformations are operations that create a new RDD from an existing one. They are lazy, meaning they are not executed immediately but are recorded to be executed when an action is called. Examples include "map", "filter", and "reduceByKey".

Actions are operations that trigger the execution of transformations and return a result to the driver program or write it to storage. Examples include "collect", "count", and "saveAsTextFile".

## RDD Operations

### Actions

Actions are operations that trigger the execution of transformations and return a result to the driver program or write it to storage.

- **Collect**: Returns all the elements of the RDD as an array to the driver program.

```python
rdd = sc.parallelize([1, 2, 3, 4])
result = rdd.collect()  # [1, 2, 3, 4]
```
  
- **Count**: count: Returns the number of elements in the RDD.

```python
rdd = sc.parallelize([1, 2, 3, 4])
result = rdd.count()  # 4
```

- **First**: Returns the first element of the RDD.

```python
rdd = sc.parallelize([1, 2, 3, 4])
result = rdd.first()  # 1
```

- **Take**: Returns an array with the first n elements of the RDD.

```python
rdd = sc.parallelize([1, 2, 3, 4])
result = rdd.take(2)  # [1, 2]

```


### Transformations

Transformations are operations that create a new RDD from an existing one.

- map: Applies a function to each element of the RDD and returns a new RDD with the results.

```python

```

- filter: Returns a new RDD containing only the elements that satisfy a predicate.

```python
rdd = sc.parallelize([1, 2, 3, 4])
result = rdd.filter(lambda x: x % 2 == 0).collect()  # [2, 4]
```

- flatMap: Similar to map, but each input item can be mapped to zero or more output items (i.e., it returns a flattened list).

```python
rdd = sc.parallelize([1, 2, 3])
result = rdd.flatMap(lambda x: (x, x * 2)).collect()  # [1, 2, 2, 4, 3, 6]
```

- reduceByKey: Groups data with the same key and applies a reduction function on each group.

```python
rdd = sc.parallelize([('a', 1), ('b', 1), ('a', 1)])
result = rdd.reduceByKey(lambda a, b: a + b).collect()  # [('a', 2), ('b', 1)]
```

### Read 

RDDs can be created by reading data from various sources, such as local files, HDFS, or external databases.

- Read from text file:

```python
rdd = sc.textFile("path/to/textfile.txt")
```


### Write RDDs from / to text files

RDDs can be saved to text files, allowing you to persist the results of your computations.

```python
rdd = sc.parallelize([1, 2, 3, 4])
rdd.saveAsTextFile("path/to/outputdir")
```

In summary, RDDs are a fundamental component of Apache Spark, providing a robust and flexible way to perform distributed data processing. Understanding RDD characteristics, transformations, and actions is crucial for effectively utilizing Spark's capabilities for big data analytics.

---------------------------------------------
# V. Spark DataFrane 

DataFrames in Apache Spark provide a higher-level abstraction than RDDs, offering a powerful and flexible way to perform data processing tasks. They are similar to data frames in R or Python's pandas library but optimized for distributed computing.

## What's a Dataframe?

A DataFrame is a distributed collection of data organized into named columns. It is conceptually equivalent to a table in a relational database or a data frame in R or Python. DataFrames provide a more expressive and flexible API than RDDs, making it easier to manipulate structured data.

- Example 1: Creating a DataFrame from a list of tuples

```python
from pyspark.sql import SparkSession

# Initialize SparkSession
spark = SparkSession.builder.appName("example").getOrCreate()

# Create a DataFrame
data = [("Alice", 29), ("Bob", 31), ("Catherine", 27)]
df = spark.createDataFrame(data, ["Name", "Age"])

# Show the DataFrame
df.show()
```

- Example 2: Creating a DataFrame from a CSV file

```python
# Read a CSV file into a DataFrame
df = spark.read.csv("path/to/file.csv", header=True, inferSchema=True)

# Show the DataFrame
df.show()
```

## Dataframe advantes over RDDs in Spark.

DataFrames provide several advantages over RDDs, including:

- Schema Information: DataFrames have a schema, meaning the data is organized into named columns. This allows Spark to perform more optimizations during execution.
- Optimized Execution: DataFrames use the Catalyst optimizer, a query optimizer that can perform advanced optimizations and generate efficient execution plans.
- Ease of Use: The API for DataFrames is more expressive and user-friendly, supporting a wide range of operations similar to SQL.
- Integration with SQL: DataFrames can be queried using SQL syntax, making it easier for users familiar with SQL to perform data analysis.

Example 1: Using schema information for optimization

```python
# Define schema explicitly
from pyspark.sql.types import StructType, StructField, StringType, IntegerType

schema = StructType([
    StructField("Name", StringType(), True),
    StructField("Age", IntegerType(), True)
])

# Create DataFrame with schema
df = spark.createDataFrame(data, schema)

# Show the DataFrame
df.show()
```

Example 2: Performing SQL queries on a DataFrame

```python
# Register DataFrame as a temporary view
df.createOrReplaceTempView("people")

# Query the DataFrame using SQL
sqlDF = spark.sql("SELECT Name, Age FROM people WHERE Age > 28")

# Show the result
sqlDF.show()
```

## Why we should use a Dataframe in Spark?

DataFrames are preferred over RDDs in Spark for several reasons:

- **Performance**: DataFrames are optimized using the Catalyst optimizer and Tungsten execution engine, providing significant performance improvements over RDDs.
- **Ease of Data Manipulation**: DataFrames offer a high-level API for data manipulation, making it easier to perform complex transformations and aggregations.
- **Compatibility with Other Data Sources**: DataFrames can easily integrate with various data sources, including JSON, CSV, Parquet, and JDBC, simplifying data ingestion and export.
- **Enhanced Analytics**: DataFrames support advanced analytics functions, including grouping, aggregation, and statistical functions, which are more challenging to implement with RDDs.

**Example 1**: Performance optimization using Catalyst optimizer

```python
# Perform a group by operation with aggregation
df.groupBy("Age").count().show()
```

**Example 2**: Ease of data manipulation and integration with other data sources

```python
# Read data from a JSON file
jsonDF = spark.read.json("path/to/file.json")

# Perform a simple transformation
jsonDF.select("Name", "Age").where("Age > 28").show()
```

DataFrames in Spark provide a powerful, flexible, and efficient way to handle large-scale data processing tasks. They offer significant advantages over RDDs, including optimized execution, ease of use, and compatibility with various data sources, making them an essential tool for data engineers and data scientists.

---------------------------------------------

# VI. Creating DataFrames from Varios Data Sources

## Common Data Sources for Apache Spark

1. **Flat Files**: These include text files, CSV, JSON, XML, and other plain text formats stored in local file systems or distributed storage systems.
2. **Data Warehouses**: Structured data stored in data warehousing solutions like Amazon Redshift, Google BigQuery, and Apache Hive.
3. **Data Lakes**: Large repositories that store vast amounts of raw data in its native format, such as Amazon S3, Azure Data Lake Storage, and Hadoop Distributed File System (HDFS).
4. **Web Data**: Data scraped or fetched from web APIs, web pages, and online data sources.
5. **Databases**: Traditional relational databases (RDBMS) like MySQL, PostgreSQL, SQL Server, and NoSQL databases like MongoDB and Cassandra.
6. **Streaming Data Sources: Real-time data streams from platforms like Apache Kafka, Amazon Kinesis, and Apache Flume.

## Data Format

Here is a list of eight data formats that Apache Spark can read and write:

1. **CSV (Comma-Separated Values)**: A plain text format used to store tabular data.
2. **JSON (JavaScript Object Notation)**: A lightweight data interchange format that is easy for humans to read and write and easy for machines to parse and generate.
3. **Parquet**: A columnar storage file format optimized for use with big data processing frameworks.
4. **ORC (Optimized Row Columnar)**: A highly efficient columnar storage format for Hadoop workloads.
5. **Avro**: A row-based storage format that provides efficient serialization of data.
6. **Text**: Simple text files, where each line is a single record.
7. **XML** (Extensible Markup Language): A markup language that defines a set of rules for encoding documents in a format that is both human-readable and machine-readable.
8. **Delta Lake**: An open-source storage layer that brings ACID transactions to Apache Spark and big data workloads.

## Creating DataFrames from Various Data Sources

Here is a list of eight data formats that Apache Spark can read and write:

1. **CSV (Comma-Separated Values)**: A plain text format used to store tabular data.
2. **JSON (JavaScript Object Notation)**: A lightweight data interchange format that is easy for humans to read and write and easy for machines to parse and generate.
3. **Parquet**: A columnar storage file format optimized for use with big data processing frameworks.
4. **ORC (Optimized Row Columnar)**: A highly efficient columnar storage format for Hadoop workloads.
5. **Avro**: A row-based storage format that provides efficient serialization of data.
6. **Text**: Simple text files, where each line is a single record.
7. **XML (Extensible Markup Language)**: A markup language that defines a set of rules for encoding documents in a format that is both human-readable and machine-readable.
8. **Delta Lake**: An open-source storage layer that brings ACID transactions to Apache Spark and big data workloads.

### 1. Creating DataFrames from Flat Files

**CSV Files**

```python
from pyspark.sql import SparkSession

# Initialize SparkSession
spark = SparkSession.builder.appName("CSVExample").getOrCreate()

# Create DataFrame from CSV file
df = spark.read.csv("path/to/file.csv", header=True, inferSchema=True)

# Show the DataFrame
df.show()
```

**JSON Files**

```python
# Create DataFrame from JSON file
df = spark.read.json("path/to/file.json")

# Show the DataFrame
df.show()
```

**Text Files**

```python
# Create DataFrame from Text file
df = spark.read.text("path/to/file.txt")

# Show the DataFrame
df.show()
```

### 2. Creating DataFrames from Databases

**MySQL**

```python
# Create DataFrame from MySQL
df = spark.read.format("jdbc").option("url", "jdbc:mysql://localhost:3306/mydatabase") \
    .option("dbtable", "mytable") \
    .option("user", "myuser") \
    .option("password", "mypassword") \
    .load()

# Show the DataFrame
df.show()
```

**PostgreSQL**

```python
# Create DataFrame from MySQL
df = spark.read.format("jdbc").option("url", "jdbc:mysql://localhost:3306/mydatabase") \
    .option("dbtable", "mytable") \
    .option("user", "myuser") \
    .option("password", "mypassword") \
    .load()

# Show the DataFrame
df.show()
```

### 3. Creating DataFrames from Data Warehouses

**Apache Hive**

```python
# Configure Hive support
spark = SparkSession.builder.appName("HiveExample").enableHiveSupport().getOrCreate()

# Create DataFrame from Hive table
df = spark.sql("SELECT * FROM my_hive_table")

# Show the DataFrame
df.show()
```

**Amazon Redshift**

```python
# Create DataFrame from Redshift
df = spark.read.format("jdbc").option("url", "jdbc:redshift://examplecluster.abc123xyz789.us-west-2.redshift.amazonaws.com:5439/mydatabase") \
    .option("dbtable", "mytable") \
    .option("user", "myuser") \
    .option("password", "mypassword") \
    .load()

# Show the DataFrame
df.show()
```

### 4. Creating DataFrames from Data Lakes

**Amazon S3**

```python
# Read from S3
df = spark.read.csv("s3a://bucket-name/path/to/file.csv", header=True, inferSchema=True)

# Show the DataFrame
df.show()
```

**Azure Data Lake Storage**

```python
# Read from Azure Data Lake Storage
df = spark.read.csv("adl://example.azuredatalakestore.net/path/to/file.csv", header=True, inferSchema=True)

# Show the DataFrame
df.show()
```

### 5. Creating DataFrames from Web Data

**Web APIs**

```python
import requests
from pyspark.sql import SparkSession

# Fetch data from web API
response = requests.get("https://api.example.com/data")
data = response.json()

# Initialize SparkSession
spark = SparkSession.builder.appName("WebAPIExample").getOrCreate()

# Create DataFrame from JSON data
df = spark.createDataFrame(data)

# Show the DataFrame
df.show()

```


### 6. Creating DataFrames from Streaming Data Sources

**Apache Kafka**

```python
# Create DataFrame from Kafka
df = spark.read.format("kafka").option("kafka.bootstrap.servers", "localhost:9092") \
    .option("subscribe", "topic1") \
    .load()

# Show the DataFrame
df.show()
```

By leveraging these data sources and formats, Apache Spark allows you to create DataFrames that can be easily manipulated and analyzed, providing powerful tools for big data processing and analytics.

---------------------------------------------
# VII.Data Wrangling in Spark DataFrame 

## What's Data Wrangling ?

Data wrangling, also known as data munging, is the process of transforming and mapping data from its raw form into a more usable format. This often involves several steps, including cleaning, structuring, enriching, and validating the data. The goal of data wrangling is to make raw data more accessible and useful for analysis.

### Steps Involved in Data Wrangling

1. **Data Collection**: Gathering raw data from various sources such as databases, files, web APIs, or data lakes.
2. **Data Cleaning**: Identifying and correcting errors in the data. This includes handling missing values, removing duplicates, correcting inconsistencies, and filtering out irrelevant data.
3. **Data Transformation**: Converting data into a more appropriate format or structure. This can involve normalizing, aggregating, or scaling the data.
4. **Data Enrichment**: Enhancing the dataset by adding relevant information from other sources.
5. **Data Validation**: Ensuring the data meets the required quality and integrity standards. This step often involves verifying data types, ranges, and consistency.
6. **Data Structuring**: Organizing the data into a format or schema that is suitable for analysis or machine learning. This might include creating new columns, merging datasets, or pivoting data.

### Purpose of Data Wrangling

The primary purpose of data wrangling is to prepare data for analysis or machine learning by ensuring it is clean, structured, and enriched. This process is crucial because raw data is often messy and not immediately suitable for analysis. Data wrangling helps in:

1. **Improving Data Quality**: Cleaning and transforming data ensures that the dataset is accurate, complete, and free from errors, which is essential for reliable analysis.
2. **Enhancing Data Usability**: Structuring and formatting data makes it easier to analyze and visualize, enabling better decision-making.
3. **Facilitating Data Integration**: Data wrangling allows for the merging of data from different sources, providing a comprehensive view of the information.
4. **Enabling Advanced Analytics**: Preparing data properly is a prerequisite for applying advanced analytics techniques such as machine learning, as these methods require clean and well-structured data.

## Operarions

Data wrangling can be performed at multiple levels, including ingestion, column operations, row operations, general transformations of the DataFrame structure, specific character manipulations, time series structuring, and handling other formats such as images, audio, and video.

### 1. For Ingestion

- **Reading Data**: Ingest data from various sources like CSV, JSON, Parquet, Avro, ORC, JDBC, HDFS, S3, and more.

```python
df = spark.read.csv("path/to/file.csv", header=True, inferSchema=True)
df = spark.read.json("path/to/file.json")
df = spark.read.parquet("path/to/file.parquet")
df = spark.read.jdbc(url="jdbc:mysql://localhost:3306/db", table="table_name", properties={"user": "root", "password": "password"})
```

- **Schema Definition**: Define schemas explicitly when reading data to ensure correct data types.

```python
from pyspark.sql.types import StructType, StructField, StringType, IntegerType
schema = StructType([
    StructField("name", StringType(), True),
    StructField("age", IntegerType(), True)
])
df = spark.read.schema(schema).csv("path/to/file.csv", header=True)
```

- **Handling Missing Values**: Specify how to handle missing values during ingestion.

```python
df = spark.read.option("mode", "DROPMALFORMED").csv("path/to/file.csv", header=True)
```

### 2. Column Operations

- **Selecting Columns**: Select specific columns.

```python
df = df.select("name", "age")
```

- **Renaming Columns**: Rename columns.

```python
df = df.withColumnRenamed("old_name", "new_name")
```

- **Adding Columns**: Add new columns based on existing data.

```python
from pyspark.sql.functions import col, lit
df = df.withColumn("new_col", col("age") + 5)
df = df.withColumn("constant_col", lit(1))
```
  
- **Dropping Columns**: Remove columns from the DataFrame.

```python
df = df.drop("unnecessary_column")
```

- **Changing Data Types**: Convert column data types.

```python
df = df.withColumn("age", col("age").cast("string"))
```

### 3. Row Operations

- **Filtering Rows**: Filter rows based on a condition.

```python
df = df.filter(col("age") > 18)
```

- **Removing Duplicates**: Drop duplicate rows.

```python
df = df.dropDuplicates(["name", "age"])
```

- **Handling Missing Values**: Handle missing values by dropping or filling.

```python
df = df.na.drop()
df = df.na.fill({"age": 0, "name": "unknown"})
```

### 4. General Transformation of DataFrame Structure

- **Sorting Data**: Sort the DataFrame by columns.

```python
df = df.sort("age", ascending=False)
```
 
- **Grouping and Aggregation**: Group by columns and perform aggregations.

```python
df = df.groupBy("age").count()
df = df.groupBy("department").agg({"salary": "avg", "age": "max"})
```

- **Pivoting Data**: Pivot the DataFrame.

```python
df = df.groupBy("department").pivot("year").sum("salary")
```
 
- **Joining DataFrames**: Join multiple DataFrames.

```python
df1 = df1.join(df2, df1["id"] == df2["id"], "inner")
```

### 5. Working with Characters

- **String Manipulations**: Perform operations like trimming, upper/lower case conversion, substring extraction.

```python
from pyspark.sql.functions import lower, upper, trim, substring
df = df.withColumn("lower_name", lower(col("name")))
df = df.withColumn("upper_name", upper(col("name")))
df = df.withColumn("trimmed_name", trim(col("name")))
df = df.withColumn("sub_name", substring(col("name"), 1, 3))
```
 
- **Replacing Values**: Replace specific values in a column.

```python
df = df.withColumn("name", regexp_replace(col("name"), "old_value", "new_value"))
```

### 6. Working with Time Series

- **Date and Time Functions**: Extract or manipulate date and time information.

```python
from pyspark.sql.functions import year, month, dayofmonth, hour, minute, second, to_date, to_timestamp
df = df.withColumn("year", year(col("timestamp")))
df = df.withColumn("month", month(col("timestamp")))
df = df.withColumn("day", dayofmonth(col("timestamp")))
df = df.withColumn("date", to_date(col("timestamp")))
df = df.withColumn("datetime", to_timestamp(col("date_string"), "yyyy-MM-dd HH:mm:ss"))
```

- **Window Functions**: Perform calculations over a sliding window.

```python
from pyspark.sql.window import Window
from pyspark.sql.functions import row_number
window_spec = Window.partitionBy("department").orderBy("salary")
df = df.withColumn("rank", row_number().over(window_spec))
```

### 7. Handling Other Formats (Audio, Video, Images)

- **Reading Binary Files**: Read binary files like images.

```python
binary_df = spark.read.format("binaryFile").load("path/to/images/*")
```

- Using External Libraries: Use external libraries for specific formats.

1. **Audio**: Use libraries like pydub to process audio files.
2. **Video**: Use libraries like opencv for video processing.
3. **Images**: Use libraries like PIL or pyspark.ml.image for image processing

```python
from pyspark.ml.image import ImageSchema
image_df = ImageSchema.readImages("path/to/images")
```

By utilizing these operations, you can effectively wrangle data in Apache Spark, transforming it into a format that is suitable for analysis or machine learning. Each operation helps to clean, structure, and enhance the data, ensuring that it meets the necessary quality and usability standards.

---------------------------------------------
# VIII. Spark SQL 

Spark SQL is a module in Apache Spark that integrates relational processing with Spark's functional programming API. It allows you to query structured data inside Spark programs using SQL as well as the DataFrame API. This integration enables powerful and expressive data processing capabilities, leveraging the strengths of both relational and functional paradigms.

## What's Spark SQL ?

Spark SQL is a Spark module for structured data processing. It provides a programming abstraction called DataFrames and can also act as a distributed SQL query engine. It allows for seamless integration between SQL queries and complex analytics, providing a unified interface for querying and manipulating structured data.

Spark SQL provides several advantages, including:

- The ability to run SQL queries over data stored in various formats.
- Interoperability between SQL and Spark’s core APIs, allowing for complex data manipulation and analytics.
- Optimization through the Catalyst optimizer and Tungsten execution engine for improved performance.

## Key Features of Spark SQL.

1. **Unified Data Access**: Spark SQL provides a common way to access a variety of data sources such as Hive, Avro, Parquet, ORC, JSON, and JDBC.
2. **Hive Compatibility**: It supports querying data stored in Apache Hive, allowing for compatibility with existing Hive queries and UDFs.
3. **SQL Interface**: Allows users to run SQL queries, making it easy for those familiar with SQL to interact with Spark.
4. **Catalyst Optimizer**: A highly extensible query optimizer that ensures efficient query execution.
5. **Seamless Integration**: Integration with Spark’s core APIs allows users to intermix SQL queries with complex analytics.
6. **DataFrames and Datasets**: Provides high-level abstractions for manipulating structured data.


## Perform SQL like queries on Spark DataFrames

Spark SQL allows you to perform SQL-like queries on DataFrames using both SQL syntax and the DataFrame API. Here’s an example of both approaches:

1.  SQL Syntax:

```python
from pyspark.sql import SparkSession

# Initialize SparkSession
spark = SparkSession.builder.appName("SparkSQLExample").getOrCreate()

# Create a DataFrame
data = [("Alice", 29), ("Bob", 31), ("Catherine", 27)]
df = spark.createDataFrame(data, ["Name", "Age"])

# Register the DataFrame as a temporary view
df.createOrReplaceTempView("people")

# Perform SQL query
sqlDF = spark.sql("SELECT Name, Age FROM people WHERE Age > 28")
sqlDF.show()
```
2. DataFrame API:

```python
# Using DataFrame API
filteredDF = df.filter(df["Age"] > 28).select("Name", "Age")
filteredDF.show()
```

## Spark SQL Operations

Spark SQL supports a wide range of operations. Here are some of the key operations along with examples:

1. **Selecting Data**:

```python
from pyspark.sql import SparkSession

# Initialize SparkSession
spark = SparkSession.builder.appName("SparkSQLExample").getOrCreate()

# Create a DataFrame
data = [("Alice", 29), ("Bob", 31), ("Catherine", 27)]
df = spark.createDataFrame(data, ["Name", "Age"])

# Register the DataFrame as a temporary view
df.createOrReplaceTempView("people")

# Select specific columns
sqlDF = spark.sql("SELECT Name, Age FROM people")
sqlDF.show()
```

2. **Filtering Data**:

```python
# Filter rows based on a condition
sqlDF = spark.sql("SELECT Name, Age FROM people WHERE Age > 28")
sqlDF.show()
```

3. **Aggregating Data**:

```python
# Group by and aggregate
sqlDF = spark.sql("SELECT Age, COUNT(*) AS count FROM people GROUP BY Age")
sqlDF.show()

```

4. **Joining DataFrames**:

```python
# Create another DataFrame
data2 = [("Alice", "F"), ("Bob", "M"), ("Catherine", "F")]
df2 = spark.createDataFrame(data2, ["Name", "Gender"])

# Register the second DataFrame as a temporary view
df2.createOrReplaceTempView("people_gender")

# Join two DataFrames
sqlDF = spark.sql("SELECT p.Name, p.Age, pg.Gender FROM people p JOIN people_gender pg ON p.Name = pg.Name")
sqlDF.show()

```
5. **Sorting Data**:

```python
# Sort the DataFrame
sqlDF = spark.sql("SELECT Name, Age FROM people ORDER BY Age DESC")
sqlDF.show()

```

6. Union and UnionAll:

```python
# Union two DataFrames (Note: UnionAll is just Union in SQL context)
df_union = df.union(df2)
df_union.createOrReplaceTempView("people_union")

sqlDF = spark.sql("SELECT * FROM people_union")
sqlDF.show()
```

7. **Pivoting Data**:

```python
# Pivot the DataFrame (using GROUP BY and aggregation for pivot)
# Note: Pivot functionality in SQL syntax is complex and depends on the SQL dialect
# Example using Spark SQL:
pivotDF = df.groupBy("Name").pivot("Age").count()
pivotDF.show()
```

8. **UDFs (User-Defined Functions)**:

```python
from pyspark.sql.functions import udf
from pyspark.sql.types import IntegerType

# Define a UDF
def age_squared(age):
    return age * age

# Register the UDF
spark.udf.register("age_squared_udf", age_squared, IntegerType())

# Use the UDF in SQL
sqlDF = spark.sql("SELECT Name, Age, age_squared_udf(Age) AS AgeSquared FROM people")
sqlDF.show()

```

## Creating and managing temporary views

Temporary views in Spark SQL allow you to create a logical table that is scoped to the Spark session. These views can be queried using SQL syntax, making it easier to interact with DataFrames.

**Creating a Temporary View**:

```python
# Create a DataFrame
data = [("Alice", 29), ("Bob", 31), ("Catherine", 27)]
df = spark.createDataFrame(data, ["Name", "Age"])

# Create a temporary view
df.createOrReplaceTempView("people")
```

**Querying a Temporary View**:

```python
# Perform SQL query on the temporary view
sqlDF = spark.sql("SELECT Name, Age FROM people WHERE Age > 28")
sqlDF.show()
```

**Managing Temporary Views**:

1. Drop a Temporary View:

```python
spark.catalog.dropTempView("people")
```

2. Check if a Temporary View Exists:

```python
spark.catalog.tableExists("people")
```

3. List All Temporary Views:

```python
spark.catalog.listTables()
```

## So...

Spark SQL is a powerful component of Apache Spark that integrates SQL queries with the DataFrame API, providing a unified interface for processing structured data. By leveraging the power of SQL and the flexibility of DataFrames, Spark SQL enables efficient and scalable data processing, making it an essential tool for data engineers and analysts.

---------------------------------------------
# IX. Other Uses and Applications of PySpark

Besides performing data engineering tasks with PySpark, there are numerous other capabilities and applications that PySpark can facilitate. Here are some key areas where PySpark can be effectively utilized:

## 1. Data Analysis

PySpark provides powerful tools for data analysis, allowing you to perform complex aggregations, summarizations, and visualizations of large datasets.

**Descriptive Statistics**: Calculate summary statistics, such as mean, median, standard deviation, etc.
**Data Exploration**: Explore datasets with various filtering, grouping, and aggregation techniques.

## 2. Machine Learning

Spark's MLlib library offers scalable machine learning algorithms and utilities.

**Classification**: Algorithms like Logistic Regression, Decision Trees, Random Forests.

**Regression**: Linear Regression, Generalized Linear Models.

**Clustering**: K-means, Gaussian Mixture Models.

**Recommendation Systems**: Alternating Least Squares (ALS) for collaborative filtering.

**Feature Engineering**: Tools for transforming raw data into features suitable for machine learning models.

## 3. Graph Processing

GraphX is the graph processing API in Spark.

**Graph Algorithms**: Implement graph algorithms like PageRank, Connected Components, Triangle Counting.

**Graph Analytics**: Analyze large-scale graphs to uncover patterns and relationships.


## 4. Data Visualization

Integrate with libraries like Matplotlib, Seaborn, and Plotly to visualize data.

**Interactive Plots**: Create interactive visualizations for data exploration.

**Dashboards**: Build dashboards for real-time monitoring and reporting.


---------------------------------------------
# X.  PySpark Applications 

### 1. Aplication nª 1

### 2. Aplication nª 2

### 3. Aplication nª 3

### 4. Aplication nª 4

### 5. Aplication nª 5

---------------------------------------------
# XI. Other PySpark Resources

Staying updated with the latest developments in PySpark is crucial for anyone involved in Data field. Here is a list of some exclusive websites and resources dedicated to PySpark that can help you keep abreast of the latest trends, research, and tools.

1. **Apache Spark Official Documentation**

URL: [Apache Spark Documentation](https://spark.apache.org/documentation.html)

Description: The official documentation provides comprehensive information about all aspects of Spark, including PySpark. It includes user guides, API references, and examples.

2. **Databricks Community Edition**

URL: Databricks Community Edition

Description: Databricks offers a free Community Edition where you can practice PySpark. It also provides tutorials, notebooks, and a platform to run your Spark jobs.

3. **Spark + AI Summit**

URL: Spark + AI Summit

Description: An annual conference hosted by Databricks featuring talks, workshops, and keynotes from industry experts on Spark, AI, and machine learning. Recordings of past sessions are available online.

4. **Stack Overflow**

URL: Stack Overflow

Description: A popular Q&A platform where you can ask questions and find answers related to PySpark. The PySpark tag has a wide range of questions and answers from the community.

5. **GitHub Repositories**

URL: GitHub - Apache Spark

Description: The official GitHub repository for Apache Spark. You can explore the source code, contribute to the project, and find example projects and issues.

6. **PySpark Tutorials on Medium**

URL: Medium - PySpark

Description: Medium hosts numerous articles and tutorials on PySpark written by data scientists and engineers. It’s a great resource for learning new techniques and best practices.

7. **Kaggle Datasets and Notebooks**

URL: Kaggle - PySpark

Description: Kaggle offers datasets and notebooks where you can find and share PySpark projects. It’s a great platform for practical learning and experimentation.

8. **YouTube Channels**

URL: YouTube - PySpark

Description: There are several YouTube channels dedicated to PySpark tutorials and webinars. These videos can help you learn PySpark through visual and practical demonstrations.

9. **Coursera - Big Data Analysis with Scala and Spark**

URL: Coursera - Spark Course

Description: A course offered by Coursera that covers big data analysis using Spark. It includes hands-on projects and assignments to enhance your PySpark skills.

10. **PySpark User Mailing List**

URL: PySpark User Mailing List

Description: The user mailing list for PySpark hosted by Apache. It’s a place to discuss PySpark-related issues, share solutions, and stay updated with announcements and developments.

These resources provide a comprehensive set of tools, documentation, and community support to help you stay current with PySpark and enhance your skills in data processing and analysis.

# XII. PySpark tutorials

Some awesome YouTube videos about PySpark

1. https://www.youtube.com/watch?v=EB8lfdxpirM&t=2268s
2. https://www.youtube.com/watch?v=_C8kWso4ne4&t=10s
3. https://www.youtube.com/watch?v=sSkAuTqfBA8
4. https://www.youtube.com/watch?v=xDEzSxlsUpU&t=26724s
5. https://www.youtube.com/watch?v=GFC2gOL1p9k
6. https://www.youtube.com/watch?v=OHhNi56euvM
7. https://www.youtube.com/watch?v=S2MUhGA3lEw&t=19622s
8. https://www.youtube.com/watch?v=WyZmM6K7ubc&list=PLZoTAELRMXVNjiiawhzZ0afHcPvC8jpcg
9. https://www.youtube.com/watch?v=AGgyf9bO_8M&list=PLlUZLZydkS7_8WnK8fMENmJFSfPwxw9Fi
10. https://www.youtube.com/watch?v=6MaZoOgJa84&list=PLMWaZteqtEaJFiJ2FyIKK0YEuXwQ9YIS_


