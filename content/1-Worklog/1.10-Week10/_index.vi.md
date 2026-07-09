---
title: "Worklog Tuần 10"
date: 2026-04-17
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu:
* Chuyển luồng upload file sang S3 Upload Bucket bằng presigned URL và tách import Word thành Lambda xử lý bất đồng bộ.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| Thứ 2 | - Tìm hiểu cách tạo và sử dụng Presigned URL trên AWS S3, cấu hình IAM role tương ứng. | 22/06/2026 | 22/06/2026 |  |
| Thứ 4 | - Test upload avatar và ảnh lớp sau khi frontend chuyển sang presigned URL. | 24/06/2026 | 24/06/2026 |  |
| Thứ 6 | - Kiểm tra CloudWatch Logs của Lambda Import Word Processor khi upload file .docx hợp lệ và không hợp lệ. | 26/06/2026 | 26/06/2026 |  |

### Kết quả đạt được:
* Presigned URL hoạt động cho các luồng upload chính, file được lưu đúng prefix S3.
* Lambda Import Word có thể parse file .docx và lưu câu hỏi vào MongoDB.
