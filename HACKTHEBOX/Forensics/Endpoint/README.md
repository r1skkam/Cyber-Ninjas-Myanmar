# CHALLENGE DESCRIPTION
E Corp's sinister control over society through the chemical compound "EverLast" must be stopped. Analyze the provided network traffic capture file to uncover critical information hidden within the malicious payload. Your task is to extract the key details, including a callback endpoint used in various missions to disseminate EverLast, to help the resistance dismantle the corporation's grip on the world.

I found MySQL login and Request Query 
![image](https://github.com/user-attachments/assets/546895ee-0827-4f04-89ef-0c4dd885003f)

Export to csv file and collect all value 

![image](https://github.com/user-attachments/assets/2c119979-ec91-486e-ae96-3f648894359e)
![image](https://github.com/user-attachments/assets/f200ae15-12c3-4b5e-ad31-45a71590a48a)

I change all value to Base64 and export file as output.bin

![image](https://github.com/user-attachments/assets/ef83e3e2-f768-4374-aa4b-d3da6c573c7e)

And I check strings of output.bin file

![image](https://github.com/user-attachments/assets/7463b467-0e31-4663-8d43-43235e1b710b)

Found a Base64 of callback function 

![image](https://github.com/user-attachments/assets/3e870d85-f7d9-41ed-9128-181dc9031924)

Change Base64 in Cyberchef 

![image](https://github.com/user-attachments/assets/939477b3-a0cb-49aa-a142-086dbdc59a80)

Got flag!!

# Flag
HTB{chunk5_4nd_udf_f0r_br34kf457}


