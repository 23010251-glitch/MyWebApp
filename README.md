# PhP Programming
## 1.1. Giới thiệu
Phần này sẽ cung cấp cái nhìn tổng quan về ngôn ngữ lập trình PHP. Bạn sẽ tìm hiểu về lịch sử của PHP, lý do nó được phát triển và vai trò quan trọng của nó trong việc tạo ra các trang web động. Khái niệm về một ngôn ngữ mã nguồn mở chạy trên máy chủ (server-side scripting language) sẽ được làm rõ, giải thích cách PHP xử lý yêu cầu của người dùng và tạo ra mã HTML trả về trình duyệt.
## 1.2.  Cú pháp PHP
Đây là phần nền tảng, nơi các quy tắc để viết code PHP. Các nội dung chính bao gồm:
* Thẻ PHP: Cách bắt đầu (<?php) và kết thúc (?>) một khối mã PHP.
* Biến: Cách khai báo và sử dụng biến ($) để lưu trữ dữ liệu.
* Kiểu dữ liệu: Tìm hiểu các kiểu dữ liệu cơ bản như số nguyên, số thực, chuỗi ký tự, và mảng.
* Toán tử: Cách sử dụng các toán tử số học, so sánh và logic để thực hiện các phép tính và so sánh.
* Cú pháp câu lệnh: Hiểu rằng mỗi câu lệnh trong PHP phải kết thúc bằng dấu chấm phẩy (;).
## 1.3. Cấu trúc điều khiển
Phần này tập trung vào logic và luồng của chương trình, giúp bạn đưa ra các quyết định trong code:
* Câu lệnh điều kiện: Sử dụng if, else if, và else để thực thi các khối mã khác nhau tùy thuộc vào điều kiện đúng hay sai.
* Vòng lặp: Sử dụng các vòng lặp như for, while, và foreach để thực hiện một tác vụ lặp đi lặp lại nhiều lần một cách hiệu quả.
## 1.4. Hàm
Các hàm là những khối mã có thể tái sử dụng, giúp code có tổ chức, gọn gàng và dễ bảo trì. Trong phần này bao gồm:
* Định nghĩa và gọi hàm: Cách tạo ra một hàm của riêng bạn và cách gọi nó để thực thi.
* Truyền tham số: Cách truyền dữ liệu vào hàm để nó xử lý.
* Trả về giá trị: Cách một hàm có thể trả về kết quả sau khi thực hiện xong nhiệm vụ.
## 1.5. Vai trò của PHP trong phát triển ứng dụng web
Đây là phần tổng hợp, giải thích tại sao các kiến thức trên lại quan trọng. PHP đóng vai trò là "bộ não" của trang web, xử lý các tác vụ như:
* Tạo nội dung động: Tạo ra các trang web có nội dung thay đổi tùy theo người dùng hoặc dữ liệu từ cơ sở dữ liệu.
* Xử lý biểu mẫu: Thu thập và xử lý dữ liệu từ các form đăng nhập, đăng ký, hoặc liên hệ.
* Tương tác với cơ sở dữ liệu: Kết nối và thao tác với các cơ sở dữ liệu như MySQL để lưu trữ và truy xuất thông tin.
* Quản lý phiên và người dùng: Giúp quản lý trạng thái đăng nhập của người dùng trên trang web.

# Module 2 – Building Web Applications with Laravel
## 1. Routing (Định tuyến)
- Quản lý URL và ánh xạ đến Controller hoặc Closure.
- Khai báo route trong `routes/web.php`.
- Các phương thức: GET, POST, PUT, DELETE.
- Route Parameters & Route Model Binding.
## 2. Controllers (Bộ điều khiển)
- Điều phối logic giữa Model và View.
- Tạo controller: `php artisan make:controller`.
- RESTful controllers: `index`, `show`, `create`, `store`, `edit`, `update`, `destroy`.
## 3. Views (Giao diện hiển thị)
- View đặt trong thư mục `resources/views`.
- Blade template engine (`{{ }}`, `@directive`).
- Layouts và Template inheritance: `@extends`, `@section`, `@yield`.
## 4. Migrations (Quản lý CSDL)
- Quản lý schema bằng migration.
- Tạo migration: `php artisan make:migration`.
- Các kiểu cột: `string`, `integer`, `boolean`, `timestamps`.
- Chạy & rollback: 
  - `php artisan migrate`
  - `php artisan migrate:rollback`
## 5. Eloquent ORM (Làm việc với dữ liệu)
- ActiveRecord cho PHP, ánh xạ Model ↔ Bảng.
- CRUD cơ bản:
  - `Model::all()`
  - `Model::find(id)`
  - `Model::create([...])`
  - `$model->update([...])`
  - `$model->delete()`
- Quan hệ: One-to-One, One-to-Many, Many-to-Many.
## 6. Middleware
- Lọc request trước khi vào Controller.
- Ứng dụng: xác thực đăng nhập, kiểm tra quyền hạn, logging.
- Tạo middleware: `php artisan make:middleware`.
- Đăng ký trong `app/Http/Kernel.php`.
## 7. Authentication (Xác thực)
- Cấu hình login, register với Laravel.
- Sử dụng `Auth` facade, middleware `auth`.
- Quản lý session, bảo vệ route yêu cầu login.
---
