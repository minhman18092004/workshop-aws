---
title: "5.7. Dọn dẹp tài nguyên"
date: 2026-07-13
weight: 7
---

Sau khi hoàn thành thử nghiệm và chụp ảnh báo cáo, bạn cần thực hiện dọn dẹp các tài nguyên hạ tầng đã khởi tạo trên AWS để đảm bảo không phát sinh chi phí duy trì không đáng có trên tài khoản cá nhân.

---

#### 1. Xóa cơ sở dữ liệu Amazon RDS PostgreSQL
1. Truy cập trang điều khiển **RDS $\rightarrow$ Databases**.
2. Chọn Database instance `novatech-db`.
3. Nhấp chọn mục **Actions** ở góc phải và chọn **Delete**.
4. Bỏ tích chọn mục **Create final snapshot** (tạo bản sao lưu cuối cùng) và xác nhận đồng ý xóa.
5. Gõ chữ `delete me` vào ô xác nhận để tiến hành xóa database.

![Xác nhận xóa RDS Database](/images/5.7_1.png)
![Trạng thái đang xóa RDS Database](/images/5.7_2.png)


#### 2. Xóa các S3 Buckets
1. Truy cập dịch vụ **Amazon S3 $\rightarrow$ Buckets**.
2. Với mỗi bucket (`novatech-product-images` và `novatech-chatbot-rag`):
   - Bạn cần nhấn chọn bucket đó và nhấn nút **Empty** để xóa sạch các tệp tin lưu trữ bên trong trước.
   - Nhập `permanently delete` để xác nhận dọn dẹp đối tượng.

     ![Xác nhận dọn dẹp S3 Bucket](/images/5.7_3.png)
     ![Dọn dẹp S3 Bucket thành công](/images/5.7_4.png)

   - Quay lại trang danh sách buckets, chọn bucket và nhấn nút **Delete**.
   - Nhập tên của bucket để xác nhận xóa vĩnh viễn.

     ![Xác nhận xóa S3 Bucket](/images/5.7_5.png)
     ![Xóa S3 Bucket thành công](/images/5.7_6.png)


#### 3. Xóa Amazon Cognito User Pool
1. Truy cập dịch vụ **Cognito $\rightarrow$ User Pools**.
2. Chọn Pool `novatech-user-pool`.
3. Chọn nút **Delete user pool** ở góc phải và làm theo hướng dẫn xác nhận xóa để hủy bỏ hệ thống định danh người dùng.

   ![Xác nhận xóa Cognito User Pool](/images/5.7_7.png)
   ![Xóa Cognito User Pool thành công](/images/5.7_8.png)


#### 4. Vô hiệu hóa và xóa CloudFront Distribution
Để dọn dẹp phân phối mạng CDN đã tạo:
1. Truy cập dịch vụ **Amazon CloudFront $\rightarrow$ Distributions**.
2. Chọn Distribution đã thiết lập cho S3.
3. Nhấp chọn nút **Disable** và xác nhận để vô hiệu hóa cổng phân phối này trước khi tiến hành xóa:

   ![Vô hiệu hóa CloudFront Distribution](/images/5.7_9.png)

4. Khi trạng thái phân phối đã được vô hiệu hóa thành công, bạn sẽ nhận được thông báo sẵn sàng xóa:

   ![Trạng thái vô hiệu hóa hoàn tất](/images/5.7_10.png)

5. Tích chọn Distribution, nhấn nút **Delete** và chọn **Delete** trên popup xác nhận để gỡ bỏ hoàn toàn:

   ![Xác nhận xóa Distribution](/images/5.7_11.png)
   ![Xóa Distribution thành công](/images/5.7_12.png)



