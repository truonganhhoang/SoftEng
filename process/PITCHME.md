# Công nghệ phần mềm: Giới thiệu
## Quy trình
*  Tổng quan module
*  Vì sao cần phải xây dựng quy trình ?
*  Quy trình cổ điển

---
## Tổng quan module
### Tổng quan
- Trong module này, chúng ta sẽ khám phá quy trình phát triển phần mềm có thể giúp tạo ra đa dạng các hoạt động phức tạp để xây dựng hệ thống hiện đại như thế nào. Sử dụng trong công nghiệp, chúng tôi sẽ thảo luận về những lợi ích và hạn chế của từng phương pháp, cũng như cách chọn quy trình tốt nhất cho nhóm và dự án cụ thể của bạn.

---
### Mục tiêu
1. Tìm hiểu về các bên liên quan và các loại tài liệu họ sử dụng để liên lạc trong quá trình phát triển phần mềm.
2. Tìm hiểu về quy trình phần mềm truyền thống, bao gồm cả phương thức thác nước và xoắn ốc.
3. Tìm hiểu về quy trình phầm mềm linh hoạt hiện đại, lập trình cực hạn, hướng phát triển thử nghiệm, và phương pháp scrum.

--- 
## Quy trình phần mềm

### Vì sao cần phải xây dựng quy trình ?

---

### Quá trình 
- Xây dựng quy trình chính là trả lời các câu hỏi:
    - Chúng ta đang cố gắng xây dựng cái gì ?
    - Ai là người tham gia vào toàn bộ quá trình phát triển phần mềm?
    - Các nhóm sẽ phối hợp với nhau như thế nào ? Họ sẽ thực sự xây dựng hệ thống như thế nào ?
    - Khi nào tất cả sẽ được hoàn thành ?

---
### Các bên liên quan

- Xây dựng hệ thống phần mềm liên quan đến sự hợp tác của nhiều dự án của các bên liên quan.
    - Nhà phát triển (Developers) 
    - Đội kiểm định chất lượng (QA team)
    - Quản lý (Management)
    - Đội tiếp thị và bán hàng  (Sales and marketing team)
    - Người dùng (Users)
    - Đội hỗ trợ (Support team)

---
### Các bên liên quan

- Nhà phát triển (Developers):
    - Biến ý tưởng, tài liệu thành sản phẩm 
- Đội kiểm định chất lượng (QA team): 
    - Xác nhận sản phẩm hoạt động, đảm bảo rằng sản phẩm có thể chạy trong thực tế và có thể triển khai
- Quản lý (Management): 
    - Tham gia để giúp phối hợp giữa các nhóm khác nhau.

---
### Các bên liên quan

- Đội tiếp thị và bán hàng  (Sales and marketing team):
    - Bán sản phẩm cho khách hàng
- Người dùng (Users): 
    - Người sử dụng sản phẩm. Chúng ta hy vọng họ sẽ gửi lại những phản hồi về sản phẩm.
- Đội hỗ trợ (Support team):
    - Đội hỗ trợ người dùng liên tục, cung cấp phản hồi của người dùng cho đội kỹ thuật.

---
### Các bên liên quan
- Các bên liên quan phải giao tiếp hiệu quả và có sự đồng thuận về cách xây dựng hệ thống phần mềm.

    - => Cần những tài liệu và quy trình khác nhau để giúp mọi người hiểu rõ việc cần làm và chúng sẽ được thay đổi tùy theo nền tảng và kinh nghiệm của các stakeholders

---
### Tài liệu

- Specification : tài liệu đặc tả hệ thống
- Development : tài liệu về phong cách phát triển
- Vacidation : tài liệu xác nhận
- Deployment / Evolution : Các tài liệu triển khai và nâng cấp.

--- 
### Tài liệu

- Specification (Tài liệu đặc tả):
    - Đưa ra nhiệm vụ, mục tiêu kinh doanh, và yêu cầu bản thân.
    - Chủ yếu dành cho bên quản lý, người dùng, bán hàng ( những bên xác định hệ thống cần chức năng gì ) 
--- 
### Tài liệu
- Development (Tài liệu phát triển):

    - Kế hoạch kiến trúc hệ thống, kế hoạch thiết kế, kế hoạch thực hiện
    - Chủ yếu dành cho bên quản lý, đội phát triển và đội kiểm định chất lượng

---
### Tài liệu

- Vacidation (Tài liệu xác nhận):
    - Kế hoạch kiểm tra sản phẩm, đánh giá rủi ro
    - Đặc biệt quan trọng cho đội kiểm định chất lượng
   
- Deployment / Evolution (Tài liệu triển khai và nâng cấp):
    - Bao gồm kế hoạch phát triển và chiến lược bảo trì

---
### Tài liệu

