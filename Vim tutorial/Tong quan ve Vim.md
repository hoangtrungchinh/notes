# TỔNG QUAN VỀ VIM


## VIM LÀ GÌ?


## TẠI SAO SỬ DỤNG VIM
1. Nhanh: người dùng chỉ cần bàn phím, không cần chuột để thao tác
2. Tiện: Làm việc trên mọi môi trường, đặc biệt là Server
3. Rộng: Khả năng rộng mở cao qua các plugin, có khả năng tùy chỉnh theo ý mình

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

![vim mode](https://i.imgur.com/hLdZ4JM.png)

1. **Normal Mode**: - Được sử dụng để chỉnh sửa, sao chép, dán, di chuyển, xóa và thay đổi văn bản được thực hiện từ trong chế độ này.

2. **Insert Mode**: - Được sử dụng để update hay thay đổi data,text...

3. **Command mode**: - Chế độ này được sử dụng để lưu tài liệu, thoát khỏi chương trình, thực hiện tìm kiếm....

4. **Visual Mode (bôi đen)**: - Được sử dụng để lựa chọn hình ảnh


