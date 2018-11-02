### VIM P2 - THUC HANH

#### VD1: Làm quen ký tự . và chế độ normal node, insert mode
Ký tự "." có chức năng lặp lại lệnh gần nhất sử dụng

| 1          | 2                                                       |                                                                                           |
| ---------- | ------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| {start}    | **L**ine one<br>Line two<br>Line three<br>Line four     | Vừa mở file bằng vim                                                                      |
| x          | **i**ne one<br>Line two<br>Line three<br>Line four      | Xóa ký tự tại vị trí con trỏ                                                              |
| .          | **n**e one<br>Line two<br>Line three<br>Line four       | Lặp lại lệnh vừa thực hiện (xóa ký tự)                                                    |
| ...        | **o**ne<br>Line two<br>Line three<br>Line four          | Lặp lại 3 lần lệnh vừa thực hiện (xóa ký tự)                                              |
| dd         | **L**ine two<br>Line three<br>Line four                 | Xóa nguyên 1 dòng                                                                         |
| Esc A; Esc | Line two **;**<br>Line three<br>Line four               | Chuyển con trỏ về cuối dòng<br>Chèn thêm dấu ";"<br> Thoát insert mode về lại normal mode |
| j.         | Line two **;** <br>Line three **;**<br>Line four        | Xuống hàng và lặp lại các bước trước đó (A; Esc)                                          |
| j.         | Line two **;** <br>Line three **;**<br>Line four  **;** | Xuống hàng và lặp lại các bước trước đó (A; Esc)                                          |



#### VD2: l�m quen v?i normal mode, visual mode


| 1         | 2                                                        |     |
| --------- | -------------------------------------------------------- | --- |
| {start}   | var foo = "method("+argument1+","+argument2+")";         |     |
| f+        | var foo = "method("+argument1+","+argument2+")";         |     |
| s?+?<Esc> | var foo = "method(" + argument1+","+argument2+")";       |     |
| ;         | var foo = "method(" + argument1+","+argument2+")";       |     |
| .         | var foo = "method(" + argument1 + ","+argument2+")";     |     |
| ;.        | var foo = "method(" + argument1 + "," + argument2+")";   |     |
| ;.        | var foo = "method(" + argument1 + "," + argument2 + ")"; |     |