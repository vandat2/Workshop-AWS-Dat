---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---
### Mục tiêu tuần 7:

- Hoàn thiện lớp giao diện Streamlit và kết nối với backend FastAPI cùng các thành phần RAG hiện có.
- Xây dựng nền tảng quản lý tài khoản, phân quyền và quy trình tiếp nhận tài liệu thông qua các dịch vụ AWS.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                                                                                                                                    | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | ----------------- |
| 2    | - Rà soát giao diện, dữ liệu ứng dụng và quy trình gửi câu hỏi.<br />- Chạy thử chatbot trên giao diện mới và ghi nhận các điểm cần điều chỉnh.                                                                                      | 03/08/2026       | 03/08/2026         |                   |
| 3    | - Bổ sung FastAPI backend cho các API chat, conversation và admin.<br />- Tìm hiểu và tích hợp Amazon Cognito cho xác thực người dùng.<br />- Xây dựng Cognito<br />verification trong FastAPI.                                              | 04/08/2026       | 04/08/2026         |                   |
| 4    | - Thiết kế phân quyền RBAC theo nhóm users, editors và admins.<br />- Viết Cognito admin service để quản lý user và group.<br />- Kiểm tra các thao tác quản lý như lấy danh sách, kích hoạt, vô hiệu hóa và gán user vào group. | 05/08/2026       | 05/08/2026         |                   |
| 5    | - Xây dựng API admin tạo presigned S3 upload.<br />- Tạo S3 manifest chứa metadata, document_id, actor và object_key cho ingestion.                                                                                                                    | 06/08/2026       | 06/08/2026         |                   |
| 6    | - Xây dựng Lambda handler để tiếp nhận sự kiện tài liệu mới từ S3 hoặc SQS.<br />- Bổ sung cơ chế partial batch failure, retry và DLQ cho Lambda/SQS.                                                                                        | 07/08/2026       | 07/08/2026         |                   |

### Kết quả đạt được tuần 7:

- Hoàn thành bước kết nối giữa Streamlit, backend và core RAG để tạo thành luồng ứng dụng thống nhất.
- FastAPI backend có thêm các API phục vụ chat, conversation và admin
- Thiết lập được cơ chế xác thực và mô hình phân quyền người dùng thông qua Cognito.
- Phối hợp với thành viên nhóm khi tích hợp Streamlit UI, FastAPI backend và core RAG.
