# Báo cáo kết quả nghiên cứu

## Kết quả

|Nguồn|Thời gian nghiên cứu |
|--|--|
|https://www.youtube.com/watch?v=8t0vNu2fCCM| 10h45 - 14h ngày 24/8/2020 |

### Điểm mạnh
- Gatsby là một framework kết hợp react và graphql
- Gatsby mạnh về content managerment system, có thể lựa chọn các component giống wordpress
- khi làm freelance có thể tích hợp với wordpress làm được những website có nội dung static và dynamic

**Câu hỏi: tôi có thể xây dựng một dự án kinh doanh với gatsby và đem bán không?**

### Cài đặt
- Cài nodejs ở trang nodejs.org
- Cài lệnh `npm install -g gatsby-cli`
- tạo một project tên là hello-world dùng lệnh `gatsby new hello-world https://github.com/gatsbyjs/gatsby-starter-hello-world`

### Gatsby route
- Trong gatsby, tạo các file home.js, about.js và contact.js ở thư mục pages/ 
- Gatsby tự động tạo url `localhost:3000/home`, `localhost:3000/about`, `localhost:3000/contact`
- Có thể dùng `<Link to="contact">Contact me</Link>` thay vì dùng thẻ a để đổi route

**Nhận xét: Các trang home, about, contact cú pháp giống component react js nên khá dễ sử dụng**

