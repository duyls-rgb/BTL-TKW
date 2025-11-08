# BTL-TKW


# Quản Lý Nhân Sự (QuanLyNhanSu)

Website quản lý nhân sự với PHP và MySQL, có giao diện thân thiện, Dark Mode, thống kê, và upload ảnh hồ sơ nhân viên.

##  Tính năng chính

1. Quản lý nhân viên (thêm, sửa, xóa, tìm kiếm, hiển thị danh sách)
2. Quản lý phòng ban (thêm, sửa, xóa, liên kết nhân viên)
3. Thống kê nhân sự theo phòng ban (Chart.js)
4. Upload và quản lý ảnh hồ sơ, tự động xóa avatar cũ khi cập nhật
5. Giao diện người dùng hiện đại (Dark Mode, Toast Notification)
6. Tìm kiếm và lọc dữ liệu nhân viên
7. Kết nối và xử lý dữ liệu MySQL
8. Responsive Layout (tương thích máy tính, tablet)

##  Cấu trúc thư mục

│
├── index.html              # Trang chủ - Giới thiệu hệ thống
├── nhanvien.html           # Trang quản lý nhân viên
├── phongban.html           # Trang quản lý phòng ban
├── thongke.html            # Trang thống kê và báo cáo
│── Đọc kỹ trước khi sử dụng.txt   # Hướng dẫn cài đặt và sử dụng
├── css/
│   └── style.css           # File CSS tùy chỉnh
│
├── js/
│   └── main.js             # File JavaScript chính xử lý logic
│
├── images/
│   └── logo.svg            # Logo của hệ thống
│
└── libs/                   # (Tùy chọn - nếu cần thư viện local)
    ├── bootstrap/
    └── chartjs/

##  Cài đặt trên XAMPP

1. Tải và cài **XAMPP**: [https://www.apachefriends.org/](không nên cài vào ổ C:)
2. Giải nén toàn bộ thư mục `QuanLyNhanSu` vào `Vị trí cài\xampp\htdocs\`
3. Mở **phpMyAdmin**, tạo cơ sở dữ liệu `qlns` và import file `qlns.sql`
4. Mở trình duyệt: `http://localhost/QuanLyNhanSu/`
5. Sử dụng đầy đủ chức năng quản lý nhân viên, phòng ban và thống kê.

##  Công nghệ sử dụng

- PHP (v7+)
- MySQL
- HTML5 / CSS3 / JavaScript
- Chart.js (thống kê)
- AJAX / Fetch API
- Responsive design, Dark Mode

##  Nhóm thực hiện

1. Hà Thế Duy – Backend & CSDL
2. Phạm Minh Đức – Frontend & Giao diện
3. Vũ Phùng Quang Huy – Báo cáo & Thống kê
