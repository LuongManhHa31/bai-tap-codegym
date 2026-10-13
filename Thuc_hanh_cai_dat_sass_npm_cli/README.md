# [Thực Hành] Hướng dẫn cài đặt SASS bằng npm & SASS CLI

## 1. Kết quả kiểm tra môi trường
- **Node.js:** `v24.21.0` (đã cài đặt)
- **npm:** `11.19.0` (đã cài đặt)
- **SASS CLI:** `1.105.1` (cài đặt thành công qua `npm install -g sass`)

## 2. Các lệnh thực hành SASS CLI

### Cài đặt SASS toàn cục qua npm:
```bash
npm install -g sass
```

### Kiểm tra phiên bản SASS:
```bash
sass --version
```

### Biên dịch một file SCSS sang CSS:
```bash
sass scss/styles.scss css/styles.css
```

### Biên dịch với chế độ tự động theo dõi thay đổi (`--watch`):
```bash
sass scss/styles.scss css/styles.css --watch
```

### Biên dịch nhiều file SCSS bằng thư mục đầu vào và đầu ra:
```bash
sass scss/:css/ --watch
```

## 3. Cấu trúc thư mục bài thực hành
```text
Thuc_hanh_cai_dat_sass_npm_cli/
├── index.html        # Trang web hiển thị kết quả
├── scss/
│   └── styles.scss   # File nguồn SCSS (biến, mixin, nesting)
├── css/
│   ├── styles.css    # File CSS được SASS biên dịch tự động
│   └── styles.css.map
└── README.md
```
