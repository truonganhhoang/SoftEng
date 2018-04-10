## Công nghệ phần mềm

### Kiểm thử

---

### Tiêu đề 1

- Ý 1
    - Ý phụ 1
- Ý 2
    - Ý phụ 1

---

### Tiêu đề 1

- Ý 1
    - Ý phụ 1
- Ý 2
    - Ý phụ 1

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
    - Trong white box testing, chúng ta có quyền truy cập đầy đủ tới mã nguồn của hệ thống nhưng nếu không thì sẽ gặp khó khăn.
    - Whitebox testing có nhiều phức tạp. Hiểu code để viết test case phù hợp là quá nặng và khó khăn.
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
    - Tạo bảng với giá trị cột ứng với a, giá trị dòng ứng với b thì t có (3.58e308)^2 = 1.28e617 ô trong bảng, ứng với số trường hợp của đầu vào.
    - Không gian trạng thái: 1.28e617 trạng thái
    - Nếu muốn kiểm tra mọi trạng thái là điều không thể
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
    - Thay vì chọn các số vô cùng để kiểm tra, hãy chọn 1 số dương, 1 số âm, và các số xung quanh điểm biên.
    - Bạn có thể chọn 0, 1, 5, -1, -5
    - a,b có thể nhận 5 giá trị trên nên tổng cộng chỉ có 25 trạng thái thay vì 1.28e617 trạng thái như VD trên.
- Vẫn kiểm tra đủ các trường hợp input của hàm với mẫu trên mà không cần kiểm tra toàn bộ không gian trạng thái.

---

### Phân chia input

- VD: Hàm quản lí audio của Game Mario có thể chơi 2 định dạng âm thanh MP3 và OOG
    - Không cần thử chục ngàn tệp âm thanh vào hệ thống
    - Chỉ cần chạy 1 tệp MP3 và 1 tệp OOG

---

### Phân chia input

- VD: Mario lao vào địch thì Mario bị thương, các địch lao vào nhau thì không sao, mario nhảy qua boss, boss có thể còn sống
- Ta có 3 loại nhân vật: Mario, boss, Turtle
- Có 2 thuộc tính liên quan:
    - 2 hướng (phải/xuống) (vì nếu Mario sang phải va trúng địch thì Mario chết, còn Mario hạ cánh trúng địch thì địch chết)
    - 2 trạng thái (lớn/nhỏ) (vì Mario lớn có thể sống sót khi va trúng địch còn Mario nhỏ thì không)
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
    - Thử chọn input như VD trước: -5,-1,0,1,5 => không phụ hợp để kiểm tra các miền output.
    - Nên chọn input: 0, 1000, 60k, 3.6m để kiểm tra mỗi miền output.

---

### Phân chia output

- VD: Hàm typescript
    - setVelocity(vx: number, vy: number): Direction
    - hàm cho 2 tham số vx, vy là vận tốc nhân vật theo phương Ox và Oy
    - trả về nhân vật đó đang di chuyển trái hay phải.
- Ta tưởng tượng đồ thị với 2 trục: vx và vy với vx và vy có giá nằm trong khoảng số rộng 1,28e617.
- Trong hàm này, chúng ta chỉ quan tâm vx (vì nó tác động tới hướng trái/phải) nên
    - khi chia output ta có 2 test cases là : -1 và 1

---

### Phân tích giá trị biên

- Các thảo luận từ trước chỉ bàn về các giá trị hợp lệ của input và output.
- Chương trình không phải lúc nào cũng gặp các giá trị hợp lệ.
- Chúng ta muốn hệ thống phản ứng với cả các input không hợp lệ
- Chúng ta đã kiểm tra bên trong biên, giờ là lúc kiểm tra bên ngoài biên
- Nên công nghệ chính sử dụng là phân tích giá trị biên

---

### Phân tích giá trị biên

- VD: Hệ thống quản lí audio game Mario hỗ trợ 2 định dạng MP3 và OGG.
    - Đảm bảo khi cho file input với định dạng không hợp lệ (FLAC, VP9) vào hệ thống thì hệ thống không bị treo hoặc cư xử theo cách đã định sẵn
- Chúng ta phải nghĩ về những điều có thể xảy ra khi vấn đề input không hợp lệ diễn ra
- Tiếp VD:
    - Định dạng OGG có thể chứa video, chúng ta phải thêm test case với 1 file video OGG.

---

### Phân tích giá trị biên

- Khi phân tích giá trị biên, chúng ta cố đẩy ra ngoài biên để biết những kiểu vấn đề có thể xảy ra.
- Trong TypeScript mỗi kiểu đơn đều có 2 giá trị null và undefined, nên VD với kiểu Boolean có 4 giá trị: true/false/null/undefined
- Vậy khi kiểm thử, bạn sẽ phải thử không chỉ với true, false mà cả null và undefined để đảm bảo hàm thực sự hoạt động tốt.
- Khi đối mặt với giá trị không hợp lệ, hoặc là
    - ném ra ngoại lệ (throw exception)
    - luôn luôn là false

---

### Phân tích giá trị biên

- Trở về ví dụ hàm isGreater(a: number, b: number)
    - chúng ta đã thử với -5, -1, 0, 1, 5
    - giờ tiếp tục thử với các input không mong muốn:
        - Trong lập trình, vô cùng không thể mã hóa, nên kiểu số có giá trị lớn/nhỏ nhất giới hạn
        - khi giá trị số vượt qua giới hạn trên thì gây ra number roll over làm sai giá trị gây ra hậu quả khôn lường.
- Vậy cần kiểm thử chúng trong tình trạng tập trung cao (đảm bảo an toàn cao).

---

### Kết luận

- Cuối cùng, chúng ta không thể kiểm tra toàn diện chương trình của chúng ta. Có quá nhiều inputs và outputs để kiểm tra.
- Điều chúng ta có thể làm là chia nhỏ không gian input, output để chúng ta có thể lấy mẫu từ các phần đó.
- Ngoài ra cần phải chú ý để các input không mong muốn không làm treo chương trình bằng cách dùng phương pháp phân tích giá trị biên
- Phân tích giá trị biên giúp code không chỉ đúng mà còn phản ứng được với các input không hợp lệ