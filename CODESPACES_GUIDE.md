# Hướng dẫn sử dụng GitHub Codespaces cho Clinic Booking Website

## 📋 Mục lục
1. [GitHub Codespaces là gì?](#github-codespaces-là-gì)
2. [Lợi ích của Codespaces](#lợi-ích-của-codespaces)
3. [Cách khởi tạo Codespace](#cách-khởi-tạo-codespace)
4. [Hướng dẫn sử dụng](#hướng-dẫn-sử-dụng)
5. [Các tính năng đã cấu hình](#các-tính-năng-đã-cấu-hình)
6. [Troubleshooting](#troubleshooting)

## 🤖 GitHub Codespaces là gì?

**GitHub Codespaces** là môi trường phát triển tích hợp (IDE) chạy trên cloud, được tích hợp trực tiếp vào GitHub. Nó cho phép developers:

- **Viết code trực tiếp trên trình duyệt** mà không cần cài đặt bất kỳ phần mềm nào
- **Có môi trường phát triển nhất quán** cho tất cả thành viên team
- **Truy cập project từ bất kỳ đâu** chỉ cần có internet
- **Tiết kiệm thời gian setup** môi trường phát triển

## 🎯 Lợi ích của Codespaces

### Cho sinh viên/học sinh:
- ✅ Không cần laptop/PC mạnh - chỉ cần trình duyệt
- ✅ Không cần cài đặt Node.js, VS Code hay bất kỳ tool nào
- ✅ Làm việc nhóm dễ dàng với môi trường giống hệt nhau
- ✅ Backup tự động trên cloud GitHub

### Cho project:
- ✅ Chuẩn hóa môi trường phát triển
- ✅ Onboarding nhanh chóng cho thành viên mới
- ✅ Tránh lỗi "works on my machine"
- ✅ Tích hợp sẵn các tool cần thiết

## 🚀 Cách khởi tạo Codespace

### Bước 1: Truy cập GitHub Repository
1. Mở trình duyệt và đăng nhập GitHub
2. Truy cập: `https://github.com/phanhuuthang1612/Clinic_Booking_DACN`

### Bước 2: Tạo Codespace
1. Nhấn nút **"< > Code"** màu xanh lá
2. Chọn tab **"Codespaces"**
3. Nhấn **"Create codespace on main"** (hoặc branch bạn muốn)

### Bước 3: Chờ khởi tạo
- Codespace sẽ tự động:
  - Cài đặt Node.js 18
  - Cài đặt các VS Code extensions
  - Chạy lệnh `npm install`
  - Chuẩn bị Live Server

⏱️ **Thời gian khởi tạo**: 2-3 phút lần đầu, sau đó chỉ 30-60 giây

## 🛠️ Hướng dẫn sử dụng

### Chạy website lần đầu:
```bash
cd Clinic_Booking_website
npm run start
```

### Chạy trong chế độ development:
```bash
npm run dev
```

### Format code:
```bash
npm run format
```

### Cấu trúc thư mục:
```
Clinic_Booking_website/
├── index.html          # Trang chủ
├── Doctors.html        # Danh sách bác sĩ
├── Department.html     # Các khoa
├── services-detail.html # Chi tiết dịch vụ
├── css/               # Stylesheets
├── js/                # JavaScript files
├── img/               # Images
└── fonts/             # Font files
```

## ⚙️ Các tính năng đã cấu hình

### Extensions tự động cài đặt:
- **Live Server**: Chạy server local với auto-reload
- **Prettier**: Format code tự động
- **Auto Rename Tag**: Rename thẻ HTML tự động
- **Auto Close Tag**: Đóng thẻ HTML tự động
- **CSS Peek**: Xem CSS definition từ HTML
- **HTML CSS Class Completion**: Autocomplete CSS classes

### Cấu hình VS Code:
- **Format on save**: Tự động format khi save (Ctrl+S)
- **Live Server port**: 3000 (tự động forward)
- **Auto-reload**: Tự động reload browser khi có thay đổi
- **Prettier**: Format HTML, CSS, JavaScript

### Port forwarding:
- **Port 3000**: Live Server (public)
- **Port 5000**: Backup port
- **Port 8080**: Alternative port

## 🔧 Troubleshooting

### Live Server không chạy:
```bash
cd Clinic_Booking_website
npm install
npm run start
```

### Port bị conflict:
```bash
# Thử port khác
npx live-server --port=5000 --host=0.0.0.0 --no-browser
```

### Extensions không load:
- Reload window: `Ctrl+Shift+P` → "Developer: Reload Window"
- Hoặc restart Codespace

### Không thể access website:
1. Kiểm tra port forwarding trong tab "Ports"
2. Đảm bảo port 3000 đang chạy
3. Nhấn "Open in Browser" từ tab Ports

## 📝 Tips & Tricks

### 1. Sử dụng Command Palette:
- `Ctrl+Shift+P` (Windows/Linux) hoặc `Cmd+Shift+P` (Mac)
- Tìm kiếm các lệnh nhanh

### 2. Live Server shortcuts:
- Click chuột phải vào `index.html` → "Open with Live Server"
- Hoặc dùng shortcut `Alt+L Alt+O`

### 3. Format code nhanh:
- `Shift+Alt+F` (Windows/Linux) hoặc `Shift+Option+F` (Mac)

### 4. Toggle Terminal:
- `Ctrl+`` (backtick) để mở/đóng terminal

### 5. File Explorer:
- `Ctrl+Shift+E` để focus vào file explorer

## 💰 Billing & Limits

### Miễn phí:
- **60 giờ/tháng** cho tài khoản cá nhân
- **Unlimited** cho public repositories (với một số hạn chế)

### Tính phí:
- Sau 60 giờ: ~$0.18/giờ (tùy theo machine type)
- Có thể set spending limit để tránh bị charge

### Tiết kiệm usage:
- Đóng Codespace khi không dùng (auto-suspend sau 30 phút)
- Sử dụng "Stop codespace" thay vì "Delete"

## 📚 Tài liệu tham khảo

- [GitHub Codespaces Docs](https://docs.github.com/en/codespaces)
- [VS Code in Browser](https://code.visualstudio.com/docs/editor/vscode-web)
- [Devcontainer Configuration](https://containers.dev/)

---

**💡 Lưu ý**: Codespace sẽ tự động suspend sau 30 phút không hoạt động để tiết kiệm credits. Bạn có thể resume bất kỳ lúc nào!