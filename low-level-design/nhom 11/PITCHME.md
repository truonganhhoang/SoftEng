## THIẾT KẾ CẤP THẤP
### (Low Level Design)
---
### GIỚI THIỆU
 #### Ba quy tắc vận hành:

1) Gói gọn những gì thay đổi.

 * Áp dụng các quy tắc thiết kế trong thực hành.
 * Thiết kế hệ thống để đảm bảo dễ dàng mở rộng, phù hợp với những yêu cầu trong tương lai.
---
 #### Ba quy tắc vận hành:
 
2) Đảm bảo việc thiết kế các giao diện.

 * Có thể tái sử dụng các thành phần trong hệ thống.
 * Thu gọn hệ thống và dễ dàng sử dụng trong tương lai.
---
 #### Ba quy tắc vận hành:
 
3) Ưu tiên các thành phần thừa kế.

 * Các thành phần dễ phát triển trong tương lai.
 * Cho phép mềm dẻo và linh hoạt hơn.
 
---

### KHÁI QUÁT CÁC MẪU THIẾT KẾ

 * Cung cấp một bộ quy tắc để hệ thống phần mềm có thể tránh được những vấn đề có thể xảy ra.
 * Đưa ra một từ vựng chung để phổ biến giữa các nhà phát triển.
 * Mỗi khi thêm một mẫu thiết kế là thêm một trừu tượng.
---

#### CÁC MẪU THIẾT KẾ GỒM 3 PHẦN CHÍNH

1. Đều có 1 bộ ưu, nhược điểm chung liên kết với chúng phải chắc chắn có thể giải quyết các nhược điểm.
2. Có 1 từ vựng chung giữa các nhà phát triển, tránh việc rườm rà khi thảo luậ về các mẫu thiết kết.
3. Không nên áp dụng chúng 1 cách máy móc.

---

#### CÁC MẪU THIẾT KẾ CÓ BA LOẠI

 * Mẫu thiết kế khởi tạo : xây dựng object bằng cách mở rộng (extend).
 * Mẫu thiết kế cấu trúc: tránh được những vấn đề tiến triển trong tương lai.
 * Mẫu thiết kế hành vi: giúp dễ dàng hơn trong việc thêm các hành vi vào hệ thống tại runtime.

---

### MẤU THIẾT KẾ SINGLETON

![alt](https://allaravel.com/wp-content/uploads/2017/07/singleton-pattern-uml.png)

* Là mô hình thiết kế khởi tạo và là mẫu thiết kế đơn giản nhất.
---

#### TỔNG QUAN

* Để sử dụng rộng rãi một đối tượng (object) trong hệ thống nhưng không truyền thể hiện (instance) của object tới nơi muốn sử dụng, hoặc chỉ muốn có một thể hiện duy nhất của object.
* Không thể gọi constructor vì nó được xây dựng riêng biệt (private), mà phải gọi phương thức tĩnh getInstance để trả về thể hiện của đối tượng.
* Nếu đối tượng chưa được gán, hoặc các trường (field) là null, nó sẽ gọi hàm khởi tạo riêng.

---

#### MỘT SỐ HẠN CHẾ CỦA SINGLETON

* Sẽ phát sinh một số phức tạp nếu sử dụng nó với ngôn ngữ đa luồng.
* Thường được sử dụng trong các mẫu thiết kế khác.
* Là một biến toàn cục, cần xem xét nếu muốn phổ biến trong toàn bộ thiết kế vì chúng tỏ ra yếu kém trong việc theo dõi tình trạng của hệ thống.
* Vai trò của phương thức tĩnh khá hạn chế và cố định.
* Khiến việc kiểm tra code khó hơn.

---

### MẪU THIẾT KẾ CHIẾN LƯỢC STRATEGY

![alt](https://allaravel.com/wp-content/uploads/2017/07/Strategy-pattern-uml.png)

---

#### TỔNG QUAN

* Dễ dàng thay đổi phần mềm khi có nhu cầu mới.
* Cung cấp một giao diện chiến lược mới để có thể tiến hành bổ sung các chức năng mới cho hệ thống.
* Những gì mà mẫu thiết kế làm là ẩn các thông tin cụ thể của triển khai thuật toán khỏi client.
* Các mãu thiết kế chiến lược có thể thay đổi để bổ sung đặc tính mới, chứ không phải thay đổi chúng.

---

### MẪU THIẾT KẾ TRẠNG THÁI STATE

![alt](https://i2.wp.com/www.dofactory.com/images/diagrams/net/proxy.gif)

---

#### TỔNG QUAN

* Dễ dàng mở rộng các các chức năng của phần mềm.
* Thay đổi chương trình theo cơ chế động.
* Không phải sửa đổi các client khác nhau phụ thuộc vào trạng thái đã tồn tại trước đó.
* Mang lại một cơ chế làm các trạng thái độc lập hơn và có thể tự chứa chính nó.

