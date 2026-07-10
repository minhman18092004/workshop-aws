---
title: "Worklog Tuần 6"
date: 2026-05-27
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Mục tiêu tuần 6:

* Chuẩn bị môi trường máy chủ ứng dụng cho triển khai thực tế.
* Kết nối runtime backend với systemd, reverse proxy và luồng thanh toán.
* Chuẩn hóa cấu hình bên ngoài cho ứng dụng đã triển khai.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Rà soát cấu hình máy chủ DigitalOcean và chuẩn bị môi trường Ubuntu cho ứng dụng backend.<br>- Xác nhận máy chủ triển khai đã sẵn sàng cho truy cập từ xa và cài đặt gói cần thiết. | 25/05/2026 | 25/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 3   | - Cài đặt Java runtime và đăng ký file JAR của backend dưới dạng dịch vụ systemd.<br>- Đảm bảo dịch vụ có thể tự khởi động và chạy nền ổn định. | 26/05/2026 | 26/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 4   | - Cấu hình Nginx làm reverse proxy cho domain API và chuyển tiếp lưu lượng công khai vào cổng nội bộ của backend.<br>- Kiểm tra phản hồi của server khi đi qua lớp proxy. | 27/05/2026 | 27/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 5   | - Bổ sung HTTPS cho endpoint triển khai và giữ các giá trị runtime trong một file environment riêng.<br>- Đồng bộ cấu hình triển khai với mô hình quản lý hiện có. | 28/05/2026 | 28/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |
| 6   | - Tích hợp luồng thanh toán PayOS và kiểm tra việc sinh link thanh toán, mã QR hoạt động chính xác.<br>- Kết quả: máy chủ đã sẵn sàng cho luồng triển khai backend đầu-cuối an toàn. | 29/05/2026 | 29/05/2026 | content/5-Workshop/5.6-Non-AWS-Services/ |

### Kết quả đạt được tuần 6:

* Thiết lập được máy chủ ứng dụng với systemd và Nginx.
* Chuẩn hóa cấu hình runtime bằng file environment bên ngoài.
* Xác nhận backend triển khai được luồng thanh toán cần thiết của hệ thống.
