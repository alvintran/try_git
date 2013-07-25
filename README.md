Lớp Str
======

Lớp `Str` bao gồm các hàm static nên sử dụng chúng bạn không cần phải tạo thể hiện của lớp.

###Kiểm tra 1 chuỗi có chứa 1 chuỗi khác không###

**Method**
  
    Str::constain($haystack, $needle);

**Example**

    Str::constain("http://mytour.vn/3059-khach-san-time-door.html", "time-door"); // return true

###Kiểm tra 1 chuỗi có bắt đầu bằng chuỗi khác không###

**Method**

    Str::startsWith($haystack, $needle);

**Example**

    Str:: startsWith("http://mytour.vn/3059-khach-san-time-door.html", "time-door"); // return true

###Kiểm tra 1 chuỗi có kết thúc bằng chuỗi khác không###

**Method**

    Str::endsWith($haystack, $needle);

**Example**

    Str:: endsWith("http://mytour.vn/3059-khach-san-time-door.html", "http"); // return true
