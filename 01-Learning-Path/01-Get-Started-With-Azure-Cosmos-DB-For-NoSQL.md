
## Introduction to Azure Cosmos DB for NoSQL

### Introduction

Today’s applications need to work with real-time data, different data formats, high traffic, and changing business requirements.

Modern applications should be:

- resilient
- flexible
- scalable
- able to process real-time data
- ready for modern AI capabilities

Applications often receive data from many different sources. This data can have different shapes, different volumes, and different speeds. Because of this, developers need platforms that can adapt quickly when the business changes.

A flexible database platform helps developers build new features faster and handle changes in data volume, velocity, and structure.

### Scenario

Imagine that you are the lead developer at a retail company.

Your team is building a new online storefront. The application will use AI agents to help customers during their shopping experience. The storefront must work across different devices, including mobile devices.

When the storefront is published, the company expects a large traffic spike because of launch campaigns and sales.

As the lead developer, you need to choose a database platform.

The database should be able to handle:

- large amounts of data
- different types of data
- high-volume workloads
- high-velocity workloads
- sudden traffic growth
- fast scaling with little friction
- AI search scenarios with vectorized data

### Azure Cosmos DB

Azure Cosmos DB is a fast NoSQL database service for modern application development and AI application development at any scale.

In this module, the main goal is to understand how Azure Cosmos DB for NoSQL can solve this type of business problem.

After this section, I should be able to:

- evaluate whether Azure Cosmos DB for NoSQL is the right database for an application
- describe why Azure Cosmos DB for NoSQL is useful for modern applications

## What is Azure Cosmos DB for NoSQL
. Let's start with a few definitions and a quick tour through Azure Cosmos DB for NoSQL. This overview should help you see whether Azure Cosmos DB might be a good fit for your work.

### What is a NoSQL database?

Developers require new kinds of databases that can address the unique challenges of modern apps. NoSQL databases were designed to address needs such as:

- High volumes of data.
- Data with many different sources and forms.
- Dynamic data schemas that store different types of data.
- Using high-velocity and/or real-time data.

You define NoSQL databases by the common characteristics they share rather than by a specific formal definition. These characteristics include:

- A nonrelational data store.
- Being designed to scale out.
- Not enforcing a specific schema.

Generally, NoSQL databases don't enforce relational constraints or put locks on data, making writes fast. Also, they're often designed to horizontally scale via sharding or partitioning, which allows them to maintain high-performance regardless of size.

While there are many NoSQL data models, four broad data model families are commonly used when modeling data in a NoSQL database:

![NoSQL data models](../assets/images/2-nosql-db.png)

Moving forward, we focus on the data model supported by Azure Cosmos DB for NoSQL: The document data model.

### Why use a NoSQL database with the document data model?

The document data model breaks data down into individual document entities. A document can be any structured data type, but JSON is commonly used as the data format. The Azure Cosmos DB for NoSQL supports JSON natively. 

![Document data model](../assets/images/2-document-db.png )

A document is an atomic entity and can have its own data form, regardless of what is stored in other documents in the same database. Because of this flexibility, there's no need for a predefined schema making it easier to build new applications rapidly. Additionally, this flexibility enables scenarios where different types of data can be stored together and where models can evolve over the lifetime of an application.

### What is a JSON document?

JavaScript Object Notation, or JSON, is a lightweight data format. JSON was built to be highly compatible with the literal notation of an object in the JavaScript language. Many frameworks, browsers, and even databases support JavaScript natively making JSON a popular format for transmitting and storing data.

Here's an example of a JSON document:

```json
{
  "device": {
    "type": "mobile"
  },
  "sentTime": "2019-11-12T13:08:42",
  "spoolRefs": [
    "6a86682c-be5a-4a4a-bacd-96c4d1c7ece6",
    "79e78fe2-93aa-4688-89db-a7278b034aa6"
  ]
}
```
As you can see, JSON is a relatively readable data format that clearly exposes its content. JSON is also relatively easy to parse and use in JavaScript applications.

### What is Azure Cosmos DB for NoSQL?
Azure Cosmos DB for NoSQL is a fast NoSQL and vector database service that offers rich querying over diverse data and supports a new generation of Generative AI applications. It helps deliver configurable and reliable performance, is globally distributed, and enables rapid development.


![Document data model](../assets/images/2-azure-cosmos-db.png)

The NoSQL API is the core or native API for working with documents. The NoSQL API supports fast, flexible development utilizing JSON documents, a query language with a familiar syntax, and client libraries for popular programming languages. Azure Cosmos DB also provides unique capabilities such as vector indexing and search, allowing users to create a new breed of Generative AI applications over users' data that can rapidly scale efficiently.

Azure Cosmos DB for NoSQL has a few advantages such as:

- Industry Leading Vector Database with vector indexing and search designed to handle high-dimensional vectors, enabling efficient and accurate vector search at any scale.
- Guaranteed speed at any scale even through bursts—with instant, limitless elasticity, fast reads, and multi-master writes, anywhere in the world.
- Fast, flexible app development with SDKs for popular languages and frameworks such as .NET, Java, Python, JavaScript and GO, as well as no-ETL (extract, transform, load) analytics.
- Ready for mission-critical applications with guaranteed business continuity, 99.999-percent availability, and enterprise-grade security.
- Fully managed and cost-effective with a fully featured serverless offering as well as instant, automatic and dynamic scaling that responds to application needs.

These capabilities make Azure Cosmos DB ideally suited for modern application development. Azure Cosmos DB for NoSQL is especially suited for applications that:

- Experience unpredictable spikes and dips in traffic
- Generate lots of data
- Need to deliver real-time user experiences
- Are depended upon for business continuity

The Azure Cosmos DB for NoSQL can store native JSON documents with flexible schema. Data is indexed automatically and is available for query using a flavor of the SQL query language designed for JSON data. The NoSQL API can be accessed using SDKs for popular frameworks such as .NET, Python, Java, Node.js and GO.

### How does Azure Cosmos DB for NoSQL work
Now that we know the basics of Azure Cosmos DB, let's see what resources and information are required to start working with an account. This information should help you decide whether Azure Cosmos DB for NoSQL works for your data set. Also, it should help you decide how much, if any, extra configuration is necessary.

### What are the components of Azure Cosmos DB for NoSQL?
 To begin using Azure Cosmos DB, you first create various resources in Azure such as accounts, databases, containers, and items.

![Azure Cosmos DB components](../assets/images/3-resource-hierarchy.png)

### Accounts
Accounts are the fundamental units of high availability and tenant isolation for SaaS applications. At the account level, you can configure the region[s] for your data in Azure Cosmos DB for NoSQL. Accounts also contain the globally unique DNS name used for API requests. You can also set the default consistency level for requests at the account level. You can manage or create accounts using the Azure portal, Azure Resource Manager templates, the Azure CLI, or Azure PowerShell.

### Databases 
Each account can contain one or more Databases. A database is a logical unit of management for containers in Azure Cosmos DB for NoSQL.

### Containers
Containers are the fundamental unit of scalability in Azure Cosmos DB for NoSQL. With Azure Cosmos DB, you provision throughput at the container level. You can also optionally configure an indexing policy or a default time-to-live value at the container level. Azure Cosmos DB for NoSQL will automatically and transparently partition the data in a container. 
### Items 
The NoSQL API for Azure Cosmos DB stores individual documents in JSON format as items within the container. Azure Cosmos DB for NoSQL natively supports JSON files and can provide fast and predictable performance because write operations on JSON documents are atomic.

![Azure Cosmos DB components](../assets/images/3-item-hierarchy.png)
