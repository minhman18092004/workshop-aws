---
title: "Worklog Tuần 11"
date: 2026-07-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---


### Mục tiêu tuần 11:

* Chuẩn bị cấu hình triển khai theo hướng GitOps.
* Tách mã nguồn ứng dụng khỏi định nghĩa hạ tầng và runtime.
* Kiểm tra khả năng theo dõi và áp dụng thay đổi cấu hình một cách rõ ràng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Rà soát cấu trúc triển khai hiện tại và quyết định những file nào cần đặt ngoài repository ứng dụng.<br>- Xác định các giá trị runtime và manifest cần chuyển sang không gian cấu hình riêng. | 29/06/2026 | 29/06/2026 | content/1-Worklog/1.12-Week12/ |
| 3   | - Tạo hoặc dọn lại cấu trúc repository triển khai chuyên cho file YAML và compose.<br>- Giữ cấu hình deploy tập trung và tách biệt với mã nguồn. | 30/06/2026 | 30/06/2026 | content/1-Worklog/1.12-Week12/ |
| 4   | - Chuẩn bị cơ chế đồng bộ theo dõi thay đổi cấu hình và áp dụng vào môi trường đích.<br>- Kiểm tra luồng triển khai có vận hành theo mô hình pull-based. | 01/07/2026 | 01/07/2026 | content/1-Worklog/1.12-Week12/ |
| 5   | - Thử tình huống lệch cấu hình và xác nhận trạng thái triển khai có thể khôi phục từ Git.<br>- Đảm bảo server luôn khớp với trạng thái trong repository. | 02/07/2026 | 02/07/2026 | content/1-Worklog/1.12-Week12/ |
| 6   | - Rà soát toàn bộ luồng triển khai và chốt các ghi chú cần thiết cho tuần monitoring cuối cùng.<br>- Kết quả: phần chuẩn bị GitOps đã hoàn tất. | 03/07/2026 | 03/07/2026 | content/1-Worklog/1.12-Week12/ |

### Kết quả đạt được tuần 11:

* Tách biệt cấu hình triển khai khỏi mã nguồn ứng dụng.
* Chuẩn bị mô hình đồng bộ kiểu GitOps cho thay đổi triển khai.
* Kiểm tra được khả năng khôi phục khi cấu hình bị lệch.
