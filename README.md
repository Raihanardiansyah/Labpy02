# Labpy02

## Kasus 1: Program pemesanan tiket bioskop

### Programnya

inilah gambar dari program untuk pemesanan tiket bioskop:

![gambar1](https://github.com/Raihanardiansyah/Labpy02/blob/main/png/py1.png?raw=true)

Hasil dari progam tersebut

![gambar1](https://github.com/Raihanardiansyah/Labpy02/blob/main/png/Py2.png?raw=true)

### Penjelasan dari program tersebut:

Penjelasan Struktur Program:

1.	Input dari Pengguna:

    o Program pertama kali meminta pengguna memasukkan tipe tiket (reguler atau VIP) dan status member (ya atau tidak).
  	
    o input("Masukkan tipe tiket (reguler/vip): "): Pengguna diminta memasukkan tipe tiket, yang diubah menjadi huruf kecil dengan .lower() untuk menghindari kesalahan input karena penggunaan huruf besar/kecil.
  	
    o input("Apakah Anda member? (ya/tidak): "): Pengguna diminta memasukkan status member.

2.	Harga Tiket:

    o Dua variabel ditetapkan untuk harga tiket:
  	
	harga_reguler = Rp50.000

	harga_vip = Rp100.000

3.	Logika untuk Menentukan Harga Tiket:

    o Berdasarkan input dari pengguna, program akan menentukan harga tiket menggunakan blok if-else:
  	
python

Salin kode

if tipe_tiket == "reguler":

    harga_tiket = harga_reguler
    
elif tipe_tiket == "vip":

    harga_tiket = harga_vip
    
else:

    print("Tipe tiket tidak valid!")
    
    exit()

    
o Jika pengguna memilih "reguler", maka harga tiket akan ditetapkan sebagai Rp50.000. Jika memilih "VIP", harganya Rp100.000.
  
o Jika input yang dimasukkan tidak sesuai ("reguler" atau "vip"), program akan menampilkan pesan "Tipe tiket tidak valid!" dan menghentikan program dengan exit().

4.	Menghitung Diskon:

    o	Diskon hanya diberikan jika pengguna memiliki status member, yaitu 20% dari harga tiket.

    o	Untuk menentukan apakah pengguna mendapat diskon, digunakan operator ternary:
  	
python

Salin kode

diskon = 0.2 if member == "ya" else 0

o Jika status member "ya", diskon diatur menjadi 0.2 (20%), jika tidak, diskon diatur menjadi 0 (tidak ada diskon).

5.	Menghitung Total Harga:

o Total harga dihitung dengan mengurangi diskon dari harga tiket:
  	
python

Salin kode

total_harga = harga_tiket * (1 - diskon)

o Jika pengguna bukan member, diskon bernilai 0, sehingga total harga adalah harga tiket penuh. Jika pengguna adalah member, diskon 20% diterapkan.
    
6.	Output Total Harga:

o Setelah menghitung total harga, program menampilkan hasil dengan format:
  	
python

Salin kode

print(f"Total yang harus dibayar: Rp{total_harga}")

Contoh Jalannya Program:

•	Contoh 1:
    o	Input tipe tiket: reguler
    
    o	Input status member: tidak
    
    o	Harga tiket: Rp50.000 (karena tipe tiket reguler)
    
    o	Diskon: 0% (karena bukan member)
    
    o	Output: Total yang harus dibayar: Rp50.000
    
•	Contoh 2:

    o	Input tipe tiket: vip

    o	Input status member: ya

    o	Harga tiket: Rp100.000 (karena tipe tiket VIP)

    o	Diskon: 20% (karena status member)

    o	Output: Total yang harus dibayar: Rp80.000

### ini flowchart untuk program tersebut

![gambar1](?raw=true)

### dan ini penjelasannya

Berikut adalah penjelasan dari flowchart sistem pemesanan tiket bioskop yang menggambarkan alur logika program:

1. Mulai (Start):

- Flowchart dimulai dengan titik awal, yang menunjukkan bahwa program siap berjalan.

2. Input Tipe Tiket:

- Pengguna diminta untuk memasukkan tipe tiket yang diinginkan, apakah reguler atau VIP.

- Pada langkah ini, flowchart mengarah ke proses untuk mengecek apakah tipe tiket valid.

3. Pengecekan Validitas Tipe Tiket (Decision Point):

Di sini ada keputusan dengan dua cabang:

- Ya (Valid): Jika pengguna memasukkan tipe tiket yang benar (reguler atau VIP), alur akan berlanjut ke langkah berikutnya.

- Tidak (Tidak Valid): Jika tipe tiket tidak sesuai (misalnya pengguna memasukkan sesuatu selain "reguler" atau "VIP"), program akan menampilkan error dan berakhir (exit).

4. Input Status Member:

- Setelah tipe tiket diterima sebagai valid, pengguna diminta untuk memasukkan status apakah mereka memiliki kartu member atau tidak (ya atau tidak).

5. Pengecekan Status Member (Decision Point):

Di sini ada keputusan dengan dua cabang:

- Ya (Member): Jika pengguna adalah member, alur berlanjut ke perhitungan harga tiket dengan diskon.

- Tidak (Non-Member): Jika pengguna bukan member, alur berlanjut ke perhitungan harga tanpa diskon.

6. Menghitung Harga Tiket:

Setelah mengetahui tipe tiket dan status member, program akan menghitung harga tiket:

 - Harga Reguler: Jika pengguna memilih tiket reguler, harga ditetapkan Rp50.000.

 - Harga VIP: Jika pengguna memilih tiket VIP, harga ditetapkan Rp100.000.

7. Menghitung Diskon (Jika Member):

Jika pengguna adalah member, program akan menghitung diskon 20% dari harga tiket. Diskon ini hanya berlaku untuk pengguna yang memilih status member "ya".

8. Menghitung Total Harga:

Setelah diskon (jika ada) diterapkan, program menghitung total harga yang harus dibayar oleh pengguna.

9. Tampilkan Total Harga:

Program menampilkan total harga tiket yang harus dibayar oleh pengguna, baik dengan diskon (jika member) atau tanpa diskon (jika bukan member).

10. Selesai (End):

Flowchart berakhir di sini setelah total harga tiket ditampilkan kepada pengguna.

## Kasus 2: Program Kalkulator sederhana

### ini adalah program untuk Kasus ke 2 

![gambar1](https://github.com/Raihanardiansyah/Labpy02/blob/main/png/Pyno2.png?raw=true)

dan ini adalah hasil dari program tesebut

![gambar1](https://github.com/Raihanardiansyah/Labpy02/blob/main/png/pyno3.png?raw=true)

Berikut adalah penjelasan detail dari program kalkulator sederhana:

1. Input dari Pengguna:

Program pertama-tama meminta pengguna untuk memasukkan dua angka dan satu operator aritmatika.

Fungsi input() digunakan untuk mengambil data dari pengguna, dan angka tersebut diubah menjadi tipe float agar bisa melakukan operasi matematika:

- angka1 = float(input("Masukkan angka pertama: "))
  
- angka2 = float(input("Masukkan angka kedua: "))
  
- operator = input("Masukkan operator (+, -, *, /): ")

2. Pemilihan Operator (if-elif-else):

Setelah mendapatkan input operator, program menggunakan struktur if-elif-else untuk menentukan operasi aritmatika mana yang akan dilakukan.

If: Jika operator yang dimasukkan adalah +, maka operasi penjumlahan dilakukan:

if operator == "+":

    hasil = angka1 + angka2

Elif: Jika operator -, maka dilakukan pengurangan:

elif operator == "-":

    hasil = angka1 - angka2

Elif: Jika operator *, maka dilakukan perkalian:

elif operator == "*":

    hasil = angka1 * angka2

Elif: Jika operator /, dilakukan pembagian, tetapi dengan pengecekan tambahan apakah angka kedua adalah nol, karena pembagian dengan nol tidak diperbolehkan:

elif operator == "/":

    if angka2 != 0:
    
        hasil = angka1 / angka2
        
    else:
    
        hasil = "Kesalahan: Tidak bisa membagi dengan nol!"


3. Pengecekan Validitas Operator:

Jika pengguna memasukkan operator yang tidak valid (misalnya karakter selain +, -, *, /), program akan menampilkan pesan error:

else:

    hasil = "Operator tidak valid!"


4. Pembagian dengan Nol:

Dalam operasi pembagian, ada pengecekan apakah angka kedua (pembagi) adalah nol. Jika benar, program akan menampilkan pesan kesalahan karena pembagian dengan nol tidak diperbolehkan:

if angka2 != 0:

    hasil = angka1 / angka2
    
else:

    hasil = "Kesalahan: Tidak bisa membagi dengan nol!"

Pengecekan ini penting untuk mencegah kesalahan perhitungan dan menjaga integritas program.

5. Output Hasil:

Setelah operator dan operasi dipilih, program menghitung hasil dari operasi tersebut dan menampilkannya:

print("Hasil: ", hasil)

Jika operator tidak valid atau ada kesalahan lain, program juga akan menampilkan pesan yang sesuai.

6. Contoh Jalannya Program:

Contoh 1: Penjumlahan

Input:

Angka pertama: 5

Angka kedua: 3

Operator: +

Hasil: 5 + 3 = 8

Contoh 2: Pembagian dengan Nol

Input:

Angka pertama: 10

Angka kedua: 0

Operator: /

Hasil: Kesalahan: Tidak bisa membagi dengan nol!

Contoh 3: Operator Tidak Valid

Input:

Angka pertama: 8

Angka kedua

### Berikut Flowchart untuk Kasus 2

![gambar1](?raw=true)

Berikut adalah penjelasan dari flowchart untuk program kalkulator sederhana:

1. Mulai (Start):

Program dimulai pada titik awal, menunjukkan bahwa kalkulator siap untuk digunakan.

2. Input Angka Pertama:

Pengguna diminta untuk memasukkan angka pertama. Ini adalah salah satu dari dua angka yang akan digunakan dalam operasi aritmatika.

3. Input Angka Kedua:

Setelah memasukkan angka pertama, pengguna diminta untuk memasukkan angka kedua.

4. Input Operator:

Pengguna kemudian diminta memasukkan operator aritmatika. Operator ini bisa berupa salah satu dari empat pilihan berikut:

- untuk penjumlahan +

- untuk perkurangan -

- untuk perkalian *

- untuk pembagian /

5. Pengecekan Operator Valid atau Tidak (Decision Point):

Di titik ini, program memeriksa apakah operator yang dimasukkan valid (yaitu salah satu dari +, -, *, atau /).

- Jika operator valid, alur lanjut ke langkah selanjutnya untuk melakukan operasi.

- Jika tidak valid, program akan menampilkan pesan "Operator tidak valid" dan mengakhiri proses.

6. Pengecekan Pembagian dengan Nol (Decision Point):

- Jika pengguna memilih operator / (pembagian), program harus mengecek apakah angka kedua adalah nol.

- Jika angka kedua bukan nol, operasi pembagian akan dilakukan.

- Jika angka kedua adalah nol, program akan menampilkan pesan "Tidak bisa membagi dengan nol" dan menghentikan proses.

7. Operasi Aritmatika:

Program akan menjalankan operasi aritmatika sesuai dengan operator yang dimasukkan:

- Penjumlahan jika operator adalah +.

- Pengurangan jika operator adalah -.

- Perkalian jika operator adalah *.

- Pembagian jika operator adalah / dan angka kedua bukan nol.

8. Tampilkan Hasil:

Setelah operasi dilakukan, program akan menampilkan hasil dari perhitungan aritmatika.


9. Selesai (End):

Program berakhir setelah menampilkan hasil. Pengguna dapat menjalankan ulang program jika ingin melakukan perhitungan lain.

Kesimpulan Flowchart:

Flowchart ini menjelaskan alur dasar dari program kalkulator, mulai dari input angka dan operator, pengecekan validitas operator, pengecekan khusus untuk pembagian dengan nol, hingga penentuan operasi yang akan dilakukan. Alur ini menggunakan dua decision points (pengecekan kondisi) untuk memastikan input yang dimasukkan benar dan mencegah kesalahan dalam perhitungan.
