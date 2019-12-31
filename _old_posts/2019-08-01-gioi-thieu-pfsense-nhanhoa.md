---
date: 2019-07-31
title: Sử dụng template firewall- Pfsense trên Cloud Nhân Hòa
categories:
  - cloud-app
description: Sử dụng template Pfsense trên Cloud Nhân Hòa
type: Document
---

## I. Giới thiệu về Pfsense

![](/images/img-pfsense/pfsense-05.png)

**Ffsense** là một dạng tường lửa mã nguồn mở hoàn toàn miễn phí, được triển khai dưới dạng phần mềm, đáp ứng được các tính năng quan trọng. thường chỉ xuất hiện tại các firewall thương mại lớn như Cisco ASA, Checkpoint, Juniper... Pfsense có một cộng đồng phát triển rất tích cực, các bản cập nhập được bổ sung thường xuyên, nhằm cải thiện hơn nữa tính bảo mật, sự ổn định và sự linh hoạt. 

Mô hình firewall pfsense thường được triển khai tại các hệ thống mạng vật lý, nhằm kiểm soát và cung cấp tính năng tới toàn bộ thiết bị mạng và máy chủ bên trong hệ thống. Một số đặc điểm nổi bật của Pfsense như : 
 - Hoàn toàn miễn phí.
 - Yêu cầu cấu hình server để cài đặt rất thấp. 
 - Giao diện người dùng GUI trên WEB dễ sử dụng.
 - Đóng vai trò như Router, hỗ trợ định tuyến hệ thống mạng.
 - Là tưởng lửa tại các layer 3, layer 4 và layer 7
 - VPN theo các giao thức : OpenVPN, IP-Sec, L2TP. PPTP.
 - Hỗ trợ giám sát / phân tích mạng
 - Quản lý tên miền (DC), hỗ trợ tên miền động (Dynamic DNS)
 - Hỗ trợ triển khai dạng high availability - failover.
 - Đóng vai trò làm DHCP server, replay.
 - Đóng vai trò làm DNS forwarder, resolver.
 - Đóng vai trò làm Load banlancer - cân bằng tải cho hệ thống.
 - Đóng vai trò làm NTP cho hệ thống.
 - Hỗ trợ wake-on-lan

## II. Sử dụng dịch vụ Pfsense, firewall as a service trên hệ thống Cloud Nhân Hòa. 

Hiện nay, người dùng đã có thể sử dụng dịch vụ firewall Pfsense trên hệ thống Cloud Nhân Hòa nhằm bảo vệ và cung cấp tính năng cho hệ thống máy ảo mình. Để sử dụng dịch vụ Pfsense - Firewall as a service. Người dùng có thể thực hiện bằng 2 cách.

### Cách 1 : Đăng ký mới sử dụng Pfsense Cloud365 

Truy cập tới trang https://nhanhoa.com và đăng ký máy ảo Pfsense. 

![](/images/img-pfsense/pfsense-00.png)

### Cách 2 : Chuyển đổi sử dụng Pfsense Cloud365 

Đối với những khách hàng đang sử dụng dịch cloud VPS nhưng đang là hệ điều hành trắng hoặc các dịch vụ khác thì có thể chủ động sử dụng tính năng rebuild trên portal quản trị, chọn rebuild với image Pfsense để sử dụng.

![](/images/img-pfsense/pfsense-01.png)

![](/images/img-pfsense/pfsense-04.png)


## III. Đăng nhập và sử dụng dịch vụ firewall Pfsense

Sau khi đăng ký sử dụng hoặc chuyển đổi thành công sang template Pfsense bạn sẽ nhận được thông tin đăng nhập VPS, thông tin đăng nhập Pfsense gửi vào email đăng ký của bạn.

![](/images/img-pfsense/pfsense-02.png)

Sử dụng thông tin để đăng nhập và trang quản trị của Pfsense. Kiểm tra thông tin và sử dụng các tính năng của Pfsense đối với hệ thống của mình.

![](/images/img-pfsense/pfsense-03.png)

Hãy theo dõi các bài viết tiếp theo của Cloud Team Nhân Hòa để tìm hiểu rõ hơn các vai trò quan trọng của Pfsense trong việc bảo vệ và cung cấp các tiện ích cho hệ thống của bạn.  

Xin cảm ơn !

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`