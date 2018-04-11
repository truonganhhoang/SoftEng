---
###Nhóm 8
### Assessing Correctness: Assertions
- Vai trò: Đảm bảo mã thực thi phù hợp với hành vi được chỉ định đúng.
- Kiểm thử tự động sử dụng BDD (Behavior Driven Development): tập trung phát triển phần mềm theo hướng hành vi. BDD: giúp xây dựng hệ thống kịch bản để thực thi test dưới góc độ ngôn ngữ tự nhiên từ các yêu cầu của khách hàng.

---
### Testability
- 5 bước trong thử nghiệm hệ thống phần mềm:
	- Reach
	- Triger
	- Propagate
	- Observe
	- Interpret

- Controllability 
	- Kiểm soát được tất cả các cấu trúc mã theo cách làm cho chúng ngắn hơn, gọn gàng hơn và làm cho hệ thống dễ hiểu hơn.
	- Do đó khuyến khích lập trình viên viết bài nhiều test hơn.

- Observability
	- Chạy mã với một số đầu vào được biết đến để kích hoạt một số lỗi, sau đó xác nhận liệu nó có đúng hay không?
	- Cách dễ dàng nhất để cải thiện khả năng quan sát trong mã: là thêm các loại trả về có ý nghĩa chính xác.

- Isolateability
	- Khi bộ kiểm tra thất bại có thể nhanh chóng, dễ dàng cô lập nguyên nhân của sự thất bại.
		=> cấu trúc lại hệ thống.
- Automatability
	- là sử dụng các công cụ để thực hiện các test case.
	- dùng trong các trường hợp: 
		- kiểm thử được thực hiện lặp đi lặp lại
		- kiểm thử thủ công khó thực hiện
		- kiểm thử tốn thời gian

- Testability Wrap-Up
	- 5 bước và các tính chất giúp trong việc cải thiện:
		- REACH : Controllbility, Automatability
		- TRIGGER: Controllbility,  Isolateability, Automatability
		- PROPAGATE: Observability, Automatability
		- OBSERVE: Observability, Automatability 
		- INTERPRET

---

### Module Wrap-Up
- Xem xét đoạn mã dưới đây:
~~~javascript
	function binarySearch<T>(array: T[], key: T, comparator: (op1: T, op2: T) => number): number {
  let low = 0,
      high = array.length - 1;

  while (low <= high) {
    let mid = ((low + high) / 2) | 0;
    let comp = comparator(array[mid], key);
    if (comp < 0) {
      low = mid + 1;
    } else if (comp > 0) {
      high = mid - 1;
    } else {
      return mid;
    }
  }
  return -(low + 1);
	}
~~~
- Để đơn giản, giả sử rằng "T" là bất kỳ kiểu nào. Vì vậy, các mảng có thể là một mảng của chuỗi,....
- Hàm binarySearch ở trên yêu cầu 33 tham số truyền vào: mảng thực hiện tìm kiếm nhị phân trên (được sắp xếp), khoá tìm kiếm trong mảng này và hàm so sánh.
- Hàm so sánh này có 2 tham số truyền vào và có thể trả về 3 giá trị
	- 1 chỉ ra rằng giá trị đầu tiên lớn hơn thứ hai
	- -1 chỉ ra rằng giá trị đầu tiên nhỏ hơn thứ hai
	- 0 chỉ ra rằng hai giá trị bằng nhau
- Với những gì bạn biết về chức năng này, hãy chọn một (hoặc nhiều hơn) các ý sau:
	- Viết các test cases white-box
	- viết các test cases black-box cho hàm comparator() sử dụng input partitioning
	- Viết các khẳng định cho binarySearch, tốt hơn cho các kiểu mảng / kiểu đầu vào khác nhau 
