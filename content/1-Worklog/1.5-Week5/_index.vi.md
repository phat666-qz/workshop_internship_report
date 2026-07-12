---
title: "Worklog Tuần 5"
date: 2026-07-05
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:

* Tìm hiểu nền tảng điện toán đám mây với máy chủ ảo Amazon EC2 và các khái niệm liên quan như AMI, Security Groups, Key Pairs.
* Tìm hiểu về cơ sở dữ liệu quan hệ được quản lý (Amazon RDS) và các chiến lược sao lưu, phục hồi dữ liệu.
* Nghiên cứu cơ chế Auto Scaling để mở rộng quy mô hệ thống tự động dựa trên tải thực tế của ứng dụng.
* Nắm bắt nguyên lý hoạt động của Elastic Load Balancing (ELB) nhằm phân phối lưu lượng và đảm bảo tính sẵn sàng cao (High Availability).
* Thực hành triển khai một kiến trúc ứng dụng cơ bản kết hợp giữa EC2 (Compute) và RDS (Database) theo chuẩn AWS.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Nghiên cứu về nền tảng Amazon EC2 <br>&emsp; + Phân loại và lựa chọn các Instance Types phù hợp với workload <br>&emsp; + Khảo sát khái niệm AMI (Amazon Machine Image) và quy trình khởi tạo <br>&emsp; + Tìm hiểu vòng đời (Lifecycle) của EC2 và các mô hình mua (Purchasing options) | 18/05/2026 | 18/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - Khảo sát dịch vụ cơ sở dữ liệu quan hệ Amazon RDS <br>&emsp; + Phân tích kiến trúc triển khai Multi-AZ để đảm bảo Disaster Recovery <br>&emsp; + Tìm hiểu cơ chế Read Replica giúp giảm tải truy vấn đọc cho Database chính <br>&emsp; + Đánh giá các engine cơ sở dữ liệu hỗ trợ bởi RDS (MySQL, PostgreSQL, Aurora) | 19/05/2026 | 19/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 4 | - Nghiên cứu cơ chế Elastic Load Balancing và Auto Scaling <br>&emsp; + Phân tích thuật toán phân phối tải của Application Load Balancer (ALB) <br>&emsp; + Khảo sát cấu hình Launch Template và Auto Scaling Groups (ASG) <br>&emsp; + Xây dựng chiến lược scale-out và scale-in tự động dựa trên CloudWatch metrics | 20/05/2026 | 20/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - **Lab:** Thực hành Compute Essentials với Amazon EC2 <br>&emsp; + Triển khai máy chủ ảo Linux EC2, thiết lập Security Group và kết nối SSH <br>&emsp; + Cài đặt web server (Apache/Nginx) thông qua User Data script tự động <br>&emsp; + Giám sát tài nguyên và thử nghiệm thay đổi trạng thái instance (Stop/Terminate) | 21/05/2026 | 21/05/2026 | <https://000004.awsstudygroup.com/> |
| 6 | - **Lab:** Thực hành Database Essentials với Amazon RDS <br>&emsp; + Khởi tạo một RDS instance với engine MySQL trong Private Subnet an toàn <br>&emsp; + Cấu hình Security Group cho phép EC2 kết nối an toàn đến RDS <br>&emsp; + Thực hiện các thao tác quản trị cơ bản: Backup tự động và Snapshot thủ công | 22/05/2026 | 22/05/2026 | <https://000005.awsstudygroup.com/> |

### Kết quả đạt được tuần 5:

* Thành thạo quy trình cấp phát, cấu hình và quản trị vòng đời của máy chủ ảo EC2 trên nền tảng AWS.
* Triển khai thành công dịch vụ Amazon RDS, hiểu rõ cách cấu hình mạng lưới và bảo mật để bảo vệ cơ sở dữ liệu.
* Hiểu tư duy thiết kế hệ thống khả dụng cao (High Availability) thông qua việc kết hợp giữa ELB và Auto Scaling.
* Nắm vững kỹ năng sử dụng User Data để tự động hóa quá trình bootstrap các dịch vụ web trên EC2 instance.