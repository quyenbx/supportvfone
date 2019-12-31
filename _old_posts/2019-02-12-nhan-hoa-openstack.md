---
date: 2019-01-12
title: Giới thiệu về công nghệ ảo hóa OpenStack
categories:
  - cloud-server
description: Giới thiệu về công nghệ ảo hóa OpenStack triển khai cloud server tại cloud365
type: Document
---

Openstack là một công nghệ mới được Nhân Hòa sử dụng để xây dựng dịch vụ máy chủ ảo <a href="https://support.cloud365.vn/cloud-server/cloud-server-gioi-thieu/" target="_blank">Cloud Server</a>. Với mục đích để hỗ trợ mọi người tìm hiểu và tiếp cận được giải pháp này, Nhân Hòa sẽ chia sẻ những kiến thức sơ lược về Openstack và những đặc điểm ưu việt của nền tảng này.

## 1. OpenStack là gì?

Openstack là 1 platform mã nguồn mở dùng để triển khai điện toán đám mây, hỗ trợ cả private cloud lẫn public cloud. Nó cung cấp giải pháp xây dựng hạ tầng điện toán đám mây đơn giản, có khả năng mở rộng và nhiều tính năng phong phú. Openstack là một cloud software được thiết kế để chạy trên các sản phẩm phần cứng như x86, ARM. Nó không có yêu cầu gì về đặc tính phần mềm hay phần cứng, nó tích hợp với các hệ thống kế thừa và các sản phẩm bên thứ ba.

![](/images/img-cloud-server/04-cloudserver.png)

## 2. Kiến trúc của OpenStack

![](/images/img-cloud-server/00-cloudserver.png)

Kiến trúc tổng quan của OpenStack được chia thành 3 tầng 

- **Tầg ứng dụng (Your Application)** : Các ứng dụng/phần mềm sử dụng OpenStack
- **Tầng Hypervisor (Standard Hardware)** : Phần ứng máy chủ đã được ảo hóa để chia sẻ cho người dùng.
- **Dịch vụ OpenStack (Openstack Shared Services)** : Các thành phần cơ bản như Dashboard, Compute, Networking, API, Storage.

## 3. Mô hình  

#### Mô hình giải pháp

Điện toán đám mây OpenStack được các nhà cung cấp dịch vụ phát triển qua 3 giải pháp:

- IaaS (Infrastructure as a service): cung cấp/cho thuê cơ sở hạ tầng như thuê máy chủ...
- PaaS (Platform as a service): cung cấp nền tảng để phát triển ứng dụng
- SaaS (Software as a service): cung cấp khả năng truy cập phần mềm linh hoạt như HCM,CRM...

![](/images/img-cloud-server/01-cloudserver.png)

#### Mô hình triển khai 

Các mô hình triển khai OpenStack trên thực tế 

- Private Cloud: sử dụng trong một doanh nghiệp và không chia sẻ với bất kỳ ai nằm ngoài doanh nghiệp đóng
- Public Cloud: các dịch vụ trên nền tảng điện toán đám mây được dành cho cá nhân, tổ chức cùng thuê và sử dụng chung tài nguyên
- Hybrid Cloud: mô hình lai giữa public cloud và private cloud
- Community Cloud: các dịch vụ được các công ty cùng hợp tác xây dựng và cung cấp cho cộng đồng sử dụng

![](/images/img-cloud-server/02-cloudserver.png)

## 4. Các đặc điểm nổi bật

Với OpenStack, Cloud có khả năng phục vự và đáp ứng nhu cầu người dùng một cách toàn diện:

- Thời gian boot máy ảo, cài đặt cực kỳ nhanh chóng
- Giảm tối đa thời gian downtime
- Trang dashboard quản trị dễ dàng, thân thiện với người dùng
- Khả năng tự phục vụ - Khả năng truy cập hệ thống trên diện rộng 
- Tài nguyên được người dùng tự mua, lắp đặt và phân bổ theo nhu cầu
- Khả năng co dãn, đàn hồi của tài nguyên (nâng lên - hạ xuống CPU,RAM)
- Tự đo lường khả năng sử dụng dịch vụ bằng cách giám sát, dự phòng
- Khả năng phục hồi và sao lưu dữ liệu hoàn toàn tự động
- Tốc độ đọc dữ liệu vượt trội với ổ cứng SSD siêu tốc

## 5. Dịch vụ Cloud Openstack 365 ngày Uptime tại Nhân Hòa

Sau thời gian nghiên cứu triển khai, hệ thống cung cấp Cloud VPS/Cloud Server trên nền tảng Openstack của Nhân Hòa đã chính thức đi vào hoạt động với hiệu năng tốt hơn nhiều so với hệ thống cũ.

Hệ thống Cloud365 của Nhân Hòa cam kết các tính năng dịch vụ  : 

- Cam kết về tốc độ
- Cam kết chất lượng
- Đảm bảo an toàn
- Cảnh báo chủ động
- Hỗ trợ 24/7

![](/images/img-cloud-server/03-cloudserver.png)
