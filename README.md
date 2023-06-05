# Geographic_viz
trực quan hóa bản đồ địa lý bằng thư viện geoplotib
Giai đoạn 1: Đọc dữ liệu từ tệp CSV và hiển thị một số dòng đầu tiên của DataFrame.

Mục đích: Đọc dữ liệu từ tệp CSV ('2015.csv') và hiển thị một số dòng đầu tiên để xem dữ liệu có được tải chính xác không.
Có vẻ không có sự cố trong giai đoạn này, vì bạn không báo cáo về bất kỳ lỗi nào.
Giai đoạn 2: Đọc dữ liệu của các quốc gia từ tệp CSV và hiển thị một số dòng đầu tiên của DataFrame.

Mục đích: Đọc dữ liệu của các quốc gia từ tệp CSV ('countries.csv') và hiển thị một số dòng đầu tiên để xem dữ liệu có được tải chính xác không.
Có vẻ không có sự cố trong giai đoạn này, vì bạn không báo cáo về bất kỳ lỗi nào.
Giai đoạn 3: Chuẩn bị dữ liệu và hiển thị đồ thị bằng thư viện geoplotlib.

Mục đích: Tạo một đối tượng DataAccessObject từ DataFrame và thêm lớp KMeansLayer vào đối tượng geoplotlib. Đồng thời, cài đặt các thuộc tính bổ sung cho geoplotlib và hiển thị đồ thị bằng cách sử dụng geoplotlib.show().
Sự cố gặp phải: Bạn đã gặp cảnh báo về rò rỉ bộ nhớ và số lượng cụm nhỏ hơn mong đợi.
Khắc phục: Bạn đã thử thiết lập biến môi trường OMP_NUM_THREADS thành 1 và loại bỏ các điểm trùng lặp bằng cách sử dụng phương thức drop_duplicates() của DataFrame. Tuy nhiên, các cảnh báo vẫn tiếp tục xuất hiện.
Để có trải nghiệm tốt hơn cho lần sau, bạn có thể xem xét các điều sau:

Kiểm tra kỹ tệp dữ liệu để đảm bảo chúng không có lỗi hoặc điểm trùng lặp trước khi đọc chúng vào DataFrame.
Xem xét cách mà thuật toán KMeans được triển khai và có bất kỳ vấn đề gì đối với phiên bản sklearn hiện tại mà bạn sử dụng không. Cập nhật phiên bản sklearn có thể giúp giải quyết các vấn đề tiềm năng.
Nếu các cảnh báo không ảnh hưởng đến kết quả cuối cùng, bạn có thể tiếp tục sử dụng mã của mình và chỉ chú ý đến những cảnh báo thực sự quan trọng hoặc có ảnh hưởng đến kết quả phân tích.
Tham khảo: từ nguồn https://github.com/neerjad/DataVisualization
