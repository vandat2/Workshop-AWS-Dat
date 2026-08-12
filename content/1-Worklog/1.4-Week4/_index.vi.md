---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu tuần 4:

- Hoàn thiện trải nghiệm sử dụng của chatbot và chuẩn bị các bước cần thiết cho quá trình đưa ứng dụng lên môi trường cloud.
- Khảo sát Docker và các thành phần hạ tầng AWS liên quan đến việc triển khai, kết nối mạng và phân phối request.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                             | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                                                                        |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2    | - Kiểm tra các thao tác chính từ lúc nhập câu hỏi đến khi nhận kết quả.<br />- Chỉnh sửa các lỗi giao diện ban đầu.                                                               | 13/07/2026       | 13/07/2026         |                                                                                                                                                                                                          |
| 3    | - Tìm hiểu triển khai ứng dụng Python/FastAPI/Chainlit bằng Docker.<br />- Tìm hiểu Amazon EC2 và mô hình chạy container trên EC2.                                                       | 14/07/2026       | 14/07/2026         | [aws.amazon.com/vi/ec2](https://aws.amazon.com/vi/ec2/)                                                                                                                                                   |
| 4    | - Điều chỉnh phương án kiến trúc cloud dựa trên các thành phần đã khảo sát.<br />- Tìm hiểu cơ chế của Application Load Balancer trong việc tiếp nhận và phân phối request. | 15/07/2026       | 15/07/2026         | [aws.amazon.com/vi/elasticloadbalancing/application-load-balancer](https://aws.amazon.com/vi/elasticloadbalancing/application-load-balancer/)<br />[aws.amazon.com/vi/vpc](https://aws.amazon.com/vi/vpc/) |
| 5    | - Tìm hiểu VPC Endpoint cho Bedrock, DynamoDB và S3.<br />- Bổ sung tài liệu mô tả các luồng chính của hệ thống.<br />- Tiếp tục chỉnh sửa code retrieval và vector store.        | 16/07/2026       | 16/07/2026         | [aws.amazon.com/vi/vpc](https://aws.amazon.com/vi/vpc/)<br />[aws.amazon.com/vi/dynamodb](https://aws.amazon.com/vi/dynamodb/)                                                                             |
| 6    | - Review tiến độ nhóm và thống nhất kiến trúc cloud cho dự án Law-Chatbot.                                                                                                                  | 17/07/2026       | 17/07/2026         |                                                                                                                                                                                                          |

### Kết quả đạt được tuần 4:

- Hiểu thêm về việc sử dụng Docker để chuẩn bị ứng dụng cho môi trường triển khai trên EC2.
- Xác định được các thành phần mạng chính cần dùng khi triển khai cloud.
- Cùng nhóm review sơ đồ kiến trúc AWS và điều chỉnh các luồng S3, Lambda, RDS, Bedrock, EC2.
