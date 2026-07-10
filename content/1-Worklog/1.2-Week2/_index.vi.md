---
title: "Worklog Tuần 2"
date: 2026-04-29
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---


### Mục tiêu tuần 2:

* Hoàn thiện phương án sử dụng cơ sở dữ liệu PostgreSQL được quản lý cho dữ liệu giao dịch.
* Bảo mật cấu hình backend bằng cách tách các giá trị kết nối ra ngoài mã nguồn.
* Kiểm tra khả năng kết nối của ứng dụng với cơ sở dữ liệu sau khi áp dụng cấu hình mới.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Khởi tạo instance RDS PostgreSQL và giữ chế độ public access ở trạng thái tắt.<br>- Kiểm tra endpoint, port và vị trí VPC được dùng cho lớp dữ liệu.<br>- Kết quả: dịch vụ database đã sẵn sàng trong mạng riêng.<br>- Khó khăn: phạm vi kết nối phải được giới hạn chặt chẽ để đảm bảo an toàn.<br>- Hướng xử lý: chỉ cho phép máy chủ ứng dụng truy cập database. | 27/04/2026 | 27/04/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 3   | - Đưa thông tin kết nối database vào biến môi trường thay vì khai báo cứng.<br>- Ánh xạ các giá trị này vào cấu hình datasource của Spring Boot.<br>- Kết quả: backend có thể đọc DB_URL, DB_USERNAME và DB_PASSWORD khi khởi động.<br>- Khó khăn: các giá trị runtime phải khớp chính xác với endpoint của RDS.<br>- Hướng xử lý: kiểm tra luồng kết nối sau khi truyền cấu hình động. | 28/04/2026 | 28/04/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 4   | - Chạy backend với bộ cấu hình mới và xác nhận đường kết nối tới cơ sở dữ liệu.<br>- Kiểm tra schema và các thiết lập JPA trong profile triển khai.<br>- Kết quả: ứng dụng có thể truy cập PostgreSQL qua endpoint được quản lý.<br>- Khó khăn: chỉ cần sai host hoặc mật khẩu là quá trình khởi động bị chặn ngay.<br>- Hướng xử lý: áp dụng cùng mẫu cấu hình này cho các dịch vụ ngoài khác. | 29/04/2026 | 29/04/2026 | content/5-Workshop/5.2-RDS-Database/ |

### Kết quả đạt được tuần 2:

* Thiết lập được mô hình triển khai PostgreSQL an toàn thông qua Amazon RDS.
* Tách cấu hình database ra ngoài để backend không còn phụ thuộc vào thông tin đăng nhập hardcode.
* Xác nhận ứng dụng Spring Boot có thể kết nối ổn định với lớp dữ liệu được quản lý.
