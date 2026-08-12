---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---
### Week 6 Objectives:

- Bring all chatbot components into a unified process to test operational capability.
- Learn about logging, monitoring, alerting, and storing conversation history using AWS services.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | --- |
| 2   | - Complete the legal Q&A chatbot with end-to-end RAG flow.<br />- Test Q&A functionality after data has been loaded into vector store.<br />- Debug retrieval and embedding dimension errors. | 27/07/2026 | 27/07/2026 | |
| 3   | - Re-check the connection and query execution process on RDS PostgreSQL.<br />- Optimize answer quality by adjusting top_k, prompt template, and chunk size.<br />- Re-check retrieval and LLM timeouts. | 28/07/2026 | 28/07/2026 | |
| 4   | - Learn Amazon CloudWatch to monitor logs and application performance.<br />- Learn Amazon SNS to send alerts when system errors occur.<br />- Design CloudWatch Alarm and SNS notification flow. | 29/07/2026 | 29/07/2026 | [aws.amazon.com/vi/cloudwatch](https://aws.amazon.com/vi/cloudwatch/)<br />[aws.amazon.com/vi/sns](https://aws.amazon.com/vi/sns/) |
| 5   | - Determine how to organize conversation history data by conversation and message.<br />- Explore indexes for user-based and time-based queries along with TTL mechanism. | 30/07/2026 | 30/07/2026 | [aws.amazon.com/vi/dynamodb](https://aws.amazon.com/vi/dynamodb/) |
| 6   | - Conduct additional test scenarios for the chatbot interface.<br />- Compile errors detected during usage and adjust remaining unstable parts. | 31/07/2026 | 31/07/2026 | |

### Week 6 Achievements:

- Completed end-to-end testing of the chatbot and identified several issues requiring further attention.
- Improved system stability after checking database, retrieval, embedding, and response generation parameters.
- Established an initial approach for monitoring and alerting through CloudWatch and SNS.
- Developed a preliminary plan for organizing chat history data and storage duration.