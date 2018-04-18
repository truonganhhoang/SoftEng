## Công nghệ phần mềm

### Kiểm thử

---

### White Box Testing: Coverage

- Làm thế nào để biết rằng code của mình đã được test đủ?

---

### Mục tiêu của việc test

- Đảm bảo code thực thi đúng đặc tả
    - Liệu code đã làm đúng nhiệm vụ
- Tìm những lỗi trong code
- Hiểu được chỗ mà ta có thể tìm được lỗi

---

### Không phải mục tiêu (non-goal)

- Đảm bảo hệ thống không lỗi
    - Vì không có đủ thời gian trong hệ thống của ta
    - Và cuối cùng thì ta muốn tạo hệ thống phần mềm có ích cho người dùng

---

### Coverage - bao phủ

- Là công cụ để đo lường tỉ lệ hệ thống được thực thi bởi một bộ test
- Được tính:
    - Tỉ lệ bao phủ = (covered / (covered + uncovered)) * 100
- Gồm 2 loại:
    - Flow independent - dòng độc lập
    - Flow dependent - dòng phụ thuộc

---

### Flow independent

- Dễ tính toán
- Dễ giải thích
- Đảm bảo việc chạy từng mảnh hệ thống thành công
- Gồm: 
    - Block Coverage - Bao phủ theo khối 
    - Line Coverage - Bao phủ theo dòng (*)
    - Statement Coverage - Bao phủ theo dòng lệnh (*)
    
---

### Block Coverage

- Đo lường số các khối trong hệ thống có thể được chạy bởi bộ test
- Chứa nhiều dòng code
- Nhỏ hơn method - bao quát hơn dòng 

---

### Line Coverage

- Đo lường số các dòng trong hệ thống có thể được chạy bởi bộ test
- Trực quan
    - Vì chỉ cần nhìn vào từng dòng code và giải thích liệu chúng đã được chạy bởi bộ test hay không
---

### Statement Coverage

- Đo lường số các dòng lệnh trong hệ thống có thể được chạy bởi bộ test
- Rất giống với line coverage - trừ việc có nhiều lệnh trong 1 dòng lệnh(lệnh rẽ nhánh và loop)
- Đảm bảo mọi lệnh trong 1 dòng đều được chạy

---

### Flow dependent

- Đảm bảo các dòng code có thể thực thi cùng nhau
- Khó tính toán giải thích
- Cho ta cái nhìn rõ ràng hơn trong việc vận hành
- Gồm:
    - Branch Coverage - Bao phủ theo nhánh (*)
    - Path Coverage - Bao phủ theo đường (*) - thường ứng dụng trong thực tế
    - MCC Coverage - Mở rộng của path coverage
    
---

### Branch Coverage

- Đảm bảo ta đã chạy được cả hai nửa của lệnh rẽ nhánh
- VD: Đảm bảo 2 nhánh true và false của cầu lệnh rẽ nhánh đều được thực thi

---

### Path Coverage

- Đàm bảo ta bao được toàn bộ trường hợp có thể xảy ra trong hệ thống (rẽ nhánh)
- VD: Ta có 2 câu lệnh rẽ nhánh
    - Ta không chỉ thực thi được true và false cho mỗi nhánh
    - Ta còn chạy các bộ kết hợp của true và false (true-true; true-false; false-true; false-false: 2!)

---

### MCC Coverage

- Phiên bản mở rộng của Path Coverage
- Đảm bảo mọi trường hợp đều được tính toán độc lập đối với đầu ra của 1 hàm
- Được sử dụng trong một số hệ thống quan trọng
- Nhưng rất khó để sử dụng trong thực tiễn

---

### Coverage là 1 quá trình lặp

1. Định danh những dòng code chưa được bao phủ
1. Thiết kế các bộ test để chạy các dòng code đó
1. Viết và chạy test để đảm bảo các dòng code đó qua được các test
1. Lặp lại đến khi đạt được mục đích bao phủ - 'coverage'

---

### Wrap-up

- Thực tế, developer có khuynh hướng bắt đầu với dạng coverage đơn giản
    - line coverage
- Sau khi đạt tỉ lệ coverage cao => Chuyển sảng dạng nghiêm ngặt hơn - Path Coverage


---

### Wrap-up

- Không có ngưỡng tiêu chuẩn coverage nào là đúng
- Nghiên cứu gần đây đã cho thấy:
    - Chạy nhiều test chất lượng cao tốt hơn là tăng tỉ lệ phần trăm coverage
- Tỉ lệ coverage cao - không tương đương với việc hệ thống đúng

---

### Wrap-up

- Điểm yếu cơ bản:
    - Không kiểm tra về sự đúng đắn
    - Chỉ kiểm tra về việc vận hành hệ thống 

---

### Line và Statement Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_0.jpg?raw=true)

---

### Line và Statement Coverage

- Test 1: turtle.hit(new Mario({direction: down}));

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_1.jpg?raw=true)

---

### Line và Statement Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_2.jpg?raw=true)

---

### Line và Statement Coverage

- Test 2: turtle.hit(new Mario({direction: right, state: big}));

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_3.jpg?raw=true)

---

### Line và Statement Coverage

- Test 2: turtle.hit(new Mario({direction: right, state: big}));

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_4.jpg?raw=true)

---

### Line và Statement Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_5.jpg?raw=true)

---

### Line và Statement Coverage
- statement coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_6.jpg?raw=true)

---

### Branch và Path Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_7.jpg?raw=true)

---

### Branch và Path Coverage

- T1 và T2

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_8.jpg?raw=true)

---

### Branch Coverage

- Test 3: turtle.hit(new Turtle());

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_9.jpg?raw=true)

---

### Branch Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_10.jpg?raw=true)

---

### Path Coverage

- Tập các node theo thứ tự

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_11.jpg?raw=true)

---

### Path Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_12.jpg?raw=true)

---

### Path Coverage

- Test 4: turtle.hit(new Mario({direction: right}))

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_13.jpg?raw=true)

---

### Path Coverage

- Test 4: turtle.hit(new Mario({direction: right}))

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_14.jpg?raw=true)

---

### Path Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_15.jpg?raw=true)

---

### Path Coverage

- Test 5: boss.hit(new Mario({direction: down}))

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_16.jpg?raw=true)


---

### Path Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_17.jpg?raw=true)

---

### Recap

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_18.jpg?raw=true)

---

### Wrap-up

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_19.jpg?raw=true)


---

### Black Box Testing: Phân chia lớp tương đương

#### Slide by [Phạm Ngọc Duy](https://github.com/phamngocduy98/SoftEng)

---

### Nội dung chính

- Giới thiệu
- Phân chia lớp tương đương
- Phân chia input
- Phân chia output
- Phân tích giá trị biên

---

### Vấn đề whitebox testing:

- Vấn đề:
    - Trong white box testing, ta có quyền truy cập tới mã nguồn
    - Hiểu code để viết test case phù hợp là quá nặng và khó khăn.
    - Người thích hợp tạo test case whitebox là chính nhà phát triển.
    - Tuy nhiên Nhà phát triển có thể tạo lỗi hệ thống trong test họ tạo.
- Giải pháp: BLACK BOX TESTING

---

### Giới thiệu Black box testing

- Tập trung vào đầu vào, đầu ra, những gì hệ thống làm thay vì tập trung vào code được cài đặt như thế nào.
- Nhược điểm: 
    - Có sẵn ít dữ liệu để phân tích, phải đặt nặng vào các đặc tả code để hiểu các hành vi mong muốn.
- Ưu điểm:
    - Các bên liên quan dễ viết test case hơn
- Mục đích:
    - Tập trung vào đầu vào và đầu ra, kiểm tra triệt để không gian trạng thái để chương trình thực hiện đúng với mọi đầu vào.

---

### Giới thiệu Black box testing

- VD1: hàm cho một Boolean và trả về một Boolean.
    - Không gian trạng thái: 2 trạng thái: true/false

---

### Giới thiệu Black box testing

- VD2: hàm cho 2 số a,b, trả về true nếu a lớn hơn b
    - Trong TypeScript kiểu number từ -1.79e308 đến 1.79e308 (3.58e308 giá trị)
    - có (3.58e308)^2 = 1.28e617 trường hợp của đầu vào.
    - Không gian trạng thái: 1.28e617 trạng thái
    - Kiểm tra mọi trạng thái là điều không thể
    - Đây vẫn còn là VD đơn giản.
- Làm thế nào để xử lí quá tải này?

---

### Phân chia lớp tương đương

- Để việc kiểm tra dễ dàng hơn (không bị quá tải), cần giảm không gian trạng trái.
- Phân chia lớp tương đương: chia sẻ không gian trạng thái thành các vùng nhỏ hơn. Rồi lấy mẫu từ các vùng này để kiểm tra.
- Gồm 2 loại: 
    - Phân chia input
    - Phân chia output

---

### Phân chia input

- VD: Hàm isGreater(a: number, b: number)
    - Input a,b là một số từ 0 đến vô cùng.
    - Bạn có thể chọn 0, 1, 5, -1, -5 cho input
    - chỉ còn 25 trạng thái thay vì 1.28e617 trạng thái như VD trên.
- Vẫn kiểm tra đủ các trường hợp input của hàm với mẫu trên mà không cần kiểm tra toàn bộ không gian trạng thái.

---

### Phân chia input

- VD: Hàm quản lí audio của Game Mario có thể chơi 2 định dạng âm thanh MP3 và OOG
    - Không cần thử chục ngàn tệp âm thanh vào hệ thống
    - Chỉ cần chạy 1 tệp MP3 và 1 tệp OOG

---

### Phân chia input

- VD: Mario lao vào địch thì Mario bị thương, các địch lao vào nhau thì không sao, Mario nhảy trúng đích thì địch chết, Mario nhảy trúng boss, boss có thể còn sống
- Ta có 3 loại nhân vật: Mario, boss, Turtle
- Có 2 thuộc tính liên quan:
    - 2 hướng (phải/xuống) 
    - 2 trạng thái (lớn/nhỏ)
- Vậy Chúng ta có 4 Mario nói chung

---

### Phân chia input

- Ta có bảng ứng với các trường hợp không gian trạng thái với:
    - Dòng là 6 loại nhân vật
        - 4 Mario
        - Boss
        - Turtle
    - Cột là 2 nhân vật bị (6 nhân vật trên) va chạm vào
        - Boss
        - Turtle
- Vậy ta có tổng cộng 6 x 2 = 12 test cases

---

### Phân chia input

- So sánh với White box testing ở VD này:
    - Với white box testing cần 6 test case
    - Với black box testing chỉ cần 12 test case mà không cần xem và hiểu mã nguồn.
        - Trả lời cho câu hỏi WHAT thay vì HOW
        - Tập trung vào hành vi phản ứng lại với các tham số input hơn là xem nhà phát triển viết cài đặt thế nào
        - Thực sự giúp kiểm tra 1 cách hiệu quả

---

### Phân chia output

- là loại phân chia lớp diễn ra trên output
- xem xét các kết quả mong đợi và thiết kế test case để xác định miền output mong muốn.

---

### Phân chia output

- VD: hàm typescript: humanize(duration: number):string
    - chuyển duration mili-giây sang xâu kí tự đọc được
        - duration < 1000ms => trả về mili giây
        - 1000ms - 1min => trả về giây
        - 1min - 1h => trả về phút và giây
        - duration > 1h => trả về giờ, phút giây
---

### Phân chia output

- VD: hàm typescript: humanize(duration: number):string
    - Thử chọn input như VD trước: -5,-1,0,1,5 => không phụ hợp để kiểm tra các miền output.
    - Nên chọn input: 0, 1000, 60k, 3.6m để kiểm tra mỗi miền output.

---

### Phân chia output

- VD: Hàm typescript
    - setVelocity(vx: number, vy: number): Direction
    - hàm cho 2 tham số vx, vy là vận tốc nhân vật theo phương Ox và Oy
    - trả về nhân vật đó đang di chuyển trái hay phải.
    
---

### Phân chia output

- VD: Hàm typescript
- Ta tưởng tượng đồ thị với 2 trục: vx và vy với vx và vy có giá nằm trong khoảng số rộng 1,28e617.
- Trong hàm này, chúng ta chỉ quan tâm vx (vì nó tác động tới hướng trái/phải) nên
    - khi chia output ta có 2 test cases là : -1 và 1

---

### Phân tích giá trị biên

- Các thảo luận từ trước chỉ bàn về các giá trị hợp lệ của input và output.
- Chúng ta muốn hệ thống phản ứng với cả các input không hợp lệ
=> Công nghệ chính sử dụng là phân tích giá trị biên

---

### Phân tích giá trị biên

- VD: Hệ thống quản lí audio game Mario hỗ trợ 2 định dạng MP3 và OGG.
    - File input với định dạng không hợp lệ (FLAC, VP9) thì hệ thống không treo
    - Định dạng OGG có thể chứa video thay vì audio
- Chúng ta phải nghĩ về những điều có thể xảy ra khi vấn đề input không hợp lệ diễn ra


---

### Phân tích giá trị biên

- Trong TypeScript mỗi kiểu đơn đều có 2 giá trị null và undefined
- Vậy Boolean có 4 giá trị: true/false/null/undefined
- Khi đối mặt với giá trị không hợp lệ, hoặc là
    - ném ra ngoại lệ (throw exception)
    - luôn luôn là false

---

### Phân tích giá trị biên

- Trở về ví dụ hàm isGreater(a: number, b: number)
    - chúng ta đã thử với -5, -1, 0, 1, 5
    - giờ tiếp tục thử với các input không mong muốn:
        - Không thể hiện được vô cùng với ngôn ngữ lập trình
        - Number roll over gây ra hậu quả khôn lường.
- Vậy cần kiểm thử trong tình trạng tập trung cao (đảm bảo an toàn cao).

---

### Kết luận

- Ta không thể kiểm tra toàn diện.
- Cần chia nhỏ không gian input, output để lấy mẫu
- Cần chú ý các input không mong muốn bằng phương pháp phân tích giá trị biên
