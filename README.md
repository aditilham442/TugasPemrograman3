Pada latihan 1 kita akan mencari bilangan acak yang lebih kecil dari 0.5.
Syntaxnya:

r = int(input("Masukkan Nilai N:"))

jumlah = r+1
start = 1
stop = jumlah
for i in range(start, stop):
from random import random
a = random()
print("Data ke", i, "=>", a)
print("Selesai")

Penjelasan Algoritma

Pertama kita membuat perintah untuk memasukkan nilai n.

r = int(input("Masukkan Nilai N:"))

Lalu kita membuat variable untuk menentukan berapa jumlah data yang akan kita cari.

jumlah = r+1
start = 1
stop = jumlah

"start = 1" berarti data dimulai dari 1. "jumlah = r+1 dan stop = jumlah" berarti looping akan berhenti ketika variable 'jumlah' sudah sesuai dengan nilai yang diinput pada variable 'r'.

Lalu kita membuat syntax looping for.

for i in range(start, stop):

Looping akan terus berjalan sampai jumlah yang telah ditentukan untuk berhenti.

Setelah itu kita memasukkan fungsi untuk menampilkan nilai secara acak.

from random import random
a = random()

Terakhir kita tinggal membuat syntax untuk mengeluarkan hasil dari looping tersebut.

print("Data ke", i, "=>", a)
print("Selesai")

'i' adalah hasil dari jumlah perulangan yang telah dilakukan. Dan 'a' akan menampilkan nilai secara acak karena fungsi random yang telah diinput.
Screenshot Input & Output

Latihan1p3
Latihan 2

Latihan 2 akan menampilkan bilangan terbesar dari n buah data yang diinputkan.
Syntaxnya:

a = int()
b = 0

while a >= 0:
a = int(input("Masukkan Bilangan: "))
if a == 0:
break
if a > b:
b = a
print("Bilangan terbesar adalah :", b)
print("Selesai")

Penjelasan Algoritma

Pertama kita membuat 2 variable.

a = int()
b = 0

Variable 'a' sebagai integer yg belum diinput nilainya, dan variable 'b' bernilai 0.

Lalu kita membuat looping while.

while a >= 0:
a = int(input("Masukkan Bilangan: "))

Disini kita akan diminta untuk menginput angka pada variable 'a'. Dan apabila nilai 'a' lebih besar dari 0, maka akan terjadi perulangan.

Membuat statement untuk berhenti dari perulangan.

if a == 0:
break

Pada tahap ini apabila kita menginput nilai 0 pada variable 'a' yang diminta sebelumnya, maka kita akan berhenti dari perulangan.

Membuat statement untuk mengambil angka terbesar.

if a > b:
b = a

Disini system akan mengambil nilai 'a' terbesar untuk variable 'b'.

Menampilkan outputnya

print("Bilangan terbesar adalah :", b)
print("Selesai")

Disini kita akan menampilkan output bilangan terbesar dari angka - angka yang telah diinputkan.
Screenshot Input & Output

Latihan2p3
Program1

Pada program ini kita akan mencari keuntungan pada usaha yang telah berjalan selama 8 bulan dengan kondisi yang telah ditentukan.
Syntaxnya

modal = 100000000
laba = 0
untung = 0

for i in range(1, 9):
if i < 3:
laba = 0
untung = untung + laba
elif i < 5:
laba = modal*1/100
untung = untung + laba
elif i < 8:
laba = modal*5/100
untung = untung + laba
else:
laba = modal*3/100
untung = untung + laba
print("Laba bulan ke", i, "sebesar:", laba)
print("Total laba adalah:", untung)

Penjelasan Algoritma

Membuat variablenya. contoh:

modal = 100000000
laba = 0
untung = 0

Disini variable modal yaitu 100000000 dan variable laba dan untung adalah 0.

Lalu membuat looping for.

for i in range(1, 9):

Disini perulangan akan dimulai dari nilai 1 dan akan berhenti pada nilai akhir, yaitu 9.

Membuat kondisi pertama.

if i < 3:
laba = 0
untung = untung + laba

Disini apabila nilai 'i' kurang dari 3 maka labanya adalah 0. Artinya apabila belum bulan ke 3, maka labanya adalah 0. Untung digunakan untuk nanti menghitung total keuntungan yang didapat.

Membuat kondisi kedua.

elif i < 5:
laba = modal*1/100
untung = untung + laba

Kondisi ini adalah pada bulan ke 3 - 4, maka akan mendapatkan laba sebesar 1% atau laba = modal dikali 1 dibagi 100.

Membuat kondisi ketiga.

elif i < 8:
laba = modal*5/100
untung = untung + laba

Kondisi ini apabila belum memasuki bulan ke 8, maka akan mendapatkan laba sebesar 5%.

Membuat kondisi terakhir.

else:
laba = modal*3/100
untung = untung + laba

Ini adalah kondisi pada bulan ke 8. Laba menurun 2%, sehingga laba bulan ke 8 menjadi sebesar 3%.

Mencetak laba perbulan dan total laba selama 8 bulan.

print("Laba bulan ke", i, "sebesar:", laba)

Syntax diatas akan menampilkan hasil laba setiap bulan.

print("Total laba adalah:", untung)

Dan ini akan menampilkan total laba selama 8 bulan.
Screenshot Input & Output
