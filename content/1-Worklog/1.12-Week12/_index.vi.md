---
title: "Worklog Tuần 12"
date: 2026-07-13
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---


### Mục tiêu tuần 12:

* Thiết lập giám sát hệ thống bằng Prometheus và Grafana.
* Xác thực luồng GitOps và triển khai cuối cùng.
* Khép lại dự án bằng cấu hình ổn định, sẵn sàng cho báo cáo.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Bật endpoint Prometheus của Spring Boot Actuator và xuất các chỉ số ứng dụng.<br>- Xác nhận backend đã sẵn sàng để hệ thống giám sát thu thập dữ liệu. | 07/07/2026 | 07/07/2026 | content/1-Worklog/1.12-Week12/ |
| 3   | - Triển khai Prometheus và Grafana rồi kết nối nguồn metrics từ backend.<br>- Tạo lớp giám sát cơ bản cho toàn hệ thống. | 08/07/2026 | 08/07/2026 | content/1-Worklog/1.12-Week12/ |
| 4   | - Xây dựng các panel Grafana cho bộ nhớ JVM, thread và lưu lượng HTTP request.<br>- Kiểm tra dashboard có phản ánh đúng hành vi runtime hay không. | 09/07/2026 | 09/07/2026 | content/1-Worklog/1.12-Week12/ |
| 5   | - Rà soát đồng bộ GitOps và xác nhận thay đổi triển khai vẫn khớp với trạng thái Git.<br>- Kiểm tra tính nhất quán cấu hình sau khi hoàn tất giám sát. | 10/07/2026 | 10/07/2026 | content/1-Worklog/1.12-Week12/ |
| 6   | - Thực hiện kiểm tra hệ thống cuối cùng, thu thập các bằng chứng cuối và chuẩn bị ghi chú cho báo cáo.<br>- Kết quả: dự án được khép lại với các bước kiểm tra giám sát và triển khai đã hoàn tất. | 13/07/2026 | 13/07/2026 | content/1-Worklog/1.12-Week12/ |

### Kết quả đạt được tuần 12:

* Triển khai thành công Prometheus và Grafana để giám sát hệ thống.
* Xác nhận tính nhất quán triển khai cuối cùng thông qua kiểm tra GitOps.
* Hoàn tất timeline dự án bằng bước rà soát cuối cùng trước khi đưa vào báo cáo.
