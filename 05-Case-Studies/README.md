# 05 - Case Studies

This folder contains real-world Azure Cosmos DB design scenarios and case studies.

The purpose of this section is to understand how Cosmos DB concepts are applied in practical backend and cloud-native application design.

## Purpose

DP-420 is not only about knowing Cosmos DB features.

Many important questions are scenario-based.  
That means I need to understand how to choose the right design based on requirements such as:

- Scalability
- Latency
- Cost
- Availability
- Consistency
- Data access patterns
- Partition key strategy
- Query performance
- Multi-region design
- Event-driven processing

## Planned Case Studies

| No | Case Study | Main Focus |
|---|---|---|
| 01 | E-Commerce Order System | Partition key, order data model, query patterns |
| 02 | Multi-Tenant SaaS Application | Tenant-based partitioning and isolation |
| 03 | IoT Telemetry Platform | High write volume, time-series data, TTL |
| 04 | Product Catalog Search | Indexing, query optimization, integration |
| 05 | User Activity Tracking | Write-heavy workloads and analytical patterns |
| 06 | Event-Driven Order Processing | Change Feed and Azure Functions |
| 07 | Global Application Design | Multi-region replication and consistency |
| 08 | Financial Transaction History | Consistency, audit, and data retention |
| 09 | Gaming Leaderboard | Low latency reads and partition design |
| 10 | Notification System | Event processing and scalable reads |

## Case Study Format

Each case study will follow this structure:

```md
# Case Study Name

## Business Scenario

## Requirements

## Data Access Patterns

## Data Model

## Partition Key Choice

## Indexing Strategy

## Consistency Choice

## Performance and RU Considerations

## Possible Problems

## Final Architecture Decision

## Exam Notes
