---
title: "Worklog Tuần 4"
date: 2026-07-05
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Khảo sát chuyên sâu các khái niệm và dịch vụ lưu trữ cốt lõi trên nền tảng AWS, bao gồm Amazon S3, Amazon EBS và Amazon EFS.
* Phân tích và đánh giá sự khác biệt giữa các mô hình lưu trữ Object Storage, Block Storage và File Storage nhằm lựa chọn giải pháp tối ưu.
* Thực hành triển khai và quản trị lưu trữ Object với dịch vụ Amazon S3, áp dụng linh hoạt các phân lớp lưu trữ (Storage Classes).
* Xây dựng giải pháp Static Website Hosting trên Amazon S3, kết hợp cấu hình phân quyền bảo mật truy cập.
* Nắm bắt quy trình gán tên miền (Domain Mapping) cơ bản và thiết lập các chính sách Bucket Policy bảo vệ tài nguyên an toàn.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nghiên cứu về dịch vụ lưu trữ Object Amazon S3 <br>&emsp; + Phân tích kiến trúc lưu trữ dạng đối tượng và tính năng nổi bật của S3 <br>&emsp; + So sánh chi phí, hiệu suất của các phân lớp lưu trữ (Standard, IA, Glacier) <br>&emsp; + Thiết lập và kiểm thử các tập luật truy cập bằng Bucket Policy | 11/05/2026 | 11/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - Tìm hiểu lý thuyết hệ thống lưu trữ Block (EBS) và File (EFS) <br>&emsp; + Phân biệt đặc tính kỹ thuật giữa Block Storage và File Storage <br>&emsp; + Phân tích các trường hợp sử dụng tối ưu cho EC2 khi kết hợp cùng EBS và EFS <br>&emsp; + Tìm hiểu quy trình Snapshot và cơ chế sao lưu dữ liệu | 12/05/2026 | 12/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 4 | - Chuẩn bị dữ liệu và khởi tạo hạ tầng Amazon S3 Bucket <br>&emsp; + Chuẩn bị và kiểm tra bộ source code HTML/CSS/JS cho website tĩnh <br>&emsp; + Thực hiện khởi tạo S3 Bucket với các thiết lập bảo mật cơ bản <br>&emsp; + Kích hoạt tính năng Static Website Hosting và thiết lập trang mặc định | 13/05/2026 | 13/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - **Lab:** Triển khai Static Website Hosting trên nền tảng Amazon S3 <br>&emsp; + Thực hành upload toàn bộ thư mục mã nguồn lên S3 Bucket an toàn <br>&emsp; + Cấu hình tệp chính sách JSON cho phép quyền truy cập công khai cần thiết <br>&emsp; + Kiểm tra và khắc phục lỗi phân quyền để website hoạt động ổn định | 14/05/2026 | 14/05/2026 | <https://000057.awsstudygroup.com/> |
| 6 | - Nghiên cứu quy trình map domain và bảo mật nâng cao S3 bucket <br>&emsp; + Tìm hiểu quy trình kết nối Custom Domain Name cho S3 Website <br>&emsp; + Áp dụng các nguyên tắc bảo mật tối thiểu (Principle of Least Privilege) <br>&emsp; + Đánh giá hiệu năng lưu trữ và tổng kết kiến thức của tuần | 15/05/2026 | 15/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |

### Kết quả đạt được tuần 4:

* Nắm vững kiến trúc và tính năng của các dịch vụ lưu trữ AWS (S3, EBS, EFS), giải thích rõ ràng các ưu và nhược điểm.
* Phân biệt chính xác giữa Block Storage, File Storage và Object Storage, tự tin đề xuất giải pháp lưu trữ phù hợp cho dự án.
* Cấu hình thành công Bucket S3 với các chính sách phân quyền chi tiết (Bucket Policy) để kiểm soát nghiêm ngặt quyền truy cập.
* Hoàn thành bài thực hành triển khai một website tĩnh hoàn chỉnh lên Amazon S3, cho phép người dùng truy cập trực tiếp qua internet.
* Áp dụng thành thạo các phương pháp bảo mật cơ bản cho S3 bucket và hiểu cách thức định tuyến tên miền tuỳ chỉnh.
