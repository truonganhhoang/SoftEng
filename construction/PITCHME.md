## Công nghệ phần mềm

### Xây dựng

---

### Xây dựng

- Tính dễ đọc
- Phân tích chương trình tĩnh và linters
- Tự động hóa

---

### Tính dễ đọc

- Mục đích
	- Dễ hiểu, không cần giải thích nhiều
	- Dễ sửa đổi, bảo trì, nâng cấp hệ thống
![Tính dễ đọc](https://image.ibb.co/mD4VuS/revans2_Landscape_Parchment_Background.png)

---

### Tính dễ đọc

- Để code dễ đọc cần tránh
    - Đặt tên không rõ
    - Deep nesting
    - Sử dụng phong cách cá nhân
    - Không comment

---

![Đặt tên không rõ](https://image.ibb.co/c7uqZ7/1.png)

---

![Deep nesting](https://image.ibb.co/gXPPu7/Untitled.png)

---

![Static analize n linters](https://image.ibb.co/i0KkTn/2.png)

---

### Tự động hóa
- Đặc biệt quan trọng đối với phần mềm vì số lượng đội ngũ phát triển và sự phức tạp của quá trình phát triển phần mềm.
- Cho phép xây dựng phần mềm một cách đáng tin cậy, có thể lặp lại và trở về trạng thái ban đầu.

---
![Tự động hóa](https://image.ibb.co/cpdaZ7/x.png)

---

![Tự động hóa](https://image.ibb.co/nOt9u7/z.png)

---

### Tự động hóa
- Code để tự động hóa cần phải:
    - Có thể lặp lại: việc này rất quan trọng để các hệ thống tự động khác nhau cũng có thể xây dựng hệ thống
    - Đáng tin
    - Có thể quay lại: làm giảm thời gian cần thiết để chỉnh sửa lỗi sai và viết lại code

---

### Mã xấu
#### Bảo trì phần mềm
- Bảo trì và cải tiến phần mềm là thành phần chính trong ngân sách chi cho hệ thống.
- Sửa đổi phần mềm có thể được chia làm 4 loại:
    - Các thay đổi sửa lỗi, chiếm 21%.
    - Sửa đổi nhằm thích ứng với các yêu cầu đạt ra, chiếm 25%.
    - Những thay đổi chỉnh sửa các chức năng, chiếm 50%.
    - Các thay đổi cải thiện cấu trúc phần mềm, chỉ chiếm 4%.

---

### Mã xấu
#### Bảo trì phần mềm
- Khó khăn:
    - Theo thời gian, mã có thể trở nên phức tạp và khó đọc.
    - Thiếu bảo trì phòng ngừa rủi ro.
    - Thiếu kiến thức.
    - Áp lực về thời gian khắc phục.

---

### Mã xấu
- Khi mã nhiều, việc sửa lỗi và thêm tính năng trở nên khó khăn hơn.
- Mã xấu là đặc điểm thường có ở các hệ thống tồn tại trong thời gian dài.

---

### Mã xấu
- Martin Fowler đã xác định 5 loại mã xấu chính:
    - Bloaters : Kích thước của một số thành phần trong mã nguồn phần mềm làm chúng trở lên khó hiểu và khó thay đổi.
	VD: phương thức dài, lớp quá lớn, phương thức có danh sách tham số dài.
    - Lạm dụng cấu trúc hướng tượng.
    - Ngăn ngừa các thay đổi : làm cho khó cải tiến mã nguồn. 
	VD : phải thực hiện cùng 1 sự thay đổi trong nhiều phần khác nhau của hệ thống.
    - Mã thừa : phức tạp không cần thiết.
	VD: mã trùng lặp.
    - Kết hợp không cần thiết.

---

### Cải tiến mã nguồn
- Qua thời gian, mã nguồn bị suy giảm chất lượng do phần mềm phức tạp.
- Lập trình viên thường tìm giải pháp xử lí vấn đề nhanh chóng do áp lực về thời gian hay không nắm được thiết kế ban đầu.
- "Món nợ kĩ thuật" là biện pháp ẩn dụ chỉ hậu quả trong tương lai của những giải pháp như vậy.
- Cải tiến mã nguồn là một trong những cách phổ biến để trả "món nợ kĩ thuật".

---

### Cải tiến mã nguồn
- Mục tiêu : cải thiện thiết kế của phần mềm nhưng vẫn giữ nguyên ngữ nghĩa.
- Khi cải tiến mã nguồn, ta cần lưu ý quy tắc 3 điều sau :
    - Lần đầu tiên, ta cần tạo ra 1 tính năng và lập trình nó.
    - Lần thứ 2, ta cần tạo ra 1 tính năng tương tự hoặc giống y hệt, hãy viết lại và ghi chú điều này.
    - Tới lần thứ 3, ta cần cải tiến mã nguồn đã viết thay vì viết lại.

---

### Cải tiến mã nguồn
- Việc cải tiến mã nguồn gồm 3 bước :
    - Hiểu rõ đoạn mã.
    - Biến đổi đoạn mã.
    - Đoạn mã được chỉnh sửa khi việc biến đổi gây một số lỗi.
- Hoạt động của phần mềm cần không bị ảnh hưởng sau khi cải tiến mã nguồn.
- Ta cần kiểm thử cả trước và sau khi cải tiến.

---

### Cải tiến mã nguồn
- Cải tiến mã nguồn thường tốn kém do làm tăng thời gian phát triển phần mềm.
- Làm tăng nguy cơ xuất hiện lỗi nếu không tiến hành kiểm thử toàn diện.
- Cải tiến mã nguồn sớm thường dễ hơn là cải tiến muộn.
