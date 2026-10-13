# BẢNG PHÂN TÍCH CẤU TRÚC WEBSITE TEMPLATE THỰC TẾ

## 1. Trang web được lựa chọn phân tích: TechNews & Blog (Mẫu theo TechCrunch / Medium)

Một Website Template tiêu chuẩn trong phát triển giao diện Web bao gồm 4 phần cốt lõi:

### 1. Header (Đầu trang)
- **Vị trí:** Nằm trên cùng của trang web.
- **Nội dung:** Logo thương hiệu, tiêu đề trang (*TechNews Portal*), khẩu hiệu (slogan) và thanh tìm kiếm nhanh.
- **Vai trò:** Định vị nhận diện thương hiệu, giúp người dùng ngay lập tức hiểu được chủ đề và nội dung chính của trang web.

### 2. Navigation Menu (Thanh điều hướng)
- **Vị trí:** Ngay dưới Header hoặc tích hợp sticky trên đầu trang khi cuộn.
- **Nội dung:** Tối thiểu 4 mục liên kết chính:
  1. Trang chủ (Home)
  2. Công nghệ (Technology)
  3. Lập trình Web (Web Development)
  4. Hướng dẫn (Tutorials)
  5. Liên hệ (Contact)
- **Vai trò:** Hướng dẫn người dùng di chuyển thuận tiện giữa các trang hoặc các danh mục nội dung chính.

### 3. Content Section (Nội dung chính)
- **Vị trí:** Chiếm phần lớn diện tích trung tâm trang web.
- **Bố cục:**
  - **Bài viết tiêu điểm (Hero Article):** Ảnh đại diện lớn, tiêu đề bài viết, thông tin tác giả và đoạn trích dẫn tóm tắt.
  - **Lưới danh sách các bài viết (Card Grid):** Các thẻ tin tức hiển thị hình ảnh minh họa + tiêu đề + đoạn mô tả ngắn.
  - **Sidebar (Cột bên phải):** Chuyên mục nổi bật, bài viết xem nhiều hoặc thông tin tác giả.
- **Vai trò:** Truyền tải thông tin giá trị nhất tới người dùng, giữ chân độc giả.

### 4. Footer (Chân trang)
- **Vị trí:** Nằm ở cuối cùng của trang web.
- **Nội dung:** Thông tin bản quyền (`© 2026 TechNews. All rights reserved.`), liên kết điều khoản bảo mật, bản đồ trang web và mạng xã hội.
- **Vai trò:** Cung cấp thông tin pháp lý, kết nối doanh nghiệp và hỗ trợ người dùng khi đã cuộn xuống cuối trang.

---

## 2. Kế hoạch triển khai mã nguồn HTML & CSS
- Sử dụng thẻ ngữ nghĩa HTML5: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`.
- Sử dụng CSS Flexbox và CSS Grid để tạo bố cục gọn gàng, cân đối, tương thích tốt trên cả Desktop và Mobile.
