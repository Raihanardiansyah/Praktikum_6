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

### Fungsi hapus(nama)

Fungsi ini digunakan untuk menghapus data mahasiswa berdasarkan nama tertentu.

### 1. Akses Variabel Global:

-Menggunakan keyword global untuk memastikan fungsi bekerja pada variabel data_mahasiswa global, bukan membuat salinan lokal.

### 2. Proses Penghapusan:

-Membuat daftar baru yang hanya berisi mahasiswa yang namanya tidak sama dengan nama yang diberikan menggunakan list comprehension.

-Data mahasiswa dengan nama yang cocok dihapus secara efektif.

### 3. Konfirmasi:

Menampilkan pesan bahwa data mahasiswa dengan nama tertentu telah dihapus.

### Fungsi ubah(nama)

Fungsi ini digunakan untuk mengubah nilai mahasiswa berdasarkan nama tertentu.

### 1. Pencarian Data:

-Melakukan iterasi terhadap data_mahasiswa untuk mencari mahasiswa dengan nama yang sesuai.

### 2. Perubahan Data:

-Jika nama ditemukan, meminta pengguna untuk memasukkan nilai baru melalui input().

-Mengubah nilai (nilai) mahasiswa sesuai input pengguna.

### 3. Konfirmasi:

-Menampilkan pesan bahwa data berhasil diubah dan keluar dari fungsi menggunakan return.

### 4. Jika Tidak Ditemukan:

-Jika nama mahasiswa tidak ditemukan, menampilkan pesan bahwa data tidak ditemukan.

### Fungsi Program Secara Umum

-hapus(nama): Menghapus data mahasiswa yang memiliki nama tertentu.

-ubah(nama): Mengubah nilai mahasiswa yang memiliki nama tertentu.

Kedua fungsi ini digunakan untuk memodifikasi isi daftar data_mahasiswa dengan cara yang spesifik, disertai pesan konfirmasi untuk meningkatkan interaksi pengguna.

![Gambar4]](https://github.com/Raihanardiansyah/Praktikum_6/blob/main/ss/4.png?raw=true)

Program tersebut adalah sebuah fungsi menu() yang menampilkan menu interaktif untuk mengelola data mahasiswa. Fungsi ini menggunakan loop while untuk menjalankan program hingga pengguna memilih opsi keluar. Berikut adalah penjelasan singkat:

### Struktur Menu

### 1. Pilihan Menu:

-Menu utama menampilkan 5 opsi:

1. Tambah Data

2. Tampilkan Data

3. Hapus Data

4. Ubah Data

5. Keluar

### 2. Input Pengguna:

-Pengguna diminta untuk memasukkan pilihan menu (1-5).

### Logika Pilihan

### Opsi 1: Tambah Data:

-Memanggil fungsi tambah() untuk menambahkan data mahasiswa baru.

### Opsi 2: Tampilkan Data:

-Memanggil fungsi tampilkan() untuk menampilkan daftar mahasiswa.

### Opsi 3: Hapus Data:

-Meminta pengguna memasukkan nama mahasiswa yang akan dihapus.

-Memanggil fungsi hapus(nama) untuk menghapus data mahasiswa dengan nama tersebut.

### Opsi 4: Ubah Data:

-Meminta pengguna memasukkan nama mahasiswa yang akan diubah.

-Memanggil fungsi ubah(nama) untuk mengubah nilai mahasiswa dengan nama tersebut.

### Opsi 5: Keluar:

-Menampilkan pesan bahwa program selesai.

-Menggunakan break untuk keluar dari loop dan menghentikan program.

### Pilihan Tidak Valid:

-Jika pengguna memasukkan pilihan selain 1-5, program menampilkan pesan bahwa pilihan tidak valid dan meminta pengguna untuk mencoba lagi.

### Fungsi Program

Fungsi menu() berfungsi sebagai pengendali utama program, yang menghubungkan semua fungsi pendukung (tambah, tampilkan, hapus, dan ubah). Program ini memungkinkan pengguna untuk melakukan operasi CRUD (Create, Read, Update, Delete) pada data mahasiswa dengan antarmuka yang sederhana dan interaktif.

![Gambar5](https://github.com/Raihanardiansyah/Praktikum_6/blob/main/ss/hasil.png?raw=true)

nah berikut adalah hasil dari program tersebut yang akan memunculkan beberapa menu yang dapat kalian pilih 

![Gambar6](https://github.com/Raihanardiansyah/Praktikum_6/tree/main/ss?raw=true)

Flowchart tersebut menjelaskan alur proses pengolahan data mahasiswa dengan beberapa fitur utama yang disediakan dalam menu pilihan. Berikut adalah penjelasan singkatnya:

### 1. Tampilkan Menu Pilihan:

Pengguna diberikan beberapa opsi:

-Tambah data mahasiswa

-Tampilkan data mahasiswa

-Ubah data mahasiswa

-Hapus data mahasiswa

-Keluar dari program

### 2. Input Pilihan:

Pengguna diminta untuk memilih salah satu opsi dari menu.

-Jika pilihan valid, proses berlanjut sesuai dengan opsi yang dipilih.

-Jika tidak, proses berakhir.

### 3. Proses Berdasarkan Pilihan:

-Tambah Data Mahasiswa: Pengguna dapat memasukkan nama dan nilai mahasiswa untuk menambahkannya ke data.

-Tampilkan Data Mahasiswa: Menampilkan data mahasiswa yang telah ditambahkan.

-Ubah Data Mahasiswa: Mengedit data mahasiswa yang sudah ada.

-Hapus Data Mahasiswa: Menghapus data mahasiswa yang dipilih.

### 4. Akhir Proses:

-Jika pengguna memilih keluar atau tidak memberikan input yang valid, proses akan berakhir.

Flowchart ini menggambarkan sistem pengolahan data mahasiswa yang interaktif dan modular.
