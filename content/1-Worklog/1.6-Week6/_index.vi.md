---
title: "Worklog Tuần 6"
date: 2026-07-05
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:

* Tìm hiểu về mô hình kiến trúc phi máy chủ (Serverless Architecture) và các lợi ích về mặt vận hành, chi phí.
* Hiểu rõ dịch vụ AWS Lambda, nắm vững cách viết, đóng gói và triển khai các hàm (functions).
* Hiểu rõ cơ chế định tuyến và quản lý API với Amazon API Gateway, đóng vai trò là cửa ngõ giao tiếp cho hệ thống Serverless.
* Triển khai một hệ thống Backend phi máy chủ hoàn chỉnh, tích hợp liên hoàn giữa S3, API Gateway, Lambda và DynamoDB.
* Thiết kế và xây dựng các chuẩn RESTful API, đảm bảo tính bảo mật và khả năng mở rộng của ứng dụng.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nghiên cứu nền tảng kiến trúc Serverless trên AWS <br>&emsp; + Phân tích định nghĩa, ưu điểm và các use-cases thực tế của Serverless <br>&emsp; + Khảo sát dịch vụ AWS Lambda: Event sources, Execution environment <br>&emsp; + Tìm hiểu Amazon API Gateway và cách kết nối tích hợp với Lambda | 25/05/2026 | 25/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - **Lab:** Triển khai Serverless Backend (Phần 1: Cấu trúc dữ liệu và xử lý) <br>&emsp; + Thiết kế và khởi tạo bảng dữ liệu NoSQL với Amazon DynamoDB <br>&emsp; + Viết mã nguồn Lambda function (Python/Node.js) để tương tác với DynamoDB <br>&emsp; + Cấu hình IAM Role cấp quyền thực thi cho Lambda function an toàn | 26/05/2026 | 26/05/2026 | <https://000078.awsstudygroup.com/> |
| 4 | - **Lab:** Triển khai Serverless Backend (Phần 2: Tích hợp sự kiện) <br>&emsp; + Cấu hình S3 Event Notifications để kích hoạt (trigger) Lambda tự động <br>&emsp; + Kiểm thử luồng dữ liệu liên hoàn: Upload S3 -> Lambda -> lưu log vào DynamoDB <br>&emsp; + Đọc và phân tích log hệ thống bằng dịch vụ Amazon CloudWatch Logs | 27/05/2026 | 27/05/2026 | <https://000078.awsstudygroup.com/> |
| 5 | - Nghiên cứu thiết kế REST API và cấu hình nâng cao trên API Gateway <br>&emsp; + Ôn tập tiêu chuẩn thiết kế RESTful API (Methods: GET, POST, PUT, DELETE) <br>&emsp; + Khảo sát cấu hình Resource, Method và Integration Request trong API Gateway <br>&emsp; + Tìm hiểu về cơ chế CORS (Cross-Origin Resource Sharing) và phân quyền API | 28/05/2026 | 28/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 6 | - **Lab:** Xây dựng Serverless APIs hoàn chỉnh <br>&emsp; + Khởi tạo REST API mới trên API Gateway và định nghĩa cấu trúc tài nguyên <br>&emsp; + Liên kết các endpoints API (GET/POST) đến các Lambda functions tương ứng <br>&emsp; + Thực hiện Deploy API lên môi trường (Stage) và dùng Postman/cURL để kiểm thử | 29/05/2026 | 29/05/2026 | <https://000066.awsstudygroup.com/> |

### Kết quả đạt được tuần 6:

* Thấu hiểu toàn diện luồng xử lý request theo kiến trúc hiện đại: Client -> API Gateway -> AWS Lambda -> Database.
* Hoàn thành xuất sắc việc triển khai một Serverless Backend thực tế, kết hợp trơn tru hệ sinh thái dịch vụ S3, Lambda và DynamoDB.
* Đủ khả năng tự thiết kế và xuất bản một bộ RESTful API an toàn, có tính sẵn sàng cao thông qua API Gateway.
* Làm chủ kỹ năng cấu hình IAM Roles chuyên biệt (Least Privilege) cho từng hàm Lambda để đảm bảo an ninh thông tin.
* Biết cách sử dụng CloudWatch để giám sát, phân tích log và khắc phục sự cố (troubleshooting) trong môi trường phân tán.
