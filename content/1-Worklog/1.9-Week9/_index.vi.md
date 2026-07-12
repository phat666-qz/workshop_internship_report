---
title: "Worklog Tuần 9"
date: 2026-07-05
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Xác định phạm vi phát triển sản phẩm khả thi tối thiểu (MVP) cho dự án Examora, đảm bảo tập trung vào các tính năng cốt lõi có giá trị cao nhất.
* Tiến hành rà soát (code review) mã nguồn Frontend và Backend hiện tại để chuẩn bị cho quá trình chuyển đổi kiến trúc mượt mà.
* Chốt thiết kế kiến trúc hệ thống lai (AWS Serverless Hybrid Architecture), tận dụng linh hoạt giữa hạ tầng truyền thống và các dịch vụ quản lý trên AWS.
* Triển khai giải pháp xác thực và phân quyền toàn diện bằng Amazon Cognito kết hợp với dịch vụ gửi email tự động Amazon SES.
* Đóng gói và đưa ứng dụng Express Backend hiện tại lên môi trường AWS Lambda, đồng thời thiết lập API Gateway JWT Authorizer để bảo vệ nghiêm ngặt các API Endpoints.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Định hướng phạm vi MVP và Kiến trúc <br> - **Chi tiết:** <br>&emsp; + Phân tích yêu cầu nghiệp vụ để giới hạn các tính năng MVP thiết yếu (Đăng nhập, Quản lý hồ sơ, Làm bài thi). <br>&emsp; + Đánh giá source code Node.js/Express hiện hữu, cô lập các module phụ thuộc để dễ dàng container hóa hoặc serverless hóa. <br>&emsp; + Thống nhất bản thiết kế kiến trúc AWS Serverless Hybrid, lập sơ đồ tương tác giữa VPC nội bộ và các dịch vụ Public. | 15/06/2026 | 15/06/2026 | |
| 3 | - Tự học nhóm dịch vụ Monitoring <br> - **Thực hành:** <br>&emsp; + Nghiên cứu chuyên sâu về CloudWatch Logs để thiết lập cơ chế giám sát log tập trung cho môi trường Production. <br>&emsp; + Khảo sát cấu trúc log đặc thù của hàm AWS Lambda, bao gồm các thông số thời gian khởi tạo (Cold Start), thời gian thực thi (Duration) và bộ nhớ tiêu thụ (Billed Duration). <br>&emsp; + Viết các câu truy vấn Log Insights để lọc nhanh các lỗi Exception từ mã nguồn Node.js. | 16/06/2026 | 16/06/2026 | |
| 4 | - Chuẩn bị kịch bản kiểm thử (Test Cases) <br> - **Chi tiết:** <br>&emsp; + Lập danh sách các luồng màn hình chính (Main Flows) trên Frontend cần được kiểm duyệt sau khi thay thế hệ thống Auth cũ bằng Cognito. <br>&emsp; + Định nghĩa các kịch bản kiểm thử biên (Edge cases) cho quá trình cấp phát, hết hạn và làm mới JWT token. <br>&emsp; + Phác thảo bộ dữ liệu mẫu (Mock data) cho các nhóm người dùng khác nhau để đánh giá rủi ro bảo mật trước khi tích hợp. | 17/06/2026 | 17/06/2026 | |
| 5 | - Tích hợp và kiểm thử xác thực Cognito <br> - **Thực hành:** <br>&emsp; + Tích hợp SDK AWS Amplify hoặc thư viện AWS Cognito Identity vào ứng dụng Frontend chạy trên môi trường Local. <br>&emsp; + Thực thi toàn bộ luồng đăng nhập (Sign-in), đăng xuất (Sign-out), và khôi phục mật khẩu (Forgot Password). <br>&emsp; + Bắt và ghi nhận các ngoại lệ (Exceptions) liên quan đến Token validation, Session timeout nhằm điều chỉnh mã nguồn xử lý lỗi phía Client. | 18/06/2026 | 18/06/2026 | |
| 6 | - Kiểm thử phân quyền nhóm người dùng (User Groups) <br> - **Thực hành:** <br>&emsp; + Thực hiện mô phỏng quy trình nâng cấp quyền hạn từ nhóm `STUDENT` sang nhóm `TEACHER` trực tiếp trên Amazon Cognito Console. <br>&emsp; + Xây dựng cơ chế webhook hoặc Lambda Trigger để đồng bộ hóa trạng thái role của người dùng mới sang collection `giaovien` trong cơ sở dữ liệu MongoDB. <br>&emsp; + Kiểm chứng tính toàn vẹn dữ liệu: đảm bảo token mới sinh ra chứa đúng thông tin group và API Backend phản hồi chính xác dựa trên role. | 19/06/2026 | 19/06/2026 | |

### Kết quả đạt được tuần 9:

* Nắm bắt cấu trúc mã nguồn liên kết giữa frontend và backend, phân định rõ các module logic cần giữ lại và các thành phần cần tái cấu trúc (refactor) lên AWS.
* Triển khai hoàn chỉnh và bảo mật luồng đăng ký người dùng, tích hợp thành công gửi mã OTP qua email (Amazon SES) và quy trình xác thực đa nền tảng.
* Đồng bộ hóa mượt mà hồ sơ người dùng (User Profiles) giữa Amazon Cognito và cơ sở dữ liệu MongoDB truyền thống, đảm bảo tính nhất quán của dữ liệu.
* Di chuyển thành công nền tảng Backend API lên AWS Lambda, tận dụng tính linh hoạt và khả năng tự động mở rộng vô hạn của kiến trúc Serverless.
* Hoàn tất quá trình tích hợp API Gateway với cấu hình JWT Authorizer, xác lập hàng rào bảo mật tối ưu kiểm soát toàn bộ lưu lượng truy cập từ Frontend.