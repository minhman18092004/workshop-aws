---
title: "Blog 1"
date: 2026-07-13
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# BLOG 1: GIẢM ĐỘ TRỄ TỪ GIÂY XUỐNG MILIGIÂY: NGHỆ THUẬT CACHING TRÊN AWS

Chào mọi người, trong quá trình tối ưu hóa hệ thống, có một chỉ số luôn ám ảnh đội ngũ của chúng tôi: **Độ trễ (Latency)**. Việc nhìn thấy một trang web xoay vòng mất 2-3 giây để tải dữ liệu, trong khi người dùng liên tục nhấn F5, thực sự là một cơn ác mộng.

Thông thường, thủ phạm đằng sau 90% các nút thắt cổ chai của hệ thống là Cơ sở dữ liệu truyền thống (RDS/SQL). Khi ứng dụng phát triển, khối lượng truy vấn đến tăng lên, buộc cơ sở dữ liệu phải xử lý các câu lệnh JOIN và SELECT phức tạp từ hàng ngàn người dùng cùng lúc. Việc sử dụng CPU tăng vọt lên 90% và hệ thống bắt đầu "nghẽn".

Thay vì chọn giải pháp tốn kém là mở rộng instance cơ sở dữ liệu lên các tier đắt tiền, đội ngũ của chúng tôi đã áp dụng một kỹ thuật cloud quen thuộc nhưng mang lại hiệu quả cao: **Tối ưu hóa lớp caching với Amazon ElastiCache**. Kết quả vô cùng ấn tượng, với độ trễ giảm từ tính bằng giây xuống mức dưới miligiây, đồng thời giảm tải hoàn toàn cho cơ sở dữ liệu.

---

## 1. Amazon ElastiCache: "Trạm sơ cứu" siêu tốc trên RAM

Để hiểu tại sao giải pháp này lại nhanh như vậy, chúng ta cần xem xét bản chất của việc lưu trữ dữ liệu.

Các cơ sở dữ liệu truyền thống như MySQL hoặc PostgreSQL lưu trữ dữ liệu trên ổ đĩa (SSD/HDD). Bất kể SSD ngày nay nhanh đến đâu, việc đọc/ghi từ đĩa đều phải đi qua các lớp vật lý và các thuật toán phức tạp.

Ngược lại, **Amazon ElastiCache** là một dịch vụ lưu trữ dữ liệu trên bộ nhớ (in-memory) được quản lý hoàn toàn bởi AWS. Hệ thống này hỗ trợ hai engine rất phổ biến: Redis và Memcached. Do dữ liệu nằm hoàn toàn trong RAM, tốc độ phản hồi của ElastiCache cực kỳ nhanh, được đo bằng miligiây hoặc thậm chí là microgiây.

Thay vì buộc cơ sở dữ liệu chính phải liên tục tính toán các dữ liệu ít khi thay đổi (chẳng hạn như danh mục sản phẩm, cấu hình hệ thống, hồ sơ người dùng, các bài báo hot, v.v.), chúng tôi lưu trữ dữ liệu đó trực tiếp trong RAM của ElastiCache. Trong thiết lập này, ElastiCache đóng vai trò như một trạm sơ cứu siêu tốc, chặn đứng hầu hết các yêu cầu trước khi chúng có thể tiếp cận và gây nghẽn cơ sở dữ liệu chính.

---

## 2. Link bài viết

Xem bài viết chi tiết và tham gia thảo luận trên Facebook: 👉 [Bài viết chia sẻ trên Facebook](https://www.facebook.com/share/p/1GNrhrDMKH/)