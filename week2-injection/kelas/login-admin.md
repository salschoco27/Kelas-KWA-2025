# Login Admin - OWASP Juice Shop
Website: [OWASP Juice Shop - Injection](https://demo.owasp-juice.shop/#/score-board?categories=Injection)

## Description <br>
Log in with the administrator's user account.

## Step-by-step 
1. Cari tempat untuk login, yaitu pada **Account** lalu **Login**.
![alt text](image-1.png)
2. Terdapat Login Page, mulai dengan mencoba SQL Injection yaitu ```'OR true--'``` dan isi passwordnya dengan apa saja lalu coba login.
![alt text](image-2.png)
3. Berhasil login sebagai Admin seperti yang diminta.
![alt text](image.png)

## Coding Challenge
### Find It
![alt text](image-9.png)

### Fix It
![alt text](image-10.png)