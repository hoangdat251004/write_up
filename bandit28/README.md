# Bandit28 -> Bandit29

Như ở level trước ta cũng tạo 1 thư mục rồi dùng `git clone` vào thư mục đó.

Sau khi vào trong thư mục `repo` và đọc file `README.md` ta thấy có password của bandit29 nhưng có vẻ nó đã bị thay đổi.

![f28](https://github.com/hoangdat251004/write_up/assets/110254118/4814a9ca-9e5e-4cc6-a811-548957e41ef5)

Để xem được lịch sử chỉnh sửa ta dùng lệnh `git log`.

![image](https://github.com/hoangdat251004/write_up/assets/110254118/fa54f824-8ae2-4948-aa5f-34a44aa67d4c)
![f28 2](https://github.com/hoangdat251004/write_up/assets/110254118/3ca559fa-f2bb-4912-b62c-a98e26b3167f)

Ta thấy có 3 commit, thứ tự mới nhất từ dưới lên.

Để xem chi tiết lịch sử ta dùng lệnh `git show [commitcode]`.

![image](https://github.com/hoangdat251004/write_up/assets/110254118/4851d880-bcc1-4315-aecd-7fcb7df92078)
![image](https://github.com/hoangdat251004/write_up/assets/110254118/b7e8d1ca-a44f-4715-a8f3-4829c301b3e3)

Ta đã thấy được password trước khi bị sửa.

>**Password: tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S**
