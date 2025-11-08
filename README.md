# BTL-TKW


# 🌐 Quản Lý Nhân Sự (QuanLyNhanSu)

Website quản lý nhân sự sử dụng **PHP + MySQL**, có giao diện hiện đại, hỗ trợ **Dark Mode**, **thống kê trực quan**, và **upload ảnh hồ sơ** nhân viên.

---
## Các lỗi vẫn còn gặp

1. Lặp lại nhân viên khi load file "qlns.sql" nhiều lần (khắc phục bằng cách khởi động XAMPP theo hướng dẫn, vào "http://localhost/phpmyadmin", ở mục bên trái nhấn vào "qlns", chọn vào phần "departments" hoặc "employees", chọn các phần bị lặp và xoá 
2. Không hiển thị được địa chỉ gmail
3. Chức năng quản lý phòng ban và thống kê vẫn chưa hoàn thiện

## 🚀 Tính năng chính

1. Quản lý nhân viên (Thêm, sửa, xóa, tìm kiếm)
2. Quản lý phòng ban
3. Thống kê nhân sự theo phòng ban (Chart.js)
4. Upload và quản lý ảnh hồ sơ
5. Giao diện người dùng hiện đại (Dark Mode, Toast Notification)
6. Tìm kiếm và lọc dữ liệu nhân viên
7. Kết nối và xử lý dữ liệu MySQL
8. Responsive Layout (tương thích PC, laptop, tablet)

---

## 📁 Cấu trúc thư mục

```

QuanLyNhanSu/
│
├── index.html              # Trang chủ - Giới thiệu hệ thống
├── nhanvien.html           # Trang quản lý nhân viên
├── phongban.html           # Trang quản lý phòng ban
├── thongke.html           # Trang thống kê và báo cáo
├── Đọc kỹ trước khi sử dụng.txt       # Hướng dẫn cài đặt và sử dụng
│
├── api/
│   ├── emps.php            # API quản lý nhân viên
│   └── depts.php           # API quản lý phòng ban
│
├── inc/
│   ├── config.php          # Cấu hình kết nối MySQL
│   └── helpers.php         # Hàm tiện ích (JSON, upload, xóa file)
│
├── css/
│   └── style.css           # Giao diện CSS tùy chỉnh
│
├── config/
│   └── database.php        # Kết nối cơ sở dữ liệu
│
├── js/
│   └── main.js             # Logic xử lý frontend (fetch API, toast, dark mode)
│
├── images/
│   └── logo.svg            # Logo và icon hệ thống
│
├── uploads/
│   └── avatars/            # Lưu ảnh hồ sơ nhân viên
│
├── qlns.sql                # Cơ sở dữ liệu mẫu
├── README.md               # Tài liệu này

```

---
## Hướng dẫn cài đặt
Tải video hướng dẫn hoặc đọc hướng dẫn ở dưới

##  CHUẨN BỊ XAMPP
1. Tải XAMPP tại: https://www.apachefriends.org/download.html 
2. Cài đặt bình thường (ổ khác ngoài ổ C:).
3. Sau khi cài, mở XAMPP Control Panel (biểu tượng cam 🟧).
4. Bấm Start cho 2 dịch vụ:
   - Apache ✅
   - MySQL ✅
5. Khi cả hai dòng hiện 'Running' màu xanh lá → XAMPP đã sẵn sàng.
##  GIẢI NÉN DỰ ÁN
1. Giải nén file 'QuanLyNhanSu.zip' vào thư mục bạn chọn
2. Sau khi giải nén, bạn sẽ có thư mục:
   Ổ cứng cài\Thư mục cài\htdocs\QuanLyNhanSu\
3. Bên trong thư mục phải có:
   api\
   css\
   inc\
   js\
   images\
   uploads\
   qlns.sql
   index.html
##  TẠO CƠ SỞ DỮ LIỆU (MySQL)
1. Mở trình duyệt → gõ:
   http://localhost/phpmyadmin
2. Chọn tab 'Import' → 'Chọn tệp' → nạp file:
   Ổ cứng cài\Thư mục cài\htdocs\QuanLyNhanSu\qlns.sql
3. Nhấn 'Go' (Nhập ở phía dưới trang) để thực hiện.
4. Sau khi import, sẽ có database 'qlns' gồm 2 bảng:
   - departments
   - employees
  
##  KIỂM TRA KẾT NỐI CƠ SỞ DỮ LIỆU

1. Mở file: inc\config.php
2. Kiểm tra cấu hình:
   define('DB_HOST','localhost');
   define('DB_NAME','qlns');
   define('DB_USER','root');
   define('DB_PASS','');
3. Nếu bạn không đổi gì trong XAMPP → giữ nguyên.
   (Mặc định MySQL không có mật khẩu cho root)
   
##  CHẠY WEBSITE

1. Mở trình duyệt và gõ:
   http://localhost/QuanLyNhanSu/
2. Nếu bạn đổi cổng Apache (ví dụ 8080), gõ:
   http://localhost:8080/QuanLyNhanSu/

✅ Trang chủ sẽ hiện logo NS và nút 'Quản lý nhân viên'.
✅ Có nút 🌙 bật/tắt Dark Mode.
✅ Giao diện hiện đại, responsive.

## 💻 Công nghệ sử dụng

| Thành phần | Công nghệ |
|-------------|------------|
| Ngôn ngữ backend | PHP (v7+) |
| CSDL | MySQL |
| Frontend | HTML5, CSS3, JavaScript |
| Biểu đồ | Chart.js |
| Framework UI | Bootstrap 5 |
| Server | XAMPP (Apache + MySQL) |

##  Nhóm thực hiện

Báo cáo & Thống kê
1. Hà Thế Duy – Backend & CSDL
2. Phạm Minh Đức – Báo cáo & Thống kê
3. Vũ Phùng Quang Huy – Frontend 
4. Hoàng Văn Tùng - Giao diện
