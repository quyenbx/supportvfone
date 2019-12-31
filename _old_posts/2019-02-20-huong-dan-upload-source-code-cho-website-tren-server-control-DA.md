---
date: 2019-02-20
title: Hướng dẫn upload source code cho website trên server control Directadmin
categories:
  - cloud-app
description: Hướng dẫn upload source code cho website trên server control Directadmin
type: Document
---

DirectAdmin (hay gọi tắt là DA) là phần mềm quản lý hosting trên nhiều hệ điều hành Linux.

Có nhiều phần mềm quản lý hosting như Cpanel, Klolox, virtualmin… Trong đó DirectAdmin khá nhẹ, phù hợp nhiều cấu hình, ít chiếm tài nguyên, chức năng ít hơn Cpanel nên dễ sử dụng

## Phần 1: Thêm domain vào Directadmin 

Để thêm domain vào Directadmin chúng ta có thể thêm trực tiếp domain đó vào quản lý bởi user admin hoặc add thêm user khác để quản lý domain riêng theo từng user 

### 1. Thêm domain quản lý bởi user admin
Sau khi người dùng đăng ký sử dụng một VPS có cài đặt control Directadmin, người dùng sẽ nhận được thông tin quản trị của VPS trong đó có thông tin truy cập control Directadmin, giao diện sau khi đăng nhập Directadmin sẽ như ảnh bên dưới

![](/images/img-upload-code-DA/1.png)

Để thêm domain được quản lý bởi user admin chúng ta truy cập tới `User Level` theo ảnh bên dưới

![](/images/img-upload-code-DA/2.png)

Giao diện hiện ra ta tiếp tục thao tác theo ảnh bên dưới

![](/images/img-upload-code-DA/3.png)

Click vào `Add Another Domain` để add thêm domain

![](/images/img-upload-code-DA/4.png)

Giao diện hiện ra chúng ta nhập tên của domain muốn add vào 

![](/images/img-upload-code-DA/5.png)

Như vậy là chúng ta đã add xong domain quản lý bởi user admin

### 2. Thêm domain quản lý bởi 1 user bất kỳ

**2.1 Tạo package cho một gói hosting riêng**

Truy cập tới `Reseller Level` như ảnh bên dưới

![](/images/img-upload-code-DA/6.png)

Giao diện hiển ra ta Click vào `Add Package`

![](/images/img-upload-code-DA/7.png)

Chúng ta sẽ nhập các thông tin phù hợp cho một package theo gói cầu hình mong muốn, một số option cần quan tâm như BandWith, Disk Space, Domains, Sub-Domains, Email Accounts, Email Forwarders, MySQL Databases, Domain Pointers, Ftp Accounts, Package Name. Nếu không giới hạn thông số gói hosting chúng ta chọn Unlimited

![](/images/img-upload-code-DA/8.png)

<a name="thongtin"></a>
**2.2 Tạo một user mới**

Để tạo thêm một user mới gán theo package vừa tạo chúng ta thao tác như ảnh bên dưới

![](/images/img-upload-code-DA/9.png)

Ở giao diện hiện ta chúng ta cần nhập thông tin cho user, password , email, domain và tên package sẽ gán cho user đó.Lưu ý user này sẽ dùng để quản lý hosting và upload code

![](/images/img-upload-code-DA/10.png)

Để kiểm tra lại user và domain vừa add trên control Directadmin chúng ta thao tác như các ảnh bên dưới

![](/images/img-upload-code-DA/11.png)

![](/images/img-upload-code-DA/12.png)

## Phần 2: Upload code lên hosting

Có hai cách để upload code lên hosting

### 1. Upload code từ giao diện web Directadmin 

Chúng ta truy cập tới File Manager là thư mục quản lý source code của website

**1.1 Với domain được quản lý bởi user admin**

Chúng ta truy cập tới File Manager như ảnh bên dưới

![](/images/img-upload-code-DA/13.png)

**1.2 Với domain được quản lý bởi user bất kỳ**

Nếu chúng ta đang đăng nhập từ user admin thì chuyển qua truy cập với user bất kỳ như sau

![](/images/img-upload-code-DA/14.png)

![](/images/img-upload-code-DA/15.png)

![](/images/img-upload-code-DA/16.png)

Truy cập tới thư mục File Manager của user đó

![](/images/img-upload-code-DA/17.png)

**1.3 Upload Code**

Sau khi truy cập được tới `File Manager` chúng ta tìm tới đường dẫn chứa code của website để upload.Trong thư mục `File Manager` sẽ hiển thị như ảnh bên dưới

![](/images/img-upload-code-DA/18.png)

Đường dẫn truy cập tới thư mục chứa code của website sẽ được tìm tới theo các ảnh bên dưới

![](/images/img-upload-code-DA/19.png)

![](/images/img-upload-code-DA/20.png)

![](/images/img-upload-code-DA/21.png)

Thư mục `public_html` trong ảnh trên là thư mục chứa code của website.Sau khi click vào thư mục `Public_html` ta thao tác upload code như ảnh bên dưới

![](/images/img-upload-code-DA/22.png)

![](/images/img-upload-code-DA/23.png)

![](/images/img-upload-code-DA/24.png)

Như vậy là chúng ta đã upload file thành công.Để kiểm tra chúng ta quay lại thư mục `puclic_html` vừa truy cập sẽ thấy file cần upload đã tồn tại trong thư mục

![](/images/img-upload-code-DA/25.png)

### 2. Upload code bằng phần mềm Filezilla

Chúng ta nên dùng các phần mềm FTP để upload source code tránh trường hợp file code quá lớn khi upload bằng giao diện Directadmin sẽ bị timeout.Trong hướng dẫn này chúng tôi dùng phần mềm FTP là Filezilla

Download phần mềm filezilla <a href="https://filezilla-project.org/" target="_blank">tại đây</a>

Sau khi download và cài đặt xong filezilla trên máy tính cá nhân chúng ta mở phần mềm filezilla lên và nhập thông tin user FTP đã tạo ở [phần trước](#thongtin) để kết nối FTP tới server,hoặc truy cập bằng user admin trong trường hợp domain được quản lý bởi user admin, thao tác như ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/8.png)

![](/images/img-upload-code-cho-website-Plesk/9.png)

![](/images/img-upload-code-cho-website-Plesk/10.png)

Trong ảnh trên nhập các thông tin cần thiết như

```sh
Host: Địa chỉ IP của máy chủ
Protocol: FTP
Encryption: insecure 
Login Type: normal 
User: 
Password: 
```

Sau khi kết nối FTP thành công giao diện hiển thị như ảnh bên dưới

![](/images/img-upload-code-cho-website-Plesk/11.png)

Tiếp đến ta truy cập tới thư mục httpdocs chứa code của website trên server và thư mục chứa code muốn upload trên máy tính local

![](/images/img-upload-code-cho-website-Plesk/12.png)

![](/images/img-upload-code-cho-website-Plesk/13.png)

Click Chuột phải vào file muốn upload và click vào Upload để up file code lên server

![](/images/img-upload-code-cho-website-Plesk/14.png)

Kết quả sau khi upload file index.php như ví dụ trên chúng ta truy cập thử trình duyệt website và hiển thị nội dung như file index là thành công

![](/images/img-upload-code-DA/26.png)

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`




