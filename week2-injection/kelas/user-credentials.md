# User Credentials - OWASP Juice Shop
Website: [OWASP Juice Shop - Injection](https://demo.owasp-juice.shop/#/score-board?categories=Injection)

## Soal <br>
Retrieve a list of all user credentials via SQL Injection.

## Step-by-step 
1. Menggunakan metode yang kurang lebih sama dengan challenge Database Schema namun mengganti query nya dengan ``` apple ')) UNION SELECT 1,2,3,4,5,6,7,8,9 FROM users--``` agar bisa menampilkan kolom yang ada pada tabel users. ![alt text](image-18.png)
2. Lalu ganti kolom 1 dengan **id** dan 2 dengan **name** agar bisa menampilkan nama user. Namun ternyata menampilkan error message yang menunjukkan bahwa kolom name tidak ada.
```')) UNION SELECT id,name,email,4,5,6,7,8,9 FROM users--```  ![alt text](image-20.png)
3. Ketika coba menggantu kolom kedua dengan **email** maka muncul list email dari user yang terdaftar.![alt text](image-19.png)
4. Lalu saya mencoba lagi dengan mengganti kolom keempat dengan **password** dan muncul password yang ter encrypt pada  **description**  ![alt text](image-21.png)

## Coding Challenge
### Find It
![alt text](image-22.png)
### Fix It
![alt text](image-23.png)
