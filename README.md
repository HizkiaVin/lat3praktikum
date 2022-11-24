# Kondisional dan Perulangan
## **Struktur Kondisi**
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
\
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

## **Perulangan**
## Latihan 1
Buat program dengan perulangan bertingkat (nested) for yang
menghasilkan output sebagai berikut:

![darkmodelat3](https://user-images.githubusercontent.com/116176746/202855701-3d0c3631-a022-4f51-84c3-b4556fa11e9a.png)


Code:

```python
start = 0;
finish = 10;

for i in list(range(10)):
    for j in range(start,finish):
            print(j, end=' ')
            if j < 10:
                print('{0:>2}' .format(""), end="")
            else :
                print('{0:>1}' .format(""), end="")
    start+=1
    finish+=1
    print("")
```
Maka output yang akan ditampilkan:

![outputnested](https://user-images.githubusercontent.com/116176746/202856480-0d336411-6612-4d85-a5ac-4ba0413ecfc8.png)

>Perulangan bersarang atau perulangan bertingkat adalah sebuah perulangan yang berada atau terletak di dalam perulangan yang lain.

## Latihan 2
Program Menampilkan N Bilangan Acak Yang Lebih Kecil Dari 0.5
\
Code:
```python   
import random

jumlah= int(input("Masukkan nilai N :"))
j = 0
for i in range(jumlah):
    i = random.uniform(0.0,0.5)
    j+= 1
    print("Masukkan data ke",j, '==>',i)

jawab ="benar"
hitung = 0
while jawab == "benar":
    hitung += 1
    jawab =input("SELESAI")
```
> sebelum memasukkan kode, kita harus mengimport fungsi random terlebih dahulu.

Maka outputnya akan seperti ini: 
![output latihan1](https://user-images.githubusercontent.com/116176746/200994857-5e393f83-642d-4b55-9079-56d33747f5aa.png)

>**_for_** disebut juga sebagai counted loop (perulangan yang terhitung), yaitu
perintah yang dieksekusi secara berulang berdasarkan jumlah perulangan tertentu.
\
\
*__while__* disebut uncounted loop (perulangan yang tak terhitung), yaitu perulangan
yang dilakukan berdasarkan kondisi tertentu selama nilai kondisi bernilai TRUE.

## **Modul Praktikum 2**
## Latihan 1 : Membuat program menentukan nilai akhir

Code:
```python
nama = input("Masukkan nama:")
uts = input("Masukkan nilai UTS:")
uas = input("Masukkan nilai UAS:")
tugas = input("Masukkan nilai Tugas:")
akhir = (int(tugas) * .2) + (int(uts) * .4) + (int(uas) * .4)
keterangan = ("TIDAK LULUS", "LULUS")[akhir > 60.0]
if akhir > 80:
    huruf = "A"
elif akhir > 70:
    huruf = "B"
elif akhir > 50:
    huruf = "C"
elif akhir > 40:
    huruf = "D"
else:
    huruf = "E"
print("\nNama :",nama)
print("Nilai UTS :",uts)
print("Nilai UAS :",uas)
print("Nilai Tugas :",tugas)
print("Nilai Akhir :",akhir)
print("\nNilai Huruf :",huruf)
print("Keterangan :",keterangan)
```

Maka output yang ditampilkan:

![modul2latihan1](image/modul2latihan1.png)

.....