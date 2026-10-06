# Pertemuan 06 Nested Loop Python

Algoritma dan Pemrograman | Pertemuan 06 | 12
Nama: Zakiyatus Salsabila
NIM: 2225250225
Kelas: 3F

## Tujuan
Menggunakan nested loop, pola, akumulasi, dan pencacahan.

## Cara Menjalankan
python3 tugas/tabel_perkalian_dan_statistik.py

## Algoritma Tugas 3
1. Membaca nilai n dan melakukan validasi menggunakan while.
2. Jika n kurang dari atau sama dengan 0, pengguna diminta memasukkan nilai n kembali sampai valid.
3. Mengatur total_semua = 0 dan count_genap = 0.
4. Menggunakan loop luar dari 1 sampai n.
5. Mengatur total_baris = 0 pada setiap awal baris.
6. Menggunakan loop dalam dari 1 sampai n.
7. Menghitung hasil perkalian dengan rumus hasil = i * j.
8. Menambahkan hasil perkalian ke total_baris dan total_semua.
9. Jika hasil perkalian merupakan bilangan genap, count_genap ditambah 1.
10. Setelah loop dalam selesai, menampilkan total_baris.
11. Setelah kedua loop selesai, menampilkan total keseluruhan dan banyak hasil genap.

## Hasil Pengujian
| Test Case | Input n | Jumlah Pasangan | Total Semua | Banyak Hasil Genap | Status |
|---|---:|---:|---:|---:|---|
| 1 | 1 | 1 | 1 | 0 | Berhasil |
| 2 | 2 | 4 | 9 | 3 | Berhasil |
| 3 | 3 | 9 | 36 | 5 | Berhasil |

### Test Case 1

Input:
n = 1

Tabel perkalian:
1 × 1 = 1

Total semua:
1

Banyak hasil genap:
0

Status: Berhasil

### Test Case 2

Input:
n = 2

Tabel perkalian:
1 × 1 = 1
1 × 2 = 2
2 × 1 = 2
2 × 2 = 4

Total semua:
9

Banyak hasil genap:
3

Status: Berhasil

### Test Case 3

Input:
n = 3

Tabel perkalian:
1 × 1 = 1
1 × 2 = 2
1 × 3 = 3
2 × 1 = 2
2 × 2 = 4
2 × 3 = 6
3 × 1 = 3
3 × 2 = 6
3 × 3 = 9

Total semua:
36

Banyak hasil genap:
5

Status: Berhasil

## Analisis Efisiensi
Loop luar berjalan sebanyak n kali dan setiap loop luar menjalankan loop dalam sebanyak n kali. Jadi, jumlah operasi perkalian yang dilakukan adalah n × n atau n² kali.

Semakin besar nilai n, semakin banyak operasi yang dilakukan oleh program. Contohnya, jika n = 3 maka terdapat 9 pasangan perkalian. Jika n = 10 maka terdapat 100 pasangan perkalian.

Dengan demikian, waktu yang dibutuhkan program bertambah seiring dengan bertambahnya nilai n karena menggunakan nested loop. Kompleksitas waktu program adalah O(n²).

## Refleksi
Pada tugas ini saya belajar menggunakan nested loop atau perulangan bersarang. Nested loop digunakan karena program perlu membuat tabel perkalian dalam bentuk baris dan kolom. Loop luar digunakan untuk menentukan baris, sedangkan loop dalam digunakan untuk menentukan nilai pada setiap kolom.

Saya juga memahami bahwa total_baris perlu diatur menjadi 0 di setiap awal loop luar. Hal ini dilakukan agar jumlah pada setiap baris dihitung dari awal dan tidak tercampur dengan jumlah baris sebelumnya.

Variabel total_semua digunakan untuk menyimpan jumlah seluruh hasil perkalian dari tabel. Berbeda dengan total_baris, total_semua tidak boleh direset pada setiap baris karena harus menyimpan hasil akumulasi dari seluruh proses perkalian.

Untuk menghitung banyak hasil genap, program menggunakan count_genap. Nilai count_genap hanya ditambah ketika hasil perkalian habis dibagi 2. Dengan cara tersebut, program dapat menghitung jumlah hasil perkalian yang genap dengan benar.

Kesalahan yang dapat terjadi pada nested loop adalah salah menentukan batas loop atau salah menempatkan proses penjumlahan. Jika total_baris tidak direset pada awal loop luar, maka hasil setiap baris akan ikut menjumlahkan baris sebelumnya. Kesalahan lain adalah menambahkan count_genap tanpa melakukan pengecekan apakah hasilnya benar-benar genap.

Dari tugas ini saya menjadi lebih memahami cara kerja nested loop, akumulasi, dan pencacahan. Saya juga belajar bahwa posisi suatu variabel di dalam atau di luar loop sangat berpengaruh terhadap hasil akhir program.

Selain itu, saya memahami bahwa semakin besar nilai n, semakin banyak proses yang dilakukan karena loop dalam dijalankan sebanyak n kali untuk setiap perulangan pada loop luar. Oleh karena itu, program dengan nested loop memiliki kompleksitas waktu O(n²).
