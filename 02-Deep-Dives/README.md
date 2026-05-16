# 02 - Deep Dives

This folder contains deep technical explanations of important Azure Cosmos DB concepts.

The purpose of this section is to go beyond exam-level memorization and understand how Cosmos DB works from a real backend engineering perspective.

## Purpose

Some Cosmos DB topics are very important for both the DP-420 exam and real-world system design.

This section focuses on:

- Why a concept exists
- How it works internally
- Where it is used in real projects
- What problems it solves
- What mistakes developers commonly make
- How it affects performance, scalability, and cost

## Planned Deep Dive Topics

| No | Topic | Why it matters |
|---|---|---|
| 01 | Partition Key Deep Dive | Core of scalability, data distribution, and performance |
| 02 | Request Units RU/s | Main cost and performance model in Cosmos DB |
| 03 | Indexing Strategy | Directly affects query performance and RU consumption |
| 04 | Consistency Models | Important for distributed systems and correctness |
| 05 | ETag and Optimistic Concurrency | Prevents lost updates in concurrent systems |
| 06 | Change Feed | Useful for event-driven architecture and background processing |
| 07 | Data Modeling for NoSQL | Different from relational database modeling |
| 08 | Multi-region Replication | High availability and global distribution |
| 09 | Backup and Restore | Important for operational safety |
| 10 | Security and RBAC | Production-level access control and data protection |
| 11 | Monitoring and Troubleshooting | Required for production readiness |
| 12 | SDK Performance Best Practices | Important for real backend applications |

## Note Format

Each deep dive topic will follow this structure:

```md
# Topic Name

## Problem

## Why this concept exists

## Core idea

## How it works

## Real backend example

## Exam focus

## Common mistakes

## Final mental model
