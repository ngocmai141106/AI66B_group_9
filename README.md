**AI ĐỘNG VÀO FILE TRAIN TEST SẼ BỊ BẮN BỎ !**
Ae chạy thử code về thì đừng chạy ô số 20 và 21 nhé, nó lquan đến tạo file train test. T sợ mỗi lần chạy nó chia một kiểu khác, mà file được chia đêm qua mình đã deal với nhóm kia rồi í.
Những gì maitran đã làm đêm qua (ae có thể đọc để tham khảo làm slide):
- Load các thư viện cần thiết
- In thử vài dòng của dataset, kích thước của nó, và data type của từng cột
- Loại bỏ cột ID (không có giá trị thống kê)
- Kiểm soát NaN và những ô bị trống dưới dạng một dấu cách [ ]
- Tìm hiểu các ô bị trống dưới dạng một dấu cách [ ] này. Theo t quan sát thì mấy ô này đều có Tenure = 0 (tức là không hề gắn bó/dùng dịch vụ) nhưng Monthly charges (trả tiền hàng tháng) không hề bị trống
  Tức là có dùng dịch vụ, mâu thuẫn với Tenure 0 bên trên. Có thể do sai sót hoặc hỏng hóc dữ liệu, t drop vì sluong thiếu cũng không là gì so với size dataset
- Encode lại cột Senior citizen từ 0/1 thành Yes/No (tại các cột Có/không khác cũng để Y/N mà. làm vầy cho đẹp)
- Encode lại tất cả các cột Y/N thành 0/1
- Tách tệp X, y
- Chia train-test 8:2. Lưu thành file csv riêng.
  (Sẽ update thêm nếu kịp làm trước t6 tuần này)
