---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---
### Week 7 Objectives:

- Complete the Streamlit interface layer and connect it with FastAPI backend along with existing RAG components.
- Build a foundation for account management, authorization, and document ingestion workflow using AWS services.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | --- |
| 2   | - Review the interface, application data, and question submission flow.<br />- Test the chatbot on the new interface and record points needing adjustment. | 03/08/2026 | 03/08/2026 | |
| 3   | - Add FastAPI backend for chat, conversation, and admin APIs.<br />- Learn and integrate Amazon Cognito for user authentication.<br />- Build Cognito verification in FastAPI. | 04/08/2026 | 04/08/2026 | |
| 4   | - Design RBAC authorization according to users, editors, and admins groups.<br />- Write Cognito admin service to manage users and groups.<br />- Test management operations such as listing, enabling, disabling, and assigning users to groups. | 05/08/2026 | 05/08/2026 | |
| 5   | - Build admin API to create presigned S3 upload URLs.<br />- Create S3 manifest containing metadata, document_id, actor, and object_key for ingestion. | 06/08/2026 | 06/08/2026 | |
| 6   | - Build Lambda handler to receive new document events from S3 or SQS.<br />- Add partial batch failure mechanism, retry, and DLQ for Lambda/SQS. | 07/08/2026 | 07/08/2026 | |

### Week 7 Achievements:

- Completed the connection between Streamlit, backend, and core RAG to create a unified application flow.
- FastAPI backend added APIs serving chat, conversation, and admin functionality.
- Established authentication mechanism and user authorization model through Cognito.
- Collaborated with team members when integrating Streamlit UI, FastAPI backend, and core RAG.