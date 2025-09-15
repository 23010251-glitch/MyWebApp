# **PhP programming**
## Chương 1: Giới thiệu về PHP và Lavravel khóa Coursera (Khóa 1)
https://www.coursera.org/learn/laravel-framework-and-php/home/module/1
### 1.1 Giới thiệu PHP 
- PHP viết tắt của Hypertext Preprocessor.
- Là ngôn ngữ lập trình kịch bản (scripting language) phía máy chủ (server-side).
- Được dùng chủ yếu để tạo và phát triển các ứng dụng web động (dynamic websites).

### 1.2 Cú pháp PHP
Mã PHP được đặt trong cặp thẻ như sau:
```
<?php

```

Khai báo biến

+ Biến bắt đầu với ký hiệu $, ví dụ: $ten = "phenikaa";
+ Câu lệnh kết thúc bằng dấu ;

```
$ten = "Phenikaa";
```



Chú thích:

+ Một dòng: // đây là chú thích

+ Nhiều dòng: /* chú thích nhiều dòng */

  ```
  //đây là chú thích một dòng
  /*
   * đây là chú thích nhiều dòng
   */
  
  ```

### 1.3 Cấu trúc điều khiển
PHP hỗ trợ đầy đủ các cấu trúc điều khiển như các ngôn ngữ lập trình phổ biến khác:

#### if .. elseif ...else

Câu lệnh điều kiện: 

```
if ($tuoi >= 18)
  { echo "Đã đủ tuổi."; }
elseif ($tuoi == 17)
  { echo "Gần đủ tuổi."; }
else
  { echo "Chưa đủ tuổi."; }

```
#### Loop : For / while /do...while

Câu lệnh lặp: // for 
```
for ($i = 0; $i < 5; $i++)
    { echo $i; }

```

// while

```

while $i = 0;
while ($i < 5)
{
  echo $i;
  $i++;
}

```

// do...while
```


$i = 0;
do {
  echo $i;
  $i++;
}
while ($i < 5);

```

//Re nhanh switch..case


switch...case: 
```
$ngay = "thu hai";
switch ($ngay)
{ case "thu hai":
  echo "Hôm nay là đầu tuần.";
  break;

  case "thu ba":
  echo "Hôm nay là thứ 3.";
  break;

  default: echo "Không rõ ngày.";
}

```
### 1.4 Hàm trong PHP

+ Giống Methods trong Class
+ Hàm là khối mã thực hiện một nhiệm vụ cụ thể, tái sử dụng.

Ví dụ: 
```
function chao($ten)
{
   return "Xin chào, " . $ten;

}

```

echo chao("Minh");

Đặc điểm:

+ Có thể có hoặc không tham số.

+ Có thể trả về giá trị bằng return.

PHP cũng hỗ trợ hàm ẩn danh (anonymous functions) và các hàm callback.

### 1.5 Vai trò của PHP trong phát triển ứng dụng Web
PHP giữ vai trò cốt lõi trong lập trình web phía server, cụ thể:

Xử lý dữ liệu từ biểu mẫu (form) người dùng.

Kết nối và thao tác với cơ sở dữ liệu.

Control/Điều khiển nôi dung động (dynamic content) từ CSDL về View hoặc từ View về Model (CSDL).

Xử lý các nghiệp vụ phát triển phần mềm: 
Ví dụ: 

+ Xử lý xác thực, định dạnh và phần quyền người dùng (login, register).
+ CRUD
+ Phân tích xử lý nghiệp vụ doanh nghiệp (business logic)

Tích hợp dễ dàng với các framework Frontend, HTML, CSS, JavaScript.

Tạo API hoặc làm việc với JSON, XML.

PHP thường được sử dụng để xây dựng các hệ thống như:

Website thương mại điện tử

Hệ quản trị nội dung (CMS) như WordPress, Joomla

Diễn đàn (forums), mạng xã hội

Web service, RESTful API
