# Low level design(Thiết kế cấp thấp)
---

## Mẫu thiết kế mặt tiền (Facade)
![Facade](http://aptech.fpt.edu.vn/images/CongNghe07-04-06_pic1_large.gif)
---

## Khái quát
- Là mô hình cấu trúc giúp client sử dụng hệ thống con dễ dàng hơn bằng cách làm giảm sự phức tạp của nó
- Client không cần đọc các kiểu khai báo khác nhau và sử dụng chúng một cách độc lập, mà chỉ cần tương tác với mặt ngoài của chính nó
- Mặt tiền ẩn đi các cài đặt của các kiểu khác nhau từ máy khách
---

## Ví dụ
- Trong ví dụ, client cần biết về các lớp (class) khác nhau nhưng việc học sử dụng chúng khá phức tạp. Khi thêm vào một mặt tiền vào hệ thống, client chỉ cần tương tác với nó
- Mặt tiền sẽ chuyển các yêu cầu lên các lớp trong hệ thống con được yêu cầu
- Mặt tiền không chặn client thực hiện một số công việc mà client muốn làm. Một client có thể có sự phụ thuộc vào một thành phần trong hệ thống con, nhưng vẫn có thể sử dụng mặt tiền cho tác vụ khác của chúng
---

## Lợi ích
- Mặt tiền đơn giản hóa hệ thống con, cung cấp một chế độ xem đơn giản, giúp việc tái sử dụng mã (code) cũng dễ dàng hơn
- Lấy các giao diện (interface) làm tham số (parameter) và trả lại các loaị giao diện trong kết quả, để sử dụng lại client mà không cần dùng toàn bộ hệ thống con
---

## Một số lưu ý
- Về nguyên tắc thiết kế cấp thấp, nó khuyến khích sự kết hợp giữa client và hệ thống con
- Về nguyên tắc thiết kế chắc chắn, nó vi phạm nguyên tắc trách nhiệm đơn lẻ, do mặt tiền cung cấp quyền truy cập vào rất nhiều tác vụ trong hệ thống con
- Nên cần cân nhắc các loại hình hỗ trợ muốn có trong tương lai
---

## Mẫu thiết kế Decorator
![Decorator](https://static.dzone.com/dz1/dz-files/decorator_pattern_0.png)
---

## Khái quát
- Cho phép thêm các kết hợp tùy ý của các hành vi vào các thể hiện (instance) riêng của đối tượng thay vì thêm vào mọi thể hiện của một lớp
- Sử dụng các thành phần thừa kế bên trong, nhưng sức mạnh của mô hình lại đến từ các trường được đóng gói bên ngoài
- Kết hợp các hành vi có thể có mà không cần biên soạn trước
---

## Khái quát
- Mục đích là gói các hành vi mới vào một thể hiện của đối tượng
- Giao diện thành phần khai báo các hành vi mức cao cần được thực hiện trên tất cả các lớp trong mẫu thiết kế
- Có khả năng tạo ra các hành vi mới tại runtime
---

## Ví dụ
-Trong khung hình của game Mario, thêm một số hành vi được thêm vào để giúp trò chơi hấp dẫn trực quan hơn.
![Exp](https://i.imgur.com/joUywms.png)
---

## Ví dụ
- Nếu muốn các hành vi xảy ra độc lập thì sẽ ổn. Nhưng khi các hành vi xảy ra cùng một lúc thì nó sẽ thêm vào nhiều loại tĩnh (static) hơn, và chúng phải được triển khai
- Decorator sắp xếp các hành vi  một cách độc lập mà không phải chú ý đến các kết hợp khác nhau
- Trong trường hợp có nhiều khung trò chơi, các hành vi phải được đóng gói cho các loại khung đó
---

## Ví dụ
- Các hành vi có thể xếp chồng lên khung trò chơi và có thể sắp xếp một cách tùy ý mà không cần thêm một loại mới
- Mẫu thiết kế decorator cho phép áp dụng chúng lên từng loại khung trò chơi khác nhau
- Client có thể tham chiếu đến khung trò chơi và sắp xếp các hành vi mới một cách tự động
---

## Một số lưu ý
- Có thể thay đổi tại runtime
- Hỗ trợ nguyên tắc mở/đóng (open/close). Nếu muốn mở rộng hệ thống với hành vi mới, chỉ cần thực hiện kiểu decorator của chính nó
- Việc gỡ lỗi cũng cần đòi hỏi sự khéo léo, vì khó có thể thấy sự lớp đối tượng bên trong nó
---

## Mẫu thiết kế MVC (Model View Controller)
![MVC](https://i.stack.imgur.com/E5ynk.png)
---

## Khái quát
- Tách khung nhìn (view) khỏi việc triển khai, vì khung nhìn là những gì thay đổi nhiều nhất
- Việc tách khung hình cũng làm đơn giản khả năng kiểm thử
- MVC gồm 3 thành phần chính: mô hình (model), khung nhìn (view) và điều khiển (controller)
---

## Phần mô hình (model)
- Chứa nhiều loại đối tượng khác nhau, với hàng ngàn hàng triệu đối tượng. 
- Chứa tất cả dữ liệu của ứng dụng 
- Biết cách xác nhận tính toàn vẹn của chính nó bằng tự bảo vệ - bằng cách tự lưu vào đĩa hoặc chèn vào cơ sở dữ liệu nào đó
---

## Phần mô hình (model)
- Không biết cách tự biểu diễn (render), nó chỉ là một biểu diễn tập trung vào dữ liệu
- Có thể tái sử dụng nó một cách dễ dàng giữa các ứng dụng, vì nó là một miền độc lập
- Khi triển khai đối tượng mô hình trong MVC, chúng thường là các đối tượng trong mô hình thiết kế quan sát (observer design pattern)
---
		
## Phần khung nhìn (view)
- Hiển thị các đối tượng mô hình mà mọi người có thể quan sát
- Bất cứ khi nào mô hình cập nhật, nó sẽ thông báo sự kiện đến khung nhìn
- Nó không biết những gì thay đổi, và sẽ thực hiện gọi đối tượng mô hình và yêu cầu trạng thái của nó
- Trong hầu hết các ứng dụng xây dựng dựa trên MVC, sẽ có nhiều khung nhìn. 
- Khi observer thông báo đồng thời rằng nhiều khung hình thay đổi, chúng có thể truy xuất trạng thái cần thiết để hiển thị
---

## Phần điều khiển (controller)
- Được gắn kết chặt chẽ với khung nhìn mà nó liên kết, nó phản ứng với những thay đổi trong khung nhìn và cập nhật các mô hình phù hợp
- Chứa tất cả các logic nghiệp vụ (business logic - xử lý dữ liệu, kiểm tra ràng buộc, tính toán, xử lý yêu cầu) để phản hồi các hành động của người dùng, cập nhật mô hình theo yêu cầu cụ thể của chương trình
---

## Phần điều khiển (controller)
- Có một sự ràng buộc giữa mô hình và phần điều khiển, vì nó biết cách cập nhật trạng thái
- Có một sự ràng buộc giữa khung nhìn và phần điều khiển, các khung nhìn phải biết các mô hình chúng muốn hiển thị
---

## Cách triển khai
- Khi người dùng nhấp vào nội dung nào đó trong khung nhìn, nó gọi sự thay đổi trong điều khiển. 
- Một số logic nghiệp vụ trong điều khiển kích hoạt sự kiện cho tất cả khung nhìn
- Khi khung nhìn nhận được thông báo từ mẫu quan sát nó sẽ gọi vào đối tượng mô hình để truy xuất trạng thái nó cần để cập nhật hiển thị
---

## Ví dụ
- Đầu tiên, mô hình được dựa trên khái niệm của một hình thái (figure).
- Đối tượng hình thái đó là dữ liệu, trong game, các nhân vật sẽ có rất nhiều thông tin. Cần phân chia các hình thái để có các mô hình riêng biệt và triển khai chế độ xem
---

## Ví dụ
- Về mặt khung nhìn, nó cần biết diễn giải các đối tượng mô hình nhẹ và biến chúng thành số liệu để hiển thị. Khung nhìn sẽ cập nhật khi nó nhận phương thức thông báo từ đối tượng mô hình
- Trong trường hợp sử dụng các phím hay chuột, khung nhìn sẽ cập nhật và chuyển đầu vào thô vào bộ điều khiển. Từ đó bộ điều khiển sẽ di chuyển các đối tượng mô hình xung quanh một cách thích hợp, tất cả sẽ được lo trong bộ điều khiển
---

## Lợi ích
- MVC tách khung nhìn khỏi phần còn lại của hệ thống, điều này đem lại 4 lợi ích:
	- Giải phóng đường dẫn quan trọng cho ứng dụng bằng cách tách những người làm việc trên khung nhìn từ những người làm việc trên bộ điều khiển
	- Giúp dễ dàng trong việc thêm các khung nhìn cộng tác, vì có thể thêm nhiều khung nhìn hoạt động trên cùng một nguồn dữ liệu
---

## Lợi ích
	- Khi thêm khung nhìn mới vào hệ thống, chúng dễ dàng được thêm mà không thay đổi các thành phần khác của hệ thống đã được phát triển
	- Xét về khả năng kiểm thử, việc thử nghiệm hệ thống trên MVC dễ dàng hơn nhiều, đặc biệt là khi quản lý để đẩy càng nhiều chức năng vào bộ điều khiển càng tốt
---

## Một số lưu ý
- Nếu mô hình chứa hàng nghìn, hàng vạn đối tượng, khi chúng bắt đầu kích hoạt thông báo, mô hình có thể tràn ngập khung nhìn
- Với một số mô hình nhỏ, quá trình giải mã rất phức tạp
- Dễ dẫn đến khung nhìn lớn, và điều khiển nó là một vấn đề vì nó không dễ dàng
---

## Một số lưu ý
- Trong mô hình này, rất dễ để đặt nhiều chức năng vào khung hình. Đây thực sự là vấn đề vì khung nhìn rất khó để kiểm tra
- Cần đẩy nhiều chức năng nhất có thể ra ngoài khung nhìn và đưa nó vào điều khiển, nơi dễ kiểm tra hơn và làm khung nhìn nhẹ đi, dễ sử dụng hơn
---

## Mẫu thiết kế MVP (Model View Presenter)
![MVP](https://i-msdn.sec.s-msft.com/dynimg/IC340102.png)
---

## Khái quát
- Mẫu thiết kế MVP (Model View Presenter) là một sự hiện đại hóa trên cơ sở MVC để tăng cường khả năng kiểm thử trên hệ thống
- Giảm số lượng mã có thể có trong khung nhìn, buộc các bộ điều khiển hoặc trình bày (presenter) trong trường hợp của MVP để có nhiều tính năng hơn
---

## Khái quát
- Các thành phần của MVP tương tự MVC, có một sự khác biệt nhỏ là mô hình sẽ tương tác với tầng giữa-tầng biểu thị/trình bày (the presenter)-sử dụng một bus sự kiện
- Bus sự kiện chỉ là một thành phần của bên thứ ba kiểm duyệt sự tương tác giữa 2 tầng này 
---

## Một số khác biệt so với MVC 
- Không có bất kỳ sự phụ thuộc nào vào thành phần giao diện người dùng (UI - User Interface), điều này giúp dễ dàng trong việc kiểm thử tầng trình bày
- Ở đây, khung nhìn không kết hợp với mô hình (model). Tầng trình bày hoạt động như một đầu nối. Nó có thể cập nhật mô hình trong trạng thái truy xuất. Nó phản hồi lại để thông báo sự kiện, nhưng nó chưa bao giờ truyền đối tượng mô hình đến khung nhìn
---

## Một số khác biệt so với MVC 

- Chỉ tương tác với khung nhìn bằng kiểu nguyên thủy (chuỗi, số, mảng). Những thứ đó sẽ được hiển thị, nhưng khung nhìn không thực sự nhận các đối tượng mô hình
- Khung nhìn phải truyền dữ liệu xuống cho tầng trình bày theo định dạng đơn giản. Và cho phép tầng trình bày làm tất cả các phần logic của ứng dụng
---
		
## Cách hoạt động
- Hành động của người dùng được truyền xuống cho phần trình bày. Nếu các hành động này bao gồm dữ liệu, chỉ các phiên bản nguyên thủy của dữ liệu mới được chuyển 
- Tầng trình bày sau đó sẽ sửa đổi trạng thái nội bộ của nó và cập nhật tầng mô hình nếu cần
---

## Cách hoạt động
- Khi mô hình được cập nhật, nó sẽ kich hoạt các sự kiện được truyền lại cho tầng trình bày 
- Một khi tầng trình bày có bản cập nhật của tầng mô hình, điều tiếp theo là nó sẽ đi cập nhật khung nhìn. Bước này chỉ gửi dữ liệu nguyên thủy lên khung nhìn
---

## Một số lưu ý
- Giống như MVC, mục tiêu chính của MVP là tách rời khung nhìn từ mô hình. Nhưng khác với MVC, MVP thực thi việc tách rời này bằng cách không cho bất kỳ đối tượng mô hình nào có thể đưa nó lên màn hình
- Cần chia nhỏ tầng trình bày, để không chỉ có một đối tượng trình bày, mà về cở bản là bao gồm tất cả các logic cho toàn bộ ứng dụng
- Cách MVP dùng bus sự kiện làm thay đổi hiệu quả của hệ thống
---

## Mẫu thiết kế MVC và MVP
![MVCP](https://i.stack.imgur.com/aebJI.png)
---

## Về các mẫu thiết kế tương đương
- MVVM (model view, view model) như một chuyên biệt hóa của MVP, nơi khung nhìn và tầng trình bày được ràng buộc chặt chẽ hơn, sử dụng ràng buộc dữ liệu hai chiều
- Tất cả những mô hình thế này đều bắt đầu từ việc tách rời khung nhìn từ triển khai.
---

## Về các mẫu thiết kế tương đương
- Các thành phần phải được độc lập với nhau. Điều này làm tăng khả năng tái sử dụng của chúng. Giúp việc sửa lỗi nhanh chóng hơn, dễ dàng thêm các tính năng mới vào hệ thống
- Bằng cách phân tách các khía cạnh chính của hệ thống, theo thời gian, MVC, MVP,MVVM, meta models, tất cả các cách tiếp cận khác nhau này giúp các nhà thiết kế tốt đưa ra được các quyết định thiết kế tốt hơn
