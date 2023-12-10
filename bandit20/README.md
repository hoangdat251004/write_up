# Bandit20 -> Bandit21

> There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

Như đề bài gợi ý thì ta cần connect tới 1 localhost và truyền vào đó là password của level hiện tại.

Ở đây có 1 file tượng tự như level trước nhưng ta cần kết nối để có thể execute file.

![f20](https://github.com/hoangdat251004/write_up/assets/110254118/9654f322-885a-47f4-a804-84c6b5d9c5c6)


Vì vậy ta cần tạo 1 localhost bất kì và gửi vào password, `-l` để `listen` lệnh mà ta truyền vào và `-p` là port mà ta chọn.

Sau đó ta thực thi file với port mà ta chọn khi nãy.

![f20 1](https://github.com/hoangdat251004/write_up/assets/110254118/77f46133-ed37-476b-8be3-9eb58177aa4b)

?**Password: NvEJF7oVjkddltPSrdKEFOllh9V1IBcq**
