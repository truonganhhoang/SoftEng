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
# EXETREME PROGRAMMING

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
Gồm 12 khoá nguyên lý, nhưng chỉ có 4 nguyên lý trong đó giải nghĩa được mục đích của các tài liệu

- Tương tác cá nhân giữa các quá trình và công cụ
- Làm phần mềm trên những tài liệu chuyên biệt
- Khách hàng tương tác trên những hợp đồng đàm phán
- Nhanh nhẹn trong kế hoạch

---

#### Tương tác giữa các quá trình và công cụ
Giá trị thực sự giữa các bên, những người tham gia vào quá trình phát triển phần mềm

---
#### Làm phần mềm trên những tài liệu tham khảo chuyên biệt

Trong cách tiếp cận Agile, một chủ đề chung chúng ta thường thấy là phần mềm có khả năng xây dựng và thực thi được

---
#### Khách hàng tương tác trên những hợp đồng đàm phán
Mang lại khách hàng cho team phát triển vì thế chúng ta cần nhận sự phản hồi và trả lời nhanh và hiệu quả

---

#### Nhanh nhẹn trong kế hoạch
Sự linh hoạt trong các loại phản hồi mà khách hàng đưa cho người phát triển và người phát triển trả lời bằng những gì đạt được trong sản phẩm, đó là những gì khách hàng cần và mong muốn

---

- Những nguyên tắc trên được phát triển để tăng trách nhiệm với khách hàng trong team phát triển
- Bằng việc đưa khách hàng vào và tham gia quá trình phát triển, chúng ta có khả năng trả lời cả 2 thứ họ cần nhưng cần giữ họ cẩn thận với những thông báo những gì đang diễn ra như sản phẩm đang được phát triển
- Phương pháp Agile tăng vận tốc phát triển bằng cách giảm số lượng thời gian xây dựng những thứ không đúng
- Nên tránh những thứ sai vì khách hàng liên tục phản hồi trong suốt hướng đi của team phát triển
- Cho phép team có nhiều thí nghiệm hơn, thiết kế ra những phương án thay thế, tìm ra đâu là tốt nhất cho khách hàng
- Cho người phát triển thêm một chút linh hoạt

---

# XP
- Là nhân tố đầu tiên ảnh hưởng đến phương pháp Agile
- Cốt lõi của XP là hệ thống có thể thanh toán được tại mọi thời điểm
- Team phát triển sẽ bắt đầu từng bước nhỏ và lớn dần theo thời gian đáp lại sự phản hồi của khách hàng
- Đây là sự tương phản với nhiều cách tiếp cận truyền thống, nơi chúng ta bắt đầu cùng với 1 kế hoạch khổng lồ và cố gắng trong lúc khởi đầu sau đó xây dựng hệ thống từ trên xuống
- Đối với XP, ta bắt đầu từ dưới lên
- 5 khoá nguyên tắc

---

## 5 khoá nguyên tắc

- Giao tiếp
- Giải pháp đơn giản nhất - khả thi
- Phản hồi
- Can đảm
- Sự tôn trọng

---

### Giao tiếp

Khuyến khích các bên liên quan trao đổi với nhau tại mọi thời điểm. Nhờ vậy mà người phát triển có thể nhận được các phản hồ khả thi nhanh hơn

---

### Giải pháp đơn giản nhất - khả thi
Hơn cả những kỹ thuật sâu rộng, những giải pháp phức tạp, thứ chúng ta muốn xây dựng là 1 giải pháp đơn giản. Cố gắng thực hiện cùng khách hàng.

---

### Phản hồi

Trong giai đoạn phản hồi, khuyến khích khách hàng và người phát triển nói chuyện cùng nhau. Team phát triển luôn mong đợi những phản hồi từ khách hàng và cố gắng hành động dựa trên những phản hồi đó. Nhưng cũng có lúc team phát triển đẩy trở lại khách hàng và để họ biết khi phản hồi của họ sẽ không làm việc do quá đắt hoặc ngoài khả năng. Phản hồi theo 2 chiều, từ khách hàng đến người phát triển và ngược lại.

---

### Can đảm

Cố gắng thực hiện những thực nghiệm khác bên ngoài. Nhận phản hồi qua những thí nghiệm này, nếu chúng làm sản phẩm tốt hơn thì thật tuyệt vời. Nếu không đạt kết quả tốt thì hãy vứt nó đi. Không xem nó như sự sụt giảm về giá trị mà hãy xem nó như lợi ích học được để làm sản phẩm tốt hơn.

---

### Sự tôn trọng

Sự tôn trọng các ý kiến của các bên liên quan và thời gian của họ

---

### SCRUM

* SCRUM-BASED là hình thức chung nhất của phương pháp Agile sử dụng trong làm việc thực tế ngày nay
* Trong Scrum chúng ta có product backlog - thứ đại diện cho các vấn đề về đặc tính, lỗi và những phần đã được sửa chữa trong 1 sản phẩm
* Làm việc trong "giai đoạn nước rút" trong suốt từ 1 đến 3 tuần. Chúng ta làm dựa trên những thứ chúng ta đã biết(những công việc tồn đọng lại). Vì vậy, đây là tập hơp của những product backlog tức những sản phẩm chứa các vấn đề mà ta muốn làm việc trong 1 "giai đoạn nước rút" riêng.

---

### SCRUM

Phương pháp SCRUM-BASED không quy định chỉ thực hiện các kỹ thuật mà team đó cần dõi theo. Team sẽ tự tính toán những thứ họ hiểu rõ cho sản phẩm - thứ họ đang xây dựng. Nhưng tất cả những gì team SCRUM-BASED làm có 3 level cao của các bên liên quan

* PRODUCT OWNER
* SCRUM MASTER
* TEAM

---

## PRODUCT OWNER

* Là những người cư xử như những người được uỷ quyền khách hàng hay chính là khách hàng
* Vai trò cơ bản của họ là ưu tiên các vấn đề mà team đã làm trong 1 'giai đoạn nước rút' và đánh giá đầu ra của team để đảm bảo công việc mà team làm trên những vấn đề đó đúng như họ kỳ vọng

---

## SCRUM MASTER

* Công việc của SCRUM MASTER là quản lý quá trình phát triển
* Họ không phải những quản lý của team nhưng họ quản lý quá trình của team
* Họ đảm bảo team vẫn được theo dấu và làm việc trên những vấn đề quan trọng của 'quá trình nước rút' mà PRODUCT OWNER đã ưu tiên

---

## TEAM

* SCRUM-BASED team thường có 5 đến 7 người và giữ nhịp 1 cách kỷ luật
* Chúng ta luôn mong muốn có những người phát triển tốt, QA, và tất cả trong cùng SCRUM-BASED team, làm việc cùng nhau để phát triển 1 sản phẩm

---
# SCRUM

* PRODUCT BACKLOG
* PLANNING
* SPRINT BACKLOG

---

### PRODUCT BACKLOG

* Như đã đề cập trước đó, product backlog là tất cả các vấn đề được chỉ định cho team phát triển
* Một phần quan trọng của quá trình Scrum là tiến thẳng đến PRODUCT BACKLOG và tìm ra một quá trình lên kế hoạch toàn diện, những tập con bạn sẽ giải quyết trong một 'giai đoạn nước rút' riêng
* Mặc khi kết thúc 'giai đoạn nước rút' (trong 1 đến 3 tuần liền) nhưng với một định hướng cố định, việc ghi chú rất quan trọng, mỗi team sẽ biết 'giai đoạn nước rút diễn ra trong bao lâu'
* Khi 'giai đoạn nước rút' kết thúc sản phẩm cần trở nên có thể chuyển đổi nên bạn cần đảm bảo ràng các vấn đề chọn từ PRODUCT BACKLOG cho 'giai đoạn nước rút' có thể đạt được cùng với thời gian chỉ định cho 'giai đoạn nước rút'

---

### PLANNING

Quá trình lên kết hoạch là một bước rất quan trọng

* Nó sẽ được hoàn thành trong sự kết hợp với PRODUCT OWNER, vì PRODUCT OWNER sẽ có một vài khái niệm dựa trên những ưu tiên của họ là một trong những đặc tính của PRODUCT BACKLOG mà rất quan trọng với họ, thứ đem lại cho họ những thứ giá trị nhất.
* Nhưng trong cùng thời điểm, team kỹ thuật sẽ biết như thế nào là tốt - hoặc họ sẽ thảo luận cách tốt nhất để đưa ra các đặc tính. Bởi vì nếu họ hỏi về một đặc tính trong nhiều 'giai đoạn nước rút', nếu PRODUCT OWNER hỏi về nhiều đặc tính đem lại trong 1 giai đoạn nước rút thì vai trò của team rất quan trọng, họ sẽ đẩy trở lại và nói rằng có quá nhiều thứ phải hoàn thành, chúng ta cần tìm một sự hài lòng ở mức trung bình cho cả hai bên

---

### SPRINTS

Là tập hợp các vấn đề mà team phát triển đảm bảo rằng họ sẽ đưa vào quá trình nước rút

---

#### STAND-UP MEETING
* Là thứ xảy ra hàng ngày trong thực tế
* Nơi đâu team đến cùng nhau và gặp nhau sẽ cùng nhau thảo luận từ 10 đến 15 phút như cách mà team cập nhật tình hình với nhau, họ đã làm những gì và sẽ làm những gì tiếp theo

---

#### CEREMONY PHASE

* Đây là giai đoạn mà chúng ta hồi tưởng về 'quá trình nước rút' của họ
* Đây cũng là nơi team kỹ thuật đi đến và giới thiệu những đặc tính mà họ thêm vào sản phẩm
* Đây là cơ hội để họ phản ảnh được cụ thể những thứ được xây dựng trên các 'giai đoạn nước rút'. Cung cấp sự phản hồi tích cực cho team vù vậy họ có thể sử dụng nó để thông báo sự phát triển của team và quá trình lên kế hoạch cho những 'giai đoạn nước rút' tiếp theo.
