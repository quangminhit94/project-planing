# 1 App quét truyện tranh
Câu chuyện của chúng tôi: 

Đội ngũ dịch truyện tranh của chúng tôi tốn rất nhiều thời gian để edit truyện tranh. 

Công việc của chúng tôi là lấy các truyện tranh từ website nước ngoài đem về dịch lại thành tiếng anh và tiếng việt.

Quy trình làm việc để dịch truyện tranh bao gồm các công đoạn sau:

Tải xuống các file truyện tranh

Gõ lại nội dung lời thoại của nhân vật trong truyện ra một bản nháp

Từ nội dung nháp dịch sang tiếng việt hoặc tiếng anh

Dùng photoshop xóa phần ngôn ngữ cũ

Bỏ nội dung dịch vào phần đã xóa

Chỉnh sửa lại khung cho phù hợp vì sẽ có một số chữ dài hơn

Tải lên phần truyện được dịch vào website của chúng tôi

# Request

Chúng tôi cần một ứng dụng bao gồm các bước sau:
1. Tôi muốn chuyển đổi text trong ảnh sang text thật
2. Tôi muốn chuyển text thật sang ngôn ngữ khác
3. Tôi muốn xóa tất cả nội dung của các lời thoại cũ
4. Tôi muốn chèn nội dung mới vào khung vừa xóa
5. Tôi có thể chỉnh sửa nội dung dịch ở các vị trí được phân tích và đánh dấu

# Thiết kế
1. Việc chuyển đổi text trong ảnh sang text thật là có thể làm được 100%
2. Việc dịch ngôn ngữ từ text có thể chính xác đến 80%
3. Việc dùng tensorflow để đánh dấu khung và chèn lời thoại mới của hình ảnh là có thể làm được 100%
4. Đã ghi nhớ được vị trí khung thì cũng có thể chỉnh sửa lời thoại tại vị trí đó là đương nhiên

# Định hình một UI

1. Screen chuyển đổi: gồm một nút upload hình ảnh. Sau khi upload chuyển qua screen table và render các thông tin liên quan
2. screen Table: stt, tên ảnh, tọa độ cần sửa, nội dung cũ, nội dung mới. 1 button để render hình ảnh mới
3. Screen kết quả: hình ảnh kết quả. 1 nút dowload hình. \

![Design mockup cho app](https://i.ibb.co/XFPc4yr/design-1.png)

# Định hình logic cho app

- Hình ảnh không thể chỉnh sửa trực tiếp, chỉ có thể chỉnh sửa qua table
- Khi bấm vào tọa độ có thể scroll và hightlight bằng cách vẽ một khung màu vàng giả vào tọa độ đó
- Bấm vào tọa độ được phép chỉnh sửa trên hình có thể scroll đến vị trí bảng và focus vào dòng chứa tọa độ đó
- Canh chỉnh làm sao đừng để bị rớt chữ khỏi khung
