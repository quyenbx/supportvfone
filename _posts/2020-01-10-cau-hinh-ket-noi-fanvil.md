---
date: 2020-01-10
title: Hướng dẫn cấu hình kết nối IP Phone Fanvil với tổng đài ảo
categories:
  - Tài-Liệu
description: Hướng dẫn cấu hình kết nối IP Phone Fanvil với tổng đài ảo
type: Document
---

Bước 1 : Chúng ta cắm dây mạng internet vào cổng “LAN” của IP Phone Fanvil

Lưu ý : Trường hợp bạn đang sử dụng nhiều đường mạng (FPT,VNPT..) hay dải mạng ( 192.168.1.x ; 10.10.10.x ...) khác nhau thì bạn có thể cắm 
nối tiếp thêm 1 dây mạng từ điện thoại vào máy tính sử dụng cổng “PC” của điện thoại. Như vậy điện thoại và máy tính của bạn nằm trong cùng mạng local.
với mục đích là truy cập được vào IP local của điện thoại thông qua trình duyệt web trên máy tính

Mỗi điện thoại IP Fanvil phải được cấu hình kết nối với một tổng đài để có thể nhận cuộc gọi vào, gọi ra ngoài hoặc gọi các máy nhánh khác.

Ví dụ khi đăng ký dịch vụ tổng đài ảo <a href="https://vfone.vn/" target="_blank">Vfone.vn</a>,Bạn sẽ thiết lập được các phòng ban với nhiều máy nhánh.
Các máy nhánh này (ví dụ 101,102) được kết nối với tổng đài thông qua SIP server (ví dụ 123.123.123.123).

Bước 2 : Cấu hình điện thoại IP Fanvil,truy cập vào IP local của điện thoại thông qua trình duyệt web trên máy tính.Trong ví dụ này IP local của điện thoại là http://192.168.1.123/

Kiểm tra IP của điện thoại bằng cách nhấn phím Menu --> Status --> IP ( mặc định là DHCP được cấp từ LAN)

![](/images/cau-hinh-fanvil/fanvil.png)

Sau khi đã có IP thì mở trình duyệt web trên máy tính truy cập theo link http://192.168.1.123/
Đăng nhập với user/password từ nhà cung cấp điện thoại (Mặc định là Username : admin và Password : admin)

Bước 3 : Chúng ta truy cập vào trang quản trị của IP Phone Fanvil và chọn "Line" --> "SIP" nhập thông tin cần thiết và nhấn "Apply" để lưu lại ( thao tác như ảnh bên dưới )

![](/images/cau-hinh-fanvil/fanvil01.png)


Trong đó :

- User name: Nhập “ Id đăng nhập “ trên tổng đài ảo của bạn ví dụ : mujbm666
- Display name: Tên hiển thị trên màn hình điện thoại ví dụ : Lê Văn A
- Realm: địa chỉ IP và port của tổng đài ảo
- Register Address: địa chỉ IP máy chủ SIP cần khai báo
- Register Port: khai báo cổng tổng đài ảo
- Authentication Name: xác thực tên được ủy quyền ( Nhập lại “ Id đăng nhập “ trên tổng đài ảo của bạn )
- Authentication Password: xác thực mật khẩu được ủy quyền

Trường hợp bạn chưa biết lấy thông tin Id đăng nhập,subdomain trên tổng đài vui lòng tham khảo thêm <a href="https://support.vfone.vn/t%C3%A0i-li%E1%BB%87u/cau-hinh-zoiper/" target="_blank">Ở đây</a>

Sau khi điền thông số, bạn nhấn "Apply" thì điện thoại sẽ kết nối internet để đăng ký với tổng đài <a href="https://vfone.vn/" target="_blank">Vfone.vn</a>.
Nếu thông số đúng,các bạn quay lại tab "Information" ở mục SIP accounts --> Line 1 có trạng thái là "Registed" nghĩa là đã khai báo thành công.


Như vậy là chúng ta đã thao tác xong phần cấu hình kết nối IP Phone Fanvil với tổng đài ảo

---
<a href="https://vfone.vn/" target="_blank">Vfone.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`
