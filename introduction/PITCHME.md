## Giới thiệu

- Nội dung chính:
	- Lập trình là gì?
	- Ngôn ngữ lập trình là gì? 
---

### Lập trình là gì?

- Là một quá trình mô tả ý tưởng của bạn và chuyển đổi nó thành một định dạng mà máy tính hiểu được.
- Cốt lõi của quá trình lập trình là khiến máy tính làm điều bạn muốn nó làm.

---

### Ngôn ngữ lập trình là gì?

- Ngôn ngữ lập trình đóng vai trò trung gian giữa người và máy tính.
- Hình thức hóa ý tưởng của lập trình viên sang cách cách máy tính có thể hiểu và thực hiện.

---

### Ngôn ngữ lập trình

- Có rất nhiều ngôn ngữ lập trình khác nhau.
- Chúng phân biệt bằng các yếu tố sau: 
	+ Cú pháp của ngôn ngữ.
	+ Thứ tự thực hiện của các mã.
	+ Ý nghĩa của các mã.

---

### Ngôn ngữ lập trình
- Mỗi ngôn ngữ lập trình lại có các đặc ngữ riêng của mình.
- Một chương trình có thể có cú pháp hợp lệ nhưng lại vô nghĩa.
- Ví dụ: "foo == foo".

---

### Ngôn ngữ lập trình

- Ngôn ngữ lập trình hầu như không sử dụng các đặc ngữ chỉ để miêu tả một ngoại lệ duy nhất.
- Trong một chương trình có tính bất biến (một đối tượng một khi đã được khai báo sẽ không bị thay đổi trong suốt chương trình).
 
---

### Ngôn ngữ lập trình

- Có sự khác biệt giữa mã code và cách chúng chạy. 
- Sự khác biệt đó thường sinh ra lỗi và đó lí do các trình gỡ lỗi rất quan trọng.

---

### Ngôn ngữ lập trình


- Khi gỡ lỗi(debug):
	- Đặt một điểm dừng.
	- Kiểm tra sự khác biệt giữa các biến trong chương trình và trạng thái của chúng. 
- Trong nhiều trường hợp, ta phải xem xét từng dòng code của chương trình có thể hiểu được tất cả các trạng thái mà chương trình có thể gặp phải.
---

### Ngôn ngữ lập trình

- Ngôn ngữ lập trình có thể phân chia thành:
	+ Ngôn ngữ lập trình biên dịch.
	+ Ngôn ngữ lập trình thông dịch.

---

### Thông dịch

- Khi chương trình chạy đến dòng lệnh nào (theo thứ tự từ trên xuống dưới) thì dòng đó mới được dịch thành mã máy để chạy.

---

### Thông dịch

- Ví dụ 1:
~~~python
	declare m1() {
		print 'm1'
	}
	m1()
~~~
	+ Với ví dụ này, chương trình sẽ chạy bình thường.
	
---

### Thông dịch

- Ví dụ 2:
~~~python
	m1()
	declare m1() {
		print 'm1'
	}
~~~
	+ Với ví dụ này, chương trình sẽ báo lỗi.

---

### Biên dịch

- Đối với ngôn ngữ lập trình biên dịch, khi chương trình sẽ được dịch (bằng trình biên dịch) toàn bộ thành mã máy rồi mới thực thi.
- Lợi ích: 
	+ Phát hiện ra các lỗi cú pháp và kiểm tra tính chính xác trong mã nguồn. 
	+ Không quan trọng thứ tự mã nguồn.   

---

### Biên dịch

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
- Ví dụ trên sẽ chạy bình thường.
---

### Biên dịch

- Một ví dụ khác với JavaScript: 
~~~javascript
	m1();
	function m1() {
		console.log('m1');
	}
~~~
- Ví dụ trên cũng sẽ chạy bình thường.
---

### Ngôn ngữ lập trình

- Ngoài ra, ngôn ngữ lập trình còn có thể phân chia thành:
	+ Ngôn ngữ kiểu tĩnh.
	+ Ngôn ngữ kiểu động.

---

### Ngôn ngữ kiểu tĩnh

- Đối với biến, ta phải khai báo biến kèm kiểu dữ liệu cụ thể của nó.
- Trình biên dịch sẽ đi kiểm tra xem mọi thao tác với biến đó có thích hợp với kiểu dữ liệu của nó hay không.

---

### Ngôn ngữ kiểu tĩnh

- Xét ví dụ sau:
~~~java
	int age;
	age = 10;
	age = 100;
	age = false;
	age = '10';
~~~
- Hai phép gán ban đầu thành công nhưng chương trình sẽ báo lỗi với hai phép gán sau.

---

### Ngôn ngữ kiểu động

- Với ngôn ngữ kiểu động, chúng sẽ tự kết hợp kiểu dữ liệu với giá trị của biến.
- Xét ví dụ sau:
~~~javascript
	var age;
	age = 10;
	age = 100;
	age = false;
	age = '10';
~~~
- Một phép gán trên đều thực hiện được (biến age sẽ nhận các kiểu int, int, boolean và string tương ứng).

---

### Ngôn ngữ kiểu động

- Với cách hoạt động như vậy, ngôn ngữ kiểu động sẽ cực kì linh hoạt. 
- Tuy nhiên, việc gỡ lỗi với ngôn ngữ kiểu động sẽ khó khăn hơn so với ngôn ngữ kiểu tĩnh.

---

### Kiểu tĩnh trong TypeScript

- Ví dụ:
~~~typescript
	var age: number;
	age = 10;
	age = 100;
	age = false;
	agr = '10';
~~~
- Hai phép gán ban đầu thành công nhưng chương trình sẽ báo lỗi với hai phép gán sau.

---

### Kiểu động trong TypeScript

- Xét một ví dụ tương tự ngôn ngữ kiểu động với TypeScript:
~~~typescript
	var age;
	age = 10;
	age = 100;
	age = false;
	agr = '10';
~~~
- Kết quả tương tự ví dụ trên.

---

### Kiểu động trong TypeScript

- Giải thích: Đây là một cách thức hoạt động của JS.
- Khi ta thực hiện phép gán giá trị 10 đầu tiên cho biến age, JS sẽ ngầm định ta đã gán kiểu number cho age và giữ kiểu đó cho age đến hết chương trình.

---

### Kiểu động trong TypeScript

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

### Tổng kết 

- Từ những ví dụ trên, kết luận
	+ Java, JavaScript và TypeScript giống nhau là đều có sử dụng trình biên dịch.
	+ Java là một ngôn ngữ kiểu tĩnh.
	+ JavaScript là một ngôn ngữ kiểu động.
	+ TypeScript là ngôn ngữ kiểu tĩnh nhưng có thể tùy chọn như ngôn ngữ kiểu động.

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



