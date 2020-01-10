---
date: 2020-01-10
title: Hướng dẫn cấu hình kết nối IP Phone Yealink với tổng đài ảo
categories:
  - Tài-Liệu
description: Hướng dẫn cấu hình kết nối IP Phone Yealink với tổng đài ảo
type: Document
---

Bước 1 : Chúng ta cắm dây mạng internet vào cổng “Internet” của IP Phone Yealink (Ở đây mình đang sử dụng Điện Thoại IP Phone Yealink SIP-T19E2)

Lưu ý : Trường hợp bạn đang sử dụng nhiều đường mạng (FPT,VNPT..) hay dải mạng ( 192.168.1.x ; 10.10.10.x ...) khác nhau thì bạn có thể cắm 
nối tiếp thêm 1 dây mạng từ điện thoại vào máy tính sử dụng cổng “PC” của điện thoại. Như vậy điện thoại và máy tính của bạn nằm trong cùng mạng local.
với mục đích là truy cập được vào IP local của điện thoại thông qua trình duyệt web trên máy tính

Mỗi điện thoại IP Yealink phải được cấu hình kết nối với một tổng đài để có thể nhận cuộc gọi vào, gọi ra ngoài hoặc gọi các máy nhánh khác.

Ví dụ khi đăng ký dịch vụ tổng đài ảo <a href="https://vfone.vn/" target="_blank">Vfone.vn</a>,Bạn sẽ thiết lập được các phòng ban với nhiều máy nhánh.
Các máy nhánh này (ví dụ 101,102) được kết nối với tổng đài thông qua SIP server (ví dụ 123.123.123.123).

Bước 2 : Để cấu hình điện thoại IP Yealink,truy cập vào IP local của điện thoại thông qua trình duyệt web trên máy tính.Trong ví dụ này IP local của điện thoại là http://192.168.1.101/
Để xem IP hiện tại, nhấn phím OK khi đang trên màn hình ban đầu của điện thoại.

![](/images/cau-hinh-yealink/yealink.png)

Sau khi đã có IP thì mở trình duyệt web trên máy tính truy cập theo link http://192.168.1.101/
Đăng nhập với user/password từ nhà cung cấp điện thoại (Mặc định là Username : admin và Password : admin)

![](/images/cau-hinh-yealink/login.png)

Bước 3 : Chúng ta truy cập vào trang quản trị của IP Phone Yealink và chọn "Account" --> "Register" nhập thông tin cần thiết và thao tác như ảnh bên dưới

![](/images/cau-hinh-yealink/yealink01.png)


Trong đó :

- Line Active : Chọn Enabled
- Label : Nhập số nội bộ (Máy nhánh) ví dụ 101, 102...
- Display Name : Nhập tên cho máy nhánh ví dụ Lê Văn A...
- Register Name : Nhập " Id đăng nhập " trên tổng đài ảo của bạn
- User Name : Nhập lại " Id đăng nhập " trên tổng đài ảo của bạn
- Password : Nhập mật khẩu của máy nhánh

* SIP Server 1 :
- Server Host : Nhập nhập subdomain của tổng đài ảo và Port ví dụ như là 51000
- Transport : Để mặc định UDP
- Server Expires : Để mặc định 3600
- Server Retry Counts : Để mặc định 3 

Trường hợp bạn chưa biết lấy thông tin Id đăng nhập,subdomain vui lòng tham khảo thêm <a href="https://support.vfone.vn/t%C3%A0i-li%E1%BB%87u/cau-hinh-zoiper/" target="_blank">Ở đây</a>

Sau khi điền thông số, bạn nhấn "Confirm" thì điện thoại sẽ kết nối internet để đăng ký với tổng đài <a href="https://vfone.vn/" target="_blank">Vfone.vn</a>.
Nếu thông số đúng, trạng thái của điện thoại sẽ là "Registered". Lúc này, bạn có thể dùng điện thoại để gọi cho các số nội bộ khác, hoặc nhận cuộc gọi từ tổng đài ảo, hoặc gọi ra ngoài thông qua tổng đài.


Ngoài ra, còn có các cấu hình nâng cao khác cho điện thoại. Ví dụ dưới đây thay đổi Timezone mặc định của điện thoại.
(Lưu ý các điện thoại IP có timezone tương ứng với nơi sản xuất,có thể ở các quốc gia khác,nên giờ hiển thị trên máy bị sai so với giờ Việt Nam).

![](/images/cau-hinh-yealink/yealink02.png)

Như vậy là chúng ta đã thao tác xong phần cấu hình kết nối IP Phone Yealink với tổng đài ảo

---
<a href="https://vfone.vn/" target="_blank">Vfone.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`
