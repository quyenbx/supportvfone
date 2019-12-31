---
date: 2019-01-31
title: Giới thiệu SQL Server trong Cloud Server
categories:
  - cloud-app
description: Giới thiệu SQL Server trong Cloud Server
type: Document
---

## 1. SQL là gì? Tổng quan SQL Server

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud.png)</span>

Là phần mềm được Microsoft phát triển dựa trên RDBMS (RDBMS là viết tắt của Relational Database Management System có nghĩa là hệ quản trị cơ sỡ dữ liệu quan hệ).
Là hệ quản trị cơ sở dữ liệu quan hệ đối tượng.
Là một nền tảng độc lập.
Phần mềm sử dụng cả giao diện dòng lệnh và giao diện GUI.

Đối tượng của SQL server là các bảng dữ liệu với các cột và các hàng. Cột được gọi là trường dữ liệu và hàng là bản ghi của bảng. Cột dữ liệu và kiểu dữ liệu xác định tạo nên cấu trúc của bảng. Khi bảng được tổ chức thành một hệ thống cho một mục đích sử dụng cụ thể vào công việc nào đó sẽ trở thành một cơ sở dữ liệu.

## 2. Mục đích sử dụng của SQL Server
- Tạo cơ sở dữ liệu.
- Duy trì cơ sở dữ liệu.
- Phân tích dữ liệu 
- Tạo báo cáo

## 3. Một số phiên bản của SQL Server
- `Enterprise` - bản cao cấp nhất với đầy đủ tính năng.
- `Standard` - ít tính năng hơn Enterprise, sử dụng khi không cần dùng tới các tính năng nâng cao.
- `Workgroup` - phù hợp cho các công ty lớn với nhiều văn phòng làm việc từ xa.
- `Web` - thiết kế riêng cho các ứng dụng web.
- `Developer` - tương tự như Enterprise nhưng chỉ cấp quyền cho một người dùng duy nhất để phát triển, thử nghiệm, demo. Có thể dễ dàng nâng cấp lên bản Enterprise mà không cần cài lại.
- `Express` - bản này chỉ dùng ở mức độ đơn giản, tối đa 1 CPU và bộ nhớ 1GB, kích thước tối đa của cơ sở dữ liệu là 10GB.
- `Datacenter` - thay đổi lớn trên SQL Server 2008 R2 chính là bản Datacenter Edition. Không giới hạn bộ nhớ và hỗ trợ hơn 25 bản cài.
- `Enterprise Evaluation` - bản SQL Server Evaluation Edition là lựa chọn tuyệt vời để dùng được mọi tính năng và có được bản cài miễn phí của SQL Server để học tập và phát triển. Phiên bản này có thời gian hết hạn là 6 tháng từ ngày cài.

Phiên bản của Cloud365 hiện hỗ trợ là : SQL Server 2008, SQL server 2012, SQL Server 2014 và là phiên bản Enterprise, có thể sử dụng thử dịch vụ tại <a href="https://cloud365.vn/" target="_blank">đây</a>

## 4. Microsoft SQL trên server cloud365.vn

Microsoft SQL Server đã được cài đặt sẵn trên Cloud của cloud365, người dùng có thể chọn sử dụng cùng Plesk hoặc chỉ cài đặt hệ điều hành Windows + SQL Server:
- Windows Server 2008 + Plesk (SQL 2012)
- Windows Server 2012 + SQL 2012
- Windows Server 2012 + SQL 2014
- Windows Server 2012 + Plesk (SQL 2012)
- Windows Server 2016 + SQL 2014
- Windows Server 2016 + Plesk (SQL 2014)

Người dùng có thể thực hiện order VPS thông qua trang chủ <a href="https://nhanhoa.com/" target="_blank">nhanhoa.com</a> :

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud4.png)</span>

Hoặc có thể liên hệ trực tiếp với <a href="https://nhanhoa.com/lien-he.html" target="_blank">bộ phận kinh doanh Nhân Hòa</a>

**Với trường hợp đang sử dụng dịch vụ tại Cloud365** : người dùng có thể tự rebuild Cloud để sử dụng SQL Server (với Cloud từ gói C trở lên):

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud6.png)</span>

Chọn máy ảo, click vào `Quản lý máy aor` và chọn `REBUILD`

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud7.png)</span>

Trong phần Hệ điều hành, chọn Windows App, sau đó chọn template muốn sử dụng

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud8.png)</span>

Cần xác nhận lại nội dung `REBUILD` lại máy ảo sẽ xóa toàn bộ dữ liệu trên máy ảo cũ

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud9.png)</span>

Sau khi rebuild thành công, thông tin máy ảo sẽ được gửi tới người dùng.

## 5. Truy cập SQL server 

Sau khi nhận được thông tin Cloud365.vn cung cấp, người dùng có thể truy cập được SQL Server Database thông qua 2 cách: remote access hoặc local access. 

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud5.png)</span>

Ở đây, người dùng có thể truy cập SQL trên chính server đó như sau:

- Remote desktop vào server, truy cập `Microsoft SQL Server Management Studio`

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud1.png)</span>

- Sau khi hiện màn hình đăng nhập người dùng có thể đăng nhập bằng Windows Authentication (ở đây mặc định là tài khoản `Administrator`) hoặc bằng tài khoản admin của SQL (`sa`) mà cloud365 đã cung cấp.

- Đăng nhập thông tin chính xác người dùng có thể truy cập - thao tác với các cơ sở dữ liệu trên cloud:

<span style="display:block;text-align:center">![](/images/img-sql-cloud-server/sql_cloud3.png)</span>


---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`