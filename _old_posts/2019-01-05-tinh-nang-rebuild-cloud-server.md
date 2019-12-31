---
date: 2019-01-05
title: Tính năng rebuild cloud server
categories:
  - cloud-server
description: Hướng dẫn sử dụng tính năng rebuild cloud server
type: Document
---

Khi đăng ký sử dụng dịch vụ cloud server của Nhân Hòa bạn sẽ được cung cấp portal để hoàn toàn chủ động thao tác quản trị, cài đặt đối với cloud server của mình. Một số nhà cung cấp cấp dịch vụ cloud server khác trường hợp bạn thao tác trên cloud server của mình bị lỗi mà bạn muốn cài đặt lại hệ điều hành hay chuyển sang hệ điều hành khác để phù hợp với ứng dụng của mình bạn phải liên lệ với nhà cung cấp để được hỗ trợ, thời gian chờ đợi lâu và thâm chí bạn còn phải trả phí cho những yêu cầu này.

Hướng tới sự thuận tiện nhất cho khách hàng Nhân Hòa cung cấp chức năng rebuild cloud server cho bạn để bạn tự thao tác và lựa chọn hệ điều hành muốn thay đổi. Bạn có thể cài lại chính hệ điều hành cũ cho cloud server hoặc chuyển đổi sang hệ điều hành mới mà vẫn giữ nguyên gói cấu hình và đặt biệt là nhanh chóng và không phải trả phí.

Chi tiết cách thức rebuild cloud server bạn thực hiện theo hướng dẫn dưới đây. Ở bài hướng dẫn này thực hiện rebuild cloud server hệ điều hành **CentOS 6** sang cloud server hệ điều hành **Windows 10**.

### Các bước thực hiện

[Bước 1: Truy cập vào Nhân Hòa portal](#truycap)<br>
[Bước 2: Lựa chọn cloud server cần rebuild](#chon)<br>
[Bước 3: Lựa chọn hệ điều hành rebuild](#os)<br>
[Bước 4: Xác nhận rebuild](#xacnhan)<br>
[Bước 5: Lấy thông tin cloud server sau khi rebuild](#thongtin)<br>
[Bước 6: Kiểm tra](#kiemtra)<br>

<a name="truycap"></a>
## Bước 1: Truy cập vào Nhân Hòa portal

Bạn sử dụng thông tin đăng nhập bao gồm `email/password` để đăng nhập

<a href="https://support.cloud365.vn/account-settings/dang-nhap-portal/" target="_blank">Đăng nhập</a> portal tại địa chỉ <a href="https://portal.cloud365.vn/" target="_blank">https://portal.cloud365.vn/</a>

![](/images/img-rebuild-vps/Screenshot_202.png)

<a name="chon"></a>
## Bước 2: Lựa chọn cloud server cần rebuild

+ Click `Danh sách server`

![](/images/img-rebuild-vps/Screenshot_231.png)

+ Click vào tên cloud server cần xem thông tin

![](/images/img-rebuild-vps/Screenshot_232.png)

+ Click `Quản lý máy ảo`

![](/images/img-rebuild-vps/Screenshot_233.png)

![](/images/img-rebuild-vps/Screenshot_234.png)

<a name="os"></a>
## Bước 3: Lựa chọn hệ điều hành rebuild

Bạn lựa chọn hệ điều hành muốn rebuild cho cloud server của mình.

**Lưu ý**:-
+ Khi rebuild dữ liệu ổ cứng sẽ không được giữ lại. Máy chủ sẽ chạy với hệ điều hành mà bạn xác nhận lựa chọn để rebuild.<br>
+ Bạn có thể rebuild sang hệ điều hành Windows, Linux trắng và Linux có cài đặt ứng dụng (Plesk, Direct Admin, WHM).<br>
+ Bạn không thể rebuild sang hệ điều hành Windows server có cài đặt ứng dụng.

![](/images/img-rebuild-vps/Screenshot_236.png)

<a name="xacnhan"></a>
## Bước 4: Xác nhận rebuild

Bạn nên đọc những cảnh bảo trước khi xác nhận rebuild.

![](/images/img-rebuild-vps/Screenshot_237.png)

Chờ một vài phút để quá trình rebuild hoàn tất. 

<a name="thongtin"></a>
## Bước 5: Lấy thông tin cloud server sau khi rebuild

Sau khi rebuild thành công thông tin sẽ được gửi về email của bạn.<br>
+ Lựa chọn rebuild sang cloud server linux bạn vui lòng chờ khoảng 2-3 phút để hệ thống tự động gửi thông tin.<br>
+ Đối với rebuild sang cloud server windows bạn vui lòng chờ 8-10 phút để hệ thống gửi tự động gửi thông tin.

![](/images/img-rebuild-vps/Screenshot_238.png)

![](/images/img-rebuild-vps/Screenshot_239.png)

<a name="kiemtra"></a>
## Bước 6: Kiểm tra

+ Cloud server trước khi rebuild

![](/images/img-rebuild-vps/Screenshot_212.png)

+ Cloud server sau khi rebuild

![](/images/img-rebuild-vps/Screenshot_240.png)

Quá trình rebuild hoàn thành.

---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`