- => Tài liệu là một cơ chế chủ chốt để giảm thiểu rủi ro liên quan đến việc xây dựng các sản phẩm phần mềm bằng cách đảm bảo rằng tất cả mọi người làm việc trên cùng một kế hoạch và hiểu rõ những gì đang được xây dựng, điều gì sẽ xảy ra và khi nào được thực hiện.



---
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
- Xác định các đơn vị mà hệ thống phải cung cấp các ràng buộc trong quá trình vận hành và phát triển
- xác định mục tiêu đặt ra với hệ thống là gì qua việc bàn với khách hàng, sau đó tư liệu hóa các yêu cầu thu được trong tài liệu.

---
### Mô hình thác nước
#### 2. Thiết kế:
- Phân chia các yêu cầu cho hệ thống phần mềm, phần cứng, thiết lập nên các kiến trúc hệ thống phần mềm.
- Tiến hành thiết kế phần mềm bằng cách xây dựng và mô tả hệ thống phần mềm con cấu thành nên phầm mềm được xây dựng, và quan hệ giữa các hệ thống.

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

---
### Mô hình thác nước
* Là mô hình cổ điển
* Phương pháp áp dụng một lần
* Điều khiển hiệu quả
* Phạm vi giới hạn của vòng lặp
* Vòng đời dài
---
### Mô hình thác nước
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

- Phương pháp xoắn ốc xuất hiện trong những năm 1980 như là một sự cải tiến đối với những thiếu sót của các chiến lược phát triển thác nước truyền thống.
- Sẽ tạo ra sản phẩm nhiều lần, có thể xác nhận với khách hàng trước khi chúng ta tiếp tục phát triển và mở rộng sản phẩm.

---
### Phương pháp xoắn ốc

1. Lên kế hoạch: 
    - Lên kế hoạch hởi đầu khi phát triển dự án theo phương pháp xoắn ốc. Tìm ra những yêu cầu cho phiên bản, cho nguyên mẫu trong tương lai.
    
--- 
### Phương pháp xoắn ốc
2. Phân tích rủi ro Tiếp theo: 
    - Tìm ra những gì có thể sai, các nguồn rủi ro.
    
---
### Phương pháp xoắn ốc
3. Kỹ thuật:
    - Kỹ thuật về cơ bản là quá trình phát triển phần mềm, là nơi  triển khai hệ thống và xây dựng phần mềm.
    
---
### Phương pháp xoắn ốc
4. Xác nhận:
    - Lấy nguyên mẫu và kiểm tra với khách hàng để chắc chắn rằng nó thực sự xây dựng và cung cấp chức năng mà họ thực sự muốn. 
    - Chủ động thu thập phản hồi của khách hàng.

---
### Phương pháp xoắn ốc
- Ưu điểm:
    - Xây dựng một sản phẩm sai có lẽ là nguyên nhân phổ biến nhất khiến các hệ thống thất bại trong thực tế. Mô hình xoắn ốc cố gắng giải quyết rủi ro này bằng cách kết nối với khách hàng cuối mỗi phiên bản thiết kế để chắc chắn rằng sản phẩm đáp ứng nhu cầu của họ.

---
### Phương pháp xoắn ốc
- Nhược điểm: 
    - Chờ phản hồi của khách hàng cũng có thể thực sự làm chậm quá trình phát triển phần mềm. Khách hàng có thể trì hoãn hoặc đưa ra phản hồi ngay lập tức.



