# aws-cheat-sheet

Here's a list of questions categorized by AWS topics:

## Database Types Overview

### Amazon RDS (Relational Database Service)
- **Features:** Managed relational database service offering scaling, automated patching, backup, and recovery. Supports multiple database engines such as MySQL, PostgreSQL, Oracle, SQL Server, and MariaDB.
- **Differences:** Designed for structured data with complex transactions and queries, offering ACID (Atomicity, Consistency, Isolation, Durability) properties. Automates administrative tasks like hardware provisioning, database setup, patching, and backups.

### Amazon DynamoDB
- **Features:** Fully managed NoSQL database service designed for fast and predictable performance with seamless scalability. Supports key-value and document data models.
- **Differences:** Optimized for unstructured or semi-structured data. Provides high availability and durability across multiple AWS regions with built-in security, backup, restore, and in-memory caching.

### Amazon Aurora
- **Features:** Part of AWS RDS, it's a MySQL and PostgreSQL-compatible relational database built for the cloud, providing increased performance and availability.
- **Differences:** Automatically divides data into partitions for performance and scalability. Offers features like multi-AZ deployments, replication across three Availability Zones, and continuous backup to Amazon S3.

### Amazon Redshift
- **Features:** A fully managed, petabyte-scale data warehouse service in the cloud. It allows users to analyze data using standard SQL and existing Business Intelligence (BI) tools. It's designed for complex querying and analysis of large datasets, optimized for high performance.
- **Differences:** Compared to RDS and DynamoDB, Redshift is specifically designed for data warehousing and analytics, supporting massive volumes of data and complex query execution.

### Amazon Elasticache
- **Features:** A fully managed in-memory data store and cache service. It supports Redis and Memcached engines. Elasticache is designed to deploy, operate, and scale an in-memory data store or cache in the cloud easily.
- **Differences:** Primarily used to improve the performance of web applications by allowing you to retrieve information from fast, managed, in-memory caches, rather than relying solely on slower disk-based databases.

### Amazon DocumentDB (with MongoDB compatibility)
- **Features:** A fully managed document database service that supports MongoDB workloads. It's designed to be compatible with MongoDB, allowing users to use existing MongoDB drivers and tools. DocumentDB is designed for scalability, durability, and manageability.
- **Differences:** Targets the needs of MongoDB users specifically, providing capabilities like document storage, indexing, and query execution. It offers scalability and security for document database management.

### Amazon Neptune
- **Features:** A fully managed graph database service. It's optimized for storing billions of relationships and querying the graph with milliseconds latency. Neptune supports popular graph models like Property Graph and RDF, along with their respective query languages, Apache TinkerPop Gremlin, and SPARQL.
- **Differences:** Specifically designed for graph database use cases such as recommendation engines, fraud detection, and knowledge graphs. Unlike relational or key-value databases, Neptune is optimized for connecting data points and uncovering relationships.

### Amazon Keyspaces (for Apache Cassandra)
- **Features:** A scalable, highly available, and managed Apache Cassandra-compatible database service. It's designed for applications that require Cassandra's flexibility, scalability, and expressive query capabilities without the need to manage the underlying infrastructure.
- **Differences:** Provides the benefits of the Apache Cassandra NoSQL database system without the operational burden. It's designed for cases requiring wide-column store capabilities, such as high write and read throughput.

These services complement the AWS database ecosystem by covering a wide range of data storage, management, and analysis needs, from in-memory caching to graph databases and data warehousing.

Here's a table summarizing the features and differences of various AWS database services, including Amazon RDS, DynamoDB, Aurora, Redshift, Elasticache, DocumentDB, Neptune, and Keyspaces, in Markdown format:

| Service              | Type                   | Features                                                                                                                                                      | Differences                                                                                                                                                                   |
|----------------------|------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Amazon RDS           | Relational Database    | - Managed relational database service<br>- Supports MySQL, PostgreSQL, Oracle, SQL Server, and MariaDB<br>- Offers scaling, automated patching, backup, and recovery | - Designed for structured data with ACID properties<br>- Automates tasks like hardware provisioning, setup, patching, and backups                                            |
| Amazon DynamoDB      | NoSQL Database         | - Fully managed NoSQL database<br>- Fast and predictable performance with seamless scalability<br>- Supports key-value and document data models                  | - Optimized for unstructured or semi-structured data<br>- High availability and durability across AWS regions                                                                  |
| Amazon Aurora        | Relational Database    | - MySQL and PostgreSQL-compatible<br>- Built for the cloud, providing increased performance and availability<br>- Part of AWS RDS                                 | - Automatically divides data into partitions<br>- Offers multi-AZ deployments and continuous backup to Amazon S3                                                               |
| Amazon Redshift      | Data Warehouse         | - Petabyte-scale data warehouse<br>- Analyze data using standard SQL and existing BI tools                                                                      | - Designed for complex querying and analysis of large datasets                                                                                                                 |
| Amazon Elasticache   | In-memory Data Store   | - Managed in-memory data store and cache<br>- Supports Redis and Memcached engines                                                                              | - Improves performance of web applications by retrieving information from fast, managed, in-memory caches                                                                      |
| Amazon DocumentDB    | Document Database      | - Managed document database service<br>- Supports MongoDB workloads                                                                                            | - Provides scalability, durability, and manageability for MongoDB users                                                                                                        |
| Amazon Neptune       | Graph Database         | - Managed graph database service<br>- Optimized for storing relationships and querying with milliseconds latency<br>- Supports Property Graph and RDF             | - Designed for connecting data points and uncovering relationships in recommendation engines, fraud detection, and knowledge graphs                                           |
| Amazon Keyspaces     | Wide-column Store      | - Scalable, highly available, and managed Apache Cassandra-compatible database service                                                                          | - Offers the benefits of Apache Cassandra without the operational burden, designed for high write and read throughput                                                          |

