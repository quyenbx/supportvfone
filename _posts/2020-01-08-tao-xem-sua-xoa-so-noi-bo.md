---
date: 2020-01-08
title: Hướng dẫn tạo,xem,sửa,xóa số nội bộ
categories:
  - Tài-Liệu
description: Hướng dẫn tạo,xem,sửa,xóa số nội bộ
type: Document
---

Với phần số nội bộ này để chúng ta tạo,xem,sửa,xóa các máy nhánh cho các nhân viên theo nhu cầu

Để thao tác chúng ta truy cập vào trang quản trị của tổng đài và chọn "Số và nhóm nội bộ" --> "Danh sách số nội bộ" như hình ảnh bên dưới

![](/images/so-noi-bo/danhsachsonoibo.png)

- Thông số chung :

*Sub Domian : Tên miền dùng cho thiết lập kết nối máy nhánh trên IP Phone,App.

*Port : Thông số cổng kết nối (Ví dụ mặc định : 51000).

*Giới hạn số nội bộ : Giới hạn theo gói dịch vụ tổng số lượng máy nhánh cho phép tạo.

Lưu ý: Trên một số thiết bị khi điền thông tin host kết nối sẽ có 2 dạng:
    1- Điền domain và port riêng.
	2- Điền domain:port.

1.1 Tạo số nội bộ :

Để tạo số nội bộ chúng ta click vào Nút "+Thêm số" và một giao diện hiện ra như hình ảnh bên dưới

![](/images/so-noi-bo/taosonoibo01.png)

Tiếp theo ta nhập thông tin cần thiết và thao tác như ảnh bên dưới

![](/images/so-noi-bo/taosonoibo.png)

Trong đó :

- Id tên đăng nhập : Đây là trường tài khoản hệ thống sẽ phát sinh dựa trên số nội bộ, dùng làm tài khoản (account) khi điền thông số trên thiết bị ip phone như : Account, Username.
- Số nội bộ : quy định từ 2 chữ số đế 6 chữ số bắt đầu từ 10 đến 999999. Lưu ý nên tránh đặt số khẩn cấp làm số nội bộ để tránh không gọi được số khẩn cấp ra PSTN quốc gia.
- Tên hiển thị : đặt tên định danh cho số nội bộ, có thể đặt theo chuẩn tiếng Việt có dấu (unicode utf-8).
- Mật khẩu : trường mật khẩu nên đặt 10 ký tự bao gồm số + chữ tránh BOT hoặc người dùng khác sử dụng máy nhánh trái phép. Trên thiết bị trường này thường ghi như : Password …
- Loại : mặc định là app, chọn web khi muốn dùng số nội bộ sử dụng nghe/gọi trên trình duyệt. Lưu ý: nếu chọn loại web và sử dụng đăng nhập vào thiết bị sẽ không có tiếng khi thoại.
- Ghi âm : Mặc định sẽ bật ghi âm cuộc gọi của số nội bộ tương ứng.
- Chuyển tiếp cuộc gọi : Mặc định là tắt, khi bật ON sẽ ra 2 thông số:
   1- Chuyển tiếp trong n giây : mặc định 7 giây.
   2- Menu chọn kiểu chuyển. (menu chọn diễn giải trong những phần sau).
   
   Ý nghĩa tính năng “Chuyển tiếp cuộc gọi” này khi cuộc gọi gọi đến máy nội bộ bận hoặc reo chuông sau 7 giây không bắt máy hệ thống sẽ chuyển tiếp cuộc gọi sáng hướng khác theo tùy chọn menu.
- Phân quyền : Mặc định không phân quyền, có 2 loại quyền :
   1- Toàn quyền : Số nội bộ tương ứng được toàn quyền “rước cuộc gọi”, “nghe xen”, “nói xen” trên tất cả số nội bộ còn lại trong tổng đài.
   2- Tùy chọn : Nhóm (được quyền “rước cuộc gọi”, “nghe xen”, “nói xen” thành viên thuộc nhóm chỉ định);  Số nội bộ (được quyền “rước cuộc gọi”, “nghe xen”, “nói xen” số nỗi bộ chỉ định)
   
   Ý nghĩa tính năng “Phân quyền” dùng phân cấp và giới hạn quyền hạn của quản lý. VD: phân cấp cho nhóm trưởng chỉ nghe xen, nói xen thành viên của mình và nhóm trưởng đó không nghe xen được bất kỳ ai ngoài nhóm/số đã được thiết lập.


*Trong trường hợp chúng ta cần tạo nhiều số nội bộ cùng lúc.Ví dụ như tạo cho 10,20 nhân viên bắt đầu từ 100 -> 120 
thay vì phải tạo lần lượt từng nhân viên một chúng ta có thể click vào Nút "Tạo tự động " và một giao diện hiện ra như hình ảnh bên dưới

Chúng ta các thông tin số bắt đầu,số kết thúc

![](/images/so-noi-bo/taosotudong.png)

Như vậy là chúng ta đã tạo xong số nội bộ
 

1.2 Xem,Sửa,Xóa số nội bộ :

Để xem danh sách số nội bộ chúng ta click "Danh sách số nội bộ" 

Để sửa số nội bộ chúng ta click chọn "Số và nhóm nội bộ" --> "Danh sách số nội bộ" --> click nút "Sửa" (Biểu tượng hình bút chì) trên thanh "Công cụ" như hình ảnh bên dưới

![](/images/so-noi-bo/suasonoibo.png)

Sau đó một giao diện hiện ra để chúng ta thay đổi các thông tin như Tên,Mật khẩu,Chuyển tiếp cuộc gọi...Sau đó click "Xác nhận" như hình ảnh bên dưới

![](/images/so-noi-bo/suasonoibo01.png)

Để xóa số nội bộ chúng ta click chọn "Số và nhóm nội bộ" --> "Danh sách số nội bộ" --> click nút "Xóa" (Biểu tượng hình chữ X ) trên thanh "Công cụ" như hình ảnh bên dưới

![](/images/so-noi-bo/xoasonoibo.png)

Như vậy là chúng ta đã thao tác xong trong phần Danh sách số nội bộ

---
<a href="https://vfone.vn/" target="_blank">Vfone.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`
