# Bandit12 -> Bandit13

> The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

Trước tiên theo đề bài ta tạo ra 1 thư mục mới và copy file vào rồi giải nén file hexdump và lưu ở file `res` với câu lệnh `xxd -r data.txt > res` 

![f12](https://github.com/hoangdat251004/write_up/assets/110254118/172da6f1-4e0f-4a3a-8fa7-37886044b8e1)

Kiểm tra file `res` thấy đay là file `gzip` ta đổi tên file và giải nén nó

![f12 1](https://github.com/hoangdat251004/write_up/assets/110254118/34dc8081-9f45-49ee-9342-afe4e84966a4)

Giải nén ra 1 file `gzip` lại tiếp tục giải nén tương tự trên

![f12 2](https://github.com/hoangdat251004/write_up/assets/110254118/3e4d2fe1-ab31-4851-9ced-45bb98ed917d)

Giải nén ra file `tar`, giải nén bằng cách đổi tên và dùng câu lệnh `tar -xf res.tar`

![f12 3](https://github.com/hoangdat251004/write_up/assets/110254118/1cfab17a-4fa2-44e0-b5ac-c773f87b1781)

Tiếp tục dùng các lệnh để kiểm tra loại file và tiếp tục giải nén ta lấy được password

![f12 4](https://github.com/hoangdat251004/write_up/assets/110254118/26f8cd70-949d-412e-80f7-05a0effc468e)

> **Password: wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw**
