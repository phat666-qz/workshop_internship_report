---
title: "Worklog Tuần 11"
date: 2026-07-05
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:

* Tiến hành chia tách hoàn toàn logic chấm bài thi phức tạp ra khỏi request nộp bài của người dùng, giúp API chính chỉ làm nhiệm vụ ghi nhận.
* Ứng dụng AWS SQS (Simple Queue Service) để xây dựng Grading Queue, đóng vai trò là một bộ đệm (buffer) đáng tin cậy giữ các yêu cầu chấm bài.
* Xây dựng Lambda Grading Worker để xử lí các message từ SQS, thực hiện các phép toán chấm điểm một cách độc lập.
* Cập nhật trạng thái bài làm linh hoạt trong MongoDB để người dùng có thể theo dõi tiến độ chấm bài theo thời gian thực.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nghiên cứu và thiết kế kiến trúc xử lý bất đồng bộ (Asynchronous Architecture) cho hệ thống nộp bài thi.<br>&emsp; + Đánh giá ưu nhược điểm của AWS SQS so với các giải pháp queue khác cho bài toán cụ thể này.<br>&emsp; + Phác thảo sơ đồ luồng dữ liệu: Client -> API Gateway -> Backend -> SQS -> Lambda -> MongoDB.<br>&emsp; + Xác định cấu trúc payload chuẩn hóa cho các message đẩy vào hàng đợi SQS. | 29/06/2026 | 29/06/2026 | |
| 3 | - Triển khai và cấu hình hạ tầng AWS SQS Grading Queue trên môi trường cloud.<br>&emsp; + Cấu hình các tham số quan trọng: Visibility Timeout, Message Retention Period phù hợp với thời gian chạy của Lambda.<br>&emsp; + Tái cấu trúc API nộp bài (Submit Exam API): Ghi nhận submission với trạng thái "Đang chấm".<br>&emsp; + Lập trình chức năng đóng gói và đẩy message chứa thông tin bài thi vào SQS Queue từ Backend. | 30/06/2026 | 30/06/2026 | |
| 4 | - Xây dựng và lập trình Lambda Grading Worker đảm nhiệm việc tính điểm cốt lõi.<br>&emsp; + Tích hợp trigger từ SQS tới Lambda, cấu hình batch size phù hợp để tối ưu chi phí.<br>&emsp; + Viết logic so sánh câu trả lời của thí sinh với đáp án chuẩn, tính toán điểm số cuối cùng.<br>&emsp; + Khởi tạo kết nối tới MongoDB từ Lambda và thực hiện update document kết quả bài thi. | 01/07/2026 | 01/07/2026 | |
| 5 | - Thực hiện kiểm thử cho quy trình chấm bài tự động.<br>&emsp; + Sử dụng AWS Console hoặc CLI để gửi trực tiếp các SQS message với payload mẫu giả lập.<br>&emsp; + Theo dõi quá trình Lambda Grading Worker kích hoạt, xử lý message và ghi log.<br>&emsp; + Xác minh tính chính xác của điểm số và sự thay đổi trạng thái trong database MongoDB. | 02/07/2026 | 02/07/2026 | |
| 6 | - Tối ưu hóa quy trình quản lý lỗi trong Worker.<br>&emsp; + Khắc phục triệt để lỗi worker không nhận diện được model Mongoose khi khởi tạo kết nối database.<br>&emsp; + Bổ sung logic catch error khi quá trình chấm bài thất bại, đảm bảo cập nhật trạng thái bài làm thành "Lỗi chấm bài".<br>&emsp; + Ghi nhận toàn bộ thông tin lỗi chi tiết vào CloudWatch để phân tích và khắc phục. | 03/07/2026 | 03/07/2026 | |

### Kết quả đạt được tuần 11:

* Hệ thống backend đã tích hợp với AWS SQS. Mỗi bài thi nộp lên đều được mã hóa thành message và lưu trữ an toàn chờ xử lý, không bị mất dữ liệu.
* Lambda Grading Worker hoạt động ổn định, tự tự động nhận message từ queue, đối chiếu đáp án, tính toán điểm thi với độ chính xác tuyệt đối.
* Hệ thống đã kiểm soát tốt lifecycle của một bài nộp, từ trạng thái "Đang chấm" sang "Hoàn thành" hoặc "Lỗi", được cập nhật theo thời gian thực trên MongoDB.
* Các vấn đề phát sinh như thiếu context Mongoose model trong môi trường serverless đã được giải quyết, đảm bảo Worker không bị crash.
