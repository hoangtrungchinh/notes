### VIM P4 - THỰC HÀNH 2

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
| 3   | u          | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30    | undo                                                                                                                 |
| 4   | :s/=/:=/g  | <span style="background-color:yellow">a</span> := 0<br>b := 100<br>c := 30 | (g viết tắt của global) Thay thế tất cả ký tự = thành :=                                                             |
| 5   | u          | <span style="background-color:yellow">a</span> = 0<br>b = 100<br>c = 30    | undo                                                                                                                 |
| 6   | :s/=/:=/gc |                                                                            | (c viết tắt của confirm)  lần lượt duyệt tất cả các ký tự =, nếu đồng ý đổi thành := thì gõ y, không đồng ý thì gõ n |


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

#### Thao tác trên cửa sổ  và buffer
Tình huống: mở file a.txt, sau đó chép dòng đầu tiên của file b.txt vào cuối file a.txt

| STT | LỆNH           | Ý NGHĨA                                                                     |
| --- | -------------- | --------------------------------------------------------------------------- |
| 1   | vi a.txt       | mở file a.txt từ terminal                                                   |
| 2   | :new b.txt     | mở file b.txt, màn hình bị chia đôi, một nửa phía dưới là nội dung file này |
| 3   | {ctrl+ww}      | chuyển con trỏ qua cửa sổ  đang mở file b.txt                               |
| 4   | yy{ctrl+wq}    | sao chép dòng đầu tiên, đóng cửa sổ file b.txt                              |
| 5   | {Shift+g}p     | di chuyển con trỏ xuống cuối file và dán nội dung vừa sao chép              |
| 6   | :sp            | Chia đôi cửa sổ hiện tại theo chiều ngang                                   |
| 6   | :sp {filepath} | Mở filepath và chia đôi cửa sổ hiện tại theo chiều ngang                    |
| 7   | :vs            | Chia đôi cửa sổ hiện tại theo chiều dọc                                     |
| 7   | :vs {filepath} | Mở filepath và chia đôi cửa sổ hiện tại theo chiều dọc                      |

Tình huống: mở file a.txt, sau đó có nhu cầu mở file c.txt tại một thư mục khác để  thao tác, thao tác xong rồi đóng file c.txt rồi trở lại file a.txt

| STT | LỆNH          | Ý NGHĨA                                                                                   |
| --- | ------------- | ----------------------------------------------------------------------------------------- |
| 1   | vi a.txt      | mở file a.txt từ terminal                                                                 |
| 2   | :e .          | mở danh sách các file có trong thư mục, dùng các phím di chuyển để chọn file c.txt cần mở |
| 3   | /c.txt{Enter} | tìm kiếm và mở file c.txt                                                                 |
| 4   | :bd           | (buffer delete) thoát file hiện tại, mở lại file trước đó là a.txt                        |
 
 lưu ý: trong bước 4, trong trường hợp nếu có sửa file c.txt, muốn trở lại file a.txt mà không muốn lưu file c.txt, ta dùng lệnh **:e!** rồi mới dùng **:bd** 

 Tình huống: mở nhiều file và chuyển qua lại giữa các cửa sổ
| STT | LỆNH          | Ý NGHĨA                                      |
| --- | ------------- | -------------------------------------------- |
| 1   | vi a.txt      | mở file a.txt từ terminal                    |
| 2   | :e b.txt      | mở file b.txt từ vim                         |
| 3   | :e c.txt      | mở file c.txt từ vim                         |
| 4   | :ls           | danh sách các file được mở                   |
| 5   | :bn           | mở file kế tiếp trong số các file được mở    |
| 6   | :b {filename} | mở theo tên file (dùng tab để chọn tên file) |


