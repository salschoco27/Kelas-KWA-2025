# Flag Command - Hack The Box
Website: [PicoCTF - Cookie Monster Secret Recipe](https://play.picoctf.org/)

## Description <br>
Cookie Monster has hidden his top-secret cookie recipe somewhere on his website. As an aspiring cookie detective, your mission is to uncover this delectable secret. Can you outsmart Cookie Monster and find the hidden recipe?
Additional details will be available after launching your challenge instance.


## Step-by-step 
1. Ketika install launch muncul page login sederhana. Saya sempat mencoba untuk login menggunakan payload sql namun gagal dan teringat dengan description yang diberikan yaitu **cookie**. ![alt text](image-9.png)
2. Ketika saya inspect dan cek pada networknya terdapat 'secret recipe' dengan karakter acak. ![alt text](image-10.png)
![alt text](image-11.png)
3. Lalu saya coba untuk decrypt  menggunakan base64 dan ternyata itu flagnya. ![alt text](image-12.png)