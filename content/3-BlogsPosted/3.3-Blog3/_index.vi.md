---
title: "Blog 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---
# PDI Technologies cắt giảm 300 giờ báo cáo thủ công mỗi năm nhờ Amazon QuickSight

PDI Technologies là một tập đoàn công nghệ 40 năm tuổi, phục vụ hơn 200.000 khách hàng tại 60 quốc gia trong lĩnh vực bán lẻ tiện lợi và bán buôn xăng dầu đã áp dụng **Amazon QuickSight** để hiện đại hóa hạ tầng Business Intelligence (BI) giúp giảm hơn **300 giờ báo cáo thủ công mỗi năm**, đồng thời xây dựng nền tảng phân tích dữ liệu thống nhất cho toàn doanh nghiệp.

---

## Thách thức

Trong quá trình phát triển, PDI Technologies đã thực hiện hơn **30 thương vụ mua lại doanh nghiệp** (Mergers and Acquisitions). Điều này giúp công ty mở rộng nhanh chóng nhưng cũng khiến dữ liệu bị **phân tán trên nhiều hệ thống khác nhau**.

Mỗi phòng ban sử dụng một quy trình riêng để tổng hợp dữ liệu:

- Đội ngũ tài chính phải dành khoảng **24 giờ mỗi tháng** để tổng hợp dữ liệu từ hệ thống ERP, chuyển đổi sang định dạng phù hợp rồi mới có thể phân tích.
- Trong các giai đoạn chốt sổ cuối tháng, quy trình này phải lặp lại nhiều lần, dẫn đến tổng thời gian xử lý lên tới gần **300 giờ mỗi năm**.

Không chỉ mất thời gian, việc dữ liệu nằm rải rác ở nhiều nơi còn khiến mỗi bộ phận chỉ nhìn thấy một phần bức tranh tổng thể, gây khó khăn cho việc phối hợp và ra quyết định.

PDI cần một giải pháp có khả năng:

- Xử lý chuyển đổi dữ liệu quy mô lớn từ nhiều kho dữ liệu khác nhau.
- Cung cấp khả năng phân tích nhúng (embedded analytics) cho các giải pháp phần mềm của họ.
- Hỗ trợ triển khai BI trên toàn công ty.
- Cải thiện đáng kể hiệu quả báo cáo bằng cách giảm thiểu các quy trình thủ công.

---

## Vì sao PDI Technologies lựa chọn Amazon QuickSight?

Sau khi đánh giá nhiều giải pháp BI khác nhau, PDI Technologies lựa chọn **Amazon QuickSight** vì nền tảng này đáp ứng được ba yêu cầu quan trọng:

### 1. Khả năng nhúng (Embedded Analytics)

QuickSight cho phép nhúng các dashboard trực tiếp vào sản phẩm phần mềm của công ty. Điều này giúp **khách hàng có thể xem báo cáo và phân tích dữ liệu ngay trong ứng dụng đang sử dụng** mà không cần chuyển sang một công cụ khác.

### 2. Tích hợp sâu với hệ sinh thái AWS

QuickSight tích hợp tốt với hệ sinh thái AWS mà doanh nghiệp đang sử dụng, giúp kết nối trực tiếp với các dịch vụ lưu trữ và xử lý dữ liệu như:

- Amazon S3
- Amazon Redshift
- AWS Glue
- AWS Lambda

Nhờ vậy, kiến trúc dữ liệu được **đơn giản hóa** và giảm bớt sự phức tạp trong quá trình vận hành.

### 3. Khả năng mở rộng và hiệu năng vượt trội

Nền tảng này có khả năng mở rộng để phục vụ nhiều phòng ban cùng lúc, đồng thời xử lý hiệu quả khối lượng dữ liệu lớn thông qua công nghệ **SPICE** (Super-fast, Parallel, In-memory Calculation Engine), giúp tăng tốc quá trình phân tích và truy vấn dữ liệu.

---

## Kiến trúc kỹ thuật

Kiến trúc dữ liệu mới của PDI được thiết kế để giải quyết ba thách thức cốt lõi:

1. Hợp nhất dữ liệu từ hơn 30 công ty được mua lại.
2. Hỗ trợ phân tích thời gian thực ở quy mô lớn.
3. Phục vụ cả trường hợp sử dụng nội bộ lẫn hướng đến khách hàng.

### Luồng dữ liệu diễn ra như sau:

| Giai đoạn                                                          | Công nghệ sử dụng                                | Mô tả                                                                                                                                                                                                                                                                                                                            |
| :------------------------------------------------------------------- | :--------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Ingestion (Tiếp nhận)**                                    | AWS Glue, AWS Lambda, Amazon AppFlow                 | Dữ liệu từ các nguồn bên ngoài (tài liệu, file, và cơ sở dữ liệu) được đưa vào AWS. Mục tiêu là**hợp nhất dữ liệu từ hơn 30 công ty** đã mua lại vào một nền tảng duy nhất.                                                                                                            |
| **Storage (Lưu trữ Governed Data Lake)**                     | Amazon S3, AWS Glue Data Catalog, AWS Lake Formation | Dữ liệu sau khi tiếp nhận được lưu trữ trong**Amazon S3** làm data lake trung tâm. Các crawler của AWS Glue tự động phát hiện và lập danh mục lược đồ dữ liệu. AWS Lake Formation thực thi **kiểm soát truy cập chi tiết** và các chính sách quản trị trên toàn bộ data lake. |
| **Transformation & Quality (Chuyển đổi và Chất lượng)** | AWS Glue                                             | Dữ liệu thô trong S3 được xử lý qua các tác vụ chuyển đổi,**làm sạch, làm giàu, loại bỏ trùng lặp** và định hình lại dữ liệu thành các định dạng sẵn sàng cho phân tích.                                                                                                               |
| **Analytics (Phân tích)**                                    | Amazon Redshift                                      | Dữ liệu đã được chuyển đổi được tải vào**Amazon Redshift** để thực hiện phân tích SQL hiệu suất cao, tổng hợp và truy vấn phức tạp trên các tập dữ liệu lớn.                                                                                                                              |
| **Reporting (Báo cáo)**                                      | Amazon QuickSight                                    | **Amazon QuickSight** kết nối với Amazon Redshift để cung cấp bảng điều khiển, trực quan hóa và BI tự phục vụ cho người dùng nghiệp vụ.                                                                                                                                                                 |

## Kết quả và Lợi ích

Việc triển khai mang lại những kết quả vượt ngoài mong đợi:

-**Giảm thời gian báo cáo từ hơn 10 giờ xuống còn vài phút** – đây là lợi ích hiệu quả duy nhất lớn nhất trong toàn tổ chức. Sự giảm thiểu này cũng làm giảm rủi ro sai sót do con người và cải thiện độ chính xác của dữ liệu.

-**Đạt ROI 1600%** trong lĩnh vực tài chính bằng cách thay thế mô hình hóa thủ công bằng QuickSight Scenarios. Trước đây, nhóm tài chính dành hàng giờ để xây dựng thủ công các mô hình và cấu hình. Giờ đây, họ có thể hỗ trợ các yêu cầu phân tích chuyên sâu trong thời gian giảm đáng kể, tiết kiệm ước tính **22 giờ mỗi tháng** cho mỗi chuyên viên phân tích.

-**Mở rộng BI từ 1 nhóm lên 7 lĩnh vực chức năng:** bao gồm bán hàng, nhân sự, tài chính, tiếp thị, vận hành doanh thu, thành công của khách hàng và lãnh đạo điều hành.

-**Đạt 83% tăng hiệu quả** khi chuyển đổi quy trình báo cáo vận hành thủ công cho bộ phận bán hàng sang các báo cáo bảng điều khiển của QuickSight.

---

**Bài viết tham khảo từ blog chính thức của AWS:**
[https://aws.amazon.com/vi/blogs/business-intelligence/how-pdi-technologies-cut-300-hours-of-manual-reporting-with-amazon-quick/](https://aws.amazon.com/vi/blogs/business-intelligence/how-pdi-technologies-cut-300-hours-of-manual-reporting-with-amazon-quick/)
