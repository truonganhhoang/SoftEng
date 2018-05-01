### [View slides](https://gitpitch.com/truonganhhoang/softeng/specifications)
## Công nghệ phần mềm
=======
### Đặc tả
---
### Đặc tả
#### Giới thiệu 
- Đặc tả phần mềm kết nối khách hàng với đội ngũ phát triển lại với nhau:
    -  Khách hàng chắc chắn phần mềm làm ra là đúng yêu cầu
    -  Đội phát triển sử dụng để thiết kế và cài đặt những tính năng mà khách hàng yêu cầu
- Trong các phương thức theo kiểu agile, tài liệu đặc tả sẽ được hoàn tất trong giai đoạn cuối.
---
### Đặc tả
#### Xử lý các yêu cầu (Requirements Process)
- Các yêu cầu quy trình được chia ra làm 2 nhánh chính:
    - Các yêu cầu chức năng (Những gì hệ thống có thể thực hiện ?)
        + vd: người dùng có thể đăng xuất với 1 click
    - Các yêu cầu phi chức năng (Những gì hệ thống nên có ?):
        + vd: người dùng có thể đăng nhập bằng tài khoản google
---
### Đặc tả
#### Xử lý các yêu cầu (Requirements Process)
- Mỗi bên liên quan( stackholders) có thể có các yêu cầu phi chức năng khác nhau
    - Khách hàng quan tâm đến tính dễ sử dụng, hiệu năng, khả năng nâng cấp,..
    - Đội phát triển quan tâm đến độ tin cậy, độ phức tạp, khả năng kiểm thử, bảo trì,...
---
### Đặc tả
#### Xử lý các yêu cầu (Requirements Process)
- Các yêu cầu phi chức năng có thể mâu thuẫn với nhau
    - VD: đội phát triển cần 1 phần mềm có ít cài đặt phức tạp nhưng khách hàng lại muốn phần mềm có hiệu năng cao
    - => Các bên liên quan cần phải thống nhất với nhau về độ ưu tiên của các yêu cầu phi chức năng
- Lưu ý: Khi làm tài liệu về yêu cầu ta chỉ cần nêu những việc hệ thống sẽ làm chứ không cần quan tâm hệ thống sẽ làm những điều đó bằng cách nào
---
### Đặc tả
#### Đặc điểm của các yêu cầu( Requirements Properties)
- Các yêu cầu phải đảm bảo 4 điều kiện:
	- Hoàn thiện
	- Nhất quán
	- Chính xác
	- Xúc tích	
	
---
### Đặc tả
#### Thu thập yêu cầu( Requirements Elicitation)
Quá trình đặc tả phần mềm là lặp đi lặp lại các bước:
- Thu thập(Elicitation)
- Phân tích(Analysis)
- Cụ thể hóa(Reification)
- Thẩm định(Validation)
---
### Đặc tả
#### Các yêu cầu khác (Additional Requirements)
- Giàng buộc thiết kế (Design Constraints) 
- Giàng buộc về môi trường(Environmental Constraints)
- Sở thích của khách hàng( Preference)

---
## Xác nhận yêu cầu (Validating Requirements)

- Yêu Cầu

- Lợi ích

- Nội dung

---

## Yêu Cầu

- Việc đưa ra các yêu cầu phải dựa vào các thông tin có ý nghĩa.

- Phù hợp với yêu cầu khác hàng.

- Xác định được giá trị mà chức năng nó mang lại.

- Xác nhận yêu cầu là 1 bước quan trọng quá trình làm phần mêm !!!

---

## Lợi ích

- Trên thực tế các yêu cầu rõ ràng dễ thành công hơn các yêu cầu mơ hồ.

- Lập trình viên có thể hiểu và đánh giá các chức năng được yêu cầu.

- Lập trình viên và khách hàng có cùng một mục tiêu.

---

## Nội Dung 

- Chúng ta thường tìm thấy vấn đề trong quá trình làm phần mềm 

- Một số yêu cầu dễ thấy ta có thể viết thành 1 danh sách và làm theo danh sách

- Thực tế thì các yêu cầu phức tạp hơn nên ta xác định và đánh giá các yêu cầu bằng cách đánh giá hiệu suất.

---

## Nội Dung 
### Hiệu suất

