---
title: "Worklog Tuần 2"
date: 2026-10-05
weight: 1
chapter: false
pre: " <b> 1.2. </b> "
---


### Mục tiêu tuần 2:

* Kết nối, làm quen với các thành viên trong First Cloud AI Journey.
* Hiểu dịch vụ AWS cơ bản, cách dùng console & CLI.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - Ôn tập về các công dụng và ý nghĩa của hàm chi phí trong học máy <br> - Ôn tập về việc huấn luyện một mô hình với Gradient Descent                                                                                             | 05/10/2026   | 05/10/2026      |
| 3   | - Tìm hiểu AWS và các loại dịch vụ: <br>&emsp; + Compute <br>&emsp; + Storage <br>&emsp; + Networking <br>&emsp; + Database <br>                                            | 06/10/2026   | 06/10/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 4   | - Tìm hiểu về Cross-Validation để tận dụng tối đa dữ liệu trong học máy <br> - Xử lí dữ liệu Categorial & One-Hot Encoding: <br>&emsp; + Nominal & Ordinal Data <br>&emsp; + Phương pháp One-Hot cho Nominal data <br> - Phương pháp cho Feature Scaling: <br>&emsp; + Standardization <br>&emsp; + Min-Max Normalization <br> - **Thực hành:** <br>&emsp; + Chia tập Train/Test/Valid cho tập dữ liệu <br>&emsp; + Thực hành Feature Scaling cho một tập dữ liệu <br> &emsp; + Thực hành dùng phương pháp One-Hot cho Nominal data | 07/10/2026   | 07/10/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 5   | - Tìm hiểu EC2 cơ bản: <br>&emsp; + Instance types <br>&emsp; + AMI <br>&emsp; + EBS <br>&emsp; + Instance Lifecycle <br> - Các cách remote SSH vào EC2 <br> - Tìm hiểu Elastic IP <br> - Tìm hiểu cơ bản về S3: <br>&emsp; + Bucket, Object, Key <br>&emsp; + Storage Class <br>&emsp; + Quản lý phiên bản <br>&emsp; + Multipart Upload <br>&emsp; + Quyền truy cập <br> - **Thực hành:** <br>&emsp; + Tạo và SSH vào một EC2 <br>&emsp; + Gắn EBS vào một EC2 <br>&emsp; + Cấu hình môi trường <br>&emsp; + Cho EC2 truy cập vào S3 + Download dữ liệu từ S3 + Upload kết quả lên S3 và dọn tài nguyên tránh phát sinh chi phí                 | 08/10/2026   | 08/10/2026      | <https://cloudjourney.awsstudygroup.com/> |
| 6   | - Tìm hiểu cơ bản về Serverless <br> - Tìm hiểu về dịch vụ AWS Lambda <br> - Tìm hiểu về dịch vụ AWS Fargate <br> - So sánh giữa EC2, Lambda, Fargate trong các trường hợp khác nhau                                                                                         | 09/10/2026   | 09/10/2026      | <https://cloudjourney.awsstudygroup.com/> |


### Kết quả đạt được tuần 2:

* Hiểu được gradient descent có ý nghĩa gì? Cách mà gradient descent hoạt động trong một mô hình học máy.
  * Khái niệm Gradient descent
  * Gradient descent đóng vai trò gì trong một mô hình học máy, tác động của nó tới những tham số của hàm
  * Thuật toán của Gradient descent
  * Bên trong một mô hình được huấn luyện bằng Gradient descent sẽ như thế nào
  * Mối liên hệ của Gradient descent với Learning rate

* Phân biệt các kiểu dữ liệu của từng Feature:
  * Nominal
  * Ordinal
  * Ratio
  * Interval

* Hiểu cách ứng dụng Scaling Feature và các phương pháp của nó: 
  * Thời điểm nên dùng Scaling Feature
  * Standardization và ứng dụng
  * Min-Max Normalization và ứng dụng

* Học được cách sử dụng One-Hot Encoding trên tập dữ liệu Nominal để mô hình không bị nhận thông tin rác khi huấn luyện.

* Hiểu ứng dụng của EC2, mối liên hệ giữa EC2 và AMI.

* Tạo một EC2 sử dụng VPC mặc định bao gồm:
  * Instance Type
  * EBS (Elastic Block Store)
  * Key Pair
  * Elastic ID
  * Security Group

* Phân biệt được giữa Instance Store và EBS, khi nào nên lưu dữ liệu ở cái nào.

* Biết được cách chọn Instance Type phù hợp cho từng tác vụ:
  * Dòng P hoặc G: Có GPU của NVIDIA. Chuyên dùng để train Deep Learning hoặc chạy model nặng (như LLM)
  * Dòng R: Rất nhiều RAM. Dùng khi xử lý lượng dữ liệu lớn cần load toàn bộ tập dữ liệu vào bộ nhớ
  * Dòng C: Rất nhiều CPU. Dùng để xử lý logic, crawl data tốc độ cao
  * Dòng T hoặc M: Cân bằng CPU/RAM. Dùng làm Web Server, chạy API backend bình thường

* Hiểu được cơ bản về S3:
  * Biết cách chọn S3 cho phù hợp với nhu cầu 
  * Hiểu cách hoạt động tính năng Multipart Upload của S3
  * Biết tùy chỉnh quyền truy cập cho những đối tượng cụ thể

* Cần phải nén dữ liệu trước khi upload lên S3 để giảm đáng kể chi phí Request (Ví dụ: nén từ 1 triệu file .png khác nhau thành 1 file .zip).

* Hiểu được Serverless là gì, khi nào thì cần phải dùng Serverless.

* Biết được cách ứng dụng của các dịch vụ như EC2, Lambda, Fargate cho từng trường hợp:
  * Chi phí
  * Latency
  * Tốc độ mở rộng
  * Hỗ trợ huấn luyện AI
  * Độ trễ khởi động


