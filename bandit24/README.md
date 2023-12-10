# Bandit24 -> Bandit25

Ở bài này ta cần truy cập vào localhost với port 30002 cùng với password hiện tại nhưng phải thực hiện brute-forcing để có thể đi qua 10000 pincode.

Ta tạo 1 bash file như sau.

Duyệt từng pincode từ 0000->9999, mỗi lần sẽ truyền vào password đồng thời kết nối tới localhost nếu đúng pincode thì ta sẽ có được password.

![f24 1](https://github.com/hoangdat251004/write_up/assets/110254118/ae57d55f-91c5-42f8-b0db-4ee4ad223ed0)


Ta sẽ cấp quyền cho file bash đó.

![f24 2](https://github.com/hoangdat251004/write_up/assets/110254118/23fdc727-b782-44c2-ab82-77cd7d07fe2b)

Sau khi chạy 1 vài giấy thì ta lấy được password.

![f24](https://github.com/hoangdat251004/write_up/assets/110254118/0de30ed1-b0d2-4ce2-8efb-2aac522305e3)
