# Portfolio CV - Nguyễn Văn An

## Tên dự án

**Portfolio CV cá nhân của Nguyễn Văn An** — trang web giới thiệu hồ sơ và các dự án Frontend.

## Mô tả

Dự án là một website tĩnh dạng portfolio/CV, trình bày thông tin giới thiệu, kỹ năng, dự án tiêu biểu và thông tin liên hệ. Giao diện được thiết kế responsive theo hướng mobile-first, sử dụng HTML ngữ nghĩa và CSS thuần.

## Chức năng

- Điều hướng đến các mục Giới thiệu, Kỹ năng, Dự án và Liên hệ.
- Hiển thị ảnh đại diện, phần giới thiệu và lời kêu gọi xem dự án/liên hệ.
- Trình bày kỹ năng và các thẻ dự án mẫu.
- Cung cấp liên kết email và hồ sơ mạng xã hội.
- Tương thích với các kích thước màn hình điện thoại, máy tính bảng và máy tính.

> Các dự án và thông tin liên hệ trong trang hiện là nội dung mẫu. Hãy cập nhật trước khi sử dụng như hồ sơ cá nhân chính thức.

## Công nghệ

- **HTML5:** cấu trúc nội dung và các thành phần ngữ nghĩa.
- **CSS3:** tạo kiểu, Flexbox, CSS Grid, biến CSS và media queries responsive.
- **Không cần framework, thư viện JavaScript, trình quản lý gói hoặc bước biên dịch.** JavaScript được nhắc trong danh sách kỹ năng trên trang, nhưng website hiện tại không tải hay chạy mã JavaScript.

## Yêu cầu môi trường

- Trình duyệt hiện đại như Chrome, Edge, Firefox hoặc Safari.
- Không cần cài đặt thư viện hay phụ thuộc để mở trang.
- Để chạy máy chủ phát triển cục bộ, có thể dùng Python 3.
- Để chạy bằng container, cần Docker Desktop (Windows/macOS) hoặc Docker Engine (Linux).

## Cấu trúc dự án

```text
.
├── README.md
├── index.html
├── assets/
│   ├── css/
│   │   └── styles.css
│   └── img/
│       ├── avatar.jpg
│       └── dsdsdsdsdsdsdsd.jpg
└── BAOCAO-A2.1.docx
```

Các lệnh bên dưới cần được chạy từ thư mục gốc chứa README này.

## Cài đặt

Không có bước cài đặt phụ thuộc. Tải hoặc sao chép dự án về máy, sau đó mở thư mục gốc của dự án.

## Cấu hình và tùy chỉnh

1. Mở `index.html` để thay tên, chức danh, phần giới thiệu, danh sách kỹ năng, dự án, email và liên kết mạng xã hội.
2. Thay ảnh đại diện trong `assets/img/` và cập nhật đường dẫn ảnh tương ứng trong `index.html`. Ảnh đang hiển thị sử dụng tệp `dsdsdsdsdsdsdsd.jpg`.
3. Chỉnh màu sắc, kiểu chữ, khoảng cách và bố cục trong `assets/css/styles.css`. Các biến màu và thiết kế được khai báo ở phần `:root` đầu tệp.
4. Các thẻ dự án và liên kết `#` hiện chỉ là nội dung minh họa; thay bằng thông tin và URL thực tế.

Không có tệp cấu hình môi trường hoặc khóa API cần khai báo.

## Chạy thử

### Cách nhanh: mở trực tiếp

Mở tệp `CV--main/index.html` bằng trình duyệt. Cách này phù hợp để xem giao diện cơ bản; dùng máy chủ cục bộ nếu muốn kiểm thử trong môi trường HTTP.

### Windows

Mở PowerShell tại thư mục gốc dự án và chạy:

```powershell
py -m http.server 8000
```

Nếu lệnh `py` không có trên máy, thử:

```powershell
python -m http.server 8000
```

### macOS

Mở Terminal tại thư mục gốc dự án và chạy:

```bash
python3 -m http.server 8000
```

### Linux

Mở Terminal tại thư mục gốc dự án và chạy:

```bash
python3 -m http.server 8000
```

Sau khi máy chủ khởi động, mở [http://localhost:8000](http://localhost:8000) trên trình duyệt. Dừng máy chủ bằng `Ctrl+C`.

### Docker

Cài và khởi động Docker trước. Chạy các lệnh tại thư mục gốc dự án để phục vụ trang bằng Nginx; không cần tạo image riêng.

**Windows (PowerShell):**

```powershell
docker run --rm --name portfolio-cv -p 8080:80 -v "${PWD}:/usr/share/nginx/html:ro" nginx:alpine
```

**macOS / Linux:**

```bash
docker run --rm --name portfolio-cv -p 8080:80 -v "$PWD:/usr/share/nginx/html:ro" nginx:alpine
```

Truy cập [http://localhost:8080](http://localhost:8080). Nhấn `Ctrl+C` tại cửa sổ đang chạy Docker để dừng và xóa container.

## Kiểm tra khi chạy

- Trang tải được và hiển thị đủ phần giới thiệu, kỹ năng, dự án, liên hệ.
- Ảnh đại diện xuất hiện; nếu ảnh không hiển thị, kiểm tra đường dẫn và tên tệp trong `index.html`.
- Thử thay đổi chiều rộng cửa sổ hoặc mở trên điện thoại để kiểm tra bố cục responsive.
- Kiểm tra các liên kết email và hồ sơ sau khi thay nội dung mẫu.

## Thông tin liên hệ

Thông tin liên hệ trên website hiện là dữ liệu mẫu:

- **Email:** `an.nguyen@example.com`
- **GitHub:** `github.com/nguyenvanan`
- **LinkedIn:** `linkedin.com/in/nguyenvanan`

Hãy thay các thông tin trên bằng thông tin chính thức của chủ dự án. README này không cung cấp một kênh liên hệ riêng khác.