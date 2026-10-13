# [Bài tập] Tái cấu trúc mã CSS của các bài tập đã làm (Landing Page với SASS)

## 1. Mục tiêu bài tập
Tái cấu trúc 4 phần đã học trong chủ đề Landing Page sang SASS chuẩn mực:
1. **Navigation & Header:** Thanh điều hướng cố định và Hero Banner.
2. **Sản phẩm nổi bật:** Lưới Card sản phẩm thích ứng Responsive.
3. **Số liệu thống kê:** Khối chỉ số thành tựu với dải màu gradient.
4. **Footer:** Chân trang 4 cột chuyên nghiệp.

## 2. Các kỹ thuật SASS đã áp dụng
- **Variables:** Bảng màu thống nhất, kích thước container, khoảng cách và breakpoints.
- **Nesting:** Cấu trúc phân cấp cha - con rõ ràng, loại bỏ hoàn toàn lặp bộ chọn CSS.
- **Mixins:** `@mixin flex-center`, `@mixin flex-between`, `@mixin button-base`, `@mixin mobile`.
- **Partials / 7-1 Architecture:** Phân chia thành các module `abstracts/`, `base/`, `layout/`, `components/`.

## 3. Cấu trúc thư mục dự án
```text
Bai_tap_tai_cau_truc_css_landing_page_sass/
├── index.html                  # Giao diện Landing Page hoàn chỉnh
├── scss/
│   ├── abstracts/
│   │   ├── _variables.scss     # Định nghĩa biến màu sắc, bóng đổ, breakpoint
│   │   └── _mixins.scss        # Định nghĩa các mixin flexbox, button, responsive
│   ├── base/
│   │   └── _reset.scss         # Reset CSS cơ bản
│   ├── layout/
│   │   ├── _navigation.scss    # Dựng navigation và header
│   │   └── _footer.scss        # Dựng phần footer
│   ├── components/
│   │   ├── _buttons.scss       # Định kiểu các nút bấm
│   │   ├── _products.scss      # Dựng phần sản phẩm nổi bật
│   │   └── _statistics.scss    # Dựng phần số liệu thống kê
│   └── main.scss               # File tổng hợp import toàn bộ partials
└── css/
    ├── styles.css              # File CSS được SASS biên dịch tự động
    └── styles.css.map
```

## 4. Lệnh biên dịch bằng SASS CLI
```bash
sass scss/main.scss css/styles.css
```
Chế độ theo dõi tự động:
```bash
sass scss/main.scss css/styles.css --watch
```
