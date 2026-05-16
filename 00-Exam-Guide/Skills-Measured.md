# DP-420 Skills Measured

This file contains my high-level roadmap for the DP-420: Azure Cosmos DB Developer Specialty exam.

The goal of this file is to understand what the exam measures and how each skill area connects to real backend development.

---

## Main Exam Focus Areas

DP-420 focuses on designing and implementing cloud-native applications using Microsoft Azure Cosmos DB.

The main areas I need to understand are:

- Data modeling and partitioning
- Designing and implementing data distribution
- Integrating Azure Cosmos DB with Azure services
- Optimizing Azure Cosmos DB solutions
- Maintaining Azure Cosmos DB solutions
- Working with the Azure Cosmos DB for NoSQL SDK
- Querying data efficiently
- Creating indexing policies
- Monitoring and troubleshooting
- Security, backup, restore, and DevOps practices

---

## My Study Strategy

I will study each topic in this order:

1. Understand the concept
2. Read the official Microsoft Learn module
3. Write my own notes
4. Build a small lab if needed
5. Write exam-focused reminders
6. Add confusing parts to the Knowledge Check section
7. Create cheat sheet notes for final review

---

## Important Topics to Master

| Topic | Why It Matters |
|---|---|
| Partition Key | Core of scalability and data distribution |
| Request Units | Main performance and cost model |
| Indexing | Affects query performance and RU usage |
| Data Modeling | NoSQL modeling is different from relational design |
| Consistency Models | Important for distributed system behavior |
| Replication | Needed for global availability and failover |
| Change Feed | Used for event-driven processing |
| SDK Usage | Required for backend implementation |
| Monitoring | Required for troubleshooting and production readiness |
| Security | Important for access control and real-world systems |

---

## Personal Focus Areas

These are the areas I want to understand especially deeply:

- How to choose a good partition key
- How logical and physical partitions work
- How RU consumption is calculated
- How query design affects cost
- When to use embedded data vs referenced data
- How indexing policies change query behavior
- How ETag protects against lost updates
- How Change Feed supports event-driven architecture
- How Cosmos DB integrates with Azure Functions
- How to monitor slow or expensive queries

---

## Final Mental Model

DP-420 is not only about knowing Cosmos DB features.

The exam expects me to understand how to design a Cosmos DB solution based on:

- Access patterns
- Scale requirements
- Latency requirements
- Cost constraints
- Availability needs
- Consistency requirements
- Operational requirements

The key mindset:

> In Cosmos DB, good design starts with how the application reads and writes data at scale.