### Quy trình phần mềm
- [Đặc tả phần mềm (specifications)](https://gitpitch.com/jindojojin/softeng/master?p=process/Specification#/
---
Nhóm 3
---

## EXETREME PROGRAMMING

* Agile
* XP 

---

## Phương pháp Agile

- Xuất hiện đầu những năm 2000
- Như 1 hướng đi mới vượt trội so với phương pháp phát triển truyền thống
- Cho phép người phát triển trở nên linh hoạt hơn và sớm hoàn thiện với tốc độ cao
- Tuyên ngôn Agile

---

### Tuyên ngôn Agile
Gồm 12  nguyên lý chính,nhưng có thể rút gọn thành 4 nguyên lý cơ bản:

- Nhấn mạnh vào con người hơn là tài liệu và quy trình
- Tập trung vào sản phẩm hơn là tập trung vào tài liệu
- Khách hàng tham gia trực tiếp vào quá trình phát triển phần mềm
- Nhanh nhẹn trong kế hoạch

---

## XP
- Là nhân tố đầu tiên ảnh hưởng đến phương pháp Agile
- Cốt lõi của XP là có thể bàn giao sản phẩm bất cứ lúc nào
- Team phát triển sẽ bắt đầu từng bước nhỏ và lớn dần theo thời gian đáp lại sự phản hồi của khách hàng
- Đây là sự tương phản với nhiều cách tiếp cận truyền thống
- Đối với XP, ta bắt đầu từ dưới lên

---

## 5 nguyên tắc chính
XP tuân theo 5 nguyên tắc chính:
- Giao tiếp
- Giải pháp đơn giản, khả thi nhất
- Phản hồi
- Can đảm
- Sự tôn trọng

---

## Giao tiếp
* XP khuyến khích lập trình viên tương tác vói nhau
* Khuyến khích pair programming và pair review

---

## Giải pháp đơn giản, khả thi nhất
* Tập trung phát triển những tính năng quan trọng và cơ bản nhất
* Đảm bảo sản phẩm luôn sẵn sàng bàn giao cho khách hàng (ready to delivery)

---

## Phản hồi
* Luôn tiếp nhận phản hồi của khách hàng.
* Khuyến khích khách hàng trực tiếp tham gia vào quá trình phát triển

---

## Can đảm
* Sẵn sàng bỏ đi những tính năng không quan trọng đối với khách hàng
* Tiếp nhận mọi ý kiến cả tích cực lẫn tiêu cực của khách hàng

---

## Sự tôn trọng
* Tôn trọng những ý kiến đóng góp của đội phát triển và khách hàng

---

### SCRUM

* SCRUM là hình thức chung nhất của phương pháp Agile sử dụng trong làm việc thực tế ngày nay
* Trong Scrum chúng ta có product backlog - đại diện cho các vấn đề về chức năng, lỗi và những phần đã được sửa chữa trong 1 sản phẩm
* Làm việc trong "Sprint" trong suốt từ 1 đến 3 tuần với mỗi project backlog
---

# SCRUM
nhân sự trong SCRUM bao gồm:
* PRODUCT OWNER
* SCRUM MASTER
* TEAM

---

## PRODUCT OWNER

* Người được khách hàng uỷ quyền hay chính là khách hàng
* Vai trò cơ bản của họ là ưu tiên và đánh giá các vấn đề mà team sẽ làm trong 1 "Sprint" 

---

## SCRUM MASTER

* Công việc của SCRUM MASTER là quản lý quá trình phát triển
* Họ không trực tiếp quản lý team nhưng họ quản lý quá trình phát triển của team
* Họ đảm bảo team vẫn được theo dõi và làm việc trên những vấn đề quan trọng của "Sprint" mà PRODUCT OWNER đã ưu tiên

---

## TEAM

* Team theo Scrum thường có 5 đến 7 người và giữ nhịp 1 cách kỷ luật
* Team cần có những người phát triển tốt, QA (Quality Assurance) và tất cả trong cùng SCRUM team, làm việc cùng nhau để phát triển 1 sản phẩm

---
# SCRUM

* PRODUCT BACKLOG
* PLANNING
* SPRINT BACKLOG

---

### PRODUCT BACKLOG

* Như đã đề cập trước đó, product backlog là tất cả các vấn đề được chỉ định cho team phát triển
* Một phần quan trọng của quá trình Scrum là tiến thẳng đến PRODUCT BACKLOG và tìm ra một quá trình lên kế hoạch toàn diện, những tập con bạn sẽ giải quyết trong một "Sprint"

---


### PRODUCT BACKLOG (tiếp)
* Một khi kết thúc Sprint (trong 1 đến 3 tuần liền) với một định hướng cố định, việc ghi chú rất quan trọng, mỗi team sẽ biết "Sprint" diễn ra trong bao lâu.
* Khi Sprint kết thúc sản phẩm có thể bàn giao ngay nên bạn cần đảm bảo ràng các vấn đề chọn từ PRODUCT BACKLOG cho Sprint có thể đạt được trong khoảng thời gian chỉ định cho "Sprint"

---

### PLANNING

Quá trình lên kết hoạch là một bước rất quan trọng

* PRODUCT OWNER mong muốn team phát triển chức năng quan trọng,mang lại nhiều giá trị nhất cho mình
* Đồng thời, team kỹ thuật sẽ cân nhắc về khả năng của team có thể phát triển chức năng ấy trong 1 Sprint hay không!
---

### SPRINTS

Là tập hợp các vấn đề mà team phát triển sẽ phát triển trong 1 khoảng thời gian

---

#### STAND-UP MEETING
* Được diễn ra hàng ngày
* Team gặp nhau sẽ cùng nhau thảo luận từ 10 đến 15 phút như là team cập nhật tình những gì đã làm và sẽ làm những gì tiếp theo

---

#### CEREMONY PHASE

* Đây là giai đoạn mà chúng ta đánh giá về "Sprint"
* Đây cũng là nơi team kỹ thuật đi đến và giới thiệu những đặc tính mà họ thêm vào sản phẩm
* Đây là cơ hội để họ phản ảnh được cụ thể những thứ được xây dựng trên các "Sprint". 
