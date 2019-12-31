---
date: 2019-02-13
title: Hướng dẫn upload source code cho website trên server control Plesk
categories:
  - cloud-app
description: Hướng dẫn upload source code cho website trên server control Plesk
type: Document
---

Plesk (Plesk Control Panel) là một phần mềm dùng để quản lý hosting trong đó bao gồm các dịch vụ như Web service, Email service, DNS Service, SQL Service, PHP, ASP,... Plesk dành cho những nhà quản trị các dịch vụ như Web, Email, DNS, etc...với số lượng lớn website

## 1. Add thêm domain vào control Plesk

Chúng ta truy cập vào giao diên quản trị của Plesk từ trình duyệt website với các thông tin đăng nhập

Link: https://IP:8443 với IP là IP máy chủ của bạn
User: admin
Pass: Password của user admin

Khi chúng ta đăng nhập thành công giao diện hiển thị như ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/1.png)

Để add thêm 1 domain mới chúng ta click vào Add Domain như ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/2.png)

<a name="thongtin"></a>
Tiếp theo ta nhập các thông tin vào các trường cần thiết như ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/3.png)

Với các thông tin user và password vừa tạo ở bước trên chúng ta lưu lại để sử dụng kết nối FTP tới hosting

Sau khi đã add domain thành công chúng ta chuyển tới giao diện quản lý của domain vừa add thêm vào như ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/4.png)

Ở ảnh trên chúng ta truy cập tơi thư mục File Manager là thư mục chứa code của website vừa thêm vào

![](/images/img-upload-code-cho-website-Plesk/5.png)

## 2. Upload Code cho website

Có 2 cách để upload code lên thư mục chứa code của website trên VPS

Cách 1: Upload Source code từ giao diện control

Để upload Source Code từ control ta thao tác theo ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/6.png)

Sau khi click vào Upload chúng ta tìm tới đường dẫn chứa code lưu trên máy tính cá nhân và upload lên server

![](/images/img-upload-code-cho-website-Plesk/7.png)

Sau đó chúng ta thử truy cập website để kiểm tra kết quả

Cách 2: Upload Source Code từ phần mềm FTP như Filezilla 

Download phần mềm filezilla [tại đây](https://filezilla-project.org/)

Sau khi download và cài đặt xong filezilla trên máy tính cá nhân chúng ta mở phần mềm filezilla lên và nhập thông tin user FTP đã tạo ở [phần 1](#thongtin) để kết nối FTP tới server, thao tác như ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/8.png)

![](/images/img-upload-code-cho-website-Plesk/9.png)

![](/images/img-upload-code-cho-website-Plesk/10.png)

Trong ảnh trên nhập các thông tin cần thiết như

Host: Địa chỉ IP của máy chủ

Protocol: FTP

Encryption: insecure 

Login Type: normal 

User: 

Password: 

Sau khi kết nối FTP thành công giao diện hiển thị như ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/11.png)

Tiếp đến ta truy cập tới thư mục httpdocs chứa code của website trên server và thư mục chứa code muốn upload trên máy tính local

![](/images/img-upload-code-cho-website-Plesk/12.png)

![](/images/img-upload-code-cho-website-Plesk/13.png)

Click Chuột phải vào file muốn upload và click vào Upload để up file code lên server

![](/images/img-upload-code-cho-website-Plesk/14.png)

Như vậy là chúng ta đã upload thành công code của website lên server.Thông thường ngươi dùng lên sử dụng cách 2 để upload code lên server tránh trường hợp bị timeout khi upload quá nhiều file hoặc dung lượng  upload lớn

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`


