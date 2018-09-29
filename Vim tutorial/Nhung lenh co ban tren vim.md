#### Di chuyển con trỏ
Ta di chuyển bằng các phím:
* h (sang trái), 
* j (xuống dưới), 
* k (lên trên) và 
* l (sang phải) 

Lưu ý: Trên Vim ta cũng có thể sử dụng các phím mũi tên để điều hướng, nhưng theo kinh nghiệm của các chuyên gia thì sử dụng các phím trên sẽ nhanh hơn

#### Thao tác Xóa
* **x**: xóa một kí tự tại vị trí con trỏ hiện tại
* **dw**: xóa một từ tính từ vị trí con trỏ hiện tại đến bắt đầu của từ tiếp theo (không bao gồm kí tự đầu tiên của từ tiếp theo và xóa cả các dấu cách)
* **d** hoặc **dd**: xóa dòng hiện tại
* **d$**: xóa từ vị trí con trỏ đến hết dòng hiện tại
* **d{num}**: xóa số dòng bằng giá trị {num} tính từ dòng hiện tại (VD: xóa 10 dòng thì dùng d10)

#### Thao tác chèn
Để chèn văn bản thì các phím được sử dụng cũng chính là các phím dùng để chuyển từ chế độ normal vào chế độ insert:

* **i**: con trỏ sẽ ở luôn vị trí hiện tại
* **I**: con trỏ sẽ ở đầu dòng hiện tại
* **a**: con trỏ sẽ ở ngay sau vị trí hiện tại 1 kí tự
* **A**: con trỏ sẽ ở cuối dòng hiện tại
* **o**: VIM sẽ thêm một dòng bên dưới dòng hiện tại và đặt con trỏ tại dòng này
* **O**: tương tự o nhưng thay vì thêm 1 dòng bên dưới thì sẽ thêm 1 dòng bên trên dòng hiện tại

#### Thao tác phục hồi
Sử đụng một trong hai phím
* u
* *Ctrl + R

#### Lưu và thoát
để lưu file trong chế độ normal
* :w
* :w filename

Để thoát file ta dùng:
* :q
* :q! dùng để thoát mà không lưu thay 
* :qa để thoát tất cả các file đang mở.