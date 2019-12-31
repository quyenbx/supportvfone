---
date: 2019-02-13
title: Hướng dẫn nâng cấp cấu hình Cloud Server
categories:
  - cloud-app
description: Nâng cấp cấu hình Cloud Server
type: Document
---

Một số trường hợp, khách hàng sau một thời gian sử dụng, các site tăng trưởng về số lượng truy cập, quy mô website, hoặc đơn giản là lượng dữ liệu của website tăng lên, khiến cho lượng tài nguyên hiện có không đủ để đáp ứng. Hoặc trong trường hợp, người dùng có thể dự đoán trước được lượng truy cập sẽ tăng đột biến, như khi bạn có sự kiện hoặc đợt bán vé / giảm giá trên website, hoặc mở rộng thêm một lượng lớn các website / ứng dụng trên máy ảo.

Tại Cloud365, có rất nhiều gói cước với các cấu hình khác nhau sẵn sàng đáp ứng kịp thời nhu cầu của người dùng. Bài viết sẽ hướng dẫn khách hàng nâng cấp dịch vụ Cloud trên hệ thống của Cloud365.

## Khi nào cần phải nâng cấp cấu hình Cloud server?

Việc hoạt động không ổn định của website có thể còn do nhiều yếu tố: Phát sinh lỗi phía mã nguồn / máy chủ, lỗi đường truyền, bị tấn công ,... Với các nguyên nhân trên, khách hàng cần liên hệ với <a href="https://cloud365.vn/" target="_blank">cloud365.vn</a> để nắm thêm thông tin và tư vấn. 
Dưới đây, chỉ liệt kê ra các trường hợp liên quan đến việc quả tải về tài nguyên VPS:

**Dấu hiệu quá tải CPU, RAM**

- Website / ứng dụng mất nhiều thời gian để phản hồi hoặc không phản hồi, khi truy cập vào trang chủ hoặc trang con.
- Khách hàng có thể quan sát thêm trên <a href="https://portal.cloud365.vn/" target="_blank">portal</a> của Cloud365:

- Nguyên nhân:
    - Số lượng truy cập tới website tăng so với bình thường.
    - Thay đổi, nâng cấp mã nguồn.

**Dấu hiệu quá tải ổ cứng**

- Thông báo lỗi cơ sở dữ liệu, ví dụ:

<span style="display:block;text-align:center">![](/images/img-upgrade-cloud/upgrade_4.png)</span>

- Thông báo lỗi không truy cập được website, ví dụ:

<span style="display:block;text-align:center">![](/images/img-upgrade-cloud/upgrade_5.png)</span>

- Đăng nhập control (Directadmin, ..) đúng user / password nhưng vẫn dừng ở màn hình đăng nhập và không có thông báo lỗi
- Hoặc khi đăng nhập SSH và chạy câu lệnh `df -h` sẽ hiển thị disk full 100% (hoặc trống rất ít), ví dụ như sau:

<span style="display:block;text-align:center">![](/images/img-upgrade-cloud/upgrade_6.png)</span>

- Nguyên nhân:
    - Do service bị stop hoặc đầy ổ cứng dẫn đến lỗi khi hoạt động.
    - Có thể login vào SSH / FTP để dọn dẹp các file không sử dụng đến, hoặc liên hệ để nâng cấp.

**Kiểm tra trong phần quản lý máy ảo**
- Người dùng có thể chủ động kiểm soát tài nguyên của VPS thông qua hệ thống giám sát được tích hợp sẵn trên portal của Cloud365, cụ thể:
- Sau khi đăng nhập thành công VPS, người dùng click chuột vào máy ảo cần thống kê, sau đó thông tin tài nguyên máy ảo sẽ hiện ra ở phía bên phải.
- Bên dưới là một ví dụ về trường hợp máy ảo sử dụng 100% tài nguyên CPU, dẫn đến không ổn định dịch vụ:

<span style="display:block;text-align:center">![](/images/img-upgrade-cloud/upgrade_2.png)</span>


## Cách để nâng cấp cấu hình Cloud server

Bước 1: Khách hàng truy cập vào trang chủ <a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>để tham khảo bảng giá nâng cấp cấu hình của dịch vụ.

<span style="display:block;text-align:center">![](/images/img-upgrade-cloud/upgrade_1.png)</span>

Quý khách có thể lựa chọn giữa Cloud VPS và Cloud Server SSD cấu hình cao để phục vụ cho nhu cầu của mình

<span style="display:block;text-align:center">![](/images/img-upgrade-cloud/upgrade_3.png)</span>

Bước 2: Sau khi đã chọn được gói cấu hình phù hợp, hoặc cần tư vấn thêm từ đội ngũ kinh doanh của Cloud365, quý khách có thể liên hệ trực tiếp thông qua các kênh sau:

- Bộ phận kinh doanh
    - Điện thoại: (024) 7308 6680 (phím 1, phím 2, phím 3)
    - Email: sales@nhanhoa.com

- Bộ phận kỹ thuật
    - Điện thoại: (024) 7308 6680 (phím 4)
    - Email: support@nhanhoa.com


---
<a href="https://cloud365.vn/" target="_blank">cloud365.vn</a>

Khi cần hỗ trợ xin liên hệ với chúng tôi:

**Công ty phần mềm Nhân Hòa**
- Trụ sở Hà Nội: 32 Võ Văn Dũng, Đống Đa, Hà Nội
- Chi nhánh HCM: 270 Cao Thắng (nối dài), Phường 12,Quận 10, TP HCM
- Hotline: `19006680`