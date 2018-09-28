# TỔNG QUAN VỀ VIM


## VIM LÀ GÌ?
Vim (Vi IMproved) là một text editor phổ biến cho những lập trình viên, nó ra đời năm 1991 bởi Bram Moolenaar như một phiên bản mở rộng của Vi (viết bởi Bill Joy).  Một trong những cái tiến đáng nói là việc hỗ trợ nhiều hệ điều hành hơn, highlight code tốt hơn, hỗ trợ split màn hình và các plugin

## NGƯỜI TA SỬ DỤNG VIM VÌ 3N
1. **Nhanh**: người dùng chỉ cần bàn phím, không cần chuột để thao tác
2. **Ngon**: Làm việc trên hầu hết môi trường, đặc biệt là phổ biến nhất là Server
3. **Nhiều**: Khả năng rộng mở cao qua các plugin, có khả năng tùy chỉnh theo ý mình

## CÀI ĐẶT VIM
Mặc định Vim đã được cài sẵn, trong trường hợp chưa được cài thì chúng ta dùng lệnh

### Với Ubuntu (Unix))
    sudo apt-get update
    sudo apt-get install vim

Kiểm tra vim đã được cài đặt thành công hay chưa

    vim -v

### Với Apple OS X
    brew update 
    brew install vim && brew instal macvim
    brew link macvim

### Trên window

1. Chọn package neovim [nvim-win32.zip](nvim-win32)  hoặc [nvim-win64.zip](https://github.com/neovim/neovim/releases/download/v0.2.2/nvim-win64.zip)
2. Giản nén unzip ở bất cứ đâu
3. Mở thư mục và double-click vào nvim-qt.exe

## Các mode trên Vim

1. **Normal Mode**: - Được sử dụng để chỉnh sửa, sao chép, dán, di chuyển, xóa và thay đổi văn bản được thực hiện từ trong chế độ này.

2. **Insert Mode**: - Được sử dụng để update hay thay đổi data,text...

3. **Command mode**: - Chế độ này được sử dụng để lưu tài liệu, thoát khỏi chương trình, thực hiện tìm kiếm....

4. **Visual Mode (bôi đen)**: - Được sử dụng để lựa chọn hình ảnh

Các phím tắt để chuyển qua lại giữa các mode xin xem trong hình

![vim mode](https://i.imgur.com/hLdZ4JM.png)

## Ngôn ngữ của Vim
Có rất nhiều bạn than thở rằng không thể nhớ được các tổ hợp phím của Vim. Nguyên nhân của điều này nằm ở bạn đang học vẹt một ngôn ngữ (tổ hợp phím trong Vim) mà chả hiểu gì về ý nghĩa (Tiếng anh) của nó cả.

Vậy nên trước khi bắt đầu vào thực hành, hãy hiểu ý nghĩa ngôn ngữ vim nhé

### Động từ - Verb
| ĐỘNG TỪ | TIẾNG ANH  | Ý NGHĨA                                                           |
| ------- | ---------- | ----------------------------------------------------------------- |
| y       | Yank       | Nghĩa tương tự copy                                               |
| c       | Change/Cut | Thay đổi nội dung và cho phép chèn nội dung mới vào               |
| d       | Delete     | Xóa                                                               |
| p       | Paste      | Dán                                                               |
| f       | Find       | Tìm kiếm và di chuyển con trỏ ký tự được tìm thấy                 |
| t       | To         | Tìm kiếm và di chuyển con trỏ đến trước ký tự được tìm thấy       |
| i       | Insert     | Chèn vào trước vị trí con trỏ hiện tại. Di chuyển đến insert mode |
| a       | Append     | Chèn vào sau vị trí con trỏ hiện tại. Di chuyển đến insert mode   |


### Danh từ - Noun

| DANH TỪ | TIẾNG ANH        | Ý NGHĨA |
| ------- | ---------------- | ------- |
| w       | Word             | Từ      |
| s       | Sentence         | Câu     |
| p       | Paragraph        | Đoạn    |
| b       | Blog/parentheses | Bài     |
| t       | Tag              | Thẻ     |


### Trạng từ - Modifier 

| TRẠNG TỪ | TIẾNG ANH | Ý NGHĨA    |
| -------- | --------- | ---------- |
| a        | Around    | Xung quanh |
| i        | Inside    | Bên Trong  |

Để ý thì ở trên kia chúng ta cũng có i và a, nhưng với tư cách là động từ. Còn ở đây i, a lại có nghĩa khác là trạng từ

OK, vậy là tạm thời đã xong phần mở đầu, phần tiếp theo sẽ hướng dẫn các bạn làm thế nào để ghép các loại từ trên thành 1 câu (lệnh) trong ngôn ngữ vim nhé

## Tài liệu tham khảo
[Learn to speak vim — verbs, nouns, and modifiers!](http://yanpritzker.com/2011/12/16/learn-to-speak-vim-verbs-nouns-and-modifiers/)

