# Online CV - Ngô Quỳnh Trang (Sinh viên Kinh tế số)

Website Landing Page CV chuyên nghiệp, giao diện hiện đại, chuẩn Responsive cho máy tính, tablet và điện thoại.

---

## 📁 Cấu trúc thư mục

```text
CV/
├── index.html        # Trang giao diện chính (HTML5 chuẩn SEO)
├── style.css         # Hệ thống định dạng CSS, màu sắc, hiệu ứng, responsive
├── script.js         # Xử lý tương tác: cuộn mượt, sao chép thông tin (Toast)
├── render.yaml       # File cấu hình tự động deploy lên Render.com
├── .gitignore        # Các tệp bỏ qua khi đẩy lên Git
└── README.md         # Tài liệu hướng dẫn sử dụng & triển khai
```

---

## 💻 1. Quản lý và chỉnh sửa trên VS Code

1. Mở phần mềm **Visual Studio Code (VS Code)**.
2. Chọn **File** > **Open Folder...** > chọn thư mục `CV` này (`c:\Users\dell 7620\Desktop\CV`).
3. **Để xem trước trực tiếp (Live Preview):**
   - Cài tiện ích mở rộng **Live Server** trong VS Code (Extension ID: `ritwickdey.LiveServer`).
   - Nhấp chuột phải vào file `index.html` > chọn **Open with Live Server**.
   - Hoặc đơn giản là nhấp đúp trực tiếp vào file `index.html` để mở trong trình duyệt Chrome / Cốc Cốc / Edge.

---

## 🚀 2. Hướng dẫn đẩy lên GitHub từ VS Code

### Bước 2.1: Khởi tạo Git và Commit (đã chuẩn bị sẵn)
Mở Terminal trong VS Code (`Ctrl + ~`) hoặc PowerShell tại thư mục này và gõ:

```bash
git init
git add .
git commit -m "Khoi tao Online CV Ngo Quynh Trang"
```

### Bước 2.2: Tạo Repository trên GitHub và đẩy lên
1. Đăng nhập vào [GitHub](https://github.com).
2. Nhấn nút **New** (Tạo repository mới):
   - Đặt tên Repository, ví dụ: `cv-ngo-quynh-trang`
   - Chọn chế độ **Public**
   - **Không** tích chọn *Add a README file* (vì đã có sẵn file ở máy)
   - Bấm **Create repository**.
3. Copy 3 dòng lệnh mà GitHub cung cấp, gõ vào Terminal trong VS Code:
```bash
git branch -M main
git remote add origin https://github.com/<tai-khoan-cua-ban>/cv-ngo-quynh-trang.git
git push -u origin main
```

---

## 🌐 3. Hướng dẫn đẩy lên Render (Render.com)

Render hỗ trợ lưu trữ website tĩnh (Static Site) **hoàn toàn miễn phí**, tự động cấp chứng chỉ bảo mật HTTPS và tên miền `.onrender.com`.

### Cách triển khai cực nhanh:
1. Truy cập [render.com](https://render.com) và chọn **Sign in with GitHub**.
2. Tại màn hình Dashboard, nhấp vào nút **New +** ở góc trên bên phải > Chọn **Static Site**.
3. Kết nối với repository GitHub vừa tạo (`cv-ngo-quynh-trang`).
4. Điền các thông tin cấu hình cơ bản:
   - **Name**: `cv-ngo-quynh-trang` (hoặc tên bạn thích)
   - **Branch**: `main`
   - **Build Command**: *(Để trống)*
   - **Publish Directory**: `.` *(Dấu chấm, nghĩa là thư mục gốc chứa file `index.html`)*
5. Nhấp vào nút **Create Static Site**.
6. Render sẽ tự động triển khai chỉ sau khoảng 30 giây đến 1 phút. Bạn sẽ nhận được đường dẫn truy cập trực tiếp, ví dụ:
   `https://cv-ngo-quynh-trang.onrender.com`

---

## ✨ Điểm nổi bật của bản dựng
- **Tối ưu chuẩn hóa:** Không còn phụ thuộc vào các đoạn mã hay watermark quảng cáo của nền tảng bên thứ ba (Tempi).
- **Ảnh đại diện sắc nét:** Tải từ CDN Cloudinary với chất lượng cao.
- **Tương thích mọi thiết bị:** Tự động điều chỉnh kích thước cho màn hình từ iPhone, iPad đến Desktop.
- **Tính năng hữu ích:** Bấm sao chép số điện thoại, email với thông báo popup (Toast) mượt mà; nút gọi và gửi email trực tiếp.
