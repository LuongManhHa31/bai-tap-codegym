# [Bài tập] Tái cấu trúc mã CSS cho sẵn (Responsive Grid sang SASS)

## 1. Mục tiêu tái cấu trúc
- Thay thế toàn bộ mã CSS Inline lộn xộn trong file gốc `responsive_grid.htm` bằng hệ thống class SCSS ngữ nghĩa rõ ràng.
- Ứng dụng biến (`$grid-columns`, `$header-bg`, `$footer-bg`, `$item-bg`,...).
- Ứng dụng Mixin (`@mixin col-span($cols)`, `@mixin clearfix`, `@mixin row-wrapper`).
- Tổ chức theo mô hình thư mục module SCSS tiêu chuẩn.

## 2. Cấu trúc thư mục dự án
```text
Bai_tap_tai_cau_truc_css_responsive_grid/
├── index.html                      # File HTML đã tái cấu trúc sạch sẽ, chuẩn BEM
├── original_responsive_grid.html   # File gốc có sẵn từ CodeGym (dùng đối chiếu)
├── scss/
│   ├── abstracts/
│   │   ├── _variables.scss         # Biến số cột, bảng màu, chiều cao
│   │   └── _mixins.scss            # Mixin tính độ rộng cột và clearfix
│   ├── layout/
│   │   └── _grid.scss              # Định kiểu khung hàng và hệ thống 12 cột
│   ├── components/
│   │   └── _widgets.scss           # Định kiểu các menu item và khối nội dung
│   └── main.scss                   # File tổng hợp import các partials
└── css/
    ├── styles.css                  # File CSS đầu ra được SASS biên dịch tự động
    └── styles.css.map
```

## 3. Lệnh biên dịch bằng SASS CLI
```bash
sass scss/main.scss css/styles.css
```
Chế độ theo dõi tự động:
```bash
sass scss/main.scss css/styles.css --watch
```
