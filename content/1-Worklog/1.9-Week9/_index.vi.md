---
title: "Worklog Tuần 9"
date: 2026-07-05
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu:
* Định hướng phạm vi MVP, rà soát source code hiện tại và chốt kiến trúc AWS Serverless Hybrid cho Examora.
* Triển khai xác thực bằng Cognito/SES, đưa Express backend lên Lambda và bảo vệ API bằng API Gateway JWT Authorizer.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| Thứ 2 | - Định hướng phạm vi MVP, rà soát source code hiện tại và chốt kiến trúc AWS Serverless Hybrid. | 15/06/2026 | 15/06/2026 | |
| Thứ 3 | - Tự học nhóm dịch vụ Monitoring, tập trung vào CloudWatch Logs và cách đọc log Lambda. | 16/06/2026 | 16/06/2026 |  |
| Thứ 4 | - Chuẩn bị danh sách màn hình chính cần test sau khi chuyển xác thực sang Cognito. | 17/06/2026 | 17/06/2026 | |
| Thứ 5 | - Test login/logout bằng Cognito trên frontend local và ghi nhận lỗi token/session nếu có. | 18/06/2026 | 18/06/2026 |  |
| Thứ 6 | - Test đổi group STUDENT sang TEACHER trên Cognito và kiểm tra role MongoDB được sync sang giaovien. | 19/06/2026 | 19/06/2026 | |

### Kết quả đạt được:
* Nắm được cấu trúc frontend/backend, xác định các module giữ lại, các module cần chuyển sang AWS.
* Hoàn thành luồng đăng ký, OTP email, login, sync profile MongoDB, Lambda Backend API và test API Gateway cơ bản.
