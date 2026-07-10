---
title: "Worklog Tuần 4"
date: 2026-05-13
weight: 1
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Thiết lập lớp lưu trữ hình ảnh cho sản phẩm.
* Giữ bucket S3 ở trạng thái riêng tư và chỉ cho phép CloudFront đọc dữ liệu.
* Tách các thông số liên quan đến storage ra khỏi mã nguồn để sẵn sàng cho triển khai.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Rà soát yêu cầu lưu trữ hình ảnh sản phẩm và xác nhận lý do không nên lưu toàn bộ asset trực tiếp trên máy chủ ứng dụng.<br>- Xác định luồng lưu trữ riêng tư giữa S3 và CloudFront. | 11/05/2026 | 11/05/2026 | content/5-Workshop/5.3-S3-Storage/ |
| 3   | - Cấu hình bucket S3 và cập nhật policy truy cập để chỉ CloudFront có thể đọc object.<br>- Kiểm tra việc phân phối ảnh qua domain CDN thay vì URL gốc của bucket. | 12/05/2026 | 12/05/2026 | content/5-Workshop/5.3-S3-Storage/ |
| 4   | - Tích hợp service lưu trữ ở backend bằng AWS SDK và chuẩn bị luồng upload/xóa hình ảnh sản phẩm.<br>- Kết quả: việc xử lý ảnh có thể thực hiện thông qua API. | 13/05/2026 | 13/05/2026 | content/5-Workshop/5.3-S3-Storage/ |
| 5   | - Externalize tên bucket, region và thông tin truy cập vào biến môi trường.<br>- Giữ cấu hình triển khai tách biệt khỏi mã nguồn. | 14/05/2026 | 14/05/2026 | content/5-Workshop/5.3-S3-Storage/ |
| 6   | - Kiểm tra lại toàn bộ đường đi của ảnh từ backend đến S3 và qua CloudFront.<br>- Kết quả: luồng phân phối ảnh đã sẵn sàng cho triển khai kiểu production. | 15/05/2026 | 15/05/2026 | content/5-Workshop/5.3-S3-Storage/ |

### Kết quả đạt được tuần 4:

* Xây dựng được mô hình lưu trữ ảnh riêng tư kết hợp CDN cho sản phẩm.
* Kết nối backend với S3 bằng AWS SDK và chuẩn hóa cấu hình runtime.
* Chuẩn bị xong lớp storage cho giai đoạn triển khai và mở rộng sau này.
