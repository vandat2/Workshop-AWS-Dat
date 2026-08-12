---
title: "Week 3 Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
### Week 3 Objectives:

- Complete the question processing flow from when a user submits a request to when the chatbot generates a response based on legal data.
- Connect RAG components with the chat interface and initially determine the system deployment model on AWS.

### Tasks to be carried out this week:

| Day | Task                                                                                                                                                                       | Start Date | Completion Date | Reference Material                                                                                                                                                                                       |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2   | - Build the retrieval component for the Q&A system.<br />- Complete module retriever.py to retrieve relevant chunks.                                                       | 06/07/2026 | 06/07/2026      |                                                                                                                                                                                                          |
| 3   | - Develop prompt phrasing suitable for Vietnamese legal consulting and retrieval tasks.<br />- Design appropriate prompts for the Vietnamese legal chatbot.                | 07/07/2026 | 07/07/2026      |                                                                                                                                                                                                          |
| 4   | - Complete module generator.py to generate responses from LLM.<br />- Add the option to choose between Gemini or Amazon Bedrock providers.                                 | 08/07/2026 | 08/07/2026      |                                                                                                                                                                                                          |
| 5   | - Complete module qa_service.py to connect retriever, prompt, and generator.<br />- Build an experimental chatbot using Chainlit.<br />- Integrate Chainlit with RAG core. | 09/07/2026 | 09/07/2026      |                                                                                                                                                                                                          |
| 6   | - Learn about application architecture running on Amazon EC2.<br />- Design an initial AWS architecture diagram with ALB, EC2, RDS pgvector, and Bedrock.                  | 10/07/2026 | 10/07/2026      | [aws.amazon.com/vi/elasticloadbalancing/application-load-balancer](https://aws.amazon.com/vi/elasticloadbalancing/application-load-balancer/)<br />[aws.amazon.com/vi/ec2](https://aws.amazon.com/vi/ec2/) |

### Week 3 Achievements:

- Built a relatively complete RAG Q&A process, including data retrieval, prompt construction, and response generation.
- The chatbot can receive questions and generate responses based on retrieved legal content.
- Completed an experimental chat interface version using Chainlit and connected it with the RAG core.
- Initially developed an AWS architecture plan for the application, including application processing components, vector database, and AI services.
