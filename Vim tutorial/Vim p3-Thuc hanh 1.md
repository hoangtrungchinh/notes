### VIM P3 - THỰC HÀNH 1

#### VD1: Làm quen ký tự .
Ký tự "." có chức năng lặp lại lệnh gần nhất sử dụng

| 1          | 2                                                       |                                                                                           |
| ---------- | ------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| {start}    | <span style="background-color:blue">L</span>ine one<br>Line two<br>Line three<br>Line four     | Vừa mở file bằng vim                                                                      |
| x          | <span style="background-color:blue">i</span>ne one<br>Line two<br>Line three<br>Line four      | Xóa ký tự tại vị trí con trỏ                                                              |
| .          | <span style="background-color:blue">n</span>e one<br>Line two<br>Line three<br>Line four       | Lặp lại lệnh vừa thực hiện (xóa ký tự)                                                    |
| ...        | <span style="background-color:blue">o</span>ne<br>Line two<br>Line three<br>Line four          | Lặp lại 3 lần lệnh vừa thực hiện (xóa ký tự)                                              |
| dd         | <span style="background-color:blue">L</span>ine two<br>Line three<br>Line four                 | Xóa nguyên 1 dòng                                                                         |
| Esc A; Esc | Line two **;**<br>Line three<br>Line four               | Chuyển con trỏ về cuối dòng<br>Chèn thêm dấu ";"<br> Thoát insert mode về lại normal mode |
| j.         | Line two **;** <br>Line three **;**<br>Line four        | Xuống hàng và lặp lại các bước trước đó (A; Esc)                                          |
| j.         | Line two **;** <br>Line three **;**<br>Line four  **;** | Xuống hàng và lặp lại các bước trước đó (A; Esc)                                          |



#### VD2: Làm quen với lệnh tìm kiếm
Đây là ví dụ đơn giản cho việc tìm kiếm và thay thế

| 1         | 2                                                  |                                                                           |
| --------- | -------------------------------------------------- | ------------------------------------------------------------------------- |
| {start}   | <span style="background-color:blue">"</span>method("+argument1+","+argument2+")";         | Trạng thái đầu tiên khi vừa mở Vim                                        |
| f+        | "method("<span style="background-color:blue">+</span>argument1+","+argument2+")";        | Tìm và di chuyển con trỏ đến vị trị cần tìm (dấu +)                       |
| s␣+␣<Esc> | "method(" +<span style="background-color:blue">␣</span>argument1+","+argument2+")";       | Xóa ký tự vị trí hiện tại <br>Thêm vào ␣+␣ <br> Về lại chế độ normal node |
| ;         | "method(" + argument1 <span style="background-color:blue">+</span>","+argument2+")";      | Lặp lại các thao tác search cuối cùng f+                                  |
| .         | "method(" + argument1 +<span style="background-color:blue">␣</span>","+argument2+")";     | Lặp lại các thao tác s␣+␣<Esc>                                            |
| ;.        | "method(" + argument1 + "," +<span style="background-color:blue">␣</span>argument2+")";   | Lặp lại các thao tác f+s␣+␣<Esc>                                          |
| ;.        | "method(" + argument1 + "," + argument2 +<span style="background-color:blue">␣</span>")"; | Lặp lại các thao tác f+s␣+␣<Esc>                                          |
