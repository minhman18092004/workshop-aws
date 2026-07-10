---
title: "Worklog Tuần 10"
date: 2026-06-24
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu tuần 10:

* Container hóa các dịch vụ ứng dụng để có thể triển khai lặp lại.
* Hoàn thiện cấu hình Docker Compose và mạng giữa các service.
* Giữ các giá trị nhạy cảm ở ngoài image container.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Chỉnh sửa lại Dockerfile của frontend và backend để phần build và runtime được tách riêng.<br>- Giảm nguy cơ đưa giá trị phụ thuộc môi trường vào trong image. | 22/06/2026 | 22/06/2026 | content/1-Worklog/1.3-Week3/ |
| 3   | - Định nghĩa stack Docker Compose cho frontend, backend, database, cache và các dịch vụ phụ trợ.<br>- Kiểm tra khả năng các container phân giải được tên của nhau trên mạng nội bộ. | 23/06/2026 | 23/06/2026 | content/1-Worklog/1.3-Week3/ |
| 4   | - Cấu hình liên kết biến môi trường bên ngoài cho các container và kiểm tra các giá trị runtime riêng của từng service.<br>- Giúp việc chuyển giữa môi trường local và server trở nên dễ dàng hơn. | 24/06/2026 | 24/06/2026 | content/1-Worklog/1.3-Week3/ |
| 5   | - Bổ sung volume lưu trữ cho các dữ liệu trạng thái cần tồn tại sau khi restart hoặc tạo lại container.<br>- Xác nhận database và các dịch vụ hỗ trợ vẫn giữ được dữ liệu. | 25/06/2026 | 25/06/2026 | content/1-Worklog/1.3-Week3/ |
| 6   | - Chạy toàn bộ stack ở local và kiểm tra khả năng khởi động bằng một lệnh điều phối duy nhất.<br>- Kết quả: dự án đã sẵn sàng để kiểm thử quy trình triển khai. | 26/06/2026 | 26/06/2026 | content/1-Worklog/1.3-Week3/ |

### Kết quả đạt được tuần 10:

* Container hóa thành công các dịch vụ chính của ứng dụng.
* Xây dựng được stack Docker Compose có thể tái sử dụng.
* Giữ cấu hình runtime tách biệt khỏi image.
