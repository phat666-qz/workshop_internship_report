---
title: "Worklog Tuần 12"
date: 2026-07-05
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu tuần 12:

* Đưa ứng dụng frontend lên môi trường bằng dịch vụ AWS Amplify Hosting, thiết lập luồng build và deploy tự động.
* Thiết lập và liên kết tên miền chính thức của dự án thông qua AWS Route 53, đảm bảo tính chuyên nghiệp và dễ nhớ cho người dùng cuối.
* Tổng hợp toàn bộ kiến trúc, vấn đề, giải pháp và ước tính chi phí để xây dựng bản Project Proposal hoàn chỉnh.
* Thực hiện kiểm thử lần cuối cho toàn bộ hệ thống trước khi nộp workshop.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu về AWS Amplify Hosting và cơ chế phục vụ ứng dụng Single Page Application (SPA).<br>&emsp; + Phân tích cách Amplify xử lý build spec và quản lý các biến môi trường (environment variables).<br>&emsp; + Thực hiện liên kết repository (GitHub/GitLab) với Amplify để kích hoạt luồng CI/CD.<br>&emsp; + Cấu hình file `amplify.yml` quy định các bước cài đặt dependencies, build và deploy cho dự án React. | 06/07/2026 | 06/07/2026 | |
| 3 | - Kiểm tra và xác minh quá trình deploy thủ công trên AWS Amplify Hosting.<br>&emsp; + Giám sát build logs trên console, đảm bảo quá trình sinh static file không xảy ra lỗi.<br>&emsp; + Thiết lập Custom Domain trên Route 53, trỏ bản ghi Alias/CNAME về ứng dụng Amplify.<br>&emsp; + Xác nhận tên miền chính thức `examora.click` truy cập ổn định, chứng chỉ SSL (HTTPS) được tự động cấp phát thành công. | 07/07/2026 | 07/07/2026 | |
| 4 | - Kiểm tra lại nội dung cho bản Proposal.<br>&emsp; + Trình bày rõ ràng bài toán thực tế (Vấn đề) và cách tiếp cận, tính năng hệ thống (Giải pháp).<br>&emsp; + Vẽ và mô tả chi tiết Sơ đồ Kiến trúc Tổng thể (System Architecture Diagram) sử dụng draw.io hoặc Lucidchart.<br>&emsp; + Sử dụng AWS Pricing Calculator để lập bảng ước tính chi phí vận hành hàng tháng sát với thực tế nhất. | 08/07/2026 | 08/07/2026 | |
| 5 | - Kiểm tra lại toàn bộ dự án và nội dung để làm báo cáo workshop.<br>&emsp; + Rà soát kịch bản test case, thực hiện test lại các luồng cốt lõi và hoàn thiện tài liệu kiểm thử cuối cùng.<br>&emsp; + Thiết kế slide thuyết trình, chắt lọc các điểm nhấn về mặt công nghệ (Serverless, SQS, S3 Presigned URL).<br>&emsp; + Kiểm tra chéo (Cross-check) nội dung Workshop Report, đảm bảo văn phong chuyên nghiệp và không sai sót kỹ thuật. | 09/07/2026 | 09/07/2026 | |

### Kết quả đạt được tuần 12:

* Ứng dụng web đã được host thành công trên AWS Amplify với tốc độ tải trang nhanh, luồng CI/CD tự động build khi có code mới.
* Truy cập hệ thống mượt mà thông qua tên miền tùy chỉnh `examora.click`, kết nối được bảo mật hoàn toàn bằng chuẩn HTTPS.
* Toàn bộ nội dung, kịch bản demo và báo cáo Workshop Report đã được chuẩn bị đầy đủ.
