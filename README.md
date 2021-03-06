# DP900-notes


# DP-900

Azure Data Fundamentals


Structrued -- Table and RDBMS\
Semi Structred -- JSON, Key-value pair, graph DB.\
Unstructured -- videos, files, binary objects etc

Online Transactional Processing (OLTP).

Splitting tables out into separate groups of columns like this is called normalized.


A transaction is a sequence of operations that are atomic. All or none.\
A transactional database must adhere to the ACID (Atomicity, Consistency, Isolation, Durability) 
properties to ensure that the database remains consistent while processing transactions.




    Identify how data is defined and stored
    Identify characteristics of relational and non-relational data
    Describe and differentiate data workloads
    Describe and differentiate batch and streaming data
    
        
    Roles:--\
    Database Administrators manage databases, assigning permissions to users, 
    storing backup copies of data and restore data in case of any failures.\
    
    Data Engineers are vital in working with data, applying data cleaning routines, 
    identifying business rules, and turning data into useful information.\
    
    Data Analysts explore and analyze data to create visualizations 
    and charts to enable organizations to make informed decisions.\
    
    Azure Data Studio provides a graphical user interface for managing many different database systems.\    
    
    
    As a SQL Server professional, your primary data manipulation tool might be Transact-SQL.
    
    
    As a data engineer you might use additional technologies, such as Azure Databricks, and Azure HDInsight 
    to generate and test predictive models.
    If you're working in the non-relational field, you might use Azure Cosmos DB as your primary data store.
    To manipulate and query the data, you might use languages such as HiveQL, R, or Python.
    
    
     A good data analyst requires experience and skills in reporting tools such as Microsoft Power BI and SQL Server Reporting Services.
     
     
     All rows in the same table have the same columns.
     Some columns are used to maintain relationships between tables. This is where the relational model gets its name from.
     
     An index helps you search for data in a table.
     
     A view is a virtual table based on the result set of a query. 
     
     
     
     A key aspect of non-relational databases is that they enable you to store data in a very flexible manner.
     Non-relational databases don't impose a schema on data. 
     Instead, they focus on the data itself rather than how to structure it.
     This approach means that you can store information in a natural format, 
     that mirrors the way in which you would consume, query and use it.
     
     
     
     Non-relational data generally falls into two categories; semi-structured and non-structured.
     Non-relational data is an all-encompassing term that means anything not structured as a set of tables.
     NoSQL is a rather loose term that simply means non-relational.
     
     NoSQL (non-relational) databases generally fall into four categories: 
     key-value stores, document databases, column family databases, and graph databases.
     
     
     The focus of a key-value store is the ability to read and write data very quickly.
     Search capabilities are secondary.
     A key-value store is an excellent choice for data ingestion, 
     when a large volume of data arrives as a continual stream and must be stored immediately.
    
    A graph database stores two types of information: 
    nodes that you can think of as instances of entities, 
    and edges, which specify the relationships between nodes.
    
    Azure Cosmos DB supports graph databases using the Gremlin API.
    The Gremlin API is a standard language for creating and querying graphs.
    
    Azure Data Factory is a cloud-based data integration service that allows you to 
    create data-driven workflows for orchestrating data movement and transforming data at scale. 
    
    The term Business Intelligence (BI) refers to technologies, applications, and 
    practices for the collection, integration, analysis, and presentation of business information.
    The purpose of business intelligence is to support better decision making.
    
    Data visualization helps you to focus on the meaning of data, rather than looking at the data itself.
    
    Types of charts etc
    Scatter
    Treemap
    Matrix
    Line charts
    Bar and column charts
       
    
    -------
    The process of combining all of the local data sources is known as data warehousing.
    A data warehouse gathers data from many different sources within an organization.
    This data is then used as the source for analysis, reporting, and online analytical processing (OLAP).
    
    
    Data warehouses have to handle big data.
    Big data is the term used for large quantities of data collected in escalating volumes, 
    at higher velocities, and in a greater variety of formats than ever before.
    It can be historical (meaning stored) or real time (meaning streamed from the source). 
    Businesses typically depend on their big data to help make critical business decisions.
    
    A modern data warehouse might contain a mixture of relational and non-relational data, 
    including files, social media streams, and Internet of Things (IoT) sensor data.
    
    Azure provides a collection of services you can use to build a data warehouse solution, 
    including Azure Data Factory, Azure Data Lake Storage, Azure Databricks, Azure Synapse Analytics, and Azure Analysis Services.
    
    Data Ingestion -- Data Factory
    Data Bricks -- Tiding data, extra things for cleasing, data transformation  etc.
    Data Analysis  -- Synapse services , hub for clean business data
    Power BI can be used on data bricks for visualization and analytics
    Azure analysis services
    https://www.microsoft.com/en-us/videoplayer/embed/RE4A3RR?postJsllMsg=true
    
    Data Factory -- Data Ingestion like HiveMQ or Kafka or Firehose.
    Data Lake -- Raw storage, Staging area.
    Data Bricks -- Spark
    Azure Synapse Analytics -- like Teradata MPP  , this is a Data Warehouse.
    HDInsights -- Hadoop its uses data lake to store data.
    
    The process of analyzing streaming data and data from the Internet is known as Big Data analytics.
    Azure Synapse Analytics combines data warehousing with Big Data analytics.
    
    
    Azure Data Factory is described as a data integration service.
    The purpose of Azure Data Factory is to retrieve data from one or more data sources, 
    and convert it into a format that you process.
    You define the work performed by Azure Data Factory as a pipeline of operations.
    A pipeline can run continuously, as data is received from the various data sources. 
    GUI or Code the pipelines.
    
    
    A data lake is a repository for large quantities of raw data.
    Because the data is raw and unprocessed, it's very fast to load and update,
    but the data hasn't been put into a structure suitable for efficient analysis.
    You can think of a data lake as a staging point for your ingested data, 
    before it's massaged and converted into a format suitable for performing analytics.
    
    
    A data warehouse also stores large quantities of data, 
    but the data in a warehouse has been processed to convert it into a format for efficient analysis.
    A data lake holds raw data, but a data warehouse holds structured information.
    
    
    Azure Data Lake Storage is essentially an extension of Azure Blob storage, organized as a near-infinite file system.
    
    
    Azure Databricks is an Apache Spark environment running on Azure to provide big data processing, streaming, and machine learning.
    
    
    Azure Synapse Analytics is an analytics engine.
    It's designed to process large amounts of data very quickly.
    
    Azure Synapse Analytics leverages a massively parallel processing (MPP) architecture.
    This architecture includes a control node and a pool of compute nodes.
    
    The Compute nodes provide the computational power.
    The data to be processed is distributed evenly across the nodes.
    Users and applications send processing requests to the control node. 
    The control node sends the queries to compute nodes, which run the queries over the portion of the data that they each hold.
    When each node has finished its processing, the results are sent back to the control node where they're combined into an overall result.
    
    Azure Synapse Analytics supports two computational models: SQL pools and Spark pools.
    
    
    Azure Analysis Services enables you to build tabular models to support online analytical processing (OLAP) queries.
    
    Analysis Services includes a graphical designer to help you connect data sources together and define queries
    that combine, filter, and aggregate data.
    You can explore this data from within Analysis Services, or you can use a
    tool such as Microsoft Power BI to visualize the data presented by these models.
    
    Azure Analysis Services has significant functional overlap with Azure Synapse Analytics, 
    but it's more suited for processing on a smaller scale.
    
    Azure HDinsights is Spark pool version of synapse analytics. 
 
    
    Data Factory moves data from a data source to a destination.
    A linked service provides the information needed for Data Factory to connect to a source or destination.
    For example, you can use an Azure Blob Storage linked service to connect a storage account to Data Factory, 
    or the Azure SQL Database linked service to connect to a SQL database.
    
    
    You write and run Spark code using notebooks.
    A notebook is like a program that contains a series of steps (called cells).
    A notebook can contain cells that read data from one or more data sources, process the data, and write the results out to a data store.
    
        
    How to load a flat file (comma delimeted) from azure storage (file sahre) to Azure Synatic Analtics SQL Pool as Datawarehouse.
    https://www.microsoft.com/en-us/videoplayer/embed/RE4Asf7?postJsllMsg=true
    
    
    To analyze operational data in its original location.
    This strategy is known as hybrid transactional analytical processing (HTAP).
    
    
    Apache strom -- 
    Apache Storm is a scalable, fault tolerant platform for running real-time data processing applications.
    Storm is designed for reliability, so that events shouldn't be lost
    Storm can interoperate with a variety of event sources, including 
    Azure Event Hubs, Azure IoT Hub, Apache Kafka, and RabbitMQ .
    Storm can also write to data stores such as HDFS, Hive, HBase, Redis, and SQL databases. 
    
    
    Data lake is made up of:--
    Data Lake Store
    Data Lake Analytics
    HDInsight
   
    
    
    Microsoft Power BI is a collection of software services, apps, and connectors that work together to turn your 
    unrelated sources of data into coherent, visually immersive, and interactive insights. 
    
    
 PowerBI Service can be connected to Github and get all stats like pull requests, most contribution etc .\
 See diagram fro better undersating of PowerBI service , app and BIDesktop.![powerbi](https://user-images.githubusercontent.com/22178819/109792442-887ff780-7c39-11eb-993c-16bab8441167.JPG)

    
    Bring data into Power BI Desktop, and create a report.
    Publish to the Power BI service, where you create new visualizations or build dashboards.
    Share your dashboards with others, especially people who are on the go.
    View and interact with shared dashboards and reports in Power BI Mobile apps.
    
    Building blocks of PowerBI
    Visualizations, datasets, reports, dashboards, tiles.
    
    A collection of ready-made visuals, pre-arranged in dashboards and reports is called an app  Power BI.
    
    
 ---------------------------------------\
 Azure Data Fundamentals: Explore relational data in Azure

    Azure Data Services fall into the PaaS category.
    
    limit the range of custom administration tasks that you can perform
    these services are designed to be always on. This means that you can't shut down a database and restart it later.
    
    
    If you don't want to incur the management overhead associated with running SQL Server on a virtual machine, you can use Azure SQL Database.
    
    Azure SQL Database is available with several options: Single Database, Elastic Pool, and Managed Instance.
    
    Single DB -- Serverless and Server either ways we dont have to manage the VMs.
    
    Elastic pool -- This option is similar to Single Database, except that by default multiple 
    databases can share the same resources, such as memory, data storage space, and processing power through multiple-tenancy.
    
    However, neither Single Database nor Elastic Pool support linked servers
    The Single Database and Elastic Pool options restrict some of the administrative features available to SQL Server. 
    
    The Managed instance service automates backups, software patching, database monitoring, and other general tasks, 
    but you have full control over security and resource allocation for your databases.
    
    Managed instances depend on other Azure services such as Azure Storage for backups, Azure Event Hubs for telemetry, 
    Azure Active Directory for authentication, Azure Key Vault for Transparent Data Encryption (TDE) and a couple 
    of Azure platform services that provide security and supportability features. 
    The managed instances make connections to these services.
![Azuresql](https://user-images.githubusercontent.com/22178819/109799839-7f475880-7c42-11eb-8ee3-586ba8fc7c0a.JPG)


     if you want to lift-and-shift an on-premises SQL Server instance and all its databases to the cloud, 
     without incurring the management overhead of running SQL Server on a virtual machine. -- Managed SQL INstances are used.
     
     Automated tasks include operating system and database management system software installation and patching, 
     dynamic instance resizing and configuration, backups, database replication (including system databases), 
     high availability configuration, and configuration of health and performance monitoring data streams.
     
     
     MySQL -- Community, Standard, and Enterprise.
     
     MariaDB is a newer database management system, created by the original developers of MySQL. 
     One notable feature of MariaDB is its built-in support for temporal data. 
     A table can hold several versions of data, enabling an application to query the data as it appeared at some point in the past.
     
     PostgreSQL is a hybrid relational-object database. 
   ![3dbs](https://user-images.githubusercontent.com/22178819/109802111-65f3db80-7c45-11eb-8979-4531fcdce741.JPG)
   
   
   The Database Migration Service enables you to restore a backup of your
   on-premises databases directly to databases running in Azure Data Services. 
   
   
   The default connectivity for Azure relational data services is to disable access to the world.
   
   
   
Advanced data security implements threat protection and assessment.\
Threat protection adds security intelligence to your service.\
This intelligence monitors the service and detects unusual patterns of activity that 
could be harmful, or compromise the data managed by the service.
     
If you're connecting from within another Azure service, such as a web application running under Azure App Service, your connections have a connection policy of Redirect by default


If you're connecting from outside Azure, such as an on-premises application, your connections have a connection policy of Proxy by default. 

Denial of service (DoS) attacks are reduced by a SQL Database gateway service called DoSGuard. DoSGuard actively tracks failed logins from IP addresses.

Azure SQL Database gateway  -- Is used to connect to Azure SQL DB.

    AZure SQL -- 1443
    Azure database for Postgres 5432
    Azure Database for Mysql 3306






Dialects of SQL:--
    Transact-SQL (T-SQL). This version of SQL is used by Microsoft SQL Server and Azure SQL Database.

    pgSQL. This is the dialect, with extensions implemented in PostgreSQL.

    PL/SQL. This is the dialect used by Oracle. PL/SQL stands for Procedural Language/SQL.


    Data Manipulation Language (DML)
    Data Definition Language (DDL)


SQL doesn't provide are you sure? prompts, so be careful when using DELETE or UPDATE without a WHERE clause because you can lose or modify a lot of data.

    DML
    SELECT 	Select/Read rows from a table
    INSERT 	Insert new rows into a table
    UPDATE 	Edit/Update existing rows
    DELETE 	Delete existing rows in a table

    The following query shows an example that joins two tables, named Inventory and CustomerOrder. 
    It retrieves all rows where the value in the ID column in the Inventory table matches the value in the InventoryID column in the CustomerOrder table.
    
    SELECT *
    FROM Inventory
    JOIN CustomerOrder
    WHERE Inventory.ID = CustomerOrder.InventoryID

SQL provides aggregate functions. An aggregate function calculates a single result across a set of rows or an entire table. The example below finds the minimum value in the MyColumn1 column across all rows in the MyTable table:

    SELECT MIN(MyColumn1)
    FROM MyTable
Other aggregate fuctions MAX, AVG, SUM


DDL\
You use DDL statements to create, modify, and remove tables and other objects in a database (table, stored procedures, views, and so on).

    CREATE 	Create a new object in the database, such as a table or a view.
    ALTER 	Modify the structure of an object. For instance, altering a table to add a new column.
    DROP 	Remove an object from the database.
    RENAME 	Rename an existing object.


From where to run queries


    The query editor in the Azure portal
    The sqlcmd utility from the command line or the Azure Cloud Shell
    SQL Server Management Studio
    Azure Data Studio
    SQL Server Data Tools


------------------------- \
Azure Data Fundamentals: Explore non-relational data in Azure


    Azure Table Storage implements the NoSQL key-value model.
    In this model, the data for an item is stored as a set of fields, and the item is identified by a unique key.
    
    Azure Table Storage is a scalable key-value store held in the cloud. You create a table using an Azure storage account.
    Table storage is also callled a  structred nosql database.
    
    Azure Table Storage tables have no concept of relationships, stored procedures, secondary indexes, or foreign keys.
    
        To help ensure fast access, Azure Table Storage splits a table into partitions.
    Partitioning is a mechanism for grouping related rows, based on a common property or partition key.
    Rows that share the same partition key will be stored together.
    Partitioning not only helps to organize data, it can also improve scalability and performance:
    
    
    The columns in a table can hold numeric, string, or binary data up to 64 KB in size.
    A table can have up to 252 columns, apart from the partition and row keys.
    The maximum row size is 1 MB.
    
    The primary key for an Azure entity consists of the combined PartitionKey and RowKey properties.
    Partitions represent a collection of entities with the same PartitionKey values. 
    
    The data for each table is replicated three times within an Azure region.
    
    
    Many applications need to store large, binary data objects, such as images and video streams.
    Microsoft Azure virtual machines use blob storage for holding virtual machine disk images. 
    
    3 types of blobs in azure
     
    Block blobs. 
    A block blob is handled as a set of blocks.
    Each block can vary in size, up to 100 MB.
    A block blob can contain up to 50,000 blocks, giving a maximum size of over 4.7 TB.
    The block is the smallest amount of data that can be read or written as an individual unit.
    Block blobs are best used to store discrete, large, binary objects that change infrequently.
    
    
    Append blobs. 
    An append blob is a block blob optimized to support append operations.
    You can only add blocks to the end of an append blob; 
    updating or deleting existing blocks isn't supported. 
    Each block can vary in size, up to 4 MB.
    The maximum size of an append blob is just over 195 GB.

    Page blobs.
    A page blob is organized as a collection of fixed size 512-byte pages.
    A page blob is optimized to support random read and write operations; you can fetch and store data for a single page if necessary.
    A page blob can hold up to 8 TB of data.
    Azure uses page blobs to implement virtual disk storage for virtual machines.


Inside an Azure storage account, you create blobs inside containers. 

Blob storage provides three access tiers,\
Hot,cool, archieve



To retrieve a blob from the Archive tier, you must change the access tier to Hot or Cool.\
The blob will then be rehydrated. You can read the blob only when the rehydration process is complete.


You can create lifecycle management policies for blobs in a storage account.

fetaures are there like -- versioning, soft delete, snapshots.

Azure File storage

Azure File Storage enables you to create files shares in the cloud, and access these file shares from anywhere with an internet connection.

Azure File Storage offers two performance tiers.
The Standard tier uses hard disk-based hardware in a datacenter, and the Premium tier uses solid-state disks. 


Cosmos DB\
A document can hold up to 2 MB of data, including small binary objects.\
If you need to store larger blobs as part of a document, use Azure Blob storage, and add a reference to the blob in the document.

    Table API. 
    This interface enables you to use the Azure Table Storage API to store and retrieve documents. 
    The purpose of this interface is to enable you to switch from Table Storage to 
    Cosmos DB without requiring that you modify your existing applications.
    
    MongoDB API. (Document)
    MongoDB is another well-known document database, with its own programmatic interface. 
    Many organizations run MongoDB on-premises. 
    You can use the MongoDB API for Cosmos DB to enable a MongoDB application to run unchanged against a Cosmos DB database. 
    You can migrate the data in the MongoDB database to Cosmos DB running in the cloud,
    but continue to run your existing applications to access this data.    
    
    Cassandra API. (Column)
    Cassandra is a column family database management system. 
    This is another database management system that many organizations run on-premises. 
    The Cassandra API for Cosmos DB provides a Cassandra-like programmatic interface for Cosmos DB.
    
    Gremlin API. (Graph)
    The Gremlin API implements a graph database interface to Cosmos DB.
    
    
   The primary purpose of the Table, MongoDB, Cassandra, and Gremlin APIs is to support existing applications.
   If you are building a new application and database, you should use the SQL API.
   
   
Documents in a Cosmos DB database are organized into containers.
The documents in a container are grouped together into partitions.
A partition holds a set of documents that share a common partition key.

containers == tables.

similarity between a Cosmos DB container and a table in Azure Table storage: 
in both cases, data is partitioned and documents (rows in a table) are identified by a unique ID within a partition

Unlike Azure Table storage, documents in a Cosmos DB partition aren't sorted by ID. \
Instead, Cosmos DB maintains a separate index.\
This index contains not only the document IDs, 
but also tracks the value of every other field in each document.\
This index is created and maintained automatically.\
This index enables you to perform queries that specify criteria referencing any fields in a container, \
without incurring the need to scan the entire partition to find that data.




partition can grow up to 10 GB in size.\
Indexes are created and maintained automatically.There's virtually no administrative overhead.\
Cosmos DB provides row level authorization and adheres to strict security standards.\
The Cosmos DB SDKs can be used to build rich iOS and Android applications using the popular Xamarin framework.

Azure Cosmos DB uses the concept of Request Units per second (RU/s) to manage the performance and cost of databases.

 If you specify throughput for a database, all the containers in that database share that throughput.\
 If you specify throughput for a container, the container gets that throughput all to itself.
 
 The minimum throughput you can allocate to a database or container is 400 RU/s
 
 However, once you allocate throughput to a database or container, \
 you'll be charged for the resources provisioned, whether you use them or not.
 
 
 
 Data Lake storage is only available with a standard storage account, not premium.
 
 The total size of all files across all file shares in a storage account can't exceed 5120 GB.
 
 
 The default connectivity for Azure Cosmos DB and Azure Storage is to enable access to the world at large. 
 
 Azure Private Endpoint is a network interface that connects you privately and securely to a service powered by Azure Private Link. 


Eventual consistency provides the lowest latency and least consistency.
Strong consistency results in the highest latency but also the greatest consistency.


You can use shared access signatures (SAS) to grant limited rights to resources in an Azure storage account for a specified time period.

     security principal (Who?)
     role definition (What?)
     scope (Where?)
     
   
 Practical \
            it takes 15 min to create a cosmos db storage account.\
            database == DB in cosmos \
            container == table in cosmos 
  
  container for blob storage vs container for data lake storage.\
  While creatng a storge account with data lake storage -- select enabled for data lake and standrad as storaage type.\
  After creation of account, containers in data lake storage section is how you create stuff for data lake.
  
  For plain containers, under the overview section in left pane itself you will see containers, file shares, queues and tables.
  
  both containers i.e of data lake and of blob will be visible under the overview left pane section of containers.
  
  
  Cosmos DB uses JSON (JavaScript Object Notation) to represent the document structure.\
  Although Azure Cosmos DB is described as a NoSQL database management system, \
  the SQL API enables you to run SQL-like queries against Cosmos DB databases.
  
  
 
 
5 Types of analytics: Prescriptive, Predictive, Diagnostic, Descriptive and Cognitive Analytics\
Descriptive Analytics: -- What is happening in my business? 

Diagnostic Analytics: -- Why it is happening in your business or in general you want to know the root cause behind that, \
this is where Diagnostic analytics plays its part and helps analysts or data scientists to drill down inside the data to find the answer.

Predictive Analytics: -- what is likely to happen in the future based on previous trends and patterns?

Prescriptive Analytics: -- Prescriptive model utilizes those answers to help you determine the best course of action to choose to bypass or eliminate future issues.


Cognitive Analytics: -- Cognitive analytics combines a number of intelligent technologies like artificial intelligence, machine-learning algorithms, deep learning etc.to apply human brainlike intelligence to perform certain tasks.
