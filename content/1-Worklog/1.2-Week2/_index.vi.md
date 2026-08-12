---
title: "Worklog Tuần 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---
### Mục tiêu tuần 2:

- Cải thiện quy trình chuẩn bị dữ liệu và nâng cao độ ổn định của bước tạo index.
- Làm quen với PostgreSQL trên Amazon RDS, pgvector và dịch vụ embedding trên Amazon Bedrock.
- Tổng hợp ý tưởng, phạm vi và hướng phát triển thành proposal cho dự án.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                                                                                                          |
| ---- | --------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 2    | - Rà soát lại luồng xử lý dữ liệu pháp luật từ đầu vào đến bước chuẩn bị index.<br />- Tối ưu cách đọc metadata và content parquet theo lô nhỏ.     | 29/06/2026       | 29/06/2026         |                                                                                                                                                            |
| 3    | - Kiểm tra các bước trong quá trình tạo index và tìm cách giảm thời gian xử lý.<br />- Kiểm tra và xử lý các vấn đề phát sinh khi build dữ liệu lớn.                        | 30/06/2026       | 30/06/2026         |                                                                                                                                                            |
| 4    | - Kết nối các bước document → chunk → embedding → vector store thành một quy trình tạo index hoàn chỉnh.<br />- Thực hiện build thử và kiểm tra dữ liệu đầu ra sau từng giai đoạn.            | 01/07/2026       | 01/07/2026         |                                                                                                                                                            |
| 5    | - Xây dựng pipeline build index từ document, chunk, embedding đến vector store.<br />- Chạy thử và kiểm tra kết quả build index. | 02/07/2026       | 02/07/2026         |                                                                                                                                                            |
| 6    | - Tìm hiểu Amazon RDS PostgreSQL và extension pgvector.<br />- Tìm hiểu Amazon Bedrock Embedding.                                | 03/07/2026       | 03/07/2026         | [aws.amazon.com/vi/rds](https://aws.amazon.com/vi/rds/)<br />[aws.amazon.com/vi/bedrock/getting-started](https://aws.amazon.com/vi/bedrock/getting-started/) |

### Kết quả đạt được tuần 2:

- Cải thiện quy trình xử lý và chuẩn bị dữ liệu cho hệ thống RAG.
- Hoàn thiện hơn các bước chunking, embedding và xây dựng index.
- Hiểu được cách pgvector có thể được sử dụng để lưu trữ và truy vấn vector trên PostgreSQL.
- Nắm được vai trò của dịch vụ embedding trên Amazon Bedrock trong kiến trúc ứng dụng cloud.
- Hoàn thành proposal, qua đó xác định rõ hơn ý tưởng và hướng triển khai của dự án.
