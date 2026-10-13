# Case Study 2: Trang Web Tĩnh Giới Thiệu Về Sách (Book Landing Page)

Dự án hoàn thành trong khuôn khổ học phần **[Web Frontend] Building Website with HTML and CSS** tại CodeGym.

## 📌 Các phần chính trong website
Trang web bao gồm đầy đủ 7 thành phần theo yêu cầu:
1. **Header & Book Overview**: Navbar với hiệu ứng sticky menu khi scroll, banner giới thiệu sách cùng nút đặt mua.
2. **Author**: Giới thiệu về tác giả, hình ảnh chân dung và tiểu sử tác phẩm.
3. **Features**: Các tính năng và thông số nổi bật (Happy Readers, Books Sold, 5-Star Reviews, Community) kèm hiệu ứng animation đếm số tự động bằng JavaScript jQuery.
4. **Prices**: Bảng so sánh các gói sản phẩm (PDF Version, E-book, Paperback Print) dạng Card layout.
5. **Download**: Giới thiệu tải ứng dụng đọc sách đa nền tảng (Desktop & Mobile).
6. **Reader’s Say**: Đánh giá thực tế từ độc giả với Card layout và Bootstrap Carousel slider.
7. **Footer**: Thông tin About us, form đăng ký nhận tin (Newsletter) và liên kết mạng xã hội (Social Media).

## 📱 Khả năng Responsive
- Sử dụng **Bootstrap 4.6 Grid System** kết hợp **CSS Flexbox**.
- Tối ưu hiển thị đa kích thước màn hình qua media queries trong `css/mobile.css`:
  - Desktop (>992px)
  - Tablet (768px - 991px)
  - Mobile (<768px, 375px, 320px)

## 📁 Cấu trúc thư mục
```
Case_Study_2_Book_Landing_Page/
├── index.html        # Trang chính
├── assets/           # Hình ảnh sách, tác giả, icon, avatars
├── css/
│   ├── style.css     # CSS tuỳ chỉnh chính, Google Fonts, gradients
│   └── mobile.css    # Responsive media queries cho mobile/tablet
├── js/
│   └── main.js       # Sticky navbar và counter animation khi scroll
├── src/
│   └── index.html    # Mã nguồn tham khảo bổ trợ
└── README.md         # Tài liệu dự án
```

## 🚀 Hướng dẫn mở trang
- Mở trực tiếp file `index.html` trong trình duyệt hoặc sử dụng Live Server.
