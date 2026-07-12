---
title: "Worklog Tuần 8"
date: 2026-07-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu tuần 8:

* Hoàn thiện kiến trúc giao tiếp mượt mà giữa Frontend và hệ thống API Serverless, đảm bảo hiệu năng và tính bảo mật cao.
* Nắm vững Shared Responsibility Model của AWS để phân định rõ vai trò quản lý bảo mật giữa khách hàng và nhà cung cấp.
* Thiết lập khả năng truy vết và giám sát toàn diện thông qua việc thu thập, phân tích log của các dịch vụ đám mây (CloudTrail, CloudWatch).
* Nghiên cứu cơ chế kiểm toán tài nguyên tự động nhằm đánh giá mức độ tuân thủ cấu hình trên AWS (AWS Config).
* Lập lộ trình và kế hoạch triển khai ban đầu cho kiến trúc của dự án thực tế Examora.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Thực hành Lab Frontend <br> - **Thực hành:** <br>&emsp; + Tích hợp mã nguồn Frontend (React/Vue) với Amazon API Gateway, xử lý các phản hồi HTTP và CORS. <br>&emsp; + Đính kèm JWT Token từ Cognito vào header của các yêu cầu API để đảm bảo cơ chế xác thực an toàn tuyệt đối. <br>&emsp; + Xử lý các trạng thái lỗi phía client (401 Unauthorized, 403 Forbidden) và tối ưu hóa trải nghiệm người dùng (UX). | 08/06/2026 | 08/06/2026 | <https://000079.awsstudygroup.com/> |
| 3 | - Tìm hiểu bảo mật và giám sát <br> - **Chi tiết:** <br>&emsp; + Phân tích Mô hình Trách nhiệm Chia sẻ (Shared Responsibility Model), làm rõ trách nhiệm bảo vệ dữ liệu ở tầng ứng dụng. <br>&emsp; + Khám phá Amazon CloudTrail để theo dõi và ghi nhận lịch sử các lời gọi API diễn ra trong tài khoản AWS. <br>&emsp; + Xây dựng kịch bản kiểm toán bảo mật dựa trên nhật ký CloudTrail nhằm phát hiện các hành vi bất thường. | 09/06/2026 | 09/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 4 | - Tìm hiểu CloudWatch <br> - **Chi tiết:** <br>&emsp; + Thiết lập không gian giám sát thông qua CloudWatch Metrics, thu thập chỉ số hiệu suất của EC2, Lambda và DynamoDB. <br>&emsp; + Cấu hình CloudWatch Alarms để tự động cảnh báo (qua SNS) khi tài nguyên vượt quá ngưỡng giới hạn chỉ định. <br>&emsp; + Thu thập, lưu trữ và phân tích log hệ thống bằng CloudWatch Logs, sử dụng Log Insights để truy vấn dữ liệu theo thời gian thực. | 10/06/2026 | 10/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - Tìm hiểu AWS Config <br> - **Chi tiết:** <br>&emsp; + Khởi tạo AWS Config để ghi lại cấu hình lịch sử của các tài nguyên AWS đang hoạt động trong hệ thống. <br>&emsp; + Đánh giá mức độ tuân thủ hạ tầng bằng cách triển khai các quy tắc AWS Config Rules (Config Managed Rules). <br>&emsp; + Phân tích quy trình khắc phục tự động (Remediation) đối với các tài nguyên không tuân thủ chính sách bảo mật. | 11/06/2026 | 11/06/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 6 | - Lập kế hoạch dự án <br> - **Chi tiết:** <br>&emsp; + Tổng hợp các kỹ năng Serverless và Bảo mật đã học để thiết kế kiến trúc cấp cao cho dự án Examora. <br>&emsp; + Xác định phạm vi tính năng (MVP - Minimum Viable Product), lên danh sách các dịch vụ AWS cốt lõi sẽ áp dụng. <br>&emsp; + Xây dựng roadmap phân chia công việc chi tiết cho các tuần tiếp theo, phân bổ tài nguyên và thời gian hợp lý. | 12/06/2026 | 12/06/2026 | |

### Kết quả đạt được tuần 8:

* Xây dựng thành công kênh giao tiếp tin cậy giữa Frontend và Backend Serverless, tích hợp chuẩn xác luồng xác thực Cognito.
* Thiết lập thành công quy trình cảnh báo lỗi hệ thống qua CloudWatch và SNS.
* Có khả năng truy vết, kiểm toán lịch sử thay đổi cấu hình hạ tầng bằng CloudTrail và AWS Config để đảm bảo tuân thủ tiêu chuẩn.
* Hoàn tất lập kế hoạch triển khai dự án Examora.
