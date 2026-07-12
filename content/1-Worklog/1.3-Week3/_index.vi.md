---
title: "Worklog Tuần 3"
date: 2026-07-05
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:

* Nắm vững các khái niệm cốt lõi về mạng lưới điện toán đám mây riêng ảo thông qua Amazon Virtual Private Cloud (VPC).
* Phân tích cấu trúc địa chỉ IP, cách chia nhỏ mạng (Subnetting) và ứng dụng của Classless Inter-Domain Routing (CIDR).
* Triển khai và cấu hình các thành phần định tuyến như Route Tables và Internet Gateways (IGW) để kết nối mạng internet.
* Đánh giá và thiết lập các lớp bảo mật mạng đa tầng, kết hợp hiệu quả giữa Security Groups (Stateful) và Network ACLs (Stateless).
* Khám phá các tính năng mạng nâng cao như VPC Peering, VPC Endpoints và giám sát lưu lượng bằng VPC Flow Logs.
* Thực hành tự xây dựng một kiến trúc mạng VPC hoàn chỉnh, đảm bảo tính kết nối và bảo mật chặt chẽ.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Lý thuyết nền tảng về Amazon VPC <br>&emsp; + Tìm hiểu về IP với CIDR block và phân chia Subnet (Public/Private) <br>&emsp; + Tìm hiểu vai trò của Internet Gateway (IGW) trong việc cấp quyền truy cập internet | 04/05/2026 | 04/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 3 | - **Lab:** Thực hành Networking Essentials with Amazon Virtual Private Cloud (VPC) <br>&emsp; + Khởi tạo một VPC tùy chỉnh với không gian địa chỉ mạng riêng biệt <br>&emsp; + Cấu hình các Subnets và đính kèm Internet Gateway | 05/05/2026 | 05/05/2026 | <https://000003.awsstudygroup.com/> |
| 4 | - Tìm hiểu lý thuyết về bảo mật tầng mạng (Network Security) <br>&emsp; + So sánh cơ chế hoạt động của Security Group (tường lửa cấp instance, Stateful) <br>&emsp; + Khảo sát Network Access Control Lists - NACL (tường lửa cấp subnet, Stateless) | 06/05/2026 | 06/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 5 | - Nghiên cứu lý thuyết về định tuyến mạng (Routing) <br>&emsp; + Cấu hình và quản lý Route Table để điều hướng luồng dữ liệu (traffic routing) <br>&emsp; + Khám phá cơ chế kết nối giữa các mạng ảo độc lập thông qua VPC Peering | 07/05/2026 | 07/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |
| 6 | - Tìm hiểu về VPC Endpoints và tối ưu hóa mạng <br>&emsp; + Tìm hiểu cách truy cập dịch vụ AWS nội bộ qua VPC Endpoints (Gateway & Interface) <br>&emsp; + Giám sát, gỡ lỗi mạng bằng VPC Flow Logs và ôn tập tổng thể luồng Network | 08/05/2026 | 08/05/2026 | <https://www.youtube.com/@AWSStudyGroup> |

### Kết quả đạt được tuần 3:

* Hiểu kiến trúc của một mạng ảo Amazon VPC, bao gồm cách thức các luồng dữ liệu (traffic) di chuyển vào, ra và bên trong mạng.
* Nắm vững kỹ thuật phân bổ IP (CIDR) và quy hoạch kiến trúc Subnet (Public/Private) phù hợp với từng nhu cầu triển khai ứng dụng.
* Phân biệt rõ ràng và vận dụng linh hoạt hai lớp bảo vệ mạng: Security Groups và Network ACLs để tối ưu hóa an ninh hệ thống.
