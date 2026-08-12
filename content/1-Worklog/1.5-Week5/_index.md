---
title: "Week 5 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.5. </b> "
---
### Week 5 Objectives:

- Migrate the vector storage system from local development environment to PostgreSQL using pgvector on Amazon RDS.
- Explore methods to accelerate vector queries and begin building performance metrics for processing time of each component.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                                                                                       | Start Date | Completion Date | Reference Material                                     |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ------------------------------------------------------ |
| 2   | - Establish connection between the application and PostgreSQL on Amazon RDS.<br />- Configure environment variables for RDS connection.<br />- Test PostgreSQL connection from the application.                                                                            | 20/07/2026 | 20/07/2026      |                                                        |
| 3   | - Adjust the vector management layer to support multiple storage options: FAISS/SQLite for local and pgvector for cloud environment.<br />- Create legal_chunks table and embedding column in PostgreSQL.<br />- Test chunk and embedding insertion process into database. | 21/07/2026 | 21/07/2026      |                                                        |
| 4   | - Explore how to perform cosine similarity search using pgvector.<br />- Optimize RDS queries.<br />- Add timeout for PostgreSQL queries.                                                                                                                                  | 22/07/2026 | 22/07/2026      | [aws.amazon.com/vi/rds](https://aws.amazon.com/vi/rds/) |
| 5   | - Learn and experiment with HNSW/IVFFlat index for pgvector.<br />- Write create_hnsw_index.py and create_ivfflat_index.py scripts.<br />- Add benchmarking and latency measurement for retrieval, embedding, DB search, and LLM.                                          | 23/07/2026 | 23/07/2026      |                                                        |
| 6   | - Re-test Q&A pipeline after connecting RDS pgvector.                                                                                                                                                                                                                      | 24/07/2026 | 24/07/2026      |                                                        |

### Week 5 Achievements:

- Successfully connected the system to PostgreSQL pgvector on Amazon RDS.
- RDS configuration integrated into system via environment variables.
- Explored vector search optimization methods with pgvector.
