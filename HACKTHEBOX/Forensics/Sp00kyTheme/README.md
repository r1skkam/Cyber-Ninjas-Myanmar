# CHALLENGE DESCRIPTION
I downloaded a very nice haloween global theme for my Plasma installation and a couple of widgets! It was supposed to keep the bad spirits away while I was improving my ricing skills... Howerver, now strange things are happening and I can't figure out why...

Vitim downloaded some themes and wedget 

![image](https://github.com/user-attachments/assets/0d70e944-a37f-435e-abf2-7783d16a23bf)

Search each folder one by one and found code folder 

![image](https://github.com/user-attachments/assets/8f14cc55-d287-43af-92d2-772137320a44)

![image](https://github.com/user-attachments/assets/9d251299-521b-49ca-9d57-ca7fe79916ee)

Open utils.js with notepad and found strange command in js file 

![image](https://github.com/user-attachments/assets/d4e79e44-39b4-4264-a37d-41511a1c9cc8)

echo 952MwBHNo9lb0M2X0FzX/Eycz02MoR3X5J2XkNjb3B3eCRFS | rev | base64 -d

Command is reversing the string and decode with base64. So I put this command in kali.

![image](https://github.com/user-attachments/assets/ec744afd-98b2-4a3d-aeb0-3c93b7957cac)

Got Flag!!!

# Flag
HTB{pwn3d_by_th3m3s!?_1t_c4n_h4pp3n}

