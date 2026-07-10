---
title: "Worklog Tuần 5"
date: 2026-05-20
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---


### Mục tiêu tuần 5:

* Xây dựng quy trình gieo dữ liệu laptop có thể lặp lại.
* Làm sạch và chuẩn hóa dữ liệu đầu vào trước khi import.
* Kiểm tra các bản ghi đã nạp vào cơ sở dữ liệu.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Rà soát các trường dữ liệu cần có trong catalog sản phẩm và cách ánh xạ thuộc tính của laptop vào schema của NovaTech.<br>- Xác định cách biểu diễn tên máy, cấu hình và giá bán trong cơ sở dữ liệu. | 18/05/2026 | 18/05/2026 | content/5-Workshop/5.1-Architecture-Overview/ |
| 3   | - Xây dựng script crawl hoặc batch import để thu thập dữ liệu laptop thực tế phục vụ bộ seed ban đầu.<br>- Chuẩn bị dữ liệu thô ở định dạng phù hợp cho bước chuyển đổi sang bản ghi chuẩn hóa. | 19/05/2026 | 19/05/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 4   | - Làm sạch dữ liệu đã lấy về, chuẩn hóa giá trị thông số và loại bỏ các bản ghi trùng lặp.<br>- Đưa dữ liệu về cấu trúc nhất quán với mô hình quan hệ của hệ thống. | 20/05/2026 | 20/05/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 5   | - Import bộ dữ liệu đã làm sạch vào database và kiểm tra các quan hệ có còn hợp lệ hay không.<br>- Đảm bảo các trường thông tin quan trọng được lưu đúng sau khi chèn dữ liệu. | 21/05/2026 | 21/05/2026 | content/5-Workshop/5.2-RDS-Database/ |
| 6   | - Lấy mẫu một phần dữ liệu đã import và so sánh với dữ liệu nguồn.<br>- Kết quả: catalog seed đã đủ tin cậy để dùng cho các giai đoạn triển khai tiếp theo. | 22/05/2026 | 22/05/2026 | content/5-Workshop/5.1-Architecture-Overview/ |

### Kết quả đạt được tuần 5:

* Thiết lập được quy trình import dữ liệu laptop có thể tái sử dụng.
* Hoàn thành làm sạch và chuẩn hóa dữ liệu trước khi nạp vào database.
* Xác nhận bộ dữ liệu seed đủ ổn định để làm nền cho các chức năng sau.
