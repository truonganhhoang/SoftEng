## Công nghệ phần mềm

### Quy trình phần mềm
---

### Đặc tả phần mềm( Specifications )
#### Giới thiệu

- Đặc tả phần mềm kết nối khách hàng với đội ngũ phát triển:
    -  Khách hàng có thể chắc chắn phần mềm làm ra sẽ có những tính năng một cách chi tiết mà họ muốn
    -  Đội phát triển sử dụng tài liệu này để triển khai thiết kế và cài đặt những tính năng và khách hàng yêu cầu
- Trong các phương thức theo kiểu agile, tài liệu đặc tả một hệ thống sẽ được hoàn tất trong giai đoạn cuối của quá trình xây dựng hệ thống vì:
    - Khi lập trình viên bắt tay vào xây dựng chi tiết ở các tầng phía dưới sẽ nảy sinh một số vấn đề không lường trước
    => Phải chỉnh sửa tài liệu đặc tả và cập nhật với khách hàng.
---

#### Quá trình đặc tả các yêu cầu (Requirements Process)
- Các yêu cầu được chia ra làm 2 nhánh chính:
    - Các yêu cầu chức năng (Những gì hệ thống có thể thực hiện ?)
        vd: người dùng có thể đăng xuất với 1 click
    - Các yêu cầu phi chức năng (Những gì hệ thống nên có ?):
        -  Dễ sử dụng       
        -  Hiệu năng tốt
        -  Khả năng mở rộng
        -  Độ tin cậy
        -  Độ phức tạp
        -  Khả năng kiểm tra, bảo trì
        + vd: người dùng có thể đăng nhập bằng tài khoản google, phần mềm có khả năng chạy trên cả điện thoại lẫn máy tính,..
---
- Mỗi bên liên quan( stackholders) có thể có các yêu cầu phi chức năng khác nhau
    - Khách hàng quan tâm đến tính dễ sử dụng, hiệu năng, khả năng nâng cấp,..
    - Đội phát triển quan tâm đến độ tin cậy, độ phức tạp, khả năng kiểm thử, bảo trì,...

- Các yêu cầu phi chức năng có thể mâu thuẫn với nhau
    - VD: đội phát triển cần 1 phần mềm có ít cài đặt phức tạp nhưng khách hàng lại muốn phần mềm có hiệu năng cao( cần phải cài đặt phức tạp)
    - => Các bên liên quan cần phải thống nhất với nhau về độ ưu tiên của các yêu cầu phi chức năng
- Lưu ý: Khi làm tài liệu về yêu cầu ta chỉ cần chỉ rõ những việc hệ thống sẽ làm chứ không cần quan tâm hệ thống sẽ làm những điều đó bằng cách nào