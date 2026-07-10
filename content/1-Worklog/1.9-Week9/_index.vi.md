---
title: "Worklog Tuần 9"
date: 2026-06-17
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---


### Mục tiêu tuần 9:

* Triển khai bộ máy tính toán voucher.
* Hỗ trợ giảm giá theo phần trăm và theo số tiền cố định.
* Kiểm tra điều kiện voucher trước khi áp dụng giá cuối cùng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Rà soát các kịch bản giảm giá cần có trong luồng nghiệp vụ và xác định mô hình dữ liệu của voucher.<br>- Xác định các trường cần thiết cho quy tắc áp dụng và logic tính giá. | 15/06/2026 | 15/06/2026 | content/1-Worklog/1.9-Week9/ |
| 3   | - Cài đặt các kiểu voucher giảm theo phần trăm và giảm theo số tiền cố định.<br>- Ánh xạ thiết lập voucher vào luồng tính giá của đơn hàng. | 16/06/2026 | 16/06/2026 | content/1-Worklog/1.9-Week9/ |
| 4   | - Thêm các quy tắc kiểm tra hạn dùng, giá trị đơn tối thiểu và số lần sử dụng voucher.<br>- Đảm bảo voucher không hợp lệ bị loại trước khi tính giá. | 17/06/2026 | 17/06/2026 | content/1-Worklog/1.9-Week9/ |
| 5   | - Tính toán số tiền phải trả sau giảm giá và kiểm tra công thức bằng nhiều trường hợp khác nhau.<br>- Đảm bảo kết quả ổn định ở các tình huống biên. | 18/06/2026 | 18/06/2026 | content/1-Worklog/1.9-Week9/ |
| 6   | - Chạy kiểm thử đầu-cuối cho luồng voucher và xác nhận các quy tắc giảm giá hoạt động đúng.<br>- Kết quả: bộ máy voucher đã sẵn sàng để tích hợp vào bước thanh toán. | 19/06/2026 | 19/06/2026 | content/1-Worklog/1.9-Week9/ |

### Kết quả đạt được tuần 9:

* Xây dựng được hệ thống voucher hỗ trợ giảm theo % và giảm số tiền cố định.
* Kiểm tra thành công các quy tắc nghiệp vụ trước khi áp dụng giảm giá.
* Chuẩn bị logic voucher cho bước tích hợp thanh toán.
