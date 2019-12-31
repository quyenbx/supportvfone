---
date: 2019-03-21
title: Hướng dẫn upload source code cho website trên server control WHM
categories:
  - cloud-app
description: Hướng dẫn upload source code cho website trên server control WHM
type: Document
---

WHM là tên viết tắt của Web Host Manager, đây là một chương trình có rất nhiều tính năng mạnh mẽ cho phép người quản trị truy cập tới những vị trí cuối cùng của cPanel Hosting. WHMCS quản lý tất cả từ việc quản lý Server, quản lý DNS tên miền, quản lý khách hàng, quản lý đơn hàng...


## 1. Tạo package trong WHM

Sau khi login vào WHM với thông tin
Link đăng nhập: https://IP:2087 (Với IP là IP của VPS)
user: root
pass: "pass của user root"

Khi đăng nhập thành công giao diện hiện ra như sau

![](/images/img-upload-code-WHM/login.png)

Chúng ta sẽ tiến hành tạo package cho hệ thống như ảnh bên dưới

![](/images/img-upload-code-WHM/pk1.png)

Trong giao diện trên chúng ta nhập đủ các thông tin cần thiết cho 1 package mà chúng ta muốn thiết lập vào click vào Add để hoàn thành tạo package

<a name="thongtin"></a>
## 2. Tạo user cho người dùng

Để tạo user cho người dùng chúng ta thao tác như ảnh bên dưới

![](/images/img-upload-code-WHM/user.png)

Sau khi nhập xong các thông tin cần thiết chúng ta click vào `Create` để hoàn thành tạo user

## 3. Truy cập vào giao diện người dùng để quản trị

Sau khi tạo user ở bước trên chúng ta truy cập trang quản lý WHM của user theo thông tin user và password vừa tạo với Link `https://IP:2083` Giao diện hiện ra như sau

![](/images/img-upload-code-WHM/user1.png)

### 3.1 Upload code trên giao diện Web

Cách này chỉ áp dụng với các file cần upload có dung lượng nhỏ. Trong ví dụ này sẽ hướng dẫn upload 1 file info.php , chúng ta thao tác như ảnh bên dưới

![](/images/img-upload-code-WHM/web1.png)

![](/images/img-upload-code-WHM/web2.png)

![](/images/img-upload-code-WHM/web3.png)

![](/images/img-upload-code-WHM/web4.png)

Sau bước trên chúng ta tìm tới đường dẫn chứa file cần upload và chọn `open` là upload được file

### 3.2 Upload code bằng phần mềm FTP 

Chúng ta nên dùng các phần mềm FTP để upload source code tránh trường hợp file code quá lớn khi upload bằng giao diện Directadmin sẽ bị timeout.Trong hướng dẫn này chúng tôi dùng phần mềm FTP là Filezilla

Download phần mềm filezilla <a href="https://filezilla-project.org/" target="_blank">tại đây</a>

Sau khi download và cài đặt xong filezilla trên máy tính cá nhân chúng ta mở phần mềm filezilla lên và nhập thông tin user đã tạo ở [phần trước](#thongtin) để kết nối FTP tới server, thao tác như ảnh bên dưới

![](/images/img-upload-code-WHM/8.png)

![](/images/img-upload-code-WHM/9.png)

![](/images/img-upload-code-WHM/10.png)

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

![](/images/img-upload-code-WHM/11.png)

Tiếp đến ta truy cập tới thư mục public_html chứa code của website trên server và thư mục chứa code muốn upload trên máy tính local

![](/images/img-upload-code-WHM/12.png)

![](/images/img-upload-code-WHM/13.png)

Click Chuột phải vào file muốn upload và click vào Upload để up file code lên server

![](/images/img-upload-code-WHM/14.png)

Kết quả sau khi upload file index.php như ví dụ trên chúng ta truy cập thử trình duyệt website và hiển thị nội dung như file info là thành công

![](/images/img-upload-code-WHM/info.png)

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`


