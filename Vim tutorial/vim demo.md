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
| STT | LỆNH                     | TRẠNG THÁI                                                                                                                                                        | Ý NGHĨA                                                         |
| --- | ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| 1   | {start}                  | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30                                                                                           |
| 2   | {ctrl+v}jj               | <span style="background-color:yellow">a</span> = 0<br><span style="background-color:yellow">b</span> = 100<br><span style="background-color:yellow">c</span> = 30 | Vào visual mode, Chọn 3 dòng                                    |
| 3   | {Shift+i}int{space}{ESC} | <span style="background-color:yellow">i</span>nt a = 0<br>int b = 100<br>int c = 30                                                                               | Vào insert mode, chèn ký tự trên nhiều dòng, về lại normal mode |
| 4   | {ctrl+v}jj$              | <span style="background-color:yellow">int a = 0<br>int b = 100<br>int c = 30</span>                                                                               | Bôi đen khu vực cần thao tác                                    |
| 5   | A;{ESC}                  | <span style="background-color:yellow">i</span>nt a = 0;<br>int b = 100;<br>int c = 30;                                                                            | Chèn ký tự ở cuối dòng, về lại normal mode                      |


#### Thao tác với thanh ghi
Thường sử dụng với 2 mục đích
1. Tránh việc tình trạng dữ liệu bị đè lên bộ nhớ đệm mặc định
2. Tạo ra nhiều vị trí lưu trữ bộ nhớ đệm khác nhau, khi cần dùng bộ nhớ nào chỉ cần gọi bộ nhớ đó



| STT | LỆNH    | TRẠNG THÁI                                                                                            | Ý NGHĨA                                                         |
| --- | ------- | ----------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| 1   | {start} | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30                               |
| 2   | "ayy    | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30                               | Sao chép toàn bộ dòng hiện tại vào thanh ghi tên a              |
| 3   | j       | a = 0<br><span style="background-color:yellow">b</span> = 100<br>c = 30                               | Di chuyển con trỏ xuống dòng phía dưới                          |
| 4   | "byy    | a = 0<br><span style="background-color:yellow">b</span> = 100<br>c = 30                               | Sao chép toàn bộ dòng hiện tại vào thanh ghi tên b              |
| 5   | jyy     | a = 0<br>b = 100<br><span style="background-color:yellow">c</span> = 30                               | di chuyển đến dòng phía dưới và sao chép dòng đó vào bộ nhớ đệm |
| 6   | "ap     | a = 0<br>b = 100<br>c = 30<br><span style="background-color:yellow">a</span> = 0                      | dán nội dung của thanh ghi tên a                                |
| 7   | "bp     | a = 0<br>b = 100<br>c = 30<br>a = 0<br><span style="background-color:yellow">b</span> = 100           | dán nội dung của thanh ghi tên b từ                             |
| 8   | "bp     | a = 0<br>b = 100<br>c = 30<br>a = 0<br>b = 100<br><span style="background-color:yellow">c</span> = 30 | dán nội dung từ bộ nhớ đệm                                      |



#### Thay thế (replace)
| STT | LỆNH       | TRẠNG THÁI                                                                 | Ý NGHĨA                                                                                                              |
| --- | ---------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| 1   | {start}    | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30    |
| 2   | :s/=/:=    | <span style="background-color:yellow">a</span> := 0<br>b = 100<br>c = 30   | Thay ký tự = đầu tiên từ vị trí con trỏ thành :=                                                                     |
| 1   | u          | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30    | undo                                                                                                                 |
| 3   | :s/=/:=/g  | <span style="background-color:yellow">a</span> := 0<br>b := 100<br>c := 30 | (g viết tắt của global) Thay thế tất cả ký tự = thành :=                                                             |
| 1   | u          | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30    | undo                                                                                                                 |
| 3   | :s/=/:=/gc |                                                                            | (c viết tắt của confirm)  lần lượt duyệt tất cả các ký tự =, nếu đồng ý đổi thành := thì gõ y, không đồng ý thì gõ n |


