
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

