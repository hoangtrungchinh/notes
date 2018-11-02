### VIM P2 - THUC HANH

#### VD1: l�m quen k? t? . v� 2 ch? �? normal node, insert mode
K? t? "." c� ch?c n�ng l?p l?i l?nh g?n nh?t v?a s? d?ng

| 1          | 2                                                       |                                                                                           |
| ---------- | ------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| {start}    | **L**ine one<br>Line two<br>Line three<br>Line four     | V?a m? file b?ng vim                                                                      |
| x          | **i**ne one<br>Line two<br>Line three<br>Line four      | x�a k? t? ? v? tr� con tr?                                                                |
| .          | **n**e one<br>Line two<br>Line three<br>Line four       | L?p l?i ? ngh?a l?nh v?a g? (t?c x�a 1 k? t?)                                             |
| ...        | **o**ne<br>Line two<br>Line three<br>Line four          | l?p l?i 3 l?n l?nh v?a g? (t?c x�a 3 k? t?)                                               |
| dd         | **L**ine two<br>Line three<br>Line four                 | X�a nguy�n 1 d?ng                                                                         |
| Esc A; Esc | Line two **;**<br>Line three<br>Line four               | Chuy?n con tr? v? cu?i h�ng<br>Ch�n th�m d?u ";"<br> Tho�t insert mode v? l?i normal mode |
| j.         | Line two **;** <br>Line three **;**<br>Line four        | Xu?ng h�ng v� l?p l?i c�c b�?c �? d�ng tr�?c �� (A; Esc)                                  |
| j.         | Line two **;** <br>Line three **;**<br>Line four  **;** | Xu?ng h�ng v� l?p l?i c�c b�?c �? d�ng tr�?c �� (A; Esc)                                  |



#### VD2: l�m quen v?i normal mode, visual mode


| 1         | 2                                                        |     |
| --------- | -------------------------------------------------------- | --- |
| {start}   | var foo = "method("+argument1+","+argument2+")";         |   | 
| f+        | var foo = "method("+argument1+","+argument2+")";         |  | 
| s?+?<Esc>  | var foo = "method(" + argument1+","+argument2+")";       |  | 
| ;         | var foo = "method(" + argument1+","+argument2+")";       |  | 
| .         | var foo = "method(" + argument1 + ","+argument2+")";     |  | 
| ;.        | var foo = "method(" + argument1 + "," + argument2+")";   |  | 
| ;.        | var foo = "method(" + argument1 + "," + argument2 + ")"; |  | 