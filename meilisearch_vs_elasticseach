
Sự khác biệt chính giữa MeiliSearch và Elasticsearch là gì và tại sao chúng lại quan trọng?

Kể từ khi được thành lập vào năm 2010, Elasticsearch đã nhanh chóng trở thành một lựa chọn phổ biến trên thị trường công cụ tìm kiếm, được sử dụng trong tất cả các loại ứng dụng và bộ dữ liệu. Tuy nhiên, mặc dù không thể phủ nhận nó là một công cụ mạnh mẽ để tìm kiếm toàn văn bản nặng, nhưng nhu cầu cấu hình rộng rãi trước khi sử dụng có nghĩa là tất cả sức mạnh đó đi kèm với chi phí tài nguyên cao.

Đối với các công ty công nghệ lớn đang xử lý các bản ghi khổng lồ, Elasticsearch có thể có ý nghĩa. Nhưng khi nói đến bộ dữ liệu kích thước trung bình (tức là ít hơn năm triệu hàng) và các ứng dụng nhỏ hơn, thì điều đó đơn giản là không phù hợp với công việc. Tuy nhiên, vì trong lịch sử không có giải pháp thay thế mã nguồn mở nào, các nhà phát triển vẫn sử dụng Elastic làm giải pháp mặc định của họ và kết thúc bằng việc mất một lượng thời gian không tương xứng khi thiết lập và đào tạo.

Đây là nơi MeiliSearch xuất hiện. Cung cấp khả năng tìm kiếm nhanh, có liên quan và chịu được lỗi đánh máy với thời gian thiết lập rất nhanh, MeiliSearch là một giải pháp tuyệt vời cho bất kỳ nhà phát triển nào cần một công cụ tìm kiếm mạnh mẽ và dễ tiếp cận tập trung vào end user.

# 1 - Elasticsearch được tạo ra để làm gì?
## Lịch sử
Năm 2010, Shay Bannon giới thiệu phiên bản đầu tiên của Elasticsearch, một công cụ tìm kiếm phân tán được viết bằng Java. Được xây dựng dựa trên Lucene - một dự án do Doug Cắt bắt đầu vào năm 1999 sau khi viết bốn công cụ tìm kiếm khác cho các công ty như Apple - nó phù hợp với hầu hết mọi ứng dụng yêu cầu tìm kiếm toàn văn.

Trong khi Lucene là thứ ẩn chứa, Elasticsearch cung cấp giao diện cấp cao hơn cho người dùng: một API HTTP sử dụng các tài liệu JSON. Nó cũng cung cấp khả năng mở rộng vượt trội thông qua tính năng sharding và nhân rộng. Với việc bổ sung phần mềm trực quan và xử lý dữ liệu, Elasticsearch hiện được cung cấp như một giải pháp tích hợp đầy đủ để quản lý, giám sát và tìm kiếm dữ liệu. Tìm với từ khóa " ELK stack".

## Với sức mạnh lớn đi kèm với sự phức tạp lớn
Các trường hợp sử dụng cho Elasticsearch rất rộng, bao gồm mọi thứ từ tìm kiếm trang web đơn giản đến phân tích các bộ dữ liệu lớn.

Nhưng chỉ vì bạn có thể làm bất cứ điều gì với Elastic không có nghĩa là bạn nên làm. Để cấu hình Elasticsearch cho một cách sử dụng ứng dụng cụ thể, các nhà phát triển phải tìm hiểu khá nhiều về cách hoạt động của công cụ này. Tất nhiên, Elasticsearch cung cấp đào tạo - nhưng với một mức giá.

Elasticsearch rất mạnh mẽ khi nói đến bộ dữ liệu lớn; nó có thể nhanh chóng mở rộng quy mô theo chiều ngang và cho phép người ta xây dựng các truy vấn phức tạp. Mặt trái của điều đó là không có gì là dễ dàng. Ngay cả khi tất cả những gì bạn cần là chức năng tìm kiếm đơn giản xử lý lỗi chính tả, từ đồng nghĩa hoặc bộ lọc, bạn đang xem hàng giờ đào tạo, tài liệu và cấu hình. Đó là rất nhiều tài nguyên cho một thứ gì đó phải nhanh chóng và không gây đau đớn, đó là lý do tại sao nhiều công ty thuê các chuyên gia tư vấn của Elasticsearch để đẩy nhanh quá trình. Bạn có thấy một mô hình ở đây?