- Có thể hiểu theo nhiều cách khác nhau nhưng có thể hiểu theo 2 cách:

   + Thời Gian

   + Lưu trữ hoặc không gian

---

## Hiệu suất
### Thời gian
- Thời gian phản ứng( Thông lượng):

   + Giờ cao điểm: vd hệ thống có thể xử lí 50 người / giây.

   + Bình thường: 10 giao dịch / giây
    
- Thời gian trả lời:

   Vd: Hệ thống trả lời người dùng trong 150 mili giây.

---

## Hiệu suất
### Lưu trữ

- Bộ nhớ

- Ổ đĩa

---

## **USER STORIES**
---
1. ROLE - GOAL - BENEFIT 
2. LIMITATIONS
3. DEFINITION OF DONE
4. ENGINEERING TASKS
5. EFFORT ESTIMATE
---

## **ROLE - GOAL - BENEFIT** 
- Hiểu được mục tiêu, lợi ích những gì họ đang làm.
- Thêm, bớt tính năng có làm tăng giá trị sản phẩm?
---

## **LIMITATIONS**
- Những hạn chế của tính năng.
---

## **DEFINITION OF DONE**
- Xác nhận tính hoàn thiện của tính năng.	
---

## **ENGINEERING TASKS**
- Có giá trị cho đội ngũ phát triển.
- Theo dõi các tính năng tương tác với nhau trong hệ thống.
---

## **EFFORT ESTIMATE**
- ước tính chi phí tổng thể của một sản phẩm.
- Có nên thêm tính năng cho sản phẩm? chi phí so với hiệu quả của tính năng?


---
##Nguyên tắc INVEST##

 Sử dụng đúng đắn **User story**  thường là thách thức, đặc biệt đối với những người mới.

 Một loạt các nguyên tắc được gọi là **INVEST** được phát triển để giúp các kỹ sư và khách hàng viết nên những User story  có hiệu quả.


 **Nguyên tắc là độc lập .**

-  Điều này có nghĩa là tất cả bộ nhớ người dùng phải được độc lập riêng biệt một cách có thể.

 
-  Khi bạn có những User story độc lập, nó sẽ đem lại cho nhóm phát triển và khách hàng nhiều sự linh hoạt hơn trong việc lựa chọn từ một sản phẩm tồn đọng.Điều đó giúp họ chắc chắn chọn đúng một tập các **Story** cho sự lặp lại.


**Bổ sung trong Giai đoạn đàm phán.**


-Khiến họ đi theo những suy nghĩ của ta. Vì chúng ta không thể đánh giá về các User story có hiệu quả hay không.

- Các cuộc đàm phán thường phải dừng lại khi các tính năng bổ sung hay chi tiết bổ sung được thêm vào User story.



**Đánh giá User story**


- Nhằm đảm bảo rằng User story thực sự cung cấp  một giá trị có ý nghĩa cho sản phẩm. Và điều này cho chúng ta một cơ hội để lùi lại và suy nghĩ về lợi ích của role-goal (vai trò mục tiêu ) đối với một tính năng nào đó.


- Trải qua sự phát triển của một dự án, giá trị của các tính năng khác nhau sẽ thay đổi qua thời gian như nhu cầu của sự thay đổi sản phẩm,  như kỳ vọng của khách hàng hoặc sự thay đổi ý kiến.

=> Cần phải có khả năng nhìn lại và thực sự đánh giá giá trị của một tính năng tại thời điểm mà chúng ta đang cân nhắc xây dựng nó.


**Đánh giá các tính năng**


- Chúng ta cần có khả năng để chi trả các chi phí một cách hiệu quả cho các tính năng. 


- Nếu chúng ta không thể cung cấp một chi phí cụ thể và có ý nghĩa cho sự phát triển một tính năng, chúng ta cần  nhìn lại và thực sự thêm các chi tiết bổ xung hoặc chia nhỏ tính năng đó thành một tập các tính năng có giá trị hơn. 

=> Phải đảm bảo rằng chúng ta có sự hiểu biết cụ thể và thực tế về những chi phí cho những tính năng thực sự quan trọng.

**Các tính năng nhỏ**


