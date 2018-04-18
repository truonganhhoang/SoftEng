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

- Chúng ta nên nên quan tâm đến sự khác biệt giữa mã code và cách chúng chạy. Sự khác biệt đó thường sinh ra lỗi và đó lí do các trình gỡ lỗi rất quan trọng.
- Khi gỡ lỗi(debug), bạn nên đặt một điểm dừng.Sau đó, bạn xem xét sự khác biệt giữa các biến trong chương trình và trạng thái của chúng là gì? Tốt nhất là bạn nên xem xét từng dòng code của chương trình có thể hiểu được tất cả các trạng thái mà chương trình có thể gặp phải.
---

### Ngôn ngữ lập trình là gì?

- Ngôn ngữ lập trình có thể phân chia thành:
	+ Ngôn ngữ lập trình biên dịch.
	+ Ngôn ngữ lập trình thông dịch.

---

### Ngôn ngữ lập trình là gì?
- Đối với ngôn ngữ lập trình thông dịch, khi chương trình chạy đến dòng lệnh nào (theo thứ tự từ trên xuống dưới) thì dòng đó mới được dịch thành mã máy để chạy.

---

### Ngôn ngữ lập trình là gì?

- Để hiểu về ngôn ngữ biên dịch, ta có 2 ví dụ sau.
- Ví dụ 1:
~~~python
	declare m1() {
		print 'm1'
	}
	m1()
~~~
	+ Với ví dụ này, chương trình sẽ chạy bình thường. Hàm m1() được định nghĩa ở trên và sẽ được gọi ở dưới và kết quả là in ra m1.
	
---

### Ngôn ngữ lập trình là gì?

- Ví dụ 2:
~~~python
	m1()
	declare m1() {
		print 'm1'
	}
~~~
	+ Với ví dụ này, chương trình sẽ chạy đến lệnh gọi hàm m1(). Tuy nhiên đến đây thì máy không biết hàm m1() là gì và kết quả là chương trình sẽ dừng lại và báo lỗi.

---

### Ngôn ngữ lập trình là gì?

- Đối với ngôn ngữ lập trình biên dịch, khi chương trình sẽ được dịch (bằng trình biên dịch) toàn bộ thành mã máy rồi mới thực thi.
- Quá trình biên dịch sẽ giúp chúng ta phát hiện ra các lỗi cú pháp và kiểm tra tính chính xác trong mã nguồn. Đặc biệt là thứ tự trong mã nguồn không còn là vấn đề như với ngôn ngữ lập trình thông dịch.   

---

### Ngôn ngữ lập trình là gì?

- Một ví dụ với Java: 
~~~java
	class myClass {
		public static void main(String[] args){
			new myClass().m1();
		}

		public m1() {
			System.out.println('m1');
		}
	}
~~~
- Ví dụ trên sẽ chạy bình thường cho dù việc khai báo hàm m1() ở phía sau lời gọi hàm.
---

### Ngôn ngữ lập trình là gì?

- Một ví dụ khác với JavaScript: 
~~~javascript
	m1();
	function m1() {
		console.log('m1');
	}
~~~
- Ví dụ trên cũng sẽ chạy bình thường cho dù việc khai báo hàm m1() ở phía sau lời gọi hàm và javascript là một ngôn ngữ thông dịch. Lí do vì trong thực tế,mọi trình duyệt sẽ dùng trình biên dịch JIT để biên dịch mã JS thành mã máy trước khi thực hiện.
---

### Ngôn ngữ lập trình là gì?

- Ngoài ra, ngôn ngữ lập trình còn có thể phân chia thành:
	+ Ngôn ngữ kiểu tĩnh.
	+ Ngôn ngữ kiểu động.

---

### Ngôn ngữ lập trình là gì?

