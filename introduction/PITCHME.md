## Giới thiệu

---

### Lập trình là gì?

- Là một quá trình mô tả ý tưởng của bạn và chuyển đổi nó thành một định dạng mà máy tính hiểu được.
- Cốt lõi của quá trình lập trình là khiến máy tính làm điều bạn muốn nó làm.

---

### Ngôn ngữ lập trình là gì?

- Ngôn ngữ lập trình đóng vai trò trung gian giữa người và máy tính. Chúng hình thức hóa ý tưởng của lập trình viên sang cách  cách máy tính có thể hiểu và thực hiện.

---

### Ngôn ngữ lập trình là gì?

- Có rất nhiều ngôn ngữ lập trình khác nhau. Chúng phân biệt bằng các yếu tố sau: 
	+ Cú pháp của ngôn ngữ.
	+ Thứ tự thực hiện của các mã.
	+ Ý nghĩa của các mã.

---

### Ngôn ngữ lập trình là gì?

- Một chương trình có thể có cú pháp hợp lệ nhưng lại vô nghĩa. Ví dụ: "foo == foo" gần như vô nghĩa nhưng vẫn là một cú pháp hợp lệ.
- Mỗi ngôn ngữ lập trình lại có các đặc ngữ riêng của mình. Việc sử dụng chúng tạo sự thống nhất trong việc lập trình và đọc hiểu chương trình của các nhà phát triển.

---

### Ngôn ngữ lập trình là gì?

- Ngôn ngữ lập trình hầu như không có các đặc ngữ chỉ để miêu tả một ngoại lệ duy nhất. Điều này dễ gây khó khăn cho việc hiểu chương trình chạy thế nào.
- Ngôn ngữ lập trình có tính bất biến. Một đối tượng một khi đã được khai báo sẽ không bị thay đổi trong suốt chương trình.
 
---

### Ngôn ngữ lập trình là gì?

- Chúng nên nên quan tâm đến sự khác biệt giữa mã code và cách chúng chạy. Sự khác biệt đó thường sinh ra lỗi và đó lí do các trình gỡ lỗi rất quan trọng.
- Khi gỡ lỗi(debug), bạn nên đặt một điểm dừng.Sau đó, bạn xem xét sự khác biệt giữa các biến trong chương trình và trạng thái của chúng là gì? Tốt nhất là bạn nên xem xét từng dòng code của chương trình có thể hiểu được tất cả các trạng thái mà chương trình có thể gặp phải.
---

### Giới thiệu về ngôn ngữ lập trình TypeScript

- TypeScript là một ngôn ngữ nâng cao của Javascript 
  + Dễ dàng hơn trong phát triển các dự án lớn.
  + Hỗ trợ lập trình hướng đối tượng như kế thừa, đóng gói, constructor, abstract, interface, implement, override.
  + Hỗ trợ tổ chức các hệ thống lớn qua module, namespace.
  + Mã nguồn mở và có cộng đồng hỗ trợ lớn.

---

### Ví dụ 

@title[Đoạn chương trình TypeScript]

<p><span class="slide-title">Đoạn chương trình TypeScript</span></p>

```typescript
class Vehicle {
    name: string;
    brand: string;
    constructor (name: string, brand: string) {
        this.name = name;
        this.brand = brand;
    }

    info() {
      return "Name: " + this.name + ", brand: " + this.brand;
    }

    start() {
        return this.brand + " " + this.name + " is runing.";
    }
}

let bugati = new Vehicle("Veyon", "Bugati");
bugati.start();
```

@[1,2](You can present code inlined within your slide markdown too.)
@[9-17](Displayed using code-syntax highlighting just like your IDE.)
@[19-20](Again, all of this without ever leaving your slideshow.)

---