- Tính năng nhỏ được ước tính dễ dàng hơn, dễ lý giải về giá trị,các  tính năng dễ đàm phán hơn, và nó cũng
có khuynh hướng độc lập hơn.

- User stories nên càng nhỏ càng tốt để giúp dẫn các tính năng tiếp theo.
**Kiểm chứng**


- Nhằm đảm bảo rằng những Story có thể kiểm chứng được, để cả khách hàng và nhà phát triển có thể chắc chắn rằng tính năng đã được phát triển theo cách phù hợp với cả hai bên.

**
*NHỮNG NGUYÊN TẮC NÀY THỰC SỰ CUNG CẤP MỘT FRAMEWORK GIÚP. CHÚNG TA CÓ THỂ SỬ DỤNG KHI CHÚNG TA VIẾT STORY ĐỂ ĐẢM BẢO RẰNG CHÚNG HOÀN CHỈNH HƠN VÀ HỮU ÍCH HƠN  TRONG THỰC TẾ.***
 
---
## User Story và ví dụ về INVEST  #

###Một ví dụ cụ thể về User story:
- Như một prof ( giáo sư ), tôi muốn tạo ra một tập hợp các Repo để học sinh có thể thực hiện công việc của mình. 
####bước 1:
+ vai trò : là giáo sư
+ mục đích: tạo ra các repo
+ lợi ích: học sinh có thể làm công việc của mình
####bước 2
+ cần làm: respository names, student ids trong trường hợp này nó sẽ là các ID sinh viên và sẽ là tên người dùng GitHub
####bước 3
+ cần chạy nó như 1 command riêng lẻ
+ các test cases tự động
+ hàm ý các test case: lập trình kiểm chứng được
###bước 4
+ có thể sử dụng Github manager
####bước 5
+ ước tính chi phí: 1.5 units (units phụ thuộc vào team)
=> biết được input, định nghĩa sản phẩm và các kiểm tra nó và có 1 ước tính rõ ràng về chi phí
---
##Decomposing User Stories : 
###phân tách User Story thành những User story nhỏ hơn, dễ implement hơn
###Phần 1 : 
- Xác định các role, goals, benefit, limitation, notes, cost của câu chuyện 

- Xây dựng DoD

- Đánh giá DoD qua bộ tiêu chí INVEST

---
##Decomposing User Stories : 
###Phần 2 : 
- Xác định các thực thể trong câu chuyện(Entities)

- Liên kết các thực thể với nhau(Link entities)

- Xác định các hành động rang buộc thực thể và story(Bind actions)

- Xây dựng kịch bản cho câu chuyện (Prototype)

- Hình thức hóa các prototype đã xây dựng(Formalize)

---
##Decomposing User Stories: 
###Phần 3

####Hình thức hóa protoype bằng UML class diagram


- Class Key:  gồm 1 method keyPressed(Event)
- keyPressed sẽ gọi class Level
- Class Level: 2 trường là mario có kiểu Mario, enemies là 1 mảng các Enemy, 2 phương thức input(command) và update()
- Vì class Level chứa những nhân vật mario và enemy, nên tạo interface Figure, dùng composition
- Figure: move(Dir), hit(), collision(Figure)

---
##Decomposing User Stories: 
###Phần 4
- Giả sử người dùng bấm left arrow <- và mario sẽ va chạm với một enemy
- Đầu tiên xem xét trong class Key:
	+ nó sẽ thông dịch và chuyển left arrow đó thành thứ mà class Level có thể dùng
	+ Chuyển left arrow vào trường direction mã hóa những gì left arrow làm và đưa nó cho input() trong class Level
	+ class Direction thêm vào 1 chút trừu tượng, làm cho code phức tạp hơn trong tương lai. Ví dụ nếu người dùng dùng phím A và D để di chuyển trái và phải thay vì arrows key, ta chỉ cần capture nó với vô hướng và class Level không bị ảnh hưởng.
	+ và khi input lấy tham số này, nó gọi move với direction trên Mario, và Mario sẽ di chuyển và trả về
	+ sau đó input gọi update(), update tất cả vị trí của enemies, nên có 1 vòng for duyệt toàn bộ enemy và update chúng. Chú ý tham số direction ở đây không phải do người dùng, mà là hướng mà enemy đang di chuyển vào lần cuối update
