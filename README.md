Lớp Str
======

Lớp `Str` bao gồm các hàm static, bạn không cần phải tạo thể hiện của lớp để sử dụng chúng.

####~ Kiểm tra 1 chuỗi có chứa 1 chuỗi khác không####

**Method**
  
    Str::contains($haystack, $needle);

**Example**

    Str::contains("http://mytour.vn/3059-khach-san-time-door.html", "time-door"); // return true
    Str::contains("http://mytour.vn/3059-khach-san-time-door.html", array("time-door", "khach-san")); // return true

####~ Kiểm tra 1 chuỗi có bắt đầu bằng chuỗi khác không####

**Method**

    Str::startsWith($haystack, $needle);

**Example**

    Str::startsWith("http://mytour.vn/3059-khach-san-time-door.html", "http"); // return true
    Str::startsWith("http://mytour.vn/3059-khach-san-time-door.html", "http, html"); // return true

####~ Kiểm tra 1 chuỗi có kết thúc bằng chuỗi khác không####

**Method**

    Str::endsWith($haystack, $needle);

**Example**

    Str::endsWith("http://mytour.vn/3059-khach-san-time-door.html", "html"); // return true
    Str::endsWith("http://mytour.vn/3059-khach-san-time-door.html", "http, html"); // return true

####~ Cắt chuỗi với 1 số ký tự nhất định, tự kiểm tra vị trí dấu cách để trả về kết quả tròn từ####

**Method**

    Str::cut_string($str, $limit, $end = '...');

**Example**

    Str::cut_string("Lorem ipsum dolor sit amet, consectetur adipisicing elit.", 5);


####~ Cắt chuỗi với 1 giới hạn nhất định, cắt đúng số giới hạn truyền vào####

**Method**

    Str::limits($str, $limit, $end = '...');

**Example**

    Str::limits("Lorem ipsum dolor sit amet, consectetur adipisicing elit.", 5);

####~ Cắt chuỗi với 1 giới hạn số từ nhất định####

**Method**

    Str::words($str, $limit, $end = '...');

**Example**

    Str::words("Lorem ipsum dolor sit amet, consectetur adipisicing elit.", 5);

####~ Generate 1 chuỗi ngẫu nhiên####

**Method**

    Str::random($length = 16);

**Example**

    Str::random();

####~ Upper case 1 chuỗi####

**Method**

    Str::upper($value);

**Example**

    Str::upper("Lorem ipsum dolor sit amet, consectetur adipisicing elit.");

####~ Lower case 1 chuỗi####

**Method**

    Str::lower($value);

**Example**

    Str::lower("Lorem Ipsum Dolor Sit Amet, Consectetur Adipisicing Elit.");

####~ Lấy độ dài 1 chuỗi####

**Method**

    Str::length($value);

**Example**

    Str::length("Lorem Ipsum Dolor Sit Amet, Consectetur Adipisicing Elit.");

####~ Bỏ dấu, replace các ký tự UTF8 về ký tự Latin####

**Method**

    Str::removeAccent($value);

**Example**

    Str::removeAccent("Có con chim vành khuyên nhỏ");


####~ Convert 1 chuỗi bất kỳ về dạng "chuoi-bat-ky"####

**Method**

    Str::slug($title, $separator = "-");

**Example**

    Str:: slug("Lorem Ipsum Dolor Sit Amet, Consectetur Adipisicing Elit.");
