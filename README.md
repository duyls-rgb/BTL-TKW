# BTL-TKW


# 🌐 Quản Lý Nhân Sự (QuanLyNhanSu)

Website quản lý nhân sự sử dụng **PHP + MySQL**, có giao diện hiện đại, hỗ trợ **Dark Mode**, **thống kê trực quan**, và **upload ảnh hồ sơ** nhân viên.

---
## Các lỗi vẫn còn gặp

1.Lặp lại nhân viên khi load file "qlns.sql" nhiều lần (khắc phục bằng cách khởi động XAMPP theo hướng dẫn, vào "http://localhost/phpmyadmin", ở mục bên trái nhấn vào "qlns", chọn vào phần "departments" hoặc "employees", chọn các phần bị lặp và xoá 
2.Không hiển thị được địa chỉ gmail
3.Chức năng quản lý phòng ban và thống kê vẫn chưa hoàn thiện
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

## ⚙️ Cài đặt trên XAMPP

1. Tải và cài [XAMPP](https://www.apachefriends.org/)  
   *(Tránh cài vào ổ C, tạo thư mục để cài)*  
2. Giải nén thư mục **QuanLyNhanSu** vào: 
```

Ổ cứng cài\Thư mục cài\htdocs\

```
3. Mở **phpMyAdmin** → tạo cơ sở dữ liệu `qlns` → Import file `qlns.sql`  
4. Chạy website tại trình duyệt:  
```

[http://localhost/QuanLyNhanSu/](http://localhost/QuanLyNhanSu/)

```
5. Sử dụng các chức năng: quản lý nhân viên, phòng ban, thống kê, upload ảnh.

---

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

1. Hà Thế Duy – Backend & CSDL
2. Phạm Minh Đức – Frontend & Giao diện
3. Vũ Phùng Quang Huy – Báo cáo & Thống kê
