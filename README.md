Cấu trúc Thư mục và Tệp

-Controller: C:\xampp\htdocs\Baitapgiuaki-Khuong-21010594\app\Controllers\HelloWorld.php

-View: C:\xampp\htdocs\Baitapgiuaki-Khuong-21010594\app\Views\helloworld.php

-Routes: C:\xampp\htdocs\Baitapgiuaki-Khuong-21010594\app\Config\Routes.php


-Cấu hình lại file .htaccess trong folder public

<IfModule mod_rewrite.c>
    
    RewriteEngine On
    
    RewriteBase /Baitapgiuaki-Khuong-21010594/public/
    
    RewriteCond %{REQUEST_FILENAME} !-f
    
    RewriteCond %{REQUEST_FILENAME} !-d
    
    RewriteRule ^(.*)$ index.php/$1 [L]

</IfModule>

RewriteBase /Baitapgiuaki-Khuong-21010594/public/: Thiết lập đường dẫn cơ sở cho các quy tắc rewrite để chạy trên trình duyệt với URL: http://localhost/Baitapgiuaki-Khuong-21010594/public/helloworld



