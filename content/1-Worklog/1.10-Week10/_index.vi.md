---
title: "Worklog Tuần 10"
date: 2026-07-05
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu tuần 10:

* Tối ưu hóa quy trình tải lên tệp tin (File Upload), chuyển đổi toàn bộ luồng xử lý upload file tĩnh (như avatar, ảnh lớp học) từ việc gửi trực tiếp qua backend server sang sử dụng kiến trúc S3 Upload Bucket kết hợp với Presigned URL nhằm giảm tải băng thông cho server.
* Bóc tách tính năng import đề thi từ file Word (.docx) vốn tiêu tốn nhiều tài nguyên xử lý thành một luồng chạy ngầm riêng biệt.
* Xây dựng và cấu hình hàm Lambda để đảm nhiệm vai trò import Word (Lambda Import Word Processor), hoạt động theo cơ chế event-driven (kích hoạt khi có file upload lên S3).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu về kiến trúc và cách thức hoạt động của Presigned URL trên AWS S3.<br>&emsp; + Thiết lập kịch bản cấp phát URL có giới hạn thời gian từ Node.js (AWS SDK).<br>&emsp; + Cấu hình IAM Role và Policy an toàn, cho phép Backend sinh URL hợp lệ.<br>&emsp; + Điều chỉnh cài đặt CORS trên bucket S3 để frontend có quyền PUT trực tiếp. | 22/06/2026 | 22/06/2026 | |
| 4 | - Tối ưu lại các API liên quan đến thao tác cập nhật hình ảnh.<br>&emsp; + Test luồng upload avatar của người dùng với Presigned URL, đảm bảo file upload đúng định dạng.<br>&emsp; + Test luồng upload ảnh bìa cho lớp học, kiểm tra việc xử lý khi tệp có kích thước lớn.<br>&emsp; + Xử lý lỗi (Error handling) ở frontend khi Presigned URL hết hạn hoặc bị từ chối truy cập. | 24/06/2026 | 24/06/2026 | |
| 6 | - Giám sát và gỡ lỗi (Monitoring & Debugging) cho Lambda function thông qua CloudWatch.<br>&emsp; + Theo dõi luồng thực thi (execution stream) của Lambda Import Word Processor trên CloudWatch Logs.<br>&emsp; + Kiểm tra log khi upload file .docx hợp lệ: bóc tách text, image, lưu DB thành công.<br>&emsp; + Kiểm tra log với file không hợp lệ (sai định dạng, file hỏng): đảm bảo throw lỗi chính xác, không gây crash function. | 26/06/2026 | 26/06/2026 | |

### Kết quả đạt được tuần 10:

* Toàn bộ luồng upload chính (ảnh đại diện, ảnh lớp) đã hoạt động trơn tru qua presigned URL. Dữ liệu được lưu trữ đúng cấu trúc thư mục (prefix) trên S3.
* Hệ thống backend API không còn phải chịu tải từ việc truyền nhận file trung gian (multipart/form-data), tiết kiệm CPU và bộ nhớ.
* Lambda Import Word đã được kích hoạt thành công, có khả năng parse (phân tích cú pháp) cấu trúc file .docx phức tạp và trích xuất dữ liệu thô chuẩn xác.
* Hàm Lambda đã có thể mở kết nối tới MongoDB, chuyển đổi dữ liệu thô và lưu trữ các câu hỏi dạng trắc nghiệm/tự luận vào database.
* Các lỗi phát sinh trong quá trình Lambda chạy đã được log chi tiết lên CloudWatch.
