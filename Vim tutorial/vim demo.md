### VIM P3 - THỰC HÀNH 1 - TỔNG QUAN

#### Tạo vào lưu file
Tạo file demo.txt có nội dung sau:
> Hello world

| STT | Lệnh         | Ý nghĩa                                    |
| --- | ------------ | ------------------------------------------ |
| 1   | vim demo.txt | Chạy trong terminal, mở vim                |
| 2   | i            | Chuyển từ normal mode sang  insert mode    |
| 3   | Hello world  | Nhập nội dung file                         |
| 4   | esc          | Thoát khỏi insert mode, về lại normal mode |
| 5   | :wq          | Lưu và thoát                               |

##### Lưu ý
* Tại bước 2, có thể sử dụng các phím khác để vào insermode
* Tại bước 4: có thể dùng tổ hợp phím ctrl+c
  
#### Làm quen với các phím di chuyển
| STT | Lệnh           | Ý nghĩa                                                                                                                                                                                                                                                                                               | Giải thích                      |
| --- | -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------- |
| 1   | Trạng thái đầu | <span style="background-color:yellow">T</span>o Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> |
| 2   | l              | T<span style="background-color:yellow">o</span> Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển sang phải 1 ký tự     |
| 3   | h              | <span style="background-color:yellow">T</span>o Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển sang trái 1 ký tự     |
| 4   | j              | To Sherlock Holmes she is always the woman. <br> <span style="background-color:yellow">I</span> have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển xuống dưới 1 ký tự    |
| 5   | k              | <span style="background-color:yellow">T</span>o Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển lên trên 1 ký tự      |
| 6   | 10l            | To Sherloc<span style="background-color:yellow">k</span> Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển sang phải 10 ký tự    |
| 7   | 2j             | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eye<span style="background-color:yellow">s</span> she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển xuống dưới 2 dòng     |
| 8   | w              | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes <span style="background-color:yellow">s</span>he eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến đầu từ tiếp theo  |
| 9   | b              | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his <span style="background-color:yellow">e</span>yes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến đầu từ trước đó   |
| 10  | )              | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> <span style="background-color:yellow">I</span>t was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến đầu câu tiếp theo |
| 11  | (              | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> <span style="background-color:yellow">I</span>n his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến đầu câu trước đó  |
| 12  | }              | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler<span style="background-color:yellow">.</span><br> | Di chuyển đến đoạn tiếp đó      |
| 13  | {              | <span style="background-color:yellow">T</span>o Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến đoạn trước đó     |
| 14  | Shift+g        | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler<span style="background-color:yellow">.</span><br> | Di chuyển đến cuối file         |
| 15  | gg             | <span style="background-color:yellow">T</span>o Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến đầu file          |
| 16  | shift+4        | To Sherlock Holmes she is always the woman<span style="background-color:yellow">.</span> <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến cuối dòng         |
| 17  | 0              | <span style="background-color:yellow">T</span>o Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến đầu dòng          |
| 17  | :3             | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> <span style="background-color:yellow">I</span>n his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Di chuyển đến dòng số 3         |

* Trong bước 6 và 7: chữ số đứng trước lệnh di chuyển chỉ số lần thực hiện lệnh di chuyển đó, cách thức này áp dụng cho tất cả các lệnh di chuyển khác, ví dụ: 2) 3} 4{
* Bước 12 và 13 sẽ thấy rõ khi file có nhiều đoạn

> Một vài gợi ý:
> * Truy cập https://vim-adventures.com/
> * Đặt tay theo vị trí sau và chơi game
>     * Ngón trỏ: **j**
>     * Ngón giữa: **k**
>     * Ngón áp út: **l**
> * Lưu ý: riêng phím **h** chúng ta sử dụng ngón trỏ

#### Tìm kiếm đơn giản


| STT | LỆNH           | TRẠNG THÁI                                                                                                                                                                                                                                                                                            | GIẢI THÍCH                               |
| --- | -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| 1   | Trạng thái đầu | <span style="background-color:yellow">T</span>o Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> |
| 2   | /the           | To Sherlock Holmes she is always <span style="background-color:yellow">t</span>he woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Tìm vị trí "the" sau con trỏ             |
| 3   | n              | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any o<span style="background-color:yellow">t</span>her name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Tìm vị trí "the" tiếp theo sau con trỏ   |
| 4   | ?the           | To Sherlock Holmes she is always <span style="background-color:yellow">t</span>he woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates the whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Tìm vị trí "the" trước con trỏ           |
| 5   | n              | To Sherlock Holmes she is always the woman. <br> I have seldom heard him mention her under any other name.<br> In his eyes she eclipses and predominates <span style="background-color:yellow">t</span>he whole of her sex.<br> It was not that he felt any emotion akin to love for Irene Adler.<br> | Tìm vị trí "the" tiếp theo trước con trỏ |

Lưu ý: 
* Ở bước 5, vì đã tìm hết các từ ở trước con trỏ mà không thấy nên vim sẽ bắt đầu tìm tiếp tục ở cuối file trở lên
* Ở bước 3, để tìm hiệu quả hơn, người ta sử dụng regular expression kết hợp tìm kiếm (sẽ trình bày sau)




#### Thao tác xóa

| STT | LỆNH    | TRẠNG THÁI                                                                                            | Ý NGHĨA                             |
| --- | ------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------- |
| 1   | {start} | <span style="background-color:yellow">D</span>elete more than one word                                | Vị trí con trỏ hiện tại             |
| 2   | yyp     | Delete more than one word <br> <span style="background-color:yellow">D</span>elete more than one word | Nhân đôi dòng hiện tại              |
| 3   | dd      | <span style="background-color:yellow">D</span>elete more than one word                                | Xóa dòng hiện tại                   |
| 4   | d2w     | <span style="background-color:yellow">t</span>han one word                                            | Xóa 2 ký tự sát con trỏ             |
| 5   | u       | <span style="background-color:yellow">D</span>elete more than one word                                | Bỏ đi thao tác vừa rồi              |
| 6   | 3dw     | <span style="background-color:yellow">o</span>ne word                                                 | Xóa 3 ký tự sát con trỏ             |
| 7   | u       | <span style="background-color:yellow">D</span>elete more than one word                                | Bỏ đi thao tác vừa rồi              |
| 8   | yyp     | Delete more than one word <br> <span style="background-color:yellow">D</span>elete more than one word | Nhân đôi dòng hiện tại              |
| 9   | d/one   | Delete more than one word<br> <span style="background-color:yellow">o</span>ne word                   | Xóa từ vị trí con trỏ đên chữ "one" |
| 10  | d)      | Delete more than one word<br> <span style="background-color:yellow">_</span>                          | Xóa từ vị trí con trỏ đên hết câu   |

