# Công nghệ phần mềm: Giới thiệu
## Quy trình
* Tổng quan module
*  Why process?
*  Quy trình cổ điển

---
## Tổng quan module
### Tổng quan
Trong module này, chúng ta sẽ khám phá quy trình phát triển phần mềm có thể giúp tạo ra đa dạng các hoạt động phức tạp để xây dựng hệ thống hiện đại như thế nào. Sử dụng trong công nghiệp, chúng tôi sẽ thảo luận về những lợi ích và hạn chế của từng phương pháp, cũng như cách chọn quy trình tốt nhất cho nhóm và dự án cụ thể của bạn.
### Mục tiêu
1. Tìm hiểu về các bên liên quan và các loại tài liệu họ sử dụng để liên lạc trong quá trình phát triển phần mềm.
2. Tìm hiểu về quy trình phần mềm truyền thống, bao gồm cả phương thức thác nước và xoắn ốc.
3. Tìm hiểu về quy trình phầm mềm linh hoạt hiện đại, lập trình cực hạn, hướng phát triển thử nghiệm, và phương pháp scrum.

---
## Quy trình phần mềm

### Why Process ?

---

### Quá trình 

- Chúng ta đang cố gắng xây dựng cái gì ?
- Ai là người tham gia vào toàn bộ quá trình phát triển phần mềm?
- Các nhóm sẽ phối hợp với nhau như thế nào ? Họ sẽ thực sự xây dựng hệ thống như thế nào ?
- Khi nào tất cả sẽ được hoàn thành ?

---

### Stakeholders

- Xây dựng hệ thống phần mềm liên quan đến sự hợp tác của nhiều dự án của các bên liên quan.
    - Developers 
    - QA team 
    - Management 
    - Sales and marketing team 
    - Users 
    - Support team 

---

### Stakeholders

- Developers (nhà phát triển):
    - Biến ý tưởng, tài liệu thành sản phẩm 

- QA team ( Đội kiểm định chất lượng ): 
    - Xác nhận sản phẩm hoạt động, đảm bảo rằng sản phẩm có thể chạy trong thực tế và có thể triển khai
    
- Management ( Quản lý ): 
    - Tham gia để giúp phối hợp giữa các nhóm khác nhau.

---

### Stakeholders

- Sales and marketing team ( Đội bán hàng )
    - Bán sản phẩm cho khách hàng

- Users ( Người dùng ) 
    - Người sử dụng sản phẩm. Chúng ta hy vọng họ sẽ gửi lại những phản hồi về sản phẩm.

- Support team ( Đội hỗ trợ )
    - Đội hỗ trợ người dùng liên tục, cung cấp phản hồi của người dùng cho đội kỹ thuật.

---

- Các bên liên quan phải giao tiếp hiệu quả và có sự đồng thuận về cách xây dựng hệ thống phần mềm.

    - => Cần những tài liệu và quy trình khác nhau để giúp mọi người hiểu rõ việc cần làm
    - và chúng sẽ được thay đổi tùy theo nền tảng và kinh nghiệm của các stakeholders.

---

### Documentation

- Specification : tài liệu đặc tả hệ thống
- Development : tài liệu về phong cách phát triển
- Vacidation : tài liệu xác nhận
- Deployment / Evolution : Các tài liệu triển khai và nâng cấp.

--- 

### Documentation

- Specification

    - Đưa ra nhiệm vụ, mục tiêu kinh doanh, và yêu cầu bản thân.
    - Chủ yếu dành cho bên quản lý, người dùng, bán hàng ( những bên xác định hệ thống cần chức năng gì ) 

- Development

    - Kế hoạch kiến trúc hệ thống, kế hoạch thiết kế, kế hoạch thực hiện
    - Chủ yếu dành cho bên quản lý, đội phát triển và đội kiểm định chất lượng

---

### Documentation

- Vacidation

    - Kế hoạch kiểm tra sản phẩm, đánh giá rủi ro
    - Đặc biệt quan trọng cho đội kiểm định chất lượng
   
- Deployment / Evolution
 
    - Bao gồm kế hoạch phát triển và chiến lược bảo trì

---

### Documentation

- => Tài liệu là một cơ chế chủ chốt để giảm thiểu rủi ro liên quan đến việc xây dựng các sản phẩm phần mềm bằng cách đảm bảo rằng tất cả mọi người làm việc trên cùng một kế hoạch và hiểu rõ những gì đang được xây dựng, điều gì sẽ xảy ra và khi nào được thực hiện.

 




## Quy trình cổ điển: Thác nước và xoắn ốc
---
### Mô hình thác nước
* Đặc tả yêu cầu
* Thiết kế
* Cài đặt
* Tích hợp
* Bảo trì

---
### Mô hình thác nước
#### 1. Đặc tả yêu cầu:
Nhằm xác định các đơn vị mà hệ thống phải cung cấp các ràng buộc trong quá trình vận hành và phát triển, đồng thời xác định mục tiêu đặt ra với hệ thống là gì qua việc bàn với khách hàng, sau đó tư liệu hóa các yêu cầu thu được trong tài liệu.

---
### Mô hình thác nước
#### 2. Thiết kế:
Phân chia các yêu cầu cho hệ thống phần mềm, phần cứng, sau đó thiết lập nên các kiến trúc hệ thống phần mềm. Tiếp theo tiến hành thiết kế phần mềm bằng cách xây dựng và mô tả hệ thống phần mềm con cấu thành nên phầm mềm được xây dựng, và quan hệ giữa các hệ thống.

---
### Mô hình thác nước
#### 3. Cài đặt:
Chuyển bản thiết kế thành một tập hợp các chương trình hoặc các đơn vị chương trình.

---
### Mô hình thác nước
#### 4. Tích hợp:
Các đơn vị chương trình được tích hợp lại với nhau tạo thành hệ thống hoàn chỉnh.


---
### Mô hình thác nước
#### 5. Bảo trì:
Đưa phần mềm vao tiến hành sử dụng trong thực tế và tiến hành các sửa đổi cầ thiết nếu người dùng phát hiện ra khiếm khuyết.
### Mô hình thác nước
* Là mô hình cổ điển
* Phương pháp áp dụng một lần
* Điều khiển hiệu quả
* Phạm vi giới hạn của vòng lặp
* Vòng đời dài
* Không thích hợp với các hệ thống không rõ ràng
* Trong mô hình thác nước, năm pha trên phải thực hiện một cách tuần tự, kết thúc pha trước rồi mới thực hiện pha tiếp theo.
* Mô hình này chỉ thích hợp khi yêu cầu đã đuợc làm rõ ràng và những thay đổi sẽ được giớ hạn một cách rõ ràng trong quá trình thiết kế.


---

### Mô hình thác nước
#### Ưu điểm:
* Phù hợp với các dự án nhỏ và có yêu cầu xác định.
* Dễ phân công công việc.
* kiến trúc ổn định.
#### Nhược điểm:
* Không phù hợp với dự án lớn.
* Thời gian thực hiện lâu.
---
### Phương pháp xoắn ốc 
Phương pháp xoắn ốc xuất hiện trong những năm 1980 như là một sự cải tiến đối với những thiếu sót của các chiến lược phát triển thác nước truyền thống. Trong mô hình xoắn ốc, điều quan trọng cần lưu ý là chúng ta sẽ tạo ra sản phẩm nhiều lần, có thể xác nhận với khách hàng trước khi chúng ta tiếp tục phát triển và mở rộng sản phẩm.
Phương pháp xoắn ốc xuất hiện trong những năm 1980 như là một sự cải tiến đối với những thiếu sót của các chiến lược phát triển thác nước truyền thống. Trong mô hình xoắn ốc, điều quan trọng cần lưu ý là chúng ta sẽ tạo ra sản phẩm nhiều lần, có thể xác nhận với khách hàng trước khi chúng ta tiếp tục phát triển và mở rộng sản phẩm.
1.	Lên kế hoạch Sự khởi đầu khi phát triển dự án theo phương pháp xoắn ốc,điều đầu tiên chúng ta cần làm, chính là lập kế hoạch. Đây là nơi chúng ta tìm ra những yêu cầu cho phiên bản, cho nguyên mẫu trong tương lai.
---
2.	Phân tích rủi ro Tiếp theo, chúng ta sẽ đi vào phân tích rủi ro. Trong phân tích rủi ro, chúng ta sẽ tìm ra những gì có thể sai. Các nguồn rủi ro có trong phiên bản, trong nguyên mẫu này là gì?
---

3.	Kỹ thuật Kỹ thuật về cơ bản là quá trình phát triển phần mềm. Đây là nơi mà chúng ta sẽ triển khai hệ thống và xây dựng nó.
---
4.	Xác nhận Trong giai đoạn xác nhận của một dự án với mô hình xoắn ốc, chúng ta sẽ lấy nguyên mẫu và kiểm tra với khách hàng để chắc chắn rằng nó thực sự xây dựng và cung cấp chức năng mà họ thực sự muốn. Chúng ta sẽ chủ động thu thập phản hồi của khách hàng ở đây.
---
### Ưu điểm:  
Xây dựng một sản phẩm sai có lẽ là nguyên nhân phổ biến nhất khiến các hệ thống thất bại trong thực tế. Mô hình xoắn ốc thực sự đang cố gắng để giải quyết rủi ro này bằng cách kết nối với khách hàng cuối mỗi phiên bản thiết kế để chắc chắn rằng sản phẩm đáp ứng nhu cầu của họ.
### Nhược điểm: 
Chờ phản hồi của khách hàng cũng có thể thực sự làm chậm quá trình phát triển phần mềm. Khách hàng có thể trì hoãn hoặc đưa ra phản hồi ngay lập tức.
