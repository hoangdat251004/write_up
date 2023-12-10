# Bandit25 -> Bandit26

Ở level này sau khi đăng nhập ta có 1 file `sshkey`, dùng nó để đăng nhập vào bandit 26 thì ta bị kick ra ngay lập tức

Dùng lệnh `cat /etc/passwd` thì t có thể thấy bandit26 shell là `/usr/bin/showtext` chứ không phải là `/bin/bash`.

Dùng lệnh `cat /usr/bin/showtext` thì ta thấy có lệnh `more` và 1 lệnh `exit 0`, 1 lệnh này hiển thị lên màn hình 1 đoạn text rồi sau đó kick ta ra khỏi bandit26.

Do đó để có thể không bị kick ta cần thay đổi shell của nó.

Sau khi tìm hiểu lệnh `more` ta thấy nó dùng để hiển thị 1 đoạn text và ta có thể thực thi 1 số lệnh ngay lúc đó.

Đây là đoạn text mà nó hiển thị.

![image](https://github.com/hoangdat251004/write_up/assets/110254118/b1fd6630-ac08-4097-8f93-f5cf9fdaef86)


Do khi ta mở terminal khá to thì đoạn text sẽ được hiển thị toàn bộ ngay lập tức và thoát khỏi luôn.

Do đó ta sẽ lách bằng thu nhỏ cửa sổ terminal lại gần nhất có thể rồi connect lại bandit26 như ban đầu.

Và đây là kết quả.

![Screenshot 2023-12-10 224753](https://github.com/hoangdat251004/write_up/assets/110254118/fe57db9a-b80c-4eae-b25c-0e0f1159d7c3)

Đến đây ta có thể truy cập `vim` bằng cách nhấn phím `v` để sửa shell.

Tra google thì ta có thể sửa shell bằng lệnh `:set shell=/bin/bash`

Sau đó ta dùng lệnh `:shell` để truy cập vào shell của bandit26.

Như vậy ta đã chính thức login vào bandit26.

Khi này ta có thể dùng lệnh `cat /etc/bandit_pass/bandit26` để lấy password 

![Screenshot 2023-12-10 225641](https://github.com/hoangdat251004/write_up/assets/110254118/78f328d9-d1d5-4b96-a811-27529b4ade06)

> *Password: c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1 **
