---
title: "Week 2 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---
### Week 2 Objectives:

- Improve the data preparation process and enhance the stability of the index building step.
- Get familiar with PostgreSQL on Amazon RDS, pgvector, and the embedding service on Amazon Bedrock.
- Consolidate ideas, scope, and development direction into a project proposal.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | --- |
| 2   | - Review the legal data processing flow from input to index preparation.<br />- Optimize the reading of metadata and content parquet in small batches. | 29/06/2026 | 29/06/2026 | |
| 3   | - Review the steps in the index creation process and find ways to reduce processing time.<br />- Check and handle issues arising when building large datasets. | 30/06/2026 | 30/06/2026 | |
| 4   | - Connect the steps document → chunk → embedding → vector store into a complete index creation process.<br />- Perform a test build and verify output data after each stage. | 01/07/2026 | 01/07/2026 | |
| 5   | - Build an index building pipeline from document, chunk, embedding to vector store.<br />- Test run and verify index build results. | 02/07/2026 | 02/07/2026 | |
| 6   | - Learn about Amazon RDS PostgreSQL and the pgvector extension.<br />- Learn about Amazon Bedrock Embedding. | 03/07/2026 | 03/07/2026 | [aws.amazon.com/vi/rds](https://aws.amazon.com/vi/rds/)<br />[aws.amazon.com/vi/bedrock/getting-started](https://aws.amazon.com/vi/bedrock/getting-started/) |

### Week 2 Achievements:

- Improved the data processing and preparation process for the RAG system.
- Further completed the chunking, embedding, and index building steps.
- Understood how pgvector can be used to store and query vectors on PostgreSQL.
- Grasped the role of the embedding service on Amazon Bedrock in the cloud application architecture.
- Completed the proposal, thereby clarifying the project's ideas and implementation direction.