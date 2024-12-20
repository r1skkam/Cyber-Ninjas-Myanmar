# CHALLENGE DESCRIPTION
&quot;I told them it was too soon and in the wrong season to deploy such a website, but they assured me that theming it properly would be enough to stop the ghosts from haunting us. I was wrong.&quot; Now there is an internal breach in the `Spooky Network` and you need to find out what happened. Analyze the the network traffic and find how the scary ghosts got in and what they did.

If check http.request, we can see bash exec

![image](https://github.com/user-attachments/assets/5c295057-3e07-4257-b858-97be80eed749)

So need to search bash connection...

I found many [ PSH , ACK ] flags. 

![image](https://github.com/user-attachments/assets/b23b318f-b385-4ad5-80b2-27653726280a)

Check TCP or HTTP stream of them

![image](https://github.com/user-attachments/assets/11ab7c77-8811-4bfb-8c2c-35210f82761a)
![image](https://github.com/user-attachments/assets/ca9bdd42-f2b0-44b9-81e8-2814607bb232)

Found a base64 reverse string 

![image](https://github.com/user-attachments/assets/4e7862dc-0d6b-4ed9-a9a9-8b5c80bb6e88)

I put it in linux, reverse it and decode base64
![image](https://github.com/user-attachments/assets/30957e25-07a4-484f-9830-a8a69b455951)

Got flag!!

# Flag

HTB{j4v4_5pr1ng_just_b3c4m3_j4v4_sp00ky!!}