# 2 - MeiliSearch được tạo ra để làm gì?
MeiliSearch là một API tìm kiếm mã nguồn mở được viết bằng Rust, một ngôn ngữ lập trình hiệu quả và đáng tin cậy. Được tạo vào năm 2018 bởi Quentin Dequelen và Clement Renault, một người đóng góp cho Rust, nó mang lại hiệu suất cực cao đồng thời cho phép các nhà phát triển kiểm soát chi tiết mọi phân bổ bộ nhớ.

Với cấu trúc dữ liệu và thuật toán lấy cảm hứng từ Algolia, MeiliSearch nhằm mục đích cung cấp hiệu suất tốt nhất có thể cho tìm kiếm tức thì. Thay vì cố gắng tái tạo sức mạnh thô của Elasticsearch hoặc Lucene, MeiliSearch được xây dựng để triển khai nhanh như chớp, với chức năng tìm kiếm khi bạn nhập ngay lập tức.

Chúng tôi muốn MeiliSearch trở thành giải pháp tối ưu cho tìm kiếm của end user. Để đạt được điều đó, có ba yếu tố quan trọng cần xem xét: tốc độ, tính dễ sử dụng và dễ cài đặt.

## A. Tốc độ

MeiliSearch được thiết kế để trả lời trong vòng chưa đầy 50 mili giây. Ngưỡng tốc độ này rất quan trọng vì nó cho phép người dùng phản hồi tìm kiếm trong thời gian thực, thu hẹp cụm từ tìm kiếm của họ hoặc dừng sớm nếu họ đã tìm thấy những gì họ đang tìm kiếm.

Nó có thể chỉ tiết kiệm vài giây cho mỗi lần tìm kiếm, nhưng vài giây đó đại diện cho một sự gia tăng hiệu quả rất lớn cho người dùng. Trong mọi trường hợp, ít thời gian tìm kiếm hơn và nhiều thời gian duyệt hơn có nghĩa là nhiều nhấp chuột hơn, bán hàng tốt hơn hoặc tăng năng suất cho sản phẩm của bạn.

## B. Dễ sử dụng cho end user

Cùng với tính năng tìm kiếm tức thì, MeiliSearch cung cấp một ngôn ngữ truy vấn tự nhiên, chịu được lỗi đánh máy.

Điều này làm cho công cụ tìm kiếm cảm thấy đơn giản và trực quan. Việc các thanh tìm kiếm khiến người dùng cảm thấy như họ phải học một ngôn ngữ mới chỉ để đạt được kết quả tốt nhất đã quá phổ biến — hoặc tệ hơn, họ phải nhảy qua lại giữa tìm kiếm của mình và Google chỉ để viết đúng chính tả hoặc sản phẩm UID. MeiliSearch giúp cho việc tìm kiếm trở nên đơn giản và nhanh nhạy, vì vậy người dùng có thể tập trung vào kết quả.

## C. Dễ sử dụng cho các nhà phát triển

MeiliSearch cung cấp một bộ công cụ mở rộng để tùy chỉnh, bao gồm từ đồng nghĩa, từ dừng, quy tắc xếp hạng, v.v. Nhưng không giống như các công cụ tìm kiếm khác, các tùy chọn tùy chỉnh này chỉ là: tùy chọn.

MeiliSearch hoạt động độc lập với một cài đặt trước dễ dàng đáp ứng nhu cầu của hầu hết các ứng dụng.

Đối với MeiliSearch, chúng tôi chọn API RESTful vì hầu hết các nhà phát triển đã quen thuộc với các quy chuẩn của nó.

Vì vậy, chúng tôi đã tạo ra một công cụ tìm kiếm tức thì nhanh chóng, hiệu quả với thiết lập đơn giản. Nhưng tại sao lại dừng ở đó? Nhóm tại MeiliSearch đang nỗ lực trong việc xây dựng SDK bằng các ngôn ngữ khác nhau để người dùng có thể lập chỉ mục dữ liệu của họ nhanh nhất và dễ dàng nhất có thể (các ngôn ngữ được hỗ trợ hiện tại bao gồm Ruby, Python, JS, PHP và Golang). Trong tương lai, chúng tôi mong muốn bổ sung các tính năng để hỗ trợ tích hợp giao diện người dùng của các thanh tìm kiếm và những thứ tương tự.
