# Hướng dẫn làm việc chung 😃

1. Ghi các vấn đề vào phần Issues 🤖

2. Các thành viên thảo luận để tìm solution 🚀

3. Phân chia task để giải quyết vấn đề 👨🏽‍💻

4. Đóng nhiệm vụ khi hoàn thành 💫

# Thói quen cần có 😃

1. Khi làm vào phần issue để kiểm tra 🎰

2. Cập nhật trạng thái để xác định tiến độ 🎯

3. Sắp xếp thời gian và hoàn thành nhiệm vụ 😎

**Tạo task hoặc question càng chi tiết càng dễ làm, nếu cần quay video hoặc vẽ để trình bày 🔥**

# Cam kết thời gian làm việc của tôi

- Từ 19h đến 21h cho việc này mỗi tối
- Cam kết mỗi cuối tuần họp mặt 1 lần để tổng kết rút kinh nghiệm, chia sẻ thông tin

# Quy trình làm việc

1. Họp team xác định ý tưởng yêu cầu dự án.
2. ấn định thành viên thiết kế giao diện, thiết kế các sơ đồ, chuẩn bị môi trường làm việc có thời gian nộp cụ thể, thường là 1 tuần.
4. họp thống nhất sơ bộ về ý tưởng, thiết kế giao diện , cơ sở dữ liệu, công nghệ sử dụng cho dự án, thiết lập môi trường làm việc nhóm như build server chung, tạo bitbucket , tạo server nexus để chia sẽ thư viện với nhau…
4. Ấn định rõ quy trình làm việc , cách thức viết code , định nghĩa các tên dùng chung, yêu cầu viết unit test hay doc cho các method như thế nào…
5. Set up project , mình dùng maven, chia nhỏ thành các module như client, service, business, dao …
6. Phần ai nấy làm , giao diện, nghiệp vụ, tương tác database , service ( tạo RESTful, kết nối thực thi nghiệp vụ …, kết nối đến các nguồn tài nguyên)
7. Làm xong thì ghép lại rồi bắt đầu giao cho tester kiểm thử nếu ok thì giao phần đó cho khách hàng.
- Làm theo mô hình Scrum
-Có những kỹ thuật cụ thể để có thể chia nhỏ ra làm như vậy như tạo server giả, database giả, tạo profile, mình không thể nói hết ra đây vì còn phụ thuộc ngôn ngữ bạn dùng, nhưng cơ bản nó là vậy.

1. Viết ra userstory có dạng “Who” want to “do something”:
- User muốn xem tất cả các user khác quanh mình.
- User muốn xem profile của user khác
…
2. Tiếp đó viết tiếp vào mỗi câu vế trước và sau đoạn “This man” need “to be something” before và “This man” will “be something” after that.
3. Dựa vào user story ta sẽ có hai danh sách.
- Danh sách thứ nhất là các đại từ => Ta có danh sách Users Role
- Danh sách thứ hai là các động từ => Ta có danh sách Usercases
4. Sau khi đã gợi mở được bài toán rồi thì ta vẽ lại các usercases.
- Nếu không biết vẽ thì ta có thể vẽ ra giấy sao cho em nhìn được các tương tác giữa các usercase là được.
- Với mỗi usercase lúc này ta sẽ định nghĩa xem hệ thống của ta phản hồi lại như thế nào?
5. Dựa trên việc ta biết hệ thống phản hồi ra sao nghĩa là ta biết được sản phẩm của em cần phải làm gì.
- Lúc này ta sẽ lựa chọn công nghệ để hoàn thành các công việc ta cần.
VD:
- Dùng gì để liên lạc với APi
- Dùng gì để load ảnh.
6. Khi đã lựa chọn xong, phần nào không chọn được ta phải nghiên cứu xem làm như thế nào trước.
7. Khi hoàn thành các bước trên ta tiến hành estimate và gửi cho khách hàng để họ xem.
8. Thống nhất được với khách hàng rồi thì ta tiến hành chia module dựa trên các usercase.
- Việc chia module này hiểu đơn giản là chia hệ thống thành các phần riêng biệt sao cho khi thay đổi một phần nào đó thì các phần khác sẽ không bị ảnh hưởng => Dựa trên kinh nghiệm là nhiều.
9. Sau khi chia được module tức là ta đã làm xong phần thiết kế hệ thống ở mức overview. Bước tiếp theo là detail design.
10. Sau khi thiết kế xong hết thì bắt đầu code.
- Tuy nhiên các bước trên đây chỉ mang tính lí thuyết được mô tả trong giáo trình PMBox. Giờ lâu không đọc cũng vừa liệt kê vừa phịa thêm là chủ yếu. Về thực tế thì bọn anh hay thực hiện coding ngay từ bước thứ 8. Bước estimate thường làm nó dài ra thêm khoảng 25% để dành cho việc nghiên cứu trong lúc code luôn. Bỏ qua bước số 5 để estimate sớm cho khách hàng.

# Bí quyết đơn giản để code bất cứ thứ gì

Đặt vấn đề: Bạn đang mở vscode và đang có một button của material-ui, bạn muốn custom style của button này nhưng không biết làm thế nào là hiệu quả nhất

- Bước 1: Mở google tìm từ khóa "how to custom theme in material-ui"
  - Tìm những kết quả ở trang doc chính thống trước https://material-ui.com/customization/theming/
  - Ta được một từ khóa createMuiTheme kèm ví dụ **Codesandbox**: https://codesandbox.io/s/rbtj4?file=/demo.js:499-580
- Bước 2: Vào vscode, copy một số đoạn code và custom lại cho đúng logic của mình
  - Bạn phải **debug đoạn code**. Bạn có thể dùng kỹ thuật console.log hoặc debug breakpoint. 
- Bước 3: Điều chỉnh lại các thông số cho chuẩn
  - Chỉ cần nắm được thông tin chứa trong phần debug bạn có thể suy nghĩ ra logic mình còn thiếu
  - Nếu vẫn chưa giải quyết vấn đề xong bạn đọc lại doc và truy xuất core bên trong node_module/
