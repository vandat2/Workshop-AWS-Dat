---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu tuần 6:

- Đưa toàn bộ các thành phần của chatbot vào cùng một quy trình để kiểm tra khả năng vận hành
- Tìm hiểu logging, monitoring, alerting và lưu lịch sử hội thoại bằng các dịch vụ AWS

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                |
| ---- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | -------------------------------------------------------------------------------------------------------------------------------- |
| 2    | - Hoàn thiện chatbot hỏi đáp pháp luật với luồng RAG end-to-end.<br />- Kiểm thử chức năng hỏi đáp sau khi dữ liệu đã được nạp vào vector store.<br />- Debug lỗi retrieval và embedding dimension.                          | 27/07/2026       | 27/07/2026         |                                                                                                                                  |
| 3    | - Kiểm tra lại quá trình kết nối và thực thi truy vấn trên RDS PostgreSQL.<br />- Tối ưu chất lượng câu trả lời bằng cách điều chỉnh top_k, prompt template và chunk size.<br />- Kiểm tra lại timeout của retrieval và LLM. | 28/07/2026       | 28/07/2026         |                                                                                                                                  |
| 4    | - Tìm hiểu Amazon CloudWatch để theo dõi log và hiệu năng ứng dụng.<br />- Tìm hiểu Amazon SNS để gửi cảnh báo khi hệ thống phát sinh lỗi.<br />- Thiết kế luồng CloudWatch Alarm và SNS notification.                         | 29/07/2026       | 29/07/2026         | [aws.amazon.com/vi/cloudwatch](https://aws.amazon.com/vi/cloudwatch/)<br />[aws.amazon.com/vi/sns](https://aws.amazon.com/vi/sns/) |
| 5    | - Xác định cách tổ chức dữ liệu lịch sử trò chuyện theo conversation và message.<br />- Khảo sát các index phục vụ truy vấn theo user và thời gian cùng cơ chế TTL.                                                                | 30/07/2026       | 30/07/2026         | [aws.amazon.com/vi/dynamodb](https://aws.amazon.com/vi/dynamodb/)                                                                 |
| 6    | - Thực hiện thêm các kịch bản kiểm thử cho giao diện chatbot.<br />- Tổng hợp lỗi phát hiện trong quá trình sử dụng và điều chỉnh các phần còn chưa ổn định.                                                                  | 31/07/2026       | 31/07/2026         |                                                                                                                                  |

### Kết quả đạt được tuần 6:

- Hoàn thành việc kiểm tra chatbot theo quy trình end-to-end và xác định được một số vấn đề cần tiếp tục xử lý.
- Cải thiện độ ổn định của hệ thống sau khi kiểm tra database, retrieval, embedding và các tham số sinh câu trả lời.
- Xây dựng được hướng tiếp cận ban đầu cho việc giám sát và cảnh báo thông qua CloudWatch và SNS.
- Có phương án sơ bộ cho việc tổ chức dữ liệu chat history và thời gian lưu trữ.
