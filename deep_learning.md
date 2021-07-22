# Deep learning 
Deep learning (còn được gọi là học cấu trúc sâu hoặc học phân cấp) là một tập hợp các thuật toán trong học máy cố gắng học ở nhiều cấp độ, tương ứng với các cấp độ trừu tượng khác nhau. Nếu chúng ta xem xét một trường hợp đơn giản, nơi có thể có hai tập hợp các tế bào thần kinh. Một bộ nơ-ron sẽ nhận một tín hiệu đầu vào và những bộ khác sẽ gửi một tín hiệu đầu ra. Khi lớp đầu vào nhận được tín hiệu đầu vào, nó sẽ chuyển phiên bản đã sửa đổi của đầu vào cho lớp tiếp theo. Trong một mạng sâu, có nhiều lớp giữa đầu vào và đầu ra, cho phép thuật toán sử dụng nhiều lớp xử lý, bao gồm nhiều phép biến đổi tuyến tính và phi tuyến tính.

Trong vài năm qua, các kỹ thuật được phát triển từ nghiên cứu Deep learning đã và đang tác động đến một loạt các công việc xử lý tín hiệu và thông tin trong phạm vi truyền thống và mới, được mở rộng bao gồm các khía cạnh chính của máy học và trí tuệ nhân tạo.

Ba lý do quan trọng cho sự phổ biến của Deep learning ngày nay là

- Khả năng xử lý của chip được tăng lên đáng kể (ví dụ: đơn vị xử lý đồ họa mục đích chung hoặc GPGPU),
- Chi phí phần cứng máy tính giảm đáng kể và
- Những tiến bộ gần đây trong học máy và nghiên cứu xử lý tín hiệu / thông tin.

Những tiến bộ này đã cho phép các phương pháp Deep learning khai thác hiệu quả các hàm phi tuyến phức hợp, có cấu trúc, để tìm hiểu các biểu diễn tính năng phân tán và phân cấp cũng như sử dụng hiệu quả cả dữ liệu được gắn nhãn và không được gắn nhãn.

Deep learning thường sử dụng mạng nơ-ron nhân tạo. Các cấp độ trong các mô hình thống kê đã học này tương ứng với các cấp độ khái niệm khác nhau, trong đó các khái niệm cấp độ cao hơn được định nghĩa từ các khái niệm cấp độ thấp hơn và các khái niệm cấp độ thấp hơn giống nhau có thể giúp xác định nhiều khái niệm cấp độ cao hơn.

Deep learning có hai khía cạnh chính:

- mô hình bao gồm nhiều lớp hoặc nhiều giai đoạn xử lý thông tin phi tuyến
- các phương pháp để học có giám sát hoặc không giám sát về biểu diễn đối tượng ở các lớp trừu tượng hơn, cao hơn liên tiếp. Deep learning nằm trong giao điểm giữa các lĩnh vực nghiên cứu của mạng nơ-ron, trí tuệ nhân tạo, mô hình đồ họa, tối ưu hóa, nhận dạng mẫu và xử lý tín hiệu.

Về mặt lịch sử, khái niệm Deep learning bắt nguồn từ nghiên cứu mạng nơ-ron nhân tạo. Mạng nơ-ron chuyển tiếp hoặc MLP có nhiều lớp ẩn, thường được gọi là mạng nơ-ron sâu (DNN), là những ví dụ điển hình về các mô hình có kiến trúc sâu. Truyền ngược (BP), được phổ biến vào năm 1980, là một thuật toán nổi tiếng để học các tham số của các mạng này. Thật không may, chỉ riêng việc truyền lại đã không hoạt động tốt trong thực tế.

Sử dụng các lớp ẩn với nhiều nơ-ron trong một DNN cải thiện đáng kể sức mạnh mô hình hóa của DNN và tạo ra nhiều cấu hình tối ưu chặt chẽ. Ngay cả khi việc học tham số bị mắc kẹt trong mức tối ưu cục bộ, DNN kết quả vẫn có thể hoạt động khá tốt vì cơ hội có mức tối ưu cục bộ kém thấp hơn so với khi một số lượng nhỏ tế bào thần kinh được sử dụng trong mạng. Tuy nhiên, việc sử dụng mạng nơ-ron sâu và rộng sẽ tạo ra nhu cầu lớn về sức mạnh tính toán trong quá trình đào tạo.

Hầu hết các kỹ thuật học máy và xử lý tín hiệu đã khai thác các kiến trúc có cấu trúc nông. Các kiến trúc này thường chứa nhiều nhất một hoặc hai lớp biến đổi đối tượng địa lý phi tuyến. Ví dụ về các kiến trúc nông là mô hình hỗn hợp Gaussian (GMM), Máy vectơ hỗ trợ (SVM), hồi quy logistic, hồi quy hạt nhân, perceptron nhiều lớp (MLP) với một lớp ẩn duy nhất bao gồm các máy học cực đoan (ELM). Ví dụ: SVM sử dụng mô hình phân tách mẫu tuyến tính nông với một hoặc không lớp biến đổi tính năng. Các kiến trúc nông đã được chứng minh là có hiệu quả trong việc giải quyết nhiều vấn đề đơn giản hoặc hạn chế tốt, nhưng sức mạnh mô hình và biểu diễn hạn chế của chúng có thể gây ra khó khăn khi xử lý các ứng dụng phức tạp hơn trong thế giới thực liên quan đến các tín hiệu tự nhiên như giọng nói của con người, âm thanh và ngôn ngữ tự nhiên, hình ảnh tự nhiên và cảnh trực quan.

