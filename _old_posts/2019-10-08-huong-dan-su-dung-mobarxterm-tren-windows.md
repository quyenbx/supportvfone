---
date: 2019-10-08
title: Hướng dẫn sử dụng MobaXterm trên windows
categories:
  - cloud-server
description: Hướng dẫn sử dụng công cụ MobaXterm trên windows
type: Document
---

Khi làm việc với các hệ điều hành như `Linux`, `Windows`... hay quản trị các thiết bị mạng `Switch`, `Router` việc truy cập quản lý, thao qua kết nối console là vô cùng bất tiện. Hiện nay có nhiều phần mềm miễn phí hỗ trợ bạn thực hiện truy cập từ xa, thao tác một cách chủ động như Putty, SecureCRT... Bài viết dưới đây sẽ hướng dẫn các bạn sử dụng công cụ `MobaXterm` được cài đặt trên hệ điều hành Windows để `SSH`, `telnet`, `remote` từ xa tới thiết bị của mình và một số tính năng hỗ trợ bổ sung khác.

![](/images/img-mobarxterm/ssh.png)

## 1. Tải và cài đặt MobaXterm

Truy cập https://mobaxterm.mobatek.net/download.html 

Lựa chọn bản miễn phí cho hệ điều hành windows để tải xuống - giải nén - cài đặt.

![](/images/img-mobarxterm/Screenshot_511.png)

**Bắt đầu cài đặt**

Click vào file vừa tải về, sau đó chọn `Next`

![](/images/img-mobarxterm/Screenshot_512.png)

Đồng ý với điều khoản sử dụng phần mềm

![](/images/img-mobarxterm/Screenshot_513.png)

Để mặc định các gợi ý cài đặt và chọn `Next` tiếp theo

![](/images/img-mobarxterm/Screenshot_514.png)

Chọn `Install` để cài đặt MobaXterm

![](/images/img-mobarxterm/Screenshot_515.png)

Sau đó chọn `Finish` để kết thúc việc cài đặt MobaXterm.

![](/images/img-mobarxterm/Screenshot_516.png)

Cài đặt thành công

## 2. Thao tác sử dụng

### 2.1. Thực hiện ssh tới một server linux

Thực hiện khởi động MobaXterm từ desktop hoặc từ thanh menu của windows.

![](/images/img-mobarxterm/Screenshot_517.png)

Thao tác connect tới server của bạn

Click `Session` -> `SSH` -> Nhập các thông tin server (IP, username, port)  -> `OK`

Thường thì các server có port SSH mặc định là `22` người quản trị có thể thay đổi port để nâng cao bảo mật bạn chú ý nhập đúng thông tin port.

![](/images/img-mobarxterm/Screenshot_526.png)

Nhập mật khẩu kết nối tới server của bạn. Một điều chú ý khi nhập mật khẩu sẽ không hiển thị dấu `********` như các công cụ khác bạn nhập chính xác hoặc bạn có thể `paste` mật khẩu vào màn hình ở dưới.

![](/images/img-mobarxterm/Screenshot_527.png)

Kết nối ssh thành công

![](/images/img-mobarxterm/Screenshot_528.png)

### 2.2. Thực hiện telnet tới một thiết bị mạng

Bạn có thể thực hiện `telnet` tới một thiết bị mạng để thao tác cấu hình, cụ thể dưới đây kết nối tới thiết bị Switch theo giao thức telnet. Port mặc định của telnet là 23.

Click `Session` -> `Telnet` -> Nhập các thông tin server -> `OK`

![](/images/img-mobarxterm/Screenshot_520.png)

Nhập mật khẩu của thiết bị. Mật khẩu không hiển thị dạng `********` bạn nhập chính xác mật khẩu hoặc paste vào màn hình ở dưới.

![](/images/img-mobarxterm/Screenshot_521.png)

Vậy bạn đã kết nối từ xa tới Switch thành công.

### 2.4. Một số tính năng khác MobaXterm hỗ trợ

**Network scan**: Tính năng MobaXterm hỗ trợ để scan các IP trong cùng dải mạng

Click `Tools` -> `Network scanner` -> Nhập thông tin về network của bạn muốn kiểm tra.

![](/images/img-mobarxterm/Screenshot_522.png)

Kết quả cho bạn là trong dải mạng của bạn có những IP nào đang online, đang hoạt động qua giao thức nào.

![](/images/img-mobarxterm/Screenshot_523.png)

**Port scan**: Kiểm tra xem một server đang mở những port nào.

Click `Tools` -> `Ports scanner` -> Nhập thông tin IP bạn muốn kiểm tra.

![](/images/img-mobarxterm/Screenshot_524.png)

Kết quả là server kiểm tra đang mở port nào.

![](/images/img-mobarxterm/Screenshot_525.png)

Trên là những hướng dẫn cơ bản cho bạn để sử dụng công cụ MobaXterm.

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`