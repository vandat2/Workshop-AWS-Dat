---
title: "Worklog Tuần 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.3. </b> "
---
### Mục tiêu tuần 3:

- Hoàn thiện quy trình xử lý câu hỏi từ lúc người dùng gửi yêu cầu đến khi chatbot tạo câu trả lời dựa trên dữ liệu pháp luật.
- Kết nối các thành phần RAG với giao diện chat và bước đầu xác định mô hình triển khai hệ thống trên AWS.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                              | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                                                  |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2    | - Xây dựng phần truy xuất cho hệ thống hỏi đáp.<br />- Hoàn thiện module retriever.py để truy xuất chunk liên quan.                                                                      | 06/07/2026       | 06/07/2026         |                                                                                                                                                                                                    |
| 3    | - Xây dựng cách diễn đạt prompt phù hợp với bài toán tư vấn, tra cứu pháp luật Việt Nam.<br />- Thiết kế prompt phù hợp cho chatbot pháp luật Việt Nam.                         | 07/07/2026       | 07/07/2026         |                                                                                                                                                                                                    |
| 4    | - Hoàn thiện module generator.py để sinh câu trả lời từ LLM.<br />- Bổ sung khả năng chọn provider Gemini hoặc Amazon Bedrock.                                                            | 08/07/2026       | 08/07/2026         |                                                                                                                                                                                                    |
| 5    | - Hoàn thiện module qa_service.py để kết nối retriever, prompt và generator.<br />- Xây dựng chatbot hội thoại thử nghiệm bằng Chainlit trong.<br />- Tích hợp Chainlit với RAG core. | 09/07/2026       | 09/07/2026         |                                                                                                                                                                                                    |
| 6    | - Tìm hiểu kiến trúc ứng dụng chạy trên Amazon EC2.<br />- Thiết kế sơ đồ kiến trúc AWS ban đầu với ALB, EC2, RDS pgvector và Bedrock.                                              | 10/07/2026       | 10/07/2026         | [aws.amazon.com/vi/elasticloadbalancing/application-load-balancer](https://aws.amazon.com/vi/elasticloadbalancing/application-load-balancer/)[aws.amazon.com/vi/ec2](https://aws.amazon.com/vi/ec2/) |

### Kết quả đạt được tuần 3:

- Xây dựng được quy trình hỏi đáp RAG tương đối hoàn chỉnh, bao gồm truy xuất dữ liệu, xây dựng prompt và sinh câu trả lời.
- Chatbot có thể tiếp nhận câu hỏi và tạo phản hồi dựa trên các nội dung pháp luật được truy xuất.
- Hoàn thiện phiên bản giao diện chat thử nghiệm bằng Chainlit và kết nối với phần lõi RAG.
- Bước đầu xây dựng phương án kiến trúc AWS cho ứng dụng, gồm các thành phần xử lý ứng dụng, cơ sở dữ liệu vector và dịch vụ AI.