#### Thao tác sao chép

| STT | LỆNH    | TRẠNG THÁI                                                                                                 | Ý NGHĨA                                     |
| --- | ------- | ---------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| 1   | {start} | <span style="background-color:yellow">C</span>opy more than one word                                       | Vị trí con trỏ hiện tại                     |
| 2   | yw      | <span style="background-color:yellow">C</span>opy more than one word                                       | copy một từ tại vị trí con trỏ (chữ "Copy") |
| 3   | shift+p | Copy<span style="background-color:yellow">_</span>Copy more than one word                                  | Dán vào trước vị trí con trỏ                |
| 4   | yyp     | Copy Copy more than one word<br> <span style="background-color:yellow">C</span>opy Copy more than one word | Copy và dán 1 dòng                          |

#### Thao tác chọn nhiều dòng
| STT | LỆNH                  | TRẠNG THÁI                                                                                                                                                  | Ý NGHĨA                                                         |
| --- | --------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| 1   | {start}                  | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30                                                                                           |
| 2   | {ctrl+v}jj               | <span style="background-color:yellow">a</span> = 0<br><span style="background-color:yellow">b</span> = 100<br><span style="background-color:yellow">c</span> = 30 | Vào visual mode, Chọn 3 dòng                                    |
| 3   | {Shift+i}int{space}{ESC} | <span style="background-color:yellow">i</span>nt a = 0<br>int b = 100<br>int c = 30                                                                               | Vào insert mode, chèn ký tự trên nhiều dòng, về lại normal mode |
| 4   | {ctrl+v}jj$              | <span style="background-color:yellow">int a = 0<br>int b = 100<br>int c = 30</span>                                                                               | Bôi đen khu vực cần thao tác                                    |
| 5   | A;{ESC}                  | <span style="background-color:yellow">i</span>nt a = 0;<br>int b = 100;<br>int c = 30;                                                                            | Chèn ký tự ở cuối dòng, về lại normal mode                      |


#### Thao tác với thanh ghi
| STT | LỆNH    | TRẠNG THÁI       | Ý NGHĨA |
| --- | ------- | ---------------- | ------- |
| 1   | {start}                  | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30                             
| 2   | "ayy                  | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30                             | Sao chép toàn bộ dòng hiện tại vào biến a trong bộ nhớ đệm
| 3   | j                  | a = 0<br><span style="background-color:yellow">b</span> = 100<br>c = 30                             | Di chuyển con trỏ xuống dòng thứ 2
| 4   | "byy                  | a = 0<br><span style="background-color:yellow">b</span> = 100<br>c = 30                             | Sao chép toàn bộ dòng hiện tại vào biến b trong bộ nhớ đệm