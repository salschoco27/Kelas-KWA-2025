# NoSQL Manipulation - OWASP Juice Shop
Website: [OWASP Juice Shop - Injection](https://demo.owasp-juice.shop/#/score-board?categories=Injection)

## Description <br>
Update multiple product reviews at the same time.

## Step-by-step 
1. Coba untuk menuliskan review sebagai Admin pada prodyct random. ![alt text](image-27.png)
2. Setelah review disubmit ternyata kita bisa mengedit review tersebut.![alt text](image-28.png)
3. Dan ketika dicek menggunakan BurpSuite terdapat endpoint ```/rest/products/reviews dengan metode PATCH yang biasa digunakan untuk mengupdate. ![alt text](image-29.png)
4. Maka dari itu langsung saja saya Send to Repeater dan coba untuk mengupdate message nya menjadi **helloo**
```sql
{
    "id":{"$ne":-1},
    "message": "helloo"
}
```
![alt text](image-25.png)

5. Setelah dijalankan muncul semua reviews yang telah berhasil terupdate. ![alt text](image-26.png)

## Coding Challenge
### Find It
![alt text](image-30.png)
### Fix It
![alt text](image-31.png)

