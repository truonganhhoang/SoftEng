### Properties and Process

#### Terminology

- Phần quan trọng nhất mà chúng ta thường đề cập đến là tình huống kiểm thử riêng biệt (individual test case).
- Một Test Case chỉ chỉ ra rõ ràng duy nhất một hành vi trong chương trình, nhưng chúng ta thường không chỉ thực thi một Test Case, mà phải thực thi một tập hợp nhiều Test Case,và chúng được gọi là "test suites" (bộ kiểm thử)

---
### Properties and Process

#### Terminology

-  Code đang được mỗi test case độc lập đánh giá được gọi là "Code Under Test"
- Đôi khi điều này cũng được đề cập như là "System Under Test"
- Vậy "code under test" và "system under test" đều đại diện cho code mà đang được đánh giá bởi một test case độc lập

---
### Properties and Process

#### Terminology

- Ở mức độ cao, có hai kỹ thuật chính chúng ta có thể dùng để viết test case:
  + Thứ nhất là "white box testing"- kiểm thử hộp trắng
  + Kỹ thuật còn lại gọi là "black box testing" - kiểm thử hộp đen
- Nếu chúng ta viết một test case mà không bao giờ sai hay không thể phát hiện lỗi trong code under test thì nó không có giá trị gì.
- Vậy nên giữ hiệu quả là rất quan trọng khi ta thiết kế các tests, bất kể chúng là white box tests hay black box tests.

---
### Properties and Process

#### Properties of Test

Có thêm một số các tính chất ở mức độ cao mà chúng ta muốn các test cases phải có để chúng có thể trở thành công cụ tốt nhất cho nhóm phát triển.
- Các test cases phải thực thi thật nhanh
- Các kết quả phải đáng tin cậy
- Những lỗi của test suite giúp ta cô lập được các bugs
- Lỗi của ta mô phỏng người dùng

---
### Properties and Process

#### Kind of Tests
- Tốc độ: bài test nhanh và bài test chậm
- Cô lập các khiếm khuyết: bị cô lập và không bị cô lập

Trong một hệ thống phần mềm, nếu bạn chỉ thực thi một phương thức, thì rất nhanh chóng để nhận được kết quả rằng phương thức đó đúng hay không

---
### Properties and Process

#### Kind of Tests

##### Thử nghiệm chấp nhận (acceptance test)
- Các bài acceptance test được thực hiện bởi người nhận phần mềm ở nơi đầu tiên
- Các tests này thường không được tự động hóa
- Chúng cũng rất chậm vì chúng không được thực hiện thường xuyên trong suốt quá trình phát triển

---

##### Thử nghiệm tích hợp (integration test)
- Integration test ít cô lập hơn so với unit test
- Chậm hơn unit tests bởi vì chúng thực hiện nhiều phần hệ thống cùng một lúc
- Cô lập hơn một chút so với acceptance tests

---

##### Thử nghiệm hệ thống (System tests)
- System tests thử nghiệm các phần rộng của hệ thống cùng một lúc
- Kiểm tra để đảm bảo rằng tất cả hệ thống làm việc cùng nhau một cách hiệu quả
- System test được thực hiện bởi đội phát triển
- Chạy trên nền tảng liên tục

---

#### Kind of Tests
- Các unit test sẽ cho bạn biết, hey, các từng phần riêng đều hoạt động tốt và thành công
- Integration tests bảo cho bạn rằng các đơn vị cũng hoạt động tốt với nhau.
- System tests chạy và báo với bạn rằng cả hệ thống có thể hoàn thành nhiệm vụ một cách hiệu quả
- Cuối cùng, vào cuối của quá trình phát triển, một khi khách hàng được tham gia, acceptance tests đảm bảo rằng thứ bạn tin là đúng sẽ giống với mong đợi của khách hàng về thứ họ tin là đúng.

---

#### Unit and system properties

##### Tốc độ
- Unit test nhanh:
  + Chúng thực hiện các phần rất nhỏ của hệ thống
  + Chúng rất hạn hẹp nên ít phải thực hiện và chúng kết thúc là khá nhanh
- System test khá chậm:
  + Nó chạy phần lớn của hệ thống.
  + Càng có nhiều code chạy thì nó càng chậm

---

#### Unit and system properties

##### Độ tin cậy
- Unit test có độ tin cậy rất tốt:
  + Chúng chỉ thực hiện một phương pháp tại một thời điểm mà không có bất kỳ phụ thuộc bên ngoài
  + Chúng có rất nhiều cơ chế kiểm soát để đảm bảo
- Điều này là vấn đề lớn cho System test:
  + Phụ thuộc bên ngoài

---

#### Unit and system properties

##### Cô lập lỗi
- Với unit tests, vì chúng đang chạy những bit nhỏ của hệ thống, khi có một lỗi, bạn có thể tìm trong test đó và xem chính xác những gì đã gây ra lỗi và cố gắng tìm ra những gì đã xảy ra.
- Với system test, khi một test không thành công, nó có thể là hàng ngàn hoặc hàng chục ngàn dòng code mà lỗi đó nảy sinh, vì vậy thật khó có thể xác định được điều gì đang xảy ra ở đây.

---

#### Unit and system properties

##### Mô phỏng người dùng
- Unit tests không thực sự cho chúng ta bất kỳ cái nhìn nào về những gì một người dùng thực sự sẽ thấy
- Ngược lại, đây là điều mà các system tests thực sự mạnh mẽ: chạy nhiều tính năng tại một thời điểm.

---

#### Unit and system properties
- Hai loại test này cộng hưởng với nhau
- Chúng làm việc cùng nhau để giúp bạn biết rằng hệ thống của bạn đã được kiểm tra kĩ và hoạt động chính xác.

---

#### Red Green refactor
- Quá trình viết tests và làm cho nó vượt qua thực sự là một vòng lặp 
- Quá trình này cũng thường được gọi là "Red-Green refactor"

---

#### Red Green refactor
- Điều đầu tiên chúng ta sẽ làm là chúng ta sẽ viết một bài tests và chắc chắn rằng nó thực sự lỗi
- Sau đó chúng ta sẽ đi và viết một bản bổ sung code để vượt qua tests đó
- Tiếp theo, những gì bạn sẽ làm là bạn sẽ tái cấu trúc và mở rộng test của bạn và code đi qua.

---

#### Red Green refactor
- Chúng ta không chỉ viết một test, làm cho nó vượt qua, và tái cấu trúc hệ thống của chúng ta một lần.
- Đây thực sự là một quá trình lặp đi lặp lại mà chúng ta sẽ phải trải qua nhiều lần