Các thuật toán Deep learning tương phản với các thuật toán học nông bởi số lượng các phép biến đổi tham số hóa mà một tín hiệu gặp phải khi nó truyền từ lớp đầu vào đến lớp đầu ra. Ở đây, phép chuyển đổi tham số hóa là một đơn vị xử lý có các tham số có thể đào tạo, chẳng hạn như trọng số và ngưỡng.

Để đơn giản, chúng ta có thể nghĩ DNN như hộp đen ra quyết định. Chúng lấy một mảng số (có thể đại diện cho pixel, dạng sóng âm thanh hoặc từ), chạy một loạt các hàm trên mảng đó và xuất một hoặc nhiều số làm đầu ra. Kết quả đầu ra thường là dự đoán về một số thuộc tính mà chúng tôi đang cố gắng đoán từ đầu vào, chẳng hạn như hình ảnh có phải là hình ảnh của một con mèo hay không.


Các chức năng được chạy bên trong hộp đen được điều khiển bởi bộ nhớ của mạng nơ-ron, các mảng số được gọi là trọng số xác định cách các đầu vào được kết hợp và kết hợp lại để tạo ra kết quả. Đối phó với các vấn đề trong thế giới thực như phát hiện mèo đòi hỏi các chức năng rất phức tạp, có nghĩa là các mảng này rất lớn, chứa khoảng 60 triệu số trong trường hợp của một trong các mạng thị giác máy tính gần đây. Trở ngại lớn nhất đối với việc sử dụng mạng nơ-ron là tìm ra cách đặt tất cả các mảng lớn này thành các giá trị sẽ thực hiện tốt công việc chuyển đổi tín hiệu đầu vào thành dự đoán đầu ra.

Một trong những đặc tính lý thuyết của mạng nơ-ron khiến các nhà nghiên cứu tiếp tục nghiên cứu chúng là chúng phải có thể dạy được. Khá đơn giản để chỉ ra ở quy mô nhỏ cách bạn có thể cung cấp một loạt đầu vào mẫu và đầu ra dự kiến, đồng thời trải qua một quy trình cơ học để lấy trọng số từ các giá trị ngẫu nhiên ban đầu thành các con số tốt hơn dần dần tạo ra các dự đoán chính xác hơn.

**Kiến trúc mạng nơ-ron của Deep learning khác với các mạng nơ-ron "bình thường" như thế nào?** Kiến trúc mạng nơ-ron Deep learning khác với mạng nơ-ron "bình thường" vì chúng có nhiều lớp ẩn hơn và chúng có thể được đào tạo theo cách UNSUPERVISED hoặc SUPERVISED cho cả nhiệm vụ học tập UNSUPERVISED và SUPERVISED. Hơn nữa, mọi người thường nói về việc đào tạo một mạng sâu theo cách không có giám sát, trước khi đào tạo mạng theo cách có giám sát.

**Tại sao lại có nhiều lớp trong DNN?** Deep learning hoạt động nhờ vào kiến trúc của mạng VÀ quy trình tối ưu hóa được áp dụng cho kiến trúc đó. Mạng là một đồ thị có hướng, nghĩa là mỗi đơn vị ẩn được kết nối với nhiều đơn vị ẩn khác bên dưới nó. Vì vậy, mỗi lớp ẩn đi sâu hơn vào mạng là sự kết hợp KHÔNG TUYẾN TÍNH của các lớp bên dưới nó, bởi vì tất cả sự kết hợp và kết hợp lại của các đầu ra từ tất cả các đơn vị trước đó kết hợp với các chức năng kích hoạt của chúng. Khi quy trình TỐI ƯU HÓA được áp dụng cho mạng, mỗi lớp ẩn sau đó sẽ trở thành một tổ hợp TỐI ƯU TỐI ƯU, KHÔNG TUYẾN TÍNH của lớp bên dưới nó. Khi mỗi lớp ẩn tuần tự có ít đơn vị hơn lớp bên dưới nó, mỗi lớp ẩn cũng trở thành DỰ ÁN KÍCH THƯỚC THẤP HƠN của lớp bên dưới nó. Vì vậy, thông tin từ lớp bên dưới được tóm tắt độc đáo bằng DỰ ÁN KHÔNG TUYẾN TÍNH, TỐI ƯU, TỐI ƯU, KÍCH THƯỚC THẤP HƠN trong mỗi lớp tiếp theo của mạng sâu.

**Các vấn đề với mạng nơron sâu** Nếu các DNN được đào tạo một cách thuần túy, nhiều vấn đề có thể phát sinh. Hai vấn đề phổ biến là trang bị quá nhiều và thời gian tính toán.

Các DNN dễ bị trang bị quá mức vì các lớp trừu tượng được thêm vào, cho phép chúng mô hình hóa các phần phụ thuộc hiếm gặp trong dữ liệu huấn luyện. Overfitting Các phương pháp điều chỉnh có thể được áp dụng trong quá trình đào tạo để giúp chống lại tình trạng quá sung. Một phương pháp chính quy gần đây hơn được áp dụng cho các DNN là chính thức hóa bỏ. Khi bỏ học, một số đơn vị quân ngẫu nhiên bị bỏ qua khỏi các lớp ẩn trong quá trình huấn luyện. Điều này giúp phá vỡ các phụ thuộc hiếm có thể xảy ra trong dữ liệu huấn luyện.

Có nhiều tham số huấn luyện cần được xem xét với một DNN, chẳng hạn như kích thước (số lớp và số đơn vị trên mỗi lớp), tốc độ học và trọng số ban đầu. Việc quét qua không gian tham số để tìm các tham số tối ưu có thể không khả thi do tốn kém thời gian và tài nguyên tính toán.
