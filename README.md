# TUGAS PERTEMUAN KE 6 
|**Nama**|**NIM**|**Kelas**|**Matkul**|
|----|---|-----|------|
|Muhammad Arif Mulyanto|312310359|TI.23.A5|Basis Data|

# Soal Latihan Praktikum Pertemuan Ke 6
## 1. Tulis semua perintah-perintah SQL percobaan di atas beserta outputnya!
**1. Buat sebuah database dengan nama latihan2**

Untuk membuat database gunakan perintah sebagai berikut :

`CREATE DATABASE [nama_database]`

`CREATE DATABASE latihan2;`

lalu, setelah kita membuat database. kita masuk kedalam database tersebut dengan perintah sebagai berikut :

`USE latihan2;`
![ko1](https://github.com/MuhArifyanto/MySQL1/assets/147913440/59ec93e1-dd60-4174-9e96-5b0524539d67)


**2. Buat sebuah tabel dengan nama biodata (nama, alamat) didalam database latihan2!**

Untuk membuat Tabel gunakan perintah sebagai berikut :

`CREATE TABLE nama_tabel (
    nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran)
    );`

`CREATE TABLE biodata (
    nama varchar (100),
    alamat text
    );`
![ko2](https://github.com/MuhArifyanto/MySQL1/assets/147913440/61759bdf-6367-4bba-9e22-ff8efb0ae353)


**3. Tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom terakhir!**

Contoh :

`ALTER TABLE biodata ADD COLUMN keterangan VARCHAR (15);`

![ko3](https://github.com/MuhArifyanto/MySQL1/assets/147913440/97a0c45c-2b7e-4424-9280-0edadcd9a27c)


**4.Tambahkan kolom id(int 11) di awal (sebagai kolom pertama)!**

Untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut :

`ALTER TABLE biodata ADD COLUMN id int FIRST; `
![ko4](https://github.com/MuhArifyanto/MySQL1/assets/147913440/ee321b7b-0cd2-42a6-a5e6-a0d2146e81a2)


**5. Sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat!**

Untuk menambahkan kolom setelah kolom lain yaitu dengan perintah `AFTER`
![ko5](https://github.com/MuhArifyanto/MySQL1/assets/147913440/8dfbd6de-bd83-42c4-a754-d89591e22dce)

**6. Ubah tipe data kolom id menjadi char(11)!**

Untuk mengubah type data yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] MODIFY nama_field tipe_data_baru(ukuran);`
![ko6](https://github.com/MuhArifyanto/MySQL1/assets/147913440/aaea8f16-0abf-4dc0-859f-e0592a634208)


**7. Ubah nama kolom phone menjadi hp (char 20)!**

Untuk mengubah kolom yaitu dengan perintah sebgai berikut :

`ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);`
![ko7](https://github.com/MuhArifyanto/MySQL1/assets/147913440/5d1f3890-e786-4618-92dc-7f126ecd96a5)


**8. Tambahkan kolom email setelah kolom hp**

![ko8](https://github.com/MuhArifyanto/MySQL1/assets/147913440/6d99d122-5fff-4221-9512-5956de13967e)


**9. Hapus kolom keterangan dari tabel!**

Untuk menghapus kolom dari tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] DROP nama_field;`
![ko9](https://github.com/MuhArifyanto/MySQL1/assets/147913440/7bc3eae8-8f10-45cf-b55c-45f3ed53484a)

**10. Ganti nama tabel menjadi data_mahasiswa!**

Untuk mengganti nama tabel yaitu dengan perintah sebagai berikut :

`ALTER TABLE [nama_tabel] RENAME [nama_tabel_baru];`

![ko10](https://github.com/MuhArifyanto/MySQL1/assets/147913440/17f271ad-8169-4dbc-9c39-3840ba97d4bd)


**11. Ganti nama field id menjadi nim!**

![ko11](https://github.com/MuhArifyanto/MySQL1/assets/147913440/bbf72432-bf4a-4177-9e8a-745137b37d13)

**12. Jadikan nim sebagai PRIMARY KEY!**

Untuk menambahkan index atau key, gunakan perintah sebagai berikut :

tipe index :

- PRIMARY KEY
- UNIQUE KEY
- FULLTEXT

`ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);`
![ko12](https://github.com/MuhArifyanto/MySQL1/assets/147913440/59c8a891-dcca-44c1-839b-0ca41b9d549d)


**13. Jadikan kolom email sebagai UNIQUE KEY!**

Perintah nya sama seperti diatas, hanya saja diganti menjadi `UNIQUE KEY`
![ko13](https://github.com/MuhArifyanto/MySQL1/assets/147913440/ab5fc605-309e-42ff-8497-5ca5ce97006e)

## 2. Apa Maksud Dari INT(11) ?

- INT(11) Adalah Nama Tipe Datanya Yaitu `Integer` dan Memiliki Panjang 11 Karakter.

## 3. Ketika Kita Melihat Struktur Tabel Dengan Perintah DESC , Ada Kolom Null yang Berisi Yes dan No. Apa Maksudnya ?

- Yaitu Untuk Menjelaskan Bahwa Pada Record yg `NO` Harus diisi , Sedangkan `YES` Boleh Tidak diisi.