- Đối với ngôn ngữ lập trình kiểu tĩnh, ta khai báo 1 biến với kiểu dữ liệu cụ thể của nó. Và sau đó, trình biên dịch sẽ đi kiểm tra xem mọi thao tác với biến đó có thích hợp với kiểu dữ liệu của nó hay không.

---

### Ngôn ngữ lập trình là gì?

- Xét ví dụ sau:
~~~java
	int age;
	age = 10;
	age = 100;
	age = false;
	age = '10;'
~~~
- Với hai thao tác gán age bằng 10 và 100, chúng thực hiện bình thường vì chúng phù hợp với kiểu int của biến age.
- Nhưng 2 thao tác gán còn lại sẽ báo lỗi vì false và '10' không phù hợp với kiểu int của biến age.

---

### Ngôn ngữ lập trình là gì?

- Với ngôn ngữ kiểu động, chúng sẽ tự kết hợp kiểu dữ liệu với giá trị của biến.
- Xét ví dụ sau:
~~~javascript
	var age;
	age = 10;
	age = 100;
	age = false;
	age = '10;'
~~~
- Một phép gán trên đều thực hiện được. Biến age sẽ nhận các kiểu int, int, boolean và string tương ứng.

---

### Ngôn ngữ lập trình là gì?

- Với cách hoạt động như vậy, ngôn ngữ kiểu động sẽ cực kì linh hoạt khi ta có thể thay đổi kiểu của biến giữa chương trình. 
- Tuy nhiên, việc gỡ lỗi với ngôn ngữ kiểu động sẽ khó khăn hơn so với ngôn ngữ kiểu tĩnh.

---

### Ngôn ngữ lập trình là gì?

- Xét một ví dụ tương tự ngôn ngữ kiểu tĩnh với TypeScript:
~~~typescript
	var age: number;
	age = 10;
	age = 100;
	age = false;
	agr = '10';
~~~
- Ta đã khai báo và chỉ định kiểu cho biến age là number. Vì vậy phép gán với 10 và 100 vẫn sẽ thực hiện được còn 2 phép còn lại sẽ báo lỗi.

---

### Ngôn ngữ lập trình là gì?

- ta cũng có thể xét một ví dụ tương tự ngôn ngữ kiểu động với TypeScript:
~~~typescript
	var age;
	age = 10;
	age = 100;
	age = false;
	agr = '10';
~~~
- Bên trên hoàn toàn là một đoạn mã JS hợp lệ về mặt cú pháp. Tuy nhiên, kết quả khi chạy sẽ tương tự với ví dụ bên trên.

---

### Ngôn ngữ lập trình là gì?

- Đây là một cách thức hoạt động của JS. Khi ta khai báo biến age, ta hoàn toàn không khai báo kiểu number cho nó. Tuy nhiên, khi ta thực hiện phép gán giá trị 10 đầu tiên cho biến age, JS sẽ ngầm định ta đã gán kiểu number cho age và giữ kiểu đó cho age đến hết chương trình.

---

### Ngôn ngữ lập trình là gì?

- Tuy nhiên, ta có thể gán biến age như sau để kiểu của age có thể thay đổi mọi lúc trong chương trình như sau:
~~~typescript
	var age: any;
	age = 10;
	age = 100;
	age = false;
	agr = '10';
~~~
- Đoạn mã trên sẽ hoạt động bình thường mà không gặp bất cứ lỗi nào.

---

### Ngôn ngữ lập trình là gì?

- Tổng kết lại từ những ví dụ trên, ta có 
	+ Java, JavaScript và TypeScript giống nhau là đều có sử dụng trình biên dịch.
	+ Java là một ngôn ngữ kiểu tĩnh.
	+ JavaScript là một ngôn ngữ kiểu động.
	+ TypeScript là ngôn ngữ kiểu tĩnh nhưng có thể tùy chọn như ngôn ngữ kiểu động. Đặc biệt là TypeScript còn được hưởng lợi nhờ từ hệ sinh thái phong phú và các thư viện sẵn có của JS.

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



