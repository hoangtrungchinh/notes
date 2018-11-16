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
|4|j|To Sherlock Holmes she is always THE woman. <br> <span style="background-color:yellow">I</span> have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển xuống dưới 1 ký tự
|5|k|<span style="background-color:yellow">T</span>o Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển lên trên 1 ký tự
|6|10l|To Sherloc<span style="background-color:yellow">k</span> Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển sang phải 10 ký tự
|7|2j|To Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eye<span style="background-color:yellow">s</span> she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển xuống dưới 2 dòng
|8|w|To Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes <span style="background-color:yellow">s</span>he eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển đến đầu từ tiếp theo
|9|b|To Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his <span style="background-color:yellow">e</span>yes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển đến đầu từ trước đó
|10|)|To Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> <span style="background-color:yellow">I</span>t was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển đến đầu câu tiếp theo
|11|(|To Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> <span style="background-color:yellow">I</span>n his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển đến đầu câu trước đó
|12|}|To Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler<span style="background-color:yellow">.</span><br>|Di chuyển đến đoạn tiếp đó
|13|{|<span style="background-color:yellow">T</span>o Sherlock Holmes she is always THE woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br>|Di chuyển đến đoạn trước đó

Trong bước 6 và 7, ta thấy có chữ số đứng trước lệnh di chuyển chỉ số lần thực hiện lệnh di chuyển đó, cách thức này áp dụng cho tất cả các lệnh di chuyển khác, ví dụ: 2) 3} 4{

> Một vài gợi ý:
> * Truy cập https://vim-adventures.com/
> * Đặt tay theo vị trí sau và chơi game
>     * Ngón trỏ: **j**
>     * Ngón giữa: **k**
>     * Ngón áp út: **l**
> * Lưu ý: riêng phím **h** chúng ta sử dụng ngón trỏ