#### Đánh dấu (mark)
| STT | LỆNH                              | TRẠNG THÁI                                                                        | Ý NGHĨA                                                                        |
| --- | --------------------------------- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| 1   | {start}                           | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30           |
| 2   | ma                                | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30           | m viết tắt của mark, lệnh này có nghĩa là đánh dấu vị trí hiện tại bằng biến a |
| 3   | j                                 | a = 0<br><span style="background-color:yellow">b</span> = 100<br>c = 30           | Di chuyển con trỏ xuống dòng phía dưới                                         |
| 4   | mb                                | a = 0<br><span style="background-color:yellow">b</span> = 100<br>c = 30           | lệnh này có nghĩa là đánh dấu vị trí hiện tại bằng biến b                      |
| 5   | j                                 | a = 0<br>b = 100<br><span style="background-color:yellow">c</span> = 30           | Di chuyển con trỏ xuống dòng phía dưới                                         |
| 6   | 'a                                | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30           | di chuyển đến vị trí đánh dấu a                                                |
| 7   | 'b                                | a = 0<br><span style="background-color:yellow">b</span> = 100<br>c = 30           | di chuyển đến vị trí đánh dấu b                                                |
| 8   | {shift+g}                         | a = 0<br>b = 100<br><span style="background-color:yellow">c</span> = 30           | Di chuyển con trỏ xuống cuối file                                              |
| 9   | {shift+g}od{space}={space}40{esc} | a = 0<br>b = 100<br>c = 30<br>d = 4<span style="background-color:yellow">0</span> | Di chuyển con trỏ xuống cuối file, thêm nội dung mới                           |
| 10  | gg                                | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30<br>d = 40 | di chuyển con trỏ lên đầu file                                                 |
| 11  | `'                                | a = 0<br>b = 100<br>c = 30<br><span style="background-color:yellow">d</span> = 40 | di chuyển con trỏ đến vị trí cuối cùng thay đổi                                |

#### Thao tác trên cửa sổ 
Tình huống: mở file a.txt, sau đó chép dòng đầu tiên của file b.txt vào cuối file a.txt


| STT | LỆNH        | Ý NGHĨA                                                                     |
| --- | ----------- | --------------------------------------------------------------------------- |
| 1   | vi a.txt    | mở file a.txt từ terminal                                                   |
| 2   | :new b.txt  | mở file b.txt, màn hình bị chia đôi, một nửa phía dưới là nội dung file này |
| 3   | {ctrl+ww}   | chuyển con trỏ qua cửa sổ  đang mở file b.txt                               |
| 4   | yy{ctrl+wq} | sao chép dòng đầu tiên, đóng cửa sổ file b.txt                              |
| 5   | {Shift+g}p  | di chuyển con trỏ xuống cuối file và dán nội dung vừa sao chép              |

Tình huống: mở file a.txt, sau đó có nhu cầu mở file c.txt tại một thư mục khác để  thao tác, thao tác xong rồi đóng file c.txt rồi trở lại file a.txt

| STT | LỆNH          | Ý NGHĨA                                                                                   |
| --- | ------------- | ----------------------------------------------------------------------------------------- |
| 1   | vi a.txt      | mở file a.txt từ terminal                                                                 |
| 2   | :e .          | mở danh sách các file có trong thư mục, dùng các phím di chuyển để chọn file c.txt cần mở |
| 3   | /c.txt{Enter} | tìm kiếm và mở file c.txt                                                                 |
| 4   | :bd           | (buffer delete) thoát file hiện tại, mở lại file trước đó là a.txt                        |
 lưu ý: trong bước 4, trong trường hợp nếu có sửa file c.txt, muốn trở lại file a.txt mà không muốn lưu file c.txt, ta dùng lệnh **:e!** rồi mới dùng **:bd**