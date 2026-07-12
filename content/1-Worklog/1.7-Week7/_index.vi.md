---
title: "Worklog Tuần 7"
date: 2026-07-05
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:

* Tìm hiểu về kiến trúc cơ sở dữ liệu NoSQL, tập trung vào khả năng mở rộng và hiệu suất truy vấn của Amazon DynamoDB.
* Phân tích các pattern thiết kế dữ liệu phi quan hệ (Partition key, Sort key, Global Secondary Indexes) để tối ưu hóa việc lưu trữ và truy xuất.
* Xây dựng nền tảng vững chắc về quản lý định danh người dùng (Identity Management) và xác thực ứng dụng trong môi trường đám mây.
* Đánh giá và thiết kế giải pháp phân quyền (Authorization) chi tiết cho các tài nguyên AWS dựa trên vai trò người dùng.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu NoSQL Database <br> - **Chi tiết:** <br>&emsp; + Phân tích đặc thù kiến trúc lưu trữ của Amazon DynamoDB so với RDBMS truyền thống. <br>&emsp; + Đánh giá chiến lược định tuyến dữ liệu, cơ chế phân tán phân vùng (partitioning) và ảnh hưởng đến hiệu suất đọc/ghi. <br>&emsp; + Nghiên cứu các khái niệm về Read/Write Capacity Units (RCU/WCU) và mô hình tính phí theo nhu cầu (On-Demand). | 01/06/2026 | 01/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - Thực hành Lab NoSQL Database <br> - **Thực hành:** <br>&emsp; + Khởi tạo và cấu hình bảng DynamoDB cơ bản, thiết lập Partition Key và Sort Key phù hợp với mẫu truy vấn. <br>&emsp; + Thao tác chèn, cập nhật và truy vấn dữ liệu (Query, Scan) thông qua AWS Management Console và AWS CLI. <br>&emsp; + Khảo sát và tối ưu hóa chi phí truy vấn dữ liệu lớn bằng cách giới hạn phạm vi quét (Filter Expressions). | 02/06/2026 | 02/06/2026 | <https://000060.awsstudygroup.com/> |
| 4 | - Giới thiệu xác thực người dùng <br> - **Chi tiết:** <br>&emsp; + Phân biệt rõ ràng giữa Xác thực (Authentication - AuthN) và Phân quyền (Authorization - AuthZ) trong bảo mật ứng dụng. <br>&emsp; + Khám phá kiến trúc Amazon Cognito: Cognito User Pools (quản lý thư mục người dùng) và Identity Pools (cung cấp AWS credentials). <br>&emsp; + Nghiên cứu luồng cấp phát token (Access Token, ID Token) theo chuẩn OAuth2.0/OIDC. | 03/06/2026 | 03/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - Thực hành Lab User Authentication (Phần 1) <br> - **Thực hành:** <br>&emsp; + Xây dựng và cấu hình Cognito User Pool, thiết lập các chính sách mật khẩu và xác thực đa yếu tố (MFA). <br>&emsp; + Triển khai quy trình đăng ký, xác nhận email/SĐT và đăng nhập cho người dùng cuối qua Cognito Hosted UI. <br>&emsp; + Tùy chỉnh các thuộc tính người dùng (Custom Attributes) nhằm lưu trữ dữ liệu cá nhân hóa. | 04/06/2026 | 04/06/2026 | <https://000081.awsstudygroup.com/> |
| 6 | - Thực hành Lab User Authentication (Phần 2) <br> - **Thực hành:** <br>&emsp; + Thiết lập Cognito Identity Pool để kết nối định danh người dùng với IAM Roles, cấp quyền truy cập tài nguyên AWS. <br>&emsp; + Tích hợp hệ thống phân quyền, cho phép người dùng đã xác thực (Authenticated) gọi trực tiếp API hoặc truy cập S3. <br>&emsp; + Kiểm thử bảo mật toàn diện các luồng token và mô phỏng tấn công từ chối truy cập trên các policy đã thiết lập. | 05/06/2026 | 05/06/2026 | <https://000081.awsstudygroup.com/> |

### Kết quả đạt được tuần 7:

* Thiết kế thành công các bảng DynamoDB đáp ứng độ trễ thấp.
* Triển khai hoàn chỉnh giải pháp quản lý người dùng tập trung bằng Amazon Cognito User Pools, hỗ trợ luồng đăng ký/đăng nhập mượt mà.
* Tích hợp thành công Cognito Identity Pools với AWS IAM, trao quyền truy cập tài nguyên an toàn cho người dùng cuối theo nguyên tắc đặc quyền tối thiểu.
* Xây dựng nền tảng vững chắc để áp dụng cơ chế xác thực dựa trên JWT (JSON Web Token) cho các ứng dụng Serverless trong những giai đoạn tiếp theo.
