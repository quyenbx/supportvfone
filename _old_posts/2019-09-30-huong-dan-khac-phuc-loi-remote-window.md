---
date: 2019-09-30
title: Hướng dẫn khắc phục lỗi CredSSP remote windows
categories:
  - cloud-server
description: Hướng dẫn khắc phục lỗi CredSSP khi remote windows
type: Document
---

Đối với <a href="https://nhanhoa.com/may-chu/may-chu-cloud-server.html" target="_blank">cloud-server</a> đang chạy hệ điều hành windows để người dùng có thể truy cập từ xa vào cloud-server để quản trị và thao tác đơn giản nhất ta có thể sử dụng `Remote Desktop` windows hỗ trợ sẵn. Tùy thuộc và hệ điều hành windows nào, đang chạy OS windows version nào trong quá trình remote có thể xảy ra lỗi không remote được do nhà phát triển cập nhật để tăng độ bảo mật cho hệ điều hành. Ở bài hướng dẫn này sẽ hướng dẫn bạn khắc phục lỗi `This could be due to CredSSP encryption oracle remediation` khi remote desktop.

![](/images/image-remote-desktop/Screenshot_489.png)

Để khắc phúc lỗi này đơn giản các bạn thêm các tham số trong `registry` của windows.

## 1. Truy cập và cấu hình registry windows

+ Bấm tổ hợp phím phím `Windows + R`  và gõ vào `regedit` để mở registry.

![](/images/image-remote-desktop/Screenshot_490.png)

![](/images/image-remote-desktop/Screenshot_491.png)

## 2. Tạo CredSSP, key Parameters cho AllowEncryptionOracle

+ Truy cập theo đường dẫn `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System`.

![](/images/image-remote-desktop/Screenshot_492.png)

+ Tạo `CredSSP` nếu chưa được thiết lập.

`System` -> `New` -> `Key` đặt tên key là `CredSSP`

![](/images/image-remote-desktop/Screenshot_499.png)

![](/images/image-remote-desktop/Screenshot_493.png)

+ Trong `CredSSP` tạo key `Parameters` bên trong key `CredSSP`

`CredSSP` -> `New` -> `Key` đặt tên key là `Parameters`

![](/images/image-remote-desktop/Screenshot_500.png)

![](/images/image-remote-desktop/Screenshot_494.png)

+ Trong Parameters tạo `DWORD Value` và đặt tên là `AllowEncryptionOracle`

![](/images/image-remote-desktop/Screenshot_501.png)

![](/images/image-remote-desktop/Screenshot_495.png)

+ Chỉnh sửa `Value data` trong `AllowEncryptionOracle` là 2

`AllowEncryptionOracle` -> Chuột phải chọn `Modify`

![](/images/image-remote-desktop/Screenshot_502.png)

![](/images/image-remote-desktop/Screenshot_496.png)

## 3. Kiểm tra

Bạn thực hiện remote lại

Bấm tổ hợp phím phím `Windows + R`  và gõ vào `mstsc` để mở trình remote desktop trên windows.

![](/images/image-remote-desktop/Screenshot_498.png)

Kết quả đã khắc phục được lỗi `CredSSP remote windows`. 

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`
