---
title: "Worklog Tuần 3"
date: 2026-05-06
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Bắt đầu xây dựng nền tảng container hóa cho cả frontend và backend.
* Externalize các giá trị runtime để hệ thống có thể triển khai ở nhiều môi trường khác nhau.
* Chuẩn bị cấu trúc dự án cho quy trình triển khai theo hướng GitOps ở các tuần sau.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Rà soát luồng khởi động hiện tại của frontend và backend để xác định các giá trị nên được truyền vào lúc chạy thay vì hardcode.<br>- Lập danh sách biến môi trường cần dùng cho bước triển khai sau này. | 04/05/2026 | 04/05/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 3   | - Phác thảo cấu trúc Dockerfile ban đầu cho backend theo hướng tách riêng bước build và runtime.<br>- Giữ phần build độc lập với các thiết lập chạy ứng dụng. | 05/05/2026 | 05/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 4   | - Phác thảo Dockerfile cho frontend và kiểm tra khả năng khởi động ứng dụng bằng cấu hình ngoài.<br>- Đảm bảo image build không chứa secrets hoặc giá trị phụ thuộc môi trường. | 06/05/2026 | 06/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 5   | - Đồng bộ cách cấu hình giữa frontend và backend để cả hai dịch vụ cùng đọc được bộ giá trị triển khai.<br>- Chuẩn bị cho các bước điều phối container ở giai đoạn tiếp theo. | 07/05/2026 | 07/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 6   | - Rà soát lại cấu hình container đã chuẩn bị và kiểm tra mức độ sẵn sàng cho mô hình triển khai GitOps.<br>- Kết quả: nền tảng triển khai đã sẵn sàng cho các giai đoạn tiếp theo. | 08/05/2026 | 08/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |

### Kết quả đạt được tuần 3:

* Hoàn thành bước chuẩn bị Dockerfile ban đầu cho cả frontend và backend.
* Đưa dự án gần hơn với mô hình triển khai dựa trên môi trường bằng cách tách cấu hình runtime khỏi mã nguồn.
* Thiết lập tiền đề cần thiết cho các giai đoạn GitOps và điều phối container sau này.