This table provides a quick overview of the main features and unique aspects of each AWS database service, helping to distinguish between them based on their intended use cases and underlying technologies.

## Database Questions

### Amazon RDS Tasks:
- Which task can be automatically performed by Amazon Relational Database Service (Amazon RDS) or manually performed by a user?

### Creating DB Instance in Amazon RDS:
- Which option must be specified first when creating a database (DB) instance in Amazon Relational Database Service (Amazon RDS)?

### High Availability in Amazon RDS:
- Which task is a best practice for high availability in an Amazon Relational Database Service (Amazon RDS) database (DB) instance?

### Use Case for Amazon RDS:
- Which use case represents a reason for using Amazon Relational Database Service (Amazon RDS) instead of other database solutions?

### Amazon Aurora DB Cluster:
- What is an Amazon Aurora database (DB) cluster?

### Amazon DynamoDB Type:
- Which type of database is Amazon DynamoDB?

### Amazon DynamoDB High Availability and Scalability:
- How does Amazon DynamoDB achieve high availability and scalability across Regions?

### Partitioning in Amazon DynamoDB:
- Which statement describes the concept of partitioning in Amazon DynamoDB?

### Amazon DynamoDB Partition Keys:
- Which statement about Amazon DynamoDB partition keys is true?

### Retrieving Data from Amazon DynamoDB:
- How many ways can Amazon DynamoDB retrieve data from a DynamoDB table?

### AWS Well-Architected Framework
- **Foundational Questions Resource**: Which resource provides a set of foundational questions that customers can use to understand if their architecture aligns with cloud best practices?
- **Recovery and Disruption Mitigation Pillar**: Which AWS Well-Architected Framework pillar provides details about how to recover from failure and mitigate disruption?
- **Design Principle**: What is a key design principle when designing a framework in the cloud?

### AWS Cloud Migration and Services
- **Server Replacement Service**: A company is migrating to an AWS Cloud environment. Their servers are the last set of resources that they will migrate. Which AWS service resource can replace a traditional server?
- **Cloud Adoption Framework Perspectives**: What are the two primary perspectives in the AWS Cloud Adoption Framework (AWS CAF)?

### AWS Systems Operations
- **Automation Benefits**: What is a benefit of automating systems operations tasks?
- **Systems Operations Task**: Which of the following is a systems operations task?

### AWS Identity and Access Management (IAM)
- **IAM Policy for S3 Bucket**: A network engineer must create an AWS IAM policy for an Amazon S3 bucket. Which policy type should the engineer use?
- **IAM Best Practices**: Which statements are best practices for AWS IAM?

### AWS Command Line Interface (CLI)
- **CLI Operation Specification**: Which part of the following AWS CLI command specifies the operation to be performed?

### AWS Systems Manager
- **Document for EC2 Snapshot**: Which type of AWS Systems Manager document can take a snapshot of an Amazon EC2 instance?
- **Configuration Data Storage**: Which AWS Systems Manager capability can store configuration data?
- **Direct Connection Capability**: Which AWS Systems Manager capability can connect to an instance directly from the AWS Management Console?

### AWS CloudFormation and Automation
- **Supported Markup Languages**: Which markup languages are supported in AWS CloudFormation?
- **Service Based on Chef and Puppet**: Which AWS service is based on the Chef and Puppet automation platforms?

### Deployment and Scaling
- **Blue/Green Deployment Routing Policy**: A systems administrator wants to create a blue/green deployment infrastructure by using Amazon Route 53 to gradually phase out the blue environment. Which Route 53 routing policy should the administrator use?
- **Scaling Policy Based on CloudWatch Alarm**: Which type of scaling policy uses an Amazon CloudWatch alarm and varies the scaling response based on the size of the alarm breach?

### AWS Content Delivery and Load Balancing
- **Content Delivery Network Service**: Which Amazon Web Services (AWS) service is a content delivery network (CDN)?
- **ELB Load Balancer Type**: Which type of Elastic Load Balancing (ELB) load balancer should a network engineer use to distribute requests to a website running on an Amazon Elastic Compute Cloud (Amazon EC2) instance in a virtual private cloud (VPC)?
- **ALB Connection Request Checker**: Which component of an Application Load Balancer checks for connection requests from clients?

### AWS Container Services and Serverless
- **Serverless Container Service**: Which AWS container service can a customer use to run containers without having to manage servers?
- **Docker Container Image Management**: Which AWS service should a customer use if they must store, manage, and deploy Docker container images?
- **Work Performer in AWS Step Functions**: What performs the work in a workflow when AWS Step Functions is running?
- **Serverless Application Building Service**: Which service can a customer use to build and run applications without provisioning or managing servers?

### Web Services and Database Management
- **REST Resource Creation Method**: Which REST request method creates a resource?
- **Relational Database Service**: Which fully managed Amazon Web Services (AWS) relational database service is compatible with MySQL and PostgreSQL?
- **Data Migration and Transformation**: A customer has decided to migrate from a MySQL database that runs in their data center to Amazon RDS for MySQL. Their database must remain fully operational during the migration. In addition, the customer would like to automate data transformation when the data is migrated to AWS. Which AWS service or feature should the customer use?
- **Managed Data Warehouse Service**: Which AWS service is a fully managed data warehouse that a customer can use to run complex analytic queries?
- **Managed Database Service User Responsibility**: Which task is a database user responsible for when they use a managed database service on AWS?
- **NoSQL Support in AWS Database Services**: Which AWS database services support NoSQL applications?
