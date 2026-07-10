---
title: "Worklog Tuần 7"
date: 2026-06-03
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---


### Mục tiêu tuần 7:

* Tích hợp dịch vụ chatbot AI vào trải nghiệm sản phẩm.
* Sử dụng ngữ cảnh kiểu RAG để mô hình trả lời dựa trên dữ liệu dự án.
* Kiểm tra luồng chatbot từ API backend đến giao diện người dùng.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2   | - Rà soát luồng nghiệp vụ của chatbot và các nguồn tri thức sản phẩm sẵn có.<br>- Xác định cách trợ lý AI hỗ trợ tư vấn laptop ngay trên giao diện cửa hàng. | 01/06/2026 | 01/06/2026 | content/5-Workshop/5.1-Architecture-Overview/ |
| 3   | - Xin quyền truy cập model trên Amazon Bedrock và chuẩn bị dependency SDK runtime trong backend.<br>- Đảm bảo ứng dụng có thể gọi model đã chọn một cách an toàn. | 02/06/2026 | 02/06/2026 | content/5-Workshop/5.5-Bedrock-AI/ |
| 4   | - Triển khai service sinh phản hồi và nhúng ngữ cảnh sản phẩm đã chuẩn bị vào system prompt.<br>- Giữ cho model bám sát dữ liệu dự án thay vì trả lời chung chung. | 03/06/2026 | 03/06/2026 | content/5-Workshop/5.5-Bedrock-AI/ |
| 5   | - Kết nối API chatbot với frontend và kiểm tra widget chat có thể gửi nhận tin nhắn đúng cách.<br>- Thử một số câu hỏi tư vấn laptop để xác nhận hành vi. | 04/06/2026 | 04/06/2026 | content/5-Workshop/5.5-Bedrock-AI/ |
| 6   | - Rà soát câu trả lời và tinh chỉnh hành vi prompt khi cần thiết.<br>- Kết quả: chatbot đã có thể dùng như một tính năng tư vấn cho dự án. | 05/06/2026 | 05/06/2026 | content/5-Workshop/5.5-Bedrock-AI/ |

### Kết quả đạt được tuần 7:

* Tích hợp thành công chatbot AI với backend và frontend.
* Gắn ngữ cảnh dự án để phản hồi bám sát dữ liệu cửa hàng.
* Xác nhận chatbot đủ dùng như một tính năng tư vấn thực tế.
