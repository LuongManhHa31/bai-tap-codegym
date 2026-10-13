# [Thực hành] Tạo mixins & biến để tối ưu CSS của website mẫu

## 1. Mục tiêu
- Sử dụng biến (`$variables`) để kiểm soát toàn bộ giao diện tập trung.
- Tạo và tái sử dụng mixin (`@mixin`, `@include`) giúp giảm lặp code (DRY - Don't Repeat Yourself).
- Tách mã nguồn thành các module SCSS khoa học theo chuẩn thiết kế.

## 2. Cấu trúc thư mục dự án
```text
Thuc_hanh_tao_mixins_bien_toi_uu_css/
├── index.html                  # Giao diện HTML minh họa kết quả
├── styles_before.css           # File CSS ban đầu trước khi tối ưu
├── scss/
│   ├── abstracts/
│   │   ├── _variables.scss     # Định nghĩa các biến $primary-color, $font-large,...
│   │   └── _mixins.scss        # Định nghĩa @mixin button-style và @mixin box-style
│   ├── base/
│   │   └── _typography.scss    # Định kiểu h1, h2 theo biến font
│   ├── components/
│   │   ├── _buttons.scss       # Định kiểu nút bấm qua @include button-style
│   │   └── _cards.scss         # Định kiểu thẻ card qua @include box-style
│   └── main.scss               # File tổng hợp import tất cả các partials
└── css/
    ├── styles.css              # File CSS đầu ra được SASS biên dịch tự động
    └── styles.css.map
```

## 3. Lệnh biên dịch bằng SASS CLI
```bash
sass scss/main.scss css/styles.css
```
Chế độ tự động theo dõi (--watch):
```bash
sass scss/main.scss css/styles.css --watch
```
