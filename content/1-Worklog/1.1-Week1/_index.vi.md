---
title: "Worklog Tuần 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.1. </b> "
---
### Mục tiêu tuần 1:

- Nắm bắt cách thức làm việc tại FCJ và làm quen với định hướng của dự án Law-Chatbot.
- Thiết lập môi trường lập trình, tìm hiểu kiến trúc RAG và chuẩn bị các thành phần cốt lõi cho hệ thống tra cứu pháp luật.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                 | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                    |
| ---- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | ---------------------------------------------------- |
| 2    | - Làm quen với các thành viên trong nhóm và quy trình làm việc.<br />- Trao đổi để xác định mục tiêu, phạm vi và yêu cầu ban đầu của dự án Law-Chatbot.                                                                         | 22/06/2026       | 22/06/2026         |                                                      |
| 3    | - Khảo sát mô hình hạ tầng AWS<br />- Tìm hiểu nguyên lý hoạt động của RAG.<br />- Chuẩn bị Python, VSCode, Git cùng các dependency phục vụ quá trình phát triển.                                                                   | 23/06/2026       | 23/06/2026         |                                                      |
| 4    | - Thiết kế cấu trúc thư mục và các thành phần ban đầu của source code.<br />- Phân tích luồng xử lý RAG trong bài toán hỏi đáp và tra cứu văn bản pháp luật.                                                                   | 24/06/2026       | 24/06/2026         |                                                      |
| 5    | - Hoàn thiện thêm cấu trúc mã nguồn.<br />- Phát triển dataset_reader.py phục vụ việc nạp dữ liệu pháp luật vào pipeline.                                                                                                                 | 25/06/2026       | 25/06/2026         |                                                      |
| 6    | - Xây dựng module chunking.py để tách văn bản pháp luật thành các đoạn nhỏ.<br />- Xây dựng embeddings.py để chuyển nội dung thành vector biểu diễn.<br />- Xây dựng module vector_store.py để lưu trữ và truy vấn vector. | 26/06/2026       | 26/06/2026         | [aws.amazon.com/vi/s3](https://aws.amazon.com/vi/s3/) |

### Kết quả đạt được tuần 1:

- Bước đầu thích nghi với môi trường thực tập, cách phối hợp và các quy định làm việc tại FCJ.
- Hiểu được mục tiêu và phạm vi chính của đồ án Law-Chatbot.
- Hoàn thiện môi trường phát triển và nền móng source code cho dự án.
- Có kiến thức ban đầu về AWS và quy trình RAG phục vụ bài toán tra cứu pháp luật.
- Hoàn thành các thành phần cơ bản gồm đọc cấu hình, nạp dữ liệu, chia nhỏ văn bản, tạo embedding và quản lý vector.
