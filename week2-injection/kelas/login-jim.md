# Login Jim - OWASP Juice Shop
Website: [OWASP Juice Shop - Injection](https://demo.owasp-juice.shop/#/score-board?categories=Injection)

## Soal <br>
Log in with Jim's user account.

## Step-by-step 
1. Cari tempat untuk login, yaitu pada **Account** lalu **Login**. Namun karena kita tidak punya clue apapun untuk nama akun dari Jim, maka coba untuk mencari pada Review yang ada pada halaman All Products.
![alt text](image-1.png)
2. Dan ternyata ditemukan review dari email Jim yaitu ```jim@juice-sh.op```. Meskipun belum tentu itu Jim yang diminta namun kita coba login menggunakan email tersebut.
![alt text](image-3.png)
3. Login menggunakan email ```jim@juice-sh.op``` yang ditambahkan dengan ```'--``` untuk SQL attacknya.
![alt text](image-4.png)
4. Dan login sukses menggunakan akun tersebut!
![alt text](image-5.png)

## Coding Challenge
### Find It
![alt text](image-39.png)
### Fix It
![alt text](image-40.png)