---
date: 2019-01-25
title: WHM Control Panel tại Cloud365
categories:
  - cloud-app
description: Giới thiệu về ứng dụng WHM Control Panel trong cloud365
type: Document
---
## 1. Giới thiệu WHM và CPanel trên Cloud365

![whm](/images/img-whm-cpanel/11.png)

Đối với những Webmaster của một website bất kỳ phải dùng những công cụ của nhà cung cấp host để quản lý website của mình như: thêm domain, upload file, quản lý cơ sở dữ liệu, FTP, làm mail server, quản lí mật khẩu, các trang báo lỗi…..những công cụ đó gọi là Web Host Manager (WHM) và cPanel là một trong những WHM tốt nhất được biết đến, dễ sử dụng,linh hoạt cho tất cả mọi người từ quản trị website cho đến người quản trị máy chủ và có rất nhiều tính năng tiện dụng khác mà bạn có thể thực hiện một cách nhanh chóng , an toàn.

### WHM là gì?

WebHostManager (WHM) là một trong một hệ thống cho phép bạn quản lý đơn giản tất cả những gì trên máy chủ Web của bạn, giao diện dễ sử dụng cung cấp cho khách hàng những tiện ích mạnh mẽ nhất để kiểm soát tất cả các chức năng. Hệ thống này cũng giúp bạn cập nhật thường xuyên những phiên bản mới nhất và nâng cao giúp hệ thống quản lý mạnh mẽ hơn.

### CPanel là gì?

cPanel là một giao diện web quản lý Hosting của khách hàng và là một trong những WHM tốt nhất được biết đến trên internet.

## 2. Các tính năng chính của WHM Control Panel

### THỐNG KÊ

- 3 chương trình thống kê: Webalizer Web Stats, AWStats, Analog Stats.
- Thống kê theo tên miền phụ.
- Xem danh sách 300 khách ghe thăm website gần nhất bao gồm thông tin: IP, thời gian và nơi truy cập, trình duyệt nào và hệ điều hành khách viếng thăm sử dụng.
- Xem băng thông đã sử dụng.
- Xem nhật ký lỗi của các ngôn ngữ web phục vụ cho công tác bảo trì và sửa lỗi.
- Xem nhật ký của dịch vụ Apache, có thể tải về.

### MAIL

- Quản lý các tài khoản, tạo, xáo trộn các tạo khoản POP3, thay đổi mật khẩu và định mức tài nguyên sử dụng.
- Cấu hình tự động hoặc hướng dẫn cấu hình bằng tay cho trình duyệt mail ở máy khách như Microsoft Outlook, Microsoft Outlook Express…
- Hệ thống trả lời tự động, bộ lọc, danh sách từ chối. tạo, xóa hoặc thay đổi.
- Bộ lọc Spam Assassin.
- Thay đổi bản ghi MX đối với mỗi tên miền.
- 3 ứng dụng webmail

### FTP

- Tạo, xóa tài khoản FTP. Thay đổi mật khẩu và thư mục có thể truy cập với từng tài khoản.
- Quản lý truy cập nặc danh (anonymous access).
- Quản lý phiên làm việc FTP.
- Thay đổi thông điệp hiển thị trên nhật ký FTP.

### SAO LƯU

- Tạo các bản sao lưu của file và các CSDL, phục hồi file và CSDL trên máy chủ từ một bản sao lưu, ví dụ từ máy tính cá nhân của người dùng.

## 3. Dịch vụ WHM cPanel trên  <a href="https://nhanhoa.com/may-chu/may-chu-cloud-server.html" target="_blank">Cloud Nhân Hòa</a>.

Dịch vụ WHC Control Panel được tích hợp tự động vào Cloud Server của Nhân Hòa. Giờ đây với chỉ 1 click chuột, bạn đã có ngay dịch vụ WHM cPanel để sử dụng.

## 3.1. Đăng ký gói dùng WHM cPanel Cloud Server

![whm](/images/img-whm-cpanel/00.png)

Sau khi bạn lựa chọn cloud server có ứng dụng WHM cPanel và hoàn tất các thủ tục đăng ký, bạn sẽ nhận được thông tin quản trị cloud server, WHM cPanel qua email đăng ký của bạn.

Bạn kiểm tra email để lấy thông tin.

![whm](/images/img-whm-cpanel/01.png)

Đăng nhập vào <a href="https://portal.cloud365.vn/user/login/" target="_blank">Portal Cloud Nhân Hòa</a> để quản trị server.

![whm](/images/img-whm-cpanel/02.png)

## 3.2. Thực hiện setup WHM CPanel trên WEBGUI

Login vào giao diện WEBGUI theo thông tin từ email quản trị của Nhân Hòa.

![whm](/images/img-whm-cpanel/03.png)

Thực hiện setup với WHM Wizard. 

- Step 1 : Đồng ý với các điều khoản đặt ra. Chọn nút **Save and Go to Step 2**

![whm](/images/img-whm-cpanel/04.png)

- Step 2 : Điền thêm 3 thông tin sau :
	 
	 - Email contact
	 - Server name theo đúng chuẩn FQDN
	 - DNS thứ 2

Sau khi điền đủ các thông tin, chọn nút **Save and Go to Step 3**
	 
![whm](/images/img-whm-cpanel/05.png)

- Step 3 : Điền IP Public của VPS, chọn **Add** và **Go to Step 4**

![whm](/images/img-whm-cpanel/06.png)

- Step 4 : Giữ nguyên các giá trị và **Go to Step 5**

![whm](/images/img-whm-cpanel/07.png)

- Step 5: Giữ nguyên các cấu hình service mặc định và **Go to Step 6** 

![whm](/images/img-whm-cpanel/08.png)

- Step 6: Chọn Finish vào kết thúc quá trình setup

![whm](/images/img-whm-cpanel/09.png)

- Step 7 : Logout và đăng nhập lại để sử dụng WHM Cpanel

![whm](/images/img-whm-cpanel/10.png)

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`