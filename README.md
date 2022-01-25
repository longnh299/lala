#Các bước cài đặt dự án :

Clone Project :git clone https://gitlab.com/soict-it4409/20211/nhom14/lala.git

1.Load dependency từ composer.json : composer install
2.Tạo file .env ,copy file .env.example sang .Cấu hình file .env phù hợp với DB
3.Tạo key cho project : php artisan key:generate
4.Cache lại file .env : php artisan config:cache
5.Tạo DB : php artisan migrate
6.Tạo seed cho DB :php artisan db:seed (email :user001@gmail , password:lala để đăng nhập)
7.Cài đặt npm : npm install
8.Để thêm chạy được css :Thêm file vào trong thư mục public/css
9.Muốn sửa css/js : chạy lại npm run dev

#Các file của dự án :
###BE :làm việc ở thư mục app , database , resource/lang, route

*app/Http/Controllers : Viết các Controller chỉ để điều hướng ,k viết các hàm xử lí logic trong Controller.
*app/Http/Requests : Viết các Request
*app/Models : Viết các model
*app/Service : Viết các hàm xử lí logic
*app/Traits : Chứa các hàm được sử dụng lại nhiều lần
*database: Có các thư mục tạo database , fake dữ liệu
*resource/lang :Các file chứa các message
*route: Viết các route cho trang web

###FE :làm việc ở thư mục resource

*resource/js : Các file JS
*resource/css :Các file CSS
*resource/views/layout: layout Html cho trang web
*resource/views/pages: Các page Html của trang web
*public/images: Chứa các file .svg hoặc .png (Lưu ý sử dụng "{{asset("a/b/c")}}") ~ cd ->file "public/a/b/c"
