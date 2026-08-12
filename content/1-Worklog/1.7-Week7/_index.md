---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---
### Week 7 Objectives:

* Integrate Streamlit interface, FastAPI backend, and admin APIs.
* Add authentication, authorization, document upload, and foundational infrastructure using AWS services.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                                                                 | Start Date | Completion Date | Reference Material |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | ------------------ |
| 2   | - Integrate Streamlit interface with core RAG.<br />- Edit UI, database, and Q&A flow.<br />- Test chatbot operation on Streamlit interface.                                                                         | 03/08/2026 | 03/08/2026      |                    |
| 3   | - Add FastAPI backend for chat, conversation, and admin APIs.<br />- Learn and integrate Amazon Cognito for user authentication.<br />- Build Cognito JWT verification in FastAPI.                                   | 04/08/2026 | 04/08/2026      |                    |
| 4   | - Design RBAC authorization according to users, editors, and admins groups.<br />- Write Cognito admin service to manage users and groups.<br />- Test list, enable, disable user, and add user to group functions. | 05/08/2026 | 05/08/2026      |                    |
| 5   | - Build admin API to create presigned S3 uploads.<br />- Create S3 manifest containing metadata, document_id, actor, and object_key for ingestion.                                                                   | 06/08/2026 | 06/08/2026      |                    |
| 6   | - Write Lambda handler to receive S3 or SQS events for processing new documents.<br />- Add partial batch failure mechanism, retry, and DLQ for Lambda/SQS.                                                          | 07/08/2026 | 07/08/2026      |                    |

### Week 7 Achievements:

* Streamlit interface integrated with RAG core.
* FastAPI backend added APIs serving chat, conversation, and admin functionality.
* Added Cognito authentication and user group authorization.
* Coordinated with team members when integrating Streamlit UI, FastAPI backend, and RAG core.
* Reviewed APIs, Cognito authentication flow, and admin functions with the team.
* Verified CloudFormation templates and S3/SQS/Lambda ingestion flow with the team.
