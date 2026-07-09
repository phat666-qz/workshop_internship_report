---
title: "Worklog Tuần 11"
date: 2026-04-17
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu:
* Tách logic chấm bài khỏi request nộp bài bằng SQS Grading Queue và Lambda Grading Worker.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| Thứ 2 | - Thiết kế kiến trúc luồng xử lý bất đồng bộ với AWS SQS cho tính năng chấm bài thi. | 29/06/2026 | 29/06/2026 |  |
| Thứ 3 | - Triển khai AWS SQS Grading Queue và chỉnh sửa API nộp bài để đẩy message vào Queue. | 30/06/2026 | 30/06/2026 |  |
| Thứ 4 | - Viết Lambda Grading Worker đọc message từ SQS, tính điểm và cập nhật MongoDB. | 01/07/2026 | 01/07/2026 |  |
| Thứ 5 | - Test trực tiếp SQS message -> Lambda Grading Worker -> MongoDB result bằng payload mẫu. | 02/07/2026 | 02/07/2026 |  |
| Thứ 6 | - Ghi lại lỗi và cách xử lý khi worker thiếu model Mongoose hoặc không cập nhật trạng thái chấm bài. | 03/07/2026 | 03/07/2026 |  |

### Kết quả đạt được:
* Tách biệt thành công logic chấm bài, giảm tải cho API chính.
* Backend lưu bài làm với trạng thái đang chấm, gửi job vào SQS và worker xử lý chấm điểm/cập nhật kết quả về MongoDB.
