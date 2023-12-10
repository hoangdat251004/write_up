# Bandit22 -> Bandit23

Như bài trước ta lại `cd` tới thư mục đề cho và thực thi file có tên `cronjob_bandit23`, rồi lại thực thi thêm 1 lần nữa

![f2211](https://github.com/hoangdat251004/write_up/assets/110254118/a40a4dc3-9f57-43c5-b6aa-be4741520d19)

Ta thấy có 1 đoạn scrip hiện ra chứ không phải password.

![image](https://github.com/hoangdat251004/write_up/assets/110254118/d5a1f765-bc9d-4a31-a117-19a85f4ceb2b)

Nhìn kỹ 2 dòng lệnh này thì ta thấy `$myname` được gán là `$(whoami)` ở bandit22 hiện tại mà ta cần password cho bandit 23 nên ta sửa bằng cách thực thi câu lệnh bên dưới với `$myname` được thay bằng `bandit23`.

![image](https://github.com/hoangdat251004/write_up/assets/110254118/92910f84-8005-47e8-b0b7-7bf0dead7efc)

Thực thi dòng lệnh đó thì ta nhận dược 1 file, sau đó ta đọc file đó theo như hướng dẫn trong đọc script trên thì ta có password.

> **Password: QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G**
