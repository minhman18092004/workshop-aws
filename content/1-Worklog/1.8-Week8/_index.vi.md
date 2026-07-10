---
title: "Worklog Tuần 8"
date: 2026-06-10
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---


### Mục tiêu tuần 8:

* Cấu hình xác thực người dùng cho ứng dụng.
* Kết nối frontend với luồng đăng ký và đăng nhập của AWS Cognito.
* Đảm bảo các thông số chạy ứng dụng được nạp qua biến môi trường.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Rà soát luồng tích hợp Cognito và xác nhận các endpoint xác thực mà frontend cần sử dụng.<br>- Xác định các giá trị môi trường phải được cung cấp lúc chạy ứng dụng. | 08/06/2026 | 08/06/2026 | content/5-Workshop/5.4-Cognito-Auth/ |
| 3   | - Cấu hình Amplify và liên kết frontend với user pool cùng app client id của Cognito.<br>- Đảm bảo ứng dụng có thể đọc cấu hình xác thực từ môi trường. | 09/06/2026 | 09/06/2026 | content/5-Workshop/5.4-Cognito-Auth/ |
| 4   | - Triển khai luồng đăng ký và xác nhận tài khoản, kiểm tra quy trình tạo người dùng đầu cuối.<br>- Xác nhận trạng thái xác thực sau khi đăng ký hoạt động đúng. | 10/06/2026 | 10/06/2026 | content/5-Workshop/5.4-Cognito-Auth/ |
| 5   | - Bổ sung phần đăng nhập và kiểm tra truy cập token vào các route được bảo vệ trong ứng dụng.<br>- Thử nghiệm hành trình đăng nhập bằng một tài khoản thật. | 11/06/2026 | 11/06/2026 | content/5-Workshop/5.4-Cognito-Auth/ |
| 6   | - Rà soát lại cấu hình xác thực và xác nhận các giá trị runtime đã ổn định.<br>- Kết quả: luồng đăng nhập của người dùng đã sẵn sàng cho các bước tích hợp tiếp theo. | 12/06/2026 | 12/06/2026 | content/5-Workshop/5.4-Cognito-Auth/ |

### Kết quả đạt được tuần 8:

* Kết nối thành công frontend với luồng xác thực dựa trên Cognito.
* Externalize các thông số xác thực để nạp khi chạy ứng dụng.
* Kiểm tra thành công luồng đăng ký và đăng nhập đầu-cuối.
