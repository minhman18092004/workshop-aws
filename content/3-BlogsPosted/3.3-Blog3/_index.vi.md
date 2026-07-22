---
title: "Blog 3"
date: 2026-07-18
weight: 3
chapter: false
pre: " <b> 3.3. </b> "
---
# BLOG 3: CẠM BẪY AWS SAVINGS PLANS: TIẾT KIỆM 72% TRÊN MỘT HỆ THỐNG LÃNG PHÍ... VẪN LÀ LÃNG PHÍ!

Khi hóa đơn AWS bắt đầu "phình" to, phản xạ tự nhiên của các sếp tài chính hoặc Lead Tech là tìm cách giảm giá ngay lập tức. Và giải pháp "vàng" được đề xuất nhiều nhất chính là **AWS Savings Plans** hoặc **Reserved Instances (RI)** – cam kết dùng 1 đến 3 năm để đổi lấy mức chiết khấu khủng lên tới 72%.

Nghe thì hời đúng không? Nhưng đây lại chính là lúc chiếc bẫy tài chính xuất hiện!

---

## 1. Cái bẫy mang tên "Khóa chân vào sự lãng phí"

Hãy tưởng tượng bạn đang chạy một máy chủ EC2 dòng `m5.2xlarge` (8 vCPU, 32 GiB RAM) giá tầm **$270/tháng**. Thấy hóa đơn cao, bạn quyết định mua ngay gói Compute Savings Plans 3 năm để được giảm 50% tiền máy. Bạn thở phào nghĩ mình đã tiết kiệm được một nửa.

Nhưng sự thật là: Hệ thống của bạn thực chất chỉ dùng hết tối đa 10% CPU và RAM. Về mặt kỹ thuật, bạn chỉ cần dòng máy `m5.large` (2 vCPU, 8 GiB RAM) với giá gốc chỉ khoảng **$70/tháng** là chạy mượt mà.

Bằng việc vội vàng mua Savings Plans:
- **Tự "khóa" mình vào cấu hình thừa**: Bạn phải gắn chặt với một cấu hình dư thừa trong suốt 3 năm.
- **Trả tiền cao hơn nhu cầu thực tế**: Bạn trả **$135/tháng** (sau giảm) cho một hệ thống đáng lẽ chỉ tốn **$70/tháng** (giá gốc chưa giảm).
- **Lãng phí mỗi ngày**: Bạn vẫn đang lãng phí tiền dưới cái mác "đã được giảm giá".

---

## 2. Nghệ thuật FinOps: "Shrink First, Commit Later" (Bóp nhỏ trước, Cam kết sau)

Để không mất tiền oan, quy trình chuẩn chỉnh của các kỹ sư Cloud chuyên nghiệp luôn là: **Tối ưu hóa tài nguyên trước (Right-sizing), rồi mới mua gói cam kết sau (Commitment)**.

### Bước 1: Hãy để AWS Compute Optimizer lên tiếng
Trước khi xuống tiền cam kết, hãy bật công cụ miễn phí **AWS Compute Optimizer**. Công cụ này sử dụng AI để quét lịch sử vận hành EC2 và chỉ ra chính xác máy nào đang chạy dưới công suất, gợi ý bạn hạ cấp (downsize) hoặc chuyển sang dòng chip ARM AWS Graviton (`m7g`) tiết kiệm điện hơn.

### Bước 2: Dọn dẹp tài nguyên (Clean up)
Tắt sạch các máy chủ "mồ côi" không ai dùng ở môi trường Dev/Test trước khi đo đạc lại lượng tài nguyên thực tế cần cam kết.

### Bước 3: Chốt đơn cam kết (Commit)
Chỉ sau khi hệ thống đã được "vắt sạch mỡ thừa" và chạy đúng công suất thực tế, bạn mới dùng lượng tài nguyên đó để mua Savings Plans.

---

## 3. Con số "biết nói" từ chính AWS

Theo báo cáo chuyên sâu *"The AWS State of Cost Efficiency Report"* trên trang blog chính thức của AWS Cloud Financial Management:

> "Những doanh nghiệp kết hợp cả việc tối ưu kích thước máy chủ (rightsizing) lẫn mua các gói cam kết (commitments) sẽ nâng điểm hiệu quả chi phí nhanh hơn **gấp 4 LẦN** so với những bên chỉ chăm chăm mua Savings Plans mà không tối ưu hệ thống trước." 
> 
> *— Nguồn: AWS Cloud Financial Management Blog*

Con số **gấp 4 lần** này là minh chứng rõ ràng nhất: Tối ưu kiến trúc luôn mang lại giá trị bền vững và tiết kiệm sâu hơn rất nhiều so với việc chỉ mua các gói chiết khấu tài chính thuần túy.

---

## 4. Lời kết & Discussion

**Lời khuyên:** Mua AWS Savings Plans là cực tốt, nhưng hãy xây dựng nó trên một hạ tầng tinh gọn. **Đừng giảm giá cho sự dư thừa tài nguyên!**

Anh em ở đây có ai từng lỡ mua Savings Plans cho một hệ thống thừa thãi cấu hình chưa? Cùng chia sẻ "đau thương" hoặc thảo luận bên dưới nhé!

---

## 5. Link tham khảo

Xem bài viết chi tiết từ nguồn gốc AWS Cloud Financial Management Blog: 👉 [The AWS State of Cost Efficiency Report](https://aws.amazon.com/vi/blogs/aws-cloud-financial-management/the-aws-state-of-cost-efficiency-report/)

## 6. Link bài viết

Xem bài viết chi tiết và tham gia thảo luận trên Facebook: 👉 [Bài viết chia sẻ trên Facebook](https://www.facebook.com/groups/awsstudygroupfcj/permalink/2213983459366614/?rdid=xKQVbSx1f2LiQL6y#)