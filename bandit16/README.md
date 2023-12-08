# Bandit16 -> Bandit17

Sau khi kết nối ta dùng lệnh `nmap` với tham sô `-p`, `31000-32000` để kiểm tra các port khả dụng

![f16](https://github.com/hoangdat251004/write_up/assets/110254118/23b9030d-eb88-4a34-aea5-a3f7a519d73a)

Sau vài lần thử kết nối thì chỉ có port `31790` là khả dụng, ta có thể tìm được RSA key tại đây.

![f16 1](https://github.com/hoangdat251004/write_up/assets/110254118/29369b3c-e9a1-4b4f-96dc-f19d8717a003)

Tạo 1 thư mục rồi tạo 1 file tại đó, tạo 1 file rồi patse RSA key vào.

![f16 2](https://github.com/hoangdat251004/write_up/assets/110254118/78572038-7f6c-490f-81de-04824b142964)

Sử dụng kiến thức từ bandit13->bandit14 ta áp dụng

![f16 3](https://github.com/hoangdat251004/write_up/assets/110254118/ba3030a5-7511-47e2-bec2-23bcea715cc8)

Nhưng để ý thì thấy không thể kết nối với lỗi `bad permission` nên ta chỉnh sửa quyền truy cập 1 chút, ta thêm quyền đọc, ghi cho file chứa key rồi kết  nối lại.

![f16 4](https://github.com/hoangdat251004/write_up/assets/110254118/5a9547ac-af9e-4517-aab8-52bfa13d8150)

Sau khi kết nối lại thành công ta dùng lệnh `cat /etc/bandit_pass/bandit17` tương tự ở level trước đó thì sẽ nhận được password.

![f16 5](https://github.com/hoangdat251004/write_up/assets/110254118/4d9ec841-e16e-43fb-965f-aaa18fe6ef18)


> **Password: VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e**
