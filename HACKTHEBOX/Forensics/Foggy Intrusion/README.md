# CHALLENGE DESCRIPTION
On a fog-covered Halloween night, a secure site experienced unauthorized access under the veil of darkness. With the world outside wrapped in silence, an intruder bypassed security protocols and manipulated sensitive areas, leaving behind traceable yet perplexing clues in the logs.

When I check http request, I see GET request and POST

![image](https://github.com/user-attachments/assets/ef9fe6c6-cf99-4478-a5a4-aa0e8978c749)

When I check http response, I see all requests are failed 

![image](https://github.com/user-attachments/assets/72b51191-e53b-4c8d-8ef5-16255cefc53a)

So, I consider no need to analysis GET request but need to check POST.
Check POST request frame with TCP follow, I found some obfuscate command execution 

![image](https://github.com/user-attachments/assets/ea13ce73-b7bd-4db1-8bd7-e401d7fa9827)

Check in Cyberchef for she_exec

![image](https://github.com/user-attachments/assets/46035bd9-2fa0-4713-8955-fd7faa647052)

It is execute powershell and get-content of conf.php and output is as per below

![image](https://github.com/user-attachments/assets/d2eec78f-c5bb-446c-9515-13a45ef0ea43)

Decode with Base64 

![image](https://github.com/user-attachments/assets/aa9e9745-c2dc-4983-a371-3d87c02545a5)

Result is compressed RAW, So it is need do inflate with "Raw Inflate" 

![image](https://github.com/user-attachments/assets/9c04fe8e-bc8a-476a-adcb-c7449dddc720)

Got Flag!!

# Flag

HTB{f06_d154pp34r3d_4nd_fl46_w4s_f0und!}

