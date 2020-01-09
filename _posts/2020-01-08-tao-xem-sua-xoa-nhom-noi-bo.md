---
date: 2020-01-08
title: Hướng dẫn tạo,xem,sửa,xóa nhóm nội bộ
categories:
  - Tài-Liệu
description: Hướng dẫn tạo,xem,sửa,xóa nhóm nội bộ
type: Document
---

Để thao tác chúng ta truy cập vào trang quản trị của tổng đài và chọn "Số và nhóm nội bộ" --> "Danh sách nhóm nội bộ" như hình ảnh bên dưới

![](/images/nhom-noi-bo/danhsachnhomnoibo.png)

1.1 Tạo nhóm nội bộ :

Để tạo nhóm nội bộ chúng ta click vào Nút "+Thêm" và một giao diện hiện ra như hình ảnh bên dưới

![](/images/nhom-noi-bo/taonhomnoibo.png)

Tiếp theo ta nhập thông tin cần thiết và thao tác như ảnh bên dưới

![](/images/nhom-noi-bo/taonhomnoibo01.png)

Trong đó :

- Số nhóm : từ 2 chữ số đến 6 chữ số bắt đầu từ 10 đến 999999, không được trùng với số nội bộ đã tạo trước đó.
- Tên hiển thị : Đặt tên cho nhóm.
- Khung trái chọn thành viên (số nội bộ) click để vào khung bên phải, có thể tạo nhóm rỗng chưa có thành viên.
- Khung phải khi có thành viên sẽ có 2 tham số:
  1- Độ ưu tiên : từ 0 đến 99, mặc định là 0, số càng cao ưu tiên reo chuông càng thấp khi nhóm được gọi.
  2- Tạm dừng : Mặc định là 0, khi khác 0 thành viên đó sẽ không nhận đổ chuông khi nhóm được gọi.
  
- Quy tắc đổ chuông : (có một số quy tắc chưa dịch sát nghĩa nên giữ nguyên tiếng anh)
  * ringall : đổ chuông toàn bộ.(Mặc định).
  * roundrobin : đổ chuông lần lượt xoay vòng.
  * leastrecent : đổ chuông máy nhánh đã nhận cuộc gọi trước đó.
  * fewestcalls : ring the one with fewest completed calls from this queue.
  * random : đổ chuông ngẫu nhiên.
  * rrmemory : đổ chuông xoay vòng có ghi nhớ lượt xoay trước đó.
  * linear : đổ chuông theo định nghĩa trên file thiết lập (hiện tại không khả dụng).
  * wrandom : đổ chuông ngẫu nhiên chịu ảnh hưởng bởi độ ưu tiên nhóm.
  Lưu ý : các chế độ đổ chuông đều ảnh hưởng theo quy tắc độ ưu tiên của thành viên trong nhóm tương ứng.
  
- Nhạc chờ : Chọn danh sách nhạc chờ đã thiết lập trong phần “Danh sách nhạc chờ”.
- Ghi âm : bật để luôn ghi âm bất chấp máy nhánh thiết lập không ghi âm.
- Auto fill :  khi người gọi chờ được kết nối với các thành viên có sẵn theo cách song song cho đến khi không còn thành viên nào khả dụng hoặc không có thêm người gọi chờ.
- Ring in use : tiếp tục đổ chuông đến thành viên nhóm khi thành viên đó vẫn đang thông thoại với cuộc gọi khác.
- Thời gian đổ chuông : Mặc định 0 sẽ đổ chuông không giới hạn thời gian. Thời gian được tính bằng giây nếu lớn hơn 0. Hết thời gian đổ chuông hệ thống sẽ chuyển hướng sang menu “Hết thời gian đổ chuông”.
- Số lần lặp : Chỉ giá trị khi thời gian đổ chuông lớn hơn 0, khi lập đủ số lần thiết lập hệ thống sẽ chuyển hướng cuộc gọi sang menu “Kết thúc lặp”.
- Hàng đợi tối đa : cho phép thiết lập số lượng tối đa cuộc gọi vào nhóm trong thời điểm, giá trị = 0 tức không có giới hạn. Khi có giới hạn tối đa được thiết lập người gọi vào vượt số tối đa sẽ được chuyển hướng cuộc gọi vào menu “Đầy hàng đợi”.
- joinempty : Chọn “yes” người gọi vẫn vào hàng chờ mặc dù trong nhóm “rỗng” hoặc chưa thiết lập thành viên nhóm hoặc tất cả thành viên nhóm không online. Chọn “no” người gọi vào gặp điều kiện như trên hệ thống sẽ chuyển hướng cuộc gọi qua menu “JOINEMPTY”.

1.2 Xem,Sửa,Xóa nhóm nội bộ :

Để xem danh sách nhóm nội bộ chúng ta click "Danh sách nhóm nội bộ" 

Để sửa số nội bộ chúng ta click chọn "Số và nhóm nội bộ" --> "Danh sách nhóm nội bộ" --> click nút "Sửa" (Biểu tượng hình bút chì) trên thanh "Công cụ" như hình ảnh bên dưới

![](/images/nhom-noi-bo/suanhomnoibo.png)

Sau đó một giao diện hiện ra để chúng ta thay đổi các thông tin như Tên hiển thị,Số nội bộ trong nhóm,Quy tắc đổ chuông...Sau đó click "Xác nhận" như hình ảnh bên dưới

![](/images/nhom-noi-bo/suanhomnoibo01.png)

Để xóa số nội bộ chúng ta click chọn "Số và nhóm nội bộ" --> "Danh sách số nội bộ" --> click nút "Xóa" (Biểu tượng hình chữ X ) trên thanh "Công cụ" như hình ảnh bên dưới

![](/images/nhom-noi-bo/xoanhomnoibo.png)

Như vậy là chúng ta đã thao tác xong trong phần Danh sách nhóm nội bộ

---
<a href="https://vfone.vn/" target="_blank">Vfone.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`
