# Clinic Booking Website - Đồ án chuyên ngành

Website đặt lịch khám bệnh trực tuyến cho phòng khám.

## 🚀 GitHub Codespaces là gì?

**GitHub Codespaces** là môi trường phát triển dựa trên cloud của GitHub, cho phép bạn:

- **Phát triển từ xa**: Viết code trực tiếp trên trình duyệt mà không cần cài đặt gì trên máy tính
- **Môi trường nhất quán**: Tự động cài đặt các extension và tool cần thiết
- **Truy cập mọi nơi**: Làm việc từ bất kỳ thiết bị nào có internet
- **Tiết kiệm thời gian**: Không cần setup môi trường phát triển

## 🛠️ Cách sử dụng GitHub Codespaces cho project này

### 1. Mở project trong Codespaces
- Truy cập repository trên GitHub
- Nhấn nút **"< > Code"** màu xanh lá
- Chọn tab **"Codespaces"**
- Nhấn **"Create codespace on main"**

### 2. Chờ môi trường khởi tạo
- Codespace sẽ tự động:
  - Cài đặt Node.js
  - Cài đặt các extension VS Code cần thiết
  - Chuẩn bị Live Server
  - Cài đặt dependencies

### 3. Chạy website
Sau khi Codespace khởi động xong:
```bash
cd Clinic_Booking_website
npm run start
```

Website sẽ chạy tại `http://localhost:3000` và tự động mở trong tab mới.

## 📁 Cấu trúc thư mục

```
Clinic_Booking_DACN/
├── .devcontainer/
│   └── devcontainer.json    # Cấu hình Codespaces
├── Clinic_Booking_website/
│   ├── index.html          # Trang chủ
│   ├── Doctors.html        # Trang bác sĩ
│   ├── Department.html     # Trang khoa
│   ├── services-detail.html # Chi tiết dịch vụ
│   ├── css/               # File CSS
│   ├── js/                # File JavaScript
│   ├── img/               # Hình ảnh
│   ├── fonts/             # Font chữ
│   └── package.json       # Cấu hình npm
├── README.md
└── Use Case.png
```

## 🔧 Tính năng Codespaces đã cấu hình

### Extensions tự động cài đặt:
- **Live Server**: Chạy server local với auto-reload
- **Prettier**: Format code tự động
- **Auto Rename Tag**: Đổi tên thẻ HTML tự động
- **CSS Peek**: Xem CSS từ HTML
- **HTML CSS Class Completion**: Gợi ý class CSS

### Cấu hình tự động:
- **Port forwarding**: Tự động forward port 3000
- **Format on save**: Tự động format code khi save
- **Live reload**: Tự động reload browser khi có thay đổi

## 💡 Lợi ích của việc sử dụng Codespaces

1. **Không cần cài đặt**: Không cần cài Node.js, VS Code hay extension nào
2. **Chuẩn hóa**: Tất cả member trong team có cùng môi trường
3. **Tiết kiệm tài nguyên**: Không tốn tài nguyên máy tính cá nhân
4. **Backup tự động**: Code được lưu trên cloud GitHub
5. **Colaboration**: Dễ dàng share môi trường với teammates

## 🚀 Lệnh thường dùng

```bash
# Chạy website với Live Server
npm run start

# Chạy với auto-watch (khuyến nghị cho development)
npm run dev

# Format code
npm run format
```

## 🔗 Liên kết hữu ích

- [GitHub Codespaces Documentation](https://docs.github.com/en/codespaces)
- [VS Code in the Browser](https://code.visualstudio.com/docs/editor/vscode-web)
- [Live Server Extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

---

**Lưu ý**: GitHub Codespaces có hạn mức miễn phí 60 giờ/tháng cho tài khoản cá nhân. Sau khi hết hạn mức, bạn có thể tiếp tục sử dụng với phí tính theo giờ.