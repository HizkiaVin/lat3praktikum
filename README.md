# Kondisional dan Perulangan
## Latihan 1
Buat program sederhana dengan input 2 buah bilangan, kemudian tentukan bilangan terbesar dari kedua bilangan tersebut menggunakan statement if.
Code:
```python
print("Menentukan Nilai Terbesar dari 2 Bilangan")
a=input("Masukkan Nilai:")
b=input("Masukkan Nilai:")
if a>b :
    print("Bilangan Terbesar : "+a)
elif a<b :
    print("Bilangan Terkec  il : "+b)
else :
    print("Nilai Sama")
```
Maka outputnya adalah: 
![if latihan 1 1](https://user-images.githubusercontent.com/116176746/202186022-54542051-649b-4ec1-a56c-73c1d015a1f5.png)

>*if* merupakan kondisi utama, sedangkan *elif* adalah kondisi kedua atau ketiga hingga ke-x, sedangkan *else* adalah kondisi terakhir di mana semua kondisi sebelumnya tidak ada yang terpenuhi.

## Latihan 2
Buat program untuk mengurutkan data berdasarkan input sejumlah data (minimal 3 variable input atau lebih), kemudian tampilkan
hasilnya secara berurutan mulai dari data terkecil.

Code
```python
print("Program Mengurutukan Data")
bil1 = int(input("Bilangan ke-1: "))
bil2 = int(input("Bilangan ke-2: "))
bil3 = int(input("Bilangan ke-3: "))

#Buat variable data
data = [bil1, bil2, bil3]

#Menampilkan data
list.sort(data)
print("Urutan bilangan:", data)
```


Maka output yang akan ditampilkan:
![sort 1](https://user-images.githubusercontent.com/116176746/202194829-bee29cb8-9e53-4fe8-a11c-d934e505b068.png)
> `list.sort` berfungsi untuk mengurutkan data. 