---
title: "Worklog Tuần 2"
date: 2026-07-05
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Tìm hiểu về dịch vụ quản lý danh tính và quyền truy cập AWS Identity and Access Management (IAM).
* Phân biệt và ứng dụng hiệu quả các thành phần cốt lõi của IAM bao gồm Users, Groups, Roles và Policies.
* Triển khai nguyên tắc đặc quyền tối thiểu (Principle of Least Privilege) để đảm bảo an ninh cho tài khoản AWS.
* Nghiên cứu các phương pháp bảo mật tài khoản nâng cao như Multi-Factor Authentication (MFA) và AWS Security Token Service (STS).
* Khảo sát các khái niệm về quản lý chi phí, thanh toán (Cost Management & Billing) và giới hạn của AWS Free Tier.
* Thực hành thiết lập cảnh báo ngân sách (AWS Budgets) để chủ động kiểm soát chi phí phát sinh.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Phân tích lý thuyết tổng quan về dịch vụ IAM <br>&emsp; + Khảo sát chi tiết về IAM User, Group và cấu trúc của IAM Policy <br>&emsp; + Nghiên cứu cách áp dụng nguyên tắc đặc quyền tối thiểu (Least Privilege) | 27/04/2026 | 27/04/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - **Lab:** Thực hành Access Management with AWS Identity and Access Management (IAM) <br>&emsp; + Tạo và quản lý người dùng, nhóm người dùng trên giao diện IAM <br>&emsp; + Gắn các policy phân quyền tương ứng và kiểm thử mức độ truy cập | 28/04/2026 | 28/04/2026 | <https://000002.awsstudygroup.com/> |
| 4 | - Nghiên cứu lý thuyết IAM nâng cao <br>&emsp; + Tìm hiểu cơ chế hoạt động của IAM Role và Temporary Credentials qua STS <br>&emsp; + Triển khai Multi-Factor Authentication (MFA) và các Best Practices bảo mật | 29/04/2026 | 29/04/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - Phân tích lý thuyết về quản lý chi phí AWS <br>&emsp; + Khảo sát các công cụ Cost Management, Cost Explorer và Billing Dashboard <br>&emsp; + Tìm hiểu chi tiết các giới hạn dịch vụ trong chương trình AWS Free Tier | 30/04/2026 | 30/04/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 6 | - **Lab:** Thực hành Managing Costs with AWS Budgets <br>&emsp; + Cấu hình một ngân sách (Budget) theo dõi chi phí hàng tháng <br>&emsp; + Thiết lập các ngưỡng cảnh báo (Alert Thresholds) gửi qua email | 01/05/2026 | 01/05/2026 | <https://000007.awsstudygroup.com/> |

### Kết quả đạt được tuần 2:

* Nắm vững toàn diện phương pháp quản lý danh tính, xác thực và phân quyền trên môi trường AWS thông qua dịch vụ IAM.
* Ứng dụng thành công nguyên tắc đặc quyền tối thiểu (Least Privilege), đảm bảo mỗi thực thể chỉ có quyền truy cập vừa đủ để thực thi công việc.
* Củng cố mức độ bảo mật của tài khoản AWS bằng cách triển khai MFA và nắm bắt cơ chế cấp quyền tạm thời của IAM Role.
* Thiết lập thành công AWS Budgets, tạo ra cơ chế giám sát và cảnh báo tự động, giúp phòng tránh triệt để tình trạng vượt chi (over-spending).
