# [Thực hành] Chuyển đổi CSS có sẵn sang SASS theo chuẩn

## 1. Cấu trúc thư mục chuẩn SASS
```text
Thuc_hanh_chuyen_doi_css_sang_sass_chuan/
├── index.html                  # Giao diện HTML minh họa
├── styles_original.css         # File CSS ban đầu (trước khi chuyển đổi)
├── scss/
│   ├── abstracts/
│   │   ├── _variables.scss     # Khai báo các biến màu sắc, bóng đổ, border
│   │   └── _mixins.scss        # Khai báo mixin tái sử dụng button-style, box-shadow
│   ├── base/
│   │   └── _global.scss        # Reset và CSS cơ bản toàn trang
│   ├── layout/
│   │   └── _container.scss     # Định kiểu khung chứa .container
│   ├── components/
│   │   ├── _buttons.scss       # Định kiểu nút bấm .button
│   │   └── _cards.scss         # Định kiểu thẻ .card
│   └── main.scss               # File tổng hợp import tất cả các partials
└── css/
    ├── main.css                # File CSS đã được biên dịch tự động
    └── main.css.map
```

## 2. Lệnh biên dịch bằng SASS CLI:
```bash
sass scss/main.scss css/main.css
```
Chế độ tự động cập nhật khi sửa đổi:
```bash
sass scss/main.scss css/main.css --watch
```
