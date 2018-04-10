## Công nghệ phần mềm

### Quy trình phần mềm
---

### Đặc tả phần mềm( Specifications )
#### Giới thiệu

- Đặc tả phần mềm kết nối khách hàng với đội ngũ phát triển lại với nhau:
    -  Khách hàng có thể chắc chắn phần mềm làm ra sẽ có những tính năng một cách chi tiết mà họ muốn
    -  Đội phát triển sử dụng tài liệu này để triển khai thiết kế và cài đặt những tính năng mà khách hàng yêu cầu
---
- Trong các phương thức theo kiểu agile, tài liệu đặc tả một hệ thống sẽ được hoàn tất trong giai đoạn cuối của quá trình xây dựng hệ thống vì:
    - Khi lập trình viên bắt tay vào xây dựng chi tiết ở các tầng phía dưới sẽ nảy sinh một số vấn đề không lường trước
    => Phải chỉnh sửa tài liệu đặc tả và cập nhật với khách hàng.
---
#### Xử lý các yêu cầu (Requirements Process)
- Các yêu cầu quy trình được chia ra làm 2 nhánh chính:
    - Các yêu cầu chức năng (Những gì hệ thống có thể thực hiện ?)
        + vd: người dùng có thể đăng xuất với 1 click
    - Các yêu cầu phi chức năng (Những gì hệ thống nên có ?):
        + vd: người dùng có thể đăng nhập bằng tài khoản google, phần mềm có khả năng chạy trên cả điện thoại lẫn máy tính,..
---
- Mỗi bên liên quan( stackholders) có thể có các yêu cầu phi chức năng khác nhau
    - Khách hàng quan tâm đến tính dễ sử dụng, hiệu năng, khả năng nâng cấp,..
    - Đội phát triển quan tâm đến độ tin cậy, độ phức tạp, khả năng kiểm thử, bảo trì,...
---
- Các yêu cầu phi chức năng có thể mâu thuẫn với nhau
    - VD: đội phát triển cần 1 phần mềm có ít cài đặt phức tạp nhưng khách hàng lại muốn phần mềm có hiệu năng cao( cần phải cài đặt phức tạp)
    - => Các bên liên quan cần phải thống nhất với nhau về độ ưu tiên của các yêu cầu phi chức năng
- Lưu ý: Khi làm tài liệu về yêu cầu ta chỉ cần chỉ rõ những việc hệ thống sẽ làm chứ không cần quan tâm hệ thống sẽ làm những điều đó bằng cách nào

---
#### Đặc điểm của các yêu cầu( Requirements Properties)
- Các yêu cầu phải đảm bảo 4 điều kiện:
	- Hoàn thiện
	- Nhất quán
	- Chính xác
	- Xúc tích	
	
---
#### Thu thập yêu cầu( Requirements Elicitation)
Quá trình đặc tả phần mềm là lặp đi lặp lại các bước:
- Thu thập(Elicitation): Các bên liên quan sẽ cùng nhau đưa ra các yêu cầu cho phần mềm và chỉ rõ những yêu cầu nào sẽ được thực hiện/không được thực hiện
- Phân tích(Analysis): Kiểm tra những yêu cầu đã được thu thập để chắc chắn các yêu cầu là nhất quán và không ảnh hưởng đến các yêu cầu còn lại
- Cụ thể hóa(Reification): Viết các yêu cầu dưới dạng ngôn ngữ quy chuẩn đã có ( vd: user cases hoặc user stories )
	- Thẩm định(Validation): Mang danh sách các yêu cầu để xác nhận lại với khách hàng
--- 
#### Các yêu cầu khác (Additional Requirements)
- Giàng buộc thiết kế (Design Constraints) 
- Giàng buộc về môi trường(Environmental Constraints)
- Sở thích của khách hàng( Preference)