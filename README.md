# BTL-TKW


# Quản Lý Nhân Sự (QuanLyNhanSu_Update_v2)

Website quản lý nhân sự với PHP và MySQL, có giao diện thân thiện, Dark Mode, thống kê, và upload ảnh hồ sơ nhân viên.

## 🔹 Tính năng chính

1. Quản lý nhân viên (thêm, sửa, xóa, tìm kiếm, hiển thị danh sách)
2. Quản lý phòng ban (thêm, sửa, xóa, liên kết nhân viên)
3. Thống kê nhân sự theo phòng ban (Chart.js)
4. Upload và quản lý ảnh hồ sơ, tự động xóa avatar cũ khi cập nhật
5. Giao diện người dùng hiện đại (Dark Mode, Toast Notification)
6. Tìm kiếm và lọc dữ liệu nhân viên
7. Kết nối và xử lý dữ liệu MySQL
8. Responsive Layout (tương thích máy tính, tablet)

## 📁 Cấu trúc thư mục

QuanLyNhanSu_Update_v2/ │ ├── index.html                 # Trang chủ ├── nhanvien.html              # Trang quản lý nhân viên ├── phongban.html              # Trang quản lý phòng ban ├── thongke.html               # Trang thống kê │ ├── api/                       # Backend PHP │   ├── emps.php               # API quản lý nhân viên │   └── depts.php              # API quản lý phòng ban │ ├── inc/                       # File cấu hình và helper │   ├── config.php             # Kết nối MySQL │   └── helpers.php            # Hàm tiện ích (JSON, upload ảnh, xóa ảnh) │ ├── uploads/avatars/           # Lưu ảnh hồ sơ nhân viên ├── css/style.css              # Giao diện ├── js/main.js                 # Logic frontend ├── images/                    # Logo, icon ├── qlns.sql                   # CSDL mẫu ├── README.md                  # Hướng dẫn này └── HuongDan_v2.txt            # Hướng dẫn triển khai v2

## ⚙️ Cài đặt trên XAMPP

1. Tải và cài **XAMPP**: [https://www.apachefriends.org/](https://www.apachefriends.org/)
2. Giải nén toàn bộ thư mục `QuanLyNhanSu_Update_v2` vào `C:\xampp\htdocs\`
3. Mở **phpMyAdmin**, tạo cơ sở dữ liệu `qlns` và import file `qlns.sql`
4. Mở trình duyệt: `http://localhost/QuanLyNhanSu_Update_v2/`
5. Sử dụng đầy đủ chức năng quản lý nhân viên, phòng ban và thống kê.

## 🔹 Công nghệ sử dụng

- PHP (v7+)
- MySQL
- HTML5 / CSS3 / JavaScript
- Chart.js (thống kê)
- AJAX / Fetch API
- Responsive design, Dark Mode

## 👨‍💻 Nhóm thực hiện

1. Hà Thế Duy – Backend & CSDL
2. Phạm Minh Đức – Frontend & Giao diện
3. Vũ Phùng Quang Huy – Báo cáo & Thống kê
