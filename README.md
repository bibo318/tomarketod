# Tomarketod

Tự động yêu cầu cho Telegram Bot tiếp thị

# Mục lục

-[Tomarketod](#tomarketod)
-[Mục lục](#table-of-contents)
-[Cảnh báo](#cảnh báo)
-[Tính năng](#tính năng)
-[Đăng ký](#đăng ký)
-[Cách sử dụng](#cách sử dụng)
  -[Giới thiệu về Cấu hình](#about-config)
  -[Giới thiệu về Proxy](#about-proxy)
  -[Windows](#windows)
  -[Linux](#linux)
  -[Termux](#termux)
-[Cách lấy dữ liệu](#how-to-get-data)
-[Chạy 24/7](#chạy cho 247)
-[Thảo luận](#thảo luận)
-[Hỗ trợ công việc của tôi](#support-my-work)
-[Cảm ơn \< 3](#cảm ơn--3)

# Cảnh báo

Mọi rủi ro đều do người dùng chịu!

# Tính năng

-[x] Yêu cầu tự động
-[x] Hỗ trợ nhiều tài khoản
-[x] Trò chơi tự động chơi
-[x] Hỗ trợ proxy

# Đăng ký

Nhấp vào url sau để đăng ký: https://t.me/Tomarket_ai_bot/app?startapp=0000hnXd

# Cách sử dụng

## Về cấu hình

| Tên            | Mô tả                                                                                                                                       |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| interval        | thời gian ngừng hoạt động giữa các tài khoản                                                                                         |
| play_game       | giá trị phải bool (true/false) được đặt đúng để bật trò chơi tự động chơi sau khi xác nhận                               |
| game_point      | thấp : kiếm tiền tối thiểu khi chơi trò chơi `<br>`cao : kiếm tiền tối đa khi chơi trò chơi                                  |
| additional_time | min : thời gian bổ sung tối thiểu cho lần yêu cầu tiếp theo `<br>` max : thời gian bổ sung tối đa cho lần yêu cầu tiếp theo |

## Về proxy

Đăng ký trên trang web này để nhận proxy miễn phí: [Tại đây](https://www.webshare.io/)

Bạn có thể thêm danh sách proxy của mình ở dạng `proxies.txt` và định dạng proxy giống như ví dụ bên dưới:

Định dạng :

```
http://máy chủ:cổng
http://user:pass@host:port
```

Ví dụ :

```
http://127.0.0.1:6969
http://user:pass@127.0.0.1:6969
vớ5://127.0.0.1:6969
vớ5://user:pass@127.0.0.1:6969
```

## Windows

1. Đảm bảo máy tính của bạn đã được cài đặt python và git.

   trang web python : [https://python.org](https://python.org)

   trang web git : [https://git-scm.com/](https://git-scm.com/)
2. Sao chép kho lưu trữ này

   ```vỏ
    git clone https://github.com/bibo318/tomarketod.git
   ```
3. thư mục goto tomarketod

   ```
   cd tomarketod
   ```
4. cài đặt thư viện yêu cầu

   ```

   ```

python -m install  pip -r require.txt

```

5. Chỉnh sửa `data.txt`, nhập mã thông báo dữ liệu của bạn vào `data.txt`, tìm mã thông báo của bạn trong [Cách lấy dữ liệu](#how-to-get-data). Một dòng cho một tài khoản dữ liệu, nếu bạn muốn thêm tài khoản thứ hai, hãy thêm vào dòng mới!

6. thực hiện chương trình chính 
```

   python bot.py

```

##Linux

1. Đảm bảo máy tính của bạn đã được cài đặt python và git.
   
   trăn
   ``` vỏ
   sudo apt install python3 python3-pip
```

   git

```vỏ
sudo apt install git
```

2. Sao chép kho lưu trữ này

   ```vỏ
   git clone  https://github.com/bibo318/tomarketod.git
   ```
3. thư mục goto tomarketod

   ```vỏ
   cd tomarketod
   ```
4. Cài đặt thư viện yêu cầu

   ```
   python3 -m install pip -r require.txt
   ```
5. Chỉnh sửa `data.txt`, nhập mã thông báo dữ liệu của bạn vào `data.txt`, tìm mã thông báo của bạn trong [Cách lấy dữ liệu](#how-to-get-data). Một dòng cho một tài khoản dữ liệu, nếu bạn muốn thêm tài khoản thứ hai, hãy thêm vào dòng mới!
6. thực hiện chương trình chính

   ```
   python bot.py
   ```

## Termux

1. Hãy chắc chắn rằng termux của bạn đã được cài đặt python và git.

   trăn

   ```
   pkg install python
   ```

   git

   ```
   pkg install git
   ```
2. Sao chép kho lưu trữ này

   ```vỏ

   ```

git clone  https://github.com/bibo318/tomarketod.git

```

3. thư mục goto tomarketod
```

   cd tomarketod

```

4. cài đặt thư viện yêu cầu
```

   python -m install  pip -r require.txt

```

5. Chỉnh sửa `data.txt`, nhập mã thông báo dữ liệu của bạn vào `data.txt`, tìm mã thông báo của bạn trong [Cách lấy dữ liệu](#how-to-get-data). Một dòng cho một tài khoản dữ liệu, nếu bạn muốn thêm tài khoản thứ hai, hãy thêm vào dòng mới!

Bạn có thể chỉnh sửa data.txt bằng `nano` /`vim` /`Visual Studio Code`
6. thực hiện chương trình chính 
```

   python bot.py

```

# Cách lấy dữ liệu

Mã Javascript để nhận truy vấn (user= /query=)

```javascript
copy(decodeURIComponent(sessionStorage.SourceTarget).split('#tgWebAppData=')[1].split('&tgWebAppVersion=')[0]);console.log('data copied !\npaste ctrl + v')
```

# Run for 24/7

Bạn có thể chạy script bot 24/7 bằng vps /rdp. Bạn có thể sử dụng ứng dụng `screen` trong vps linux để chạy script bot trong quá trình nền

# Discussion

Nếu có câu hỏi hoặc điều gì đó, bạn có thể hỏi tại đây: [@debugs0](https://t.me/debugs0)

# Cảm ơn < 3
