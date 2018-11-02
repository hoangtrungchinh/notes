### VIM P2 - THUC HANH

#### VD1: làm quen k? t? . và 2 ch? ð? normal node, insert mode
K? t? "." có ch?c nãng l?p l?i l?nh g?n nh?t v?a s? d?ng

| 1          | 2                                                       |                                                                                           |
| ---------- | ------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| {start}    | **L**ine one<br>Line two<br>Line three<br>Line four     | V?a m? file b?ng vim                                                                      |
| x          | **i**ne one<br>Line two<br>Line three<br>Line four      | xóa k? t? ? v? trí con tr?                                                                |
| .          | **n**e one<br>Line two<br>Line three<br>Line four       | L?p l?i ? ngh?a l?nh v?a g? (t?c xóa 1 k? t?)                                             |
| ...        | **o**ne<br>Line two<br>Line three<br>Line four          | l?p l?i 3 l?n l?nh v?a g? (t?c xóa 3 k? t?)                                               |
| dd         | **L**ine two<br>Line three<br>Line four                 | Xóa nguyên 1 d?ng                                                                         |
| Esc A; Esc | Line two **;**<br>Line three<br>Line four               | Chuy?n con tr? v? cu?i hàng<br>Chèn thêm d?u ";"<br> Thoát insert mode v? l?i normal mode |
| j.         | Line two **;** <br>Line three **;**<br>Line four        | Xu?ng hàng và l?p l?i các bý?c ð? dùng trý?c ðó (A; Esc)                                  |
| j.         | Line two **;** <br>Line three **;**<br>Line four  **;** | Xu?ng hàng và l?p l?i các bý?c ð? dùng trý?c ðó (A; Esc)                                  |



#### VD2: làm quen v?i normal mode, visual mode


| 1         | 2                                                        |     |
| --------- | -------------------------------------------------------- | --- |
| {start}   | var foo = "method("+argument1+","+argument2+")";         |   | 
| f+        | var foo = "method("+argument1+","+argument2+")";         |  | 
| s?+?<Esc>  | var foo = "method(" + argument1+","+argument2+")";       |  | 
| ;         | var foo = "method(" + argument1+","+argument2+")";       |  | 
| .         | var foo = "method(" + argument1 + ","+argument2+")";     |  | 
| ;.        | var foo = "method(" + argument1 + "," + argument2+")";   |  | 
| ;.        | var foo = "method(" + argument1 + "," + argument2 + ")"; |  | 