# Bandit19 -> Bandit20

> To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

Sau khi connnect, ta dùng lệnh `ls -la` để kiểm tra tổng thể.

Ta thấy có file `bandit20-do` có thể thực hiện lệnh `execute`.

![Screenshot 2023-12-09 200341](https://github.com/hoangdat251004/write_up/assets/110254118/2b33f138-e6f4-45a9-8f19-8691c00738ea)

Ta thực thi file đó thì được hướng dẫn cách thực thi

![image](https://github.com/hoangdat251004/write_up/assets/110254118/987779b4-87cd-4b01-b05e-cf94700fb1f7)

Ta thực thi như hướng dẫn và được

![image](https://github.com/hoangdat251004/write_up/assets/110254118/27bcf6fb-90cb-44bc-b672-34b78f1b85ee)

Ta làm theo như gới ý của đề bài và lấy được password

![image](https://github.com/hoangdat251004/write_up/assets/110254118/a9c34b61-36b9-486f-be8e-434eaaec6bd6)

>**Password: VxCazJaVykI6W36BkBU0mJTCM8rR95XT**
