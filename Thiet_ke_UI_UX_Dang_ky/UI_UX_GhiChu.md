# Báo cáo Thực hành: Thiết kế UI/UX Giao diện Trang Đăng Ký

## 1. Giải thích luồng người dùng (User Flow)
1. **Bước 1:** Người dùng truy cập trang đăng ký (`index.html`). Hệ thống hiển thị Form đăng ký với các trường thông tin rõ ràng.
2. **Bước 2:** Người dùng nhập thông tin: *Họ tên, Email, Mật khẩu, Xác nhận mật khẩu*. Các trường đều có placeholder hướng dẫn và được đánh dấu bắt buộc (`*`).
3. **Bước 3:** Người dùng tick chọn "Đồng ý với điều khoản dịch vụ".
4. **Bước 4:** Người dùng nhấn nút **"Đăng Ký Ngay"**.
5. **Bước 5:** Nếu thông tin hợp lệ, hệ thống chuyển hướng sang trang Xác nhận (`success.html`) thông báo đăng ký thành công và hướng dẫn bước tiếp theo (kiểm tra email).

## 2. Ghi chú UI/UX đã áp dụng
Thiết kế được xây dựng dựa trên các nguyên tắc UI/UX thân thiện và hiện đại:

- **Fitts' Law (Định luật Fitts):** Nút bấm "Đăng Ký Ngay" được thiết kế với kích thước lớn, trải dài toàn bộ chiều ngang form (`width: 100%`) và có padding dày. Điều này giúp người dùng dễ dàng đưa chuột tới và nhấp (hoặc chạm trên điện thoại) mà không cần ngắm chính xác, giảm thiểu thời gian thao tác.
- **Tính trực quan và Rõ ràng:** Sử dụng độ tương phản cao (nút màu xanh tím #4F46E5 trên nền trắng). Các trường bắt buộc có dấu sao màu đỏ (`*`) để cảnh báo.
- **Giao diện hiện đại (Aesthetics):** Sử dụng phông chữ `Inter` (không chân) dễ đọc, các khối có viền bo góc (`border-radius`), và hiệu ứng đổ bóng mềm (soft box-shadow) giúp tách biệt form đăng ký với hình nền gradient phía sau. 
- **Phản hồi tương tác (Micro-interactions):** Khi người dùng di chuột hoặc click vào ô input, viền ô sẽ đổi màu xanh và tỏa bóng mờ, giúp họ nhận biết mình đang tương tác ở đâu (Focus state). Nút bấm cũng có hiệu ứng chìm xuống nhẹ khi click.
- **Responsive Design (Tương thích thiết bị):** Sử dụng `max-width` và padding linh hoạt. Trên màn hình nhỏ (như điện thoại), form sẽ tự động thu hẹp và loại bỏ các khoảng trống thừa để tận dụng tối đa diện tích hiển thị.
- **Trang phản hồi (Success Page):** Sử dụng biểu tượng dấu tích xanh lớn để tạo cảm giác an tâm và thỏa mãn cho người dùng sau khi hoàn thành một tiến trình.
