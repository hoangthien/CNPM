# Báo cáo kế hoạch lập trình và kiểm thử đơn vị

## Cài đặt môi trường lập trình
+ IDE: Visual Studio 2013 Ultimate
+ Ngôn ngữ lập trình: C#
+ .Net framework 4.5
+ Sử dụng SVN để quản lý phiên bản. (Google Code + Tortoise/RapidSVN)
+ BugZilla để quản lý tiến độ làm việc.

## Phương pháp lập trình
+ Nhóm sử dụng phương pháp lập trình hướng đối tượng, với các đối tượng chính
    * Nhân viên
    * Sổ tiết kiệm
    * Khách hàng
    * Chính sách tiết kiệm
+ Nhóm tiếp cận theo phương pháp Top - Down
    * Khái quát chương trình cần quản lý sổ tiết kiệm của khách hàng, cho phép thực hiện các thao tác _Tạo sổ_, _Gửi tiền_, _Rút tiền_.
    * Có 2 mức nhân viên: _NV thường_ & _NV Quản lý_
    * Có các chính sách tiết kiệm
        - Không kỳ hạn
        - Kỳ hạn x tháng
        - Kỳ hạn y tháng

## Tổ chức kiến trúc chương trình
+ Xây dựng chương trình dựa trên mô hình 3 lớp
    * Lớp GUI: thiết kế giao diện người dùng sử dụng Form C#
    * Lớp Logic phần mềm: xử lý các yêu cầu, các ràng buộc của chương trình, như điều kiện tạo sổ, gửi, rút tiền...
    * Lớp CSDL: lưu trữ thông tin các bảng của chương trình bao gồm thông tin người dùng, thông tin sổ tiết kiệm, lịch sử giao dịch.
+ Mô hình 3 lớp này triển khai trên 1 tầng - tức chỉ triển khai phần mềm chạy trên local.

## Quản lý phiên bản
+ Nhóm sử dụng SVN để làm chương trình quản lý phiên bản
+ Sử dụng Tortoise làm SVN client
+ Sử dụng Google Code làm SVN server

http://da-cnpm-uit-se7.googlecode.com/svn/trunk/ da-cnpm-uit-se7-read-only

## Quản lý tiến độ - Bug tracker (Issues on Google Code)

## Kế hoạch kiểm thử đơn vị (Testing)
+ Nhóm có kế hoạch sử dụng 2 phương pháp kiểm thử là kiểm thử hộp trắng và kiểm thử hộp đen
+ Kiểm thử hộp trắng:
    * Report cụ thể
    * Sau khi hoàn thành một module sẽ được đưa vào quy trình kiểm thử hộp trắng.
    * 
+ Kiểm thử hộp đen
    * Hoàn thành chương trình sẽ được kiểm thử theo phương pháp hộp đen
    * Đảm bảo các chức năng của chương trình hoạt động như dự kiến, người kiểm thử trong bước kiểm thử hộp đen không tham gia code.
+ [] Nhắc lại về yêu cầu của bản thiết kế PM -> PM sau khi code đã đáp ứng được hay chưa?
+ [ ] Thực hiện công việc đúng như kỳ vọng?
+ [ ] Có thể triển khai với các đặc tính tương tự
+ [ ] Đáp ứng đưọc mọi nhu cầu của các bên liên quan?

### Ngân hàng cần gì?
+ Cơ chế sao lưu, bảo mật
+ PM làm việc một cách khoa học, dữ liệu được ràng buộc chặt chẽ.

### Xác định các khiếm khuyết của chương trình
+ Yêu cầu thiết kế PM thiếu:
    * Sao lưu dữ liệu
    * Hiệu suất - Truy cập, quản lý từ xa
    * Bảo mật CSDL
    * Mở rộng tính năng

## Code Convention (C#)
+ Về Code Conventions, do nhóm sử dụng ngôn ngữ C# nên nhóm quyết định tuân theo chuẩn mực từ [MSDN](http://msdn.microsoft.com/en-us/library/ff926074.aspx)
