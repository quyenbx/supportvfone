---
date: 2019-07-31
title: Sử dụng template SQL-server trên Cloud Nhân Hòa
categories:
  - cloud-app
description: Sử dụng template SQL-server trên Cloud Nhân Hòa
type: Document
---

## I. Giới thiệu về SQL-server

![](/images/img-sql-server/sql-server-00.png)

SQL Server chính là một hệ quản trị dữ liệu quan hệ sử dụng câu lệnh SQL để trao đổi dữ liệu giữa máy cài SQL Server và máy Client. Một Relational Database Management System – RDBMS gồm có: databases, datase engine và các chương trình ứng dụng dùng để quản lý các bộ phận trong RDBMS và những dữ liệu khác.

SQL Server được tối ưu để có thể chạy trên môi trường cơ sở dữ liệu rất lớn (Very Large Database Environment) lên đến Tera-Byte và có thể phục vụ cùng lúc cho hàng ngàn user. SQL Server có thể kết hợp “ăn ý” với các server khác như Microsoft Internet Information Server (IIS), E-Commerce Server, Proxy Server….

Hiện tại trên hệ thống Nhân Hòa Cloud đã có template SQL server sau :
 - SQL server 2014 trên Windows server 2016
 - SQL server 2014 trên Windows server 2012
 - SQL server 2012 trên Windows server 2012


## II. Sử dụng dịch vụ SQL-server trên hệ thống Cloud Nhân Hòa. 

Hiện nay, người dùng đã có thể sử dụng dịch vụ SQL-server trên hệ thống Cloud Nhân Hòa. Người dùng có thể thực hiện bằng 2 cách.
 - Đăng ký mới cloud server SQL server
 - Chuyển đổi sử dụng (rebuild) cloud server SQL server
 
### Cách 1 : Đăng ký mới sử dụng SQL-server Cloud365 

Truy cập tới trang https://nhanhoa.com và đăng ký máy ảo SQL-server. 

![](/images/img-sql-server/sql-server-01.png)

### Cách 2 : Chuyển đổi sử dụng SQL-server Cloud365 

Đối với những khách hàng đang sử dụng dịch cloud VPS nhưng đang là hệ điều hành trắng hoặc các dịch vụ khác thì có thể chủ động sử dụng tính năng rebuild trên portal quản trị, chọn rebuild với image SQL-server để sử dụng.

![](/images/img-sql-server/sql-server-02.png)

![](/images/img-sql-server/sql-server-03.png)


## III. Đăng nhập và sử dụng dịch vụ SQL-server

Sau khi đăng ký sử dụng hoặc chuyển đổi thành công sang template SQL-server bạn sẽ nhận được thông tin đăng nhập VPS, thông tin đăng nhập SQL-server gửi vào email đăng ký của bạn.

![](/images/img-sql-server/sql-server-04.png)

Sử dụng thông tin để đăng nhập và kiểm tra với phần mềm SQL Studio Management. Kiểm tra thông tin và sử dụng các tính năng của SQL-server đối với hệ thống của mình.

![](/images/img-sql-server/sql-server-05.png)

Hãy theo dõi các bài viết tiếp theo của Cloud Team Nhân Hòa để cập nhập các thông tin mới nhất về dịch vụ SQL server của bạn.

Xin cảm ơn !

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`