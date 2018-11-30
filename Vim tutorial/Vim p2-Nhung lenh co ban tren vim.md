### VIM P2 - NHỮNG LỆNH CƠ BẢN

#### Di chuyển con trỏ
* Theo bốn hướng:
    * **h**: di chuyển sang trái 
    * **j**: di chuyển xuống dưới 
    * **k**: di chuyển lên trên
    * **l**: di chuyển sang phải 

* Theo đơn vị từ:
    * **w**: di chuyển đến đầu từ tiếp theo
    * **b**: di chuyển đến đầu từ trước đó
    * **e**: di chuyển đến cuối từ tiếp theo
    * **ge**: di chuyển đến cuối từ trước đó

* Theo đơn vị câu:
    * **(**: di chuyển đoạn câu trước đó
    * **)**: di chuyển đoạn câu tiếp theo

* Theo đơn vị dòng:
    * **shift+4**: di chuyển đến cuối dòng
    * **0**: di chuyển đến đầu dòng
    * **:{num}**: di chuyển đến dòng thứ num

* Theo đơn vị đoạn:
    * **}**: di chuyển đến đoạn tiếp theo
    * **{**: di chuyển đến đoạn trước đó

* Theo đơn vị màn hình:
    * **ctrl+f**: di chuyển con trỏ đến đầu trang màn hình tiếp theo (tương tự page down)
    * **ctrl+b**: di chuyển con trỏ đến đầu trang màn hình trước đó (tương tự page up)

* Theo đơn vị file
    * **Shift + g**: di chuyển đến cuối file
    * **gg**: di chuyển đến đầu file

#### Thao tác Xóa
* Theo đơn vị ký tự:
    * **x**: xóa một kí tự tại vị trí con trỏ hiện tại

* Theo đơn vị từ:
    * **dw**: *delete word* - xóa một từ tính từ vị trí con trỏ hiện tại đến vị trí bắt đầu của từ tiếp theo (không bao gồm kí tự đầu tiên của từ tiếp theo và xóa cả các dấu cách)
    * **daw**: *delete a word* - Xóa toàn bộ từ đang chứa con trỏ
    * **db**: xóa từ vị trí con trỏ hiện tại đến đầu từ trước đó

* Theo đơn vị dòng:    
    * **dd**: xóa dòng hiện tại
    * **d{num}**: xóa số dòng bằng giá trị {num} tính từ dòng hiện tại (VD: xóa 10 dòng thì dùng d10)
    * **d$**: xóa từ vị trí con trỏ đến hết dòng hiện tại
    
* Theo đơn vị câu:    
    * **d)**: xóa câu hiện tại

* Theo regular expresion:    
    * **d/tu_can_giu**: xóa từ vị trí con trỏ đến tu_can_giu

* Xóa trong visual mode:    
    * **shift+d**: Xóa những từ được bôi đen
    * **d**: Xóa những từ được bôi đen khi chọn theo block

#### Thao tác sao chép
* **y**: Sao chép những từ được chọn
* **yw**: Sao chép chữ ở vị trí con trỏ hiện tại
* **yy**: Sao chép dòng ở vị trí con trỏ hiện tại
* **y)**: Sao chép từ vị trí con trỏ hiện tại đến hết câu
* **y}**: Sao chép từ vị trí con trỏ hiện tại đến hết đoạn

#### Thao tác dán
* **p**: Dán các từ trong bộ nhớ đệm

#### Thao tác thay đổi
Về cơ bản thao tác này thay cho việc bôi đen, xóa, chuyển về insert mode
* **cw**: Thay đổi từ vị trí hiện tại hết hết chữ
* **c)**: Thay đổi từ vị trí hiện tại hết hết câu
* **c}**: Thay đổi từ vị trí hiện tại hết hết đoạn
* **c/tu_khong_can_doi**: Thay đổi từ vị trí hiện tại đến từ không cần đổi

#### Thao tác chèn
Để chèn văn bản thì các phím được sử dụng cũng chính là các phím dùng để chuyển từ chế độ normal vào chế độ insert:

* **i**: con trỏ sẽ ở luôn vị trí hiện tại
* **I**: con trỏ sẽ ở đầu dòng hiện tại
* **a**: con trỏ sẽ ở ngay sau vị trí hiện tại 1 kí tự
* **A**: con trỏ sẽ ở cuối dòng hiện tại
* **o**: thêm một dòng bên dưới dòng hiện tại và đặt con trỏ tại dòng này
* **O**: thêm một dòng bên trên dòng hiện tại và đặt con trỏ tại dòng này

#### Thao tác nhân đôi dòng
* **yyp**: Nhân đôi dòng hiện tại và chuyển con trỏ xuống dòng phía dưới

#### Thao tác thay đổi dạng chữ
* **gUU**: Chuyển tất cả chữ trong dòng sang chữ hoa
* **guu**: Chuyển tất cả chữ trong dòng sang chữ thường

#### Thao tác thay đổi lề dòng
* **>**: Dòng thụt về phía bên phải (tab)
* **<**: Dòng thụt về phía bên trái (shift tab)

#### Thao tác phục hồi
Sử đụng một trong hai phím
* **u**
* **Ctrl + R**

#### Mở  1 file
* **vi filename** sử dụng trong terminal
* **:e filename** sử dụng trong normal mode

#### Lưu và thoát
Để lưu file trong chế độ normal
* **:w**
* **:w filename**

Để thoát file ta dùng:
* **:q**
* **:q!** dùng để thoát mà không lưu
* **:qa** dùng để thoát tất cả các file đang mở
* **:wq** hoặc **:x**  dùng để vừa lưu vừa thoát

#### Tìm kiếm
* **/noi_dung_tim**: Tìm ở vị trí sau con trỏ
    * **n**: tìm từ kế tiếp
* **?noi_dung_tim**: Tìm ở vị trí trước con trỏ
    * **n**: tìm từ trước đó
* **\***: Tìm từ kế tiếp nằm ở vị trí con trỏ hiện tại 
* **#**: Tìm từ trước đó nằm ở vị trí con trỏ hiện tại 
 
#### Thao tác chọn (bôi đen)
* **shift+v**: chọn 1 dòng
* **Ctr+v**: chọn 1 block (dùng các phím di chuyển để  chọn blog)

#### Thao tác trên cửa sổ
* **:split**: Chia cửa sổ theo chiều ngang
* **Ctrl+ww**: Chuyển qua lại giữa các cửa sổ