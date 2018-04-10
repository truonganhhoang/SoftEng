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
    - Statement Coverage - Bao phủ theo điều kiện (*)
    
---

### Flow dependent

- Đảm bảo các dòng code có thể thực thi cùng nhau
- Khó tính toán giải thích
- Cho ta cái nhìn sâu sắc hơn trong việc vận hành
- Gồm:
    - Branch Coverage - Bao phủ theo nhánh (*)
    - Path Coverage - Bao phủ theo đường (*) - thường ứng dụng trong thực tế
    - MCC Coverage - Mở rộng của path coverage
    
---

### Coverage là 1 quá trình lặp

1. Định danh những dòng code chưa được bao phủ
1. Thiết kế các bộ test để chạy các dòng code đó
1. Viết và chạy test để đảm bảo các dòng code đó qua được các test
1. Lặp lại đến khi đạt được mục đích bao phủ - 'coverage'

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

- Test 5: boss.hit(new Mario({direction: down}))

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_16.jpg?raw=true)

---

### Path Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_17.jpg?raw=true)

---

### Path Coverage

![](https://github.com/NguyenDung98/SoftEng/blob/master/testing/imgs/white-box_17.jpg?raw=true)
