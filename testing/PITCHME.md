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

#### Slide by Phạm Ngọc Duy

---

#### Nội dung chính

- Giới thiệu
    - Vấn đề về white box testing
    - Giới thiệu black box testing
- Phân chia lớp tương đương
- Phân chia input

- Phân chia output
- Phân tích giá trị biên

---

#### Giới thiệu
##### Vấn đề whitebox testing:

- Vấn đề:
    - Trong white box testing, chúng ta có quyền truy cập đầy đủ tới mã nguồn của hệ thống nhưng nếu không thì sẽ gặp khó khăn.
    - Whitebox testing có rất nhiều phức tạp. Việc hiểu code để viết test case phù hợp là quá nặng và khó khăn.
- Giải quyết:
    - Người thích hợp tạo test case whitebox là chính nhà phát triển.
- Vấn đề nảy sinh:
    - Nhà phát triển có thể tạo lỗi hệ thống trong test họ tạo.
###### Giải pháp: BLACK BOX TESTING

---

#### Giới thiệu
##### Giới thiệu Black box testing

- Tập trung vào đầu vào, đầu ra, những gì hệ thống làm thay vì tập trung vào code được cài đặt như thế nào.

- Nhược điểm: 
    - Có sẵn ít dữ liệu để phân tích, phải đặt nặng vào các đặc tả code (trong chữ kí API) để hiểu các hành vi mong muốn.
- Ưu điểm:
    - Các bên liên quan dễ viết test case hơn
- Mục đích:
    - Tập trung vào đầu vào và đầu ra, kiểm tra triệt để không gian trạng thái để chương trình thực hiện đúng với mọi đầu vào.

---

#### Giới thiệu
##### Giới thiệu Black box testing

- VD1: hàm cho một Boolean và trả về một Boolean.
    - Không gian trạng thái: 2 trạng thái: true/false
- VD2: hàm cho 2 số a,b, trả về true nếu a lớn hơn b
    - Trong typescript kiểu number từ -1.79e308 đến 1.79e308 (3.58e308 giá trị)
    - Tạo bảng với giá trị cột ứng với a, giá trị dòng ứng với b thì t có (3.58e308)^2 = 1.28e617 ô trong bảng, ứng với số trường hợp của đầu vào.
    - Không gian trạng thái: 1.28e617 trạng thái (lớn hơn rất nhiều)
    - Nếu muốn kiểm tra mọi trạng thái là điều không thể
    - Đây vẫn còn là VD đơn giản.
###### Làm thế nào để xử lí quá tải này?

---

#### Phân chia lớp tương đương

- Để việc kiểm tra dễ dàng hơn (không bị quá tải), cần giảm không gian trạng trái.
- Phân chia lớp tương đương: chia sẻ không gian trạng thái thành các vùng nhỏ hơn. Rồi lấy mẫu từ các vùng này để kiểm tra.

---

##### Phân chia input

VD: Input là một số từ 0 đến vô cùng.
    - Thay vì chọn các số vô cùng để kiểm tra, hãy chọn 1 số dương, 1 số âm, và các số xung quanh điểm biên.
    - Bạn có thể chọn 0, 1, 5, -1, -5
    - Tổng cộng 25 trạng thái thay vì 1.28e617 trạng thái như VD trên.
- Vẫn kiểm tra đủ các trường hợp input của hàm với mẫu trên mà không cần kiểm tra toàn bộ không gian trạng thái.
VD: Game Mario có thể chơi 2 định dạng âm thanh MP3 và OOG
    - Không cần thử chục ngàn tệp âm thanh vào hệ thống
    - Chỉ cần chạy 1 tệp MP3 và 1 tệp OOG

