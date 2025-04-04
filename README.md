# Simple cookie hijacking
This simple project aims to shocase how cookie hijacking can happen.
## Instructions:
- change the server port to an available port on your machine;
- start spring boot;
- upon requesting the main page (localhost:8080/biscotti/dammi-cookie), your client will store a cookie "lang":"ENG";
![image](https://github.com/user-attachments/assets/86460fb8-7e48-46a8-a853-fc3fbc1dec00)
- visit the biscotti/saluta endpoint, that will greet you in English;
![image](https://github.com/user-attachments/assets/de414e21-cc66-4747-81f9-674e9399c15a)
- change tha cookie's value field to "ITA";
- the /saluta endpoint will then greet you in Italian as the fake cookie, that was included in your new request, tells the server your chosen language is Italian.
![image](https://github.com/user-attachments/assets/15b378d8-5639-4bed-9722-2d646d2863eb)
