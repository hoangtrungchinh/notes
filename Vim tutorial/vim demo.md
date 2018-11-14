### VIM P3 - THỰC HÀNH 1 - TỔNG QUAN

#### Tạo vào lưu file
Tạo file demo.txt có nội dung sau:
> Hello world

| STT | Lệnh         | Ý nghĩa                                    |     |
| --- | ------------ | ------------------------------------------ | --- |
| 1   | vim demo.txt | Chạy trong terminal, mở vim                |
| 2   | i            | Chuyển từ normal mode sang  insert mode    |
| 3   | Hello world  | Nhập nội dung file                         |
| 4   | esc          | Thoát khỏi insert mode, về lại normal mode |
| 5   | :wq          | Lưu và thoát                               |

##### Lưu ý
* Tại bước 2, có thể sử dụng các phím khác để vào insermode
* Tại bước 4: có thể dùng tổ hợp phím ctrl+c
  
#### Làm quen với các phím di chuyển
| STT | Lệnh         | Ý nghĩa                                    |     |
| --- | ------------ | ------------------------------------------ | --- |
|1|Trạng thái đầu|<span style="background-color:yellow">T</span>o Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|
|2|l|T<span style="background-color:yellow">o</span> Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển sang phải 1 ký tự
|3|h|<span style="background-color:yellow">T</span>o Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển sang trái 1 ký tự
|4|h|<span style="background-color:yellow">T</span>o Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển sang trái 1 ký tự


Sử dụng các phím h,j,k,l để di chuyển trong game sau
* Truy cập https://vim-adventures.com/
* Đặt tay theo vị trí sau và chơi game
    * Ngón trỏ: **j** - đi xuống
    * Ngón giữa: **k** - đi lên
    * Ngón áp út: **l** - qua phải
* Lưu ý: Sử dụng ngón trỏ đế nhấn phím **h** khi muốn di chuyển qua trái


