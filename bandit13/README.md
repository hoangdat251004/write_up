# Bandit13 -> Bandit14

> The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Note: localhost is a hostname that refers to the machine you are working on

Truy cập vào bandit13 ta thấy có 1 file sshkey.private có liên quan tới gợi ý của bài.

![f13](https://github.com/hoangdat251004/write_up/assets/110254118/16cf0ff3-11cc-4934-a40a-b598999c1188)

Sau khi tìm hiểu cách truy cập bằng SSH key ta có cách dưới đây

![image](https://github.com/hoangdat251004/write_up/assets/110254118/5249f84a-0943-430b-8549-d9468308655b)

Password luu ở `/etc/bandit_pass/bandit14` nên ta dùng lệnh cat để đọc

![image](https://github.com/hoangdat251004/write_up/assets/110254118/95cc6439-8094-4e26-ab60-1911ab2d6ffd)

> **Password: fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq**
