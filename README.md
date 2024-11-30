# Praktikum_6

### Program bagian pertama

![Gambar1](https://github.com/Raihanardiansyah/Praktikum_6/blob/main/ss/1.png?raw=true)

### berikut penjelasannya

Program tersebut adalah sebuah fungsi Python bernama tambah() yang digunakan untuk menambahkan data mahasiswa ke dalam sebuah daftar (data_mahasiswa). Berikut adalah penjelasan singkatnya:

### 1.Inisialisasi:

-data_mahasiswa adalah list kosong yang akan digunakan untuk menyimpan data mahasiswa berupa dictionary.

### 2. Fungsi tambah():

-Menampilkan garis pemisah dengan karakter "-" sebanyak 42 kali.

-Meminta pengguna memasukkan nama mahasiswa (nama) melalui fungsi input().

-Meminta pengguna memasukkan nilai mahasiswa (nilai) dan mengonversinya ke tipe float.

-Menambahkan data mahasiswa ke dalam list data_mahasiswa dalam bentuk dictionary dengan format {"nama": nama, "nilai": nilai}.

-Menampilkan pesan bahwa data berhasil ditambahkan dengan menggunakan garis pemisah berbentuk "-" dan "=".

Output Program: Setiap kali fungsi tambah() dipanggil, pengguna dapat menambahkan data baru (nama dan nilai) ke dalam daftar data_mahasiswa, dan program memberikan konfirmasi keberhasilan.

![Gambar2](https://github.com/Raihanardiansyah/Praktikum_6/blob/main/ss/2.png?raw=true)

Program tersebut merupakan fungsi tampilkan() yang digunakan untuk menampilkan daftar data mahasiswa yang sebelumnya telah disimpan dalam list data_mahasiswa. Berikut adalah penjelasan singkatnya:

### 1. Pengecekan List Kosong:

-Jika data_mahasiswa kosong (if not data_mahasiswa), program menampilkan pesan bahwa belum ada data mahasiswa dengan format yang rapi menggunakan garis pemisah.
Menampilkan Daftar Mahasiswa:

### 2. Jika data_mahasiswa tidak kosong:

-Menampilkan judul tabel "Daftar Nilai Mahasiswa A.3".

-Menampilkan header tabel dengan kolom NO, NAMA, dan NILAI.

-Menggunakan loop for dengan fungsi enumerate untuk menampilkan setiap data mahasiswa dari data_mahasiswa. Fungsi enumerate digunakan agar setiap data diberi nomor urut, dimulai dari 1.

-Format tampilan setiap baris data mahasiswa dirapikan menggunakan string f-string, dengan lebar kolom untuk nama (16 karakter) dan nilai (6 karakter).

### 3. Format Tabel:

-Setiap elemen tampilan disertai garis pemisah dengan karakter "-" untuk menjaga keterbacaan output.

Fungsi Program: Fungsi ini menampilkan daftar mahasiswa yang sudah ditambahkan. Jika belum ada data, pengguna akan diberi tahu bahwa daftar masih kosong.

![Gambar3](https://github.com/Raihanardiansyah/Praktikum_6/blob/main/ss/3.pngraw=true)

Program tersebut berisi dua fungsi, yaitu hapus(nama) dan ubah(nama), yang digunakan untuk mengelola data mahasiswa dalam daftar data_mahasiswa. Berikut penjelasan masing-masing fungsi:

Fungsi hapus(nama)
Fungsi ini digunakan untuk menghapus data mahasiswa berdasarkan nama tertentu.

Akses Variabel Global:

Menggunakan keyword global untuk memastikan fungsi bekerja pada variabel data_mahasiswa global, bukan membuat salinan lokal.
Proses Penghapusan:

Membuat daftar baru yang hanya berisi mahasiswa yang namanya tidak sama dengan nama yang diberikan menggunakan list comprehension.
Data mahasiswa dengan nama yang cocok dihapus secara efektif.
Konfirmasi:

Menampilkan pesan bahwa data mahasiswa dengan nama tertentu telah dihapus.
Fungsi ubah(nama)
Fungsi ini digunakan untuk mengubah nilai mahasiswa berdasarkan nama tertentu.

Pencarian Data:

Melakukan iterasi terhadap data_mahasiswa untuk mencari mahasiswa dengan nama yang sesuai.
Perubahan Data:

Jika nama ditemukan, meminta pengguna untuk memasukkan nilai baru melalui input().
Mengubah nilai (nilai) mahasiswa sesuai input pengguna.
Konfirmasi:

Menampilkan pesan bahwa data berhasil diubah dan keluar dari fungsi menggunakan return.
Jika Tidak Ditemukan:

Jika nama mahasiswa tidak ditemukan, menampilkan pesan bahwa data tidak ditemukan.
Fungsi Program Secara Umum
hapus(nama): Menghapus data mahasiswa yang memiliki nama tertentu.
ubah(nama): Mengubah nilai mahasiswa yang memiliki nama tertentu.
Kedua fungsi ini digunakan untuk memodifikasi isi daftar data_mahasiswa dengan cara yang spesifik, disertai pesan konfirmasi untuk meningkatkan interaksi pengguna.
