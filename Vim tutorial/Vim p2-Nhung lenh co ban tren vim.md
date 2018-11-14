### VIM P2 - NHỮNG LỆNH CƠ BẢN

#### Di chuyển con trỏ
Ta di chuyển bằng các phím:
* **h**: di chuyển sang trái 
* **j**: di chuyển xuống dưới 
* **k**: di chuyển lên trên
* **l**: di chuyển sang phải 
* **w**: di chuyển đến đầu từ tiếp theo
* **b**: di chuyển đến đầu từ trước đó
* **e**: di chuyển đến cuối từ tiếp theo
* **ge**: di chuyển đến cuối từ trước đó


#### Thao tác Xóa
* **x**: xóa một kí tự tại vị trí con trỏ hiện tại
* **dw**: *delete word* - xóa một từ tính từ vị trí con trỏ hiện tại đến vị trí bắt đầu của từ tiếp theo (không bao gồm kí tự đầu tiên của từ tiếp theo và xóa cả các dấu cách)
* **daw**: *delete a word* - Xóa toàn bộ từ đang chứa con trỏ
* **db**: xóa từ vị trí con trỏ hiện tại đến đầu từ trước đó
* **dd**: xóa dòng hiện tại
* **d$**: xóa từ vị trí con trỏ đến hết dòng hiện tại
* **d{num}**: xóa số dòng bằng giá trị {num} tính từ dòng hiện tại (VD: xóa 10 dòng thì dùng d10)

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
