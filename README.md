# latihan2-xampp

```
NAMA    : SAHRUL RIDWANSYAH
NIM     : 312210063
KELAS   : TI.22.A2
MATKUL  : BASIS DATA
```

# tugas praktikum

# 1. langkah pertama buat terlebih dahulu database dengan nama latihan2.

untuk membuat database gunakan perintah sebagai berikut:
```
create database [nama_database]
contohnya
create database latihan2
```
lalu, setelah kita membuat database selanjutnya kita masuk kedalam database tersebut dengan perintah sebagai berikut:
```
use latihan2;
```
![waduh 2](https://user-images.githubusercontent.com/115526901/230829125-588102ed-d6f4-418e-8534-7829588f0487.png)

# 2. buat sebuah tabel dengan nama biodata seperti nama, alamat didalam database latihan2.

untuk membuat table gunakan perintah sebagai berikut:
```
CREATE TABLE nama_tabel (nama_field1 tipe _data(ukuran), nama_field2 tipe_data(ukuran), ..., nama_fieldn tipe_data(ukuran));

CREATE TABLE biodata (nama VACHAR (15), alamat TEXT);
```
![waduh 1](https://user-images.githubusercontent.com/115526901/230829221-1194b51d-f953-4c18-b384-744a72faa9e4.png)

# 3. tambahkan sebuah kolom keterangan (varchar 15), sebagai kolom trakhir.
 
untuk menambahkan kolom terakhir yaitu deangan sering digunakan kata after, contoh:
```
alter table biodata add column keterangan varchar (15) after phone;
```
![waduh 3](https://user-images.githubusercontent.com/115526901/230830192-23e4d8a0-94e4-4cc0-8244-79cd0f0226f6.png)

# 4. tambahkan kolom id(int11) di awal (sebagai kolom pertama).

untuk menambahkan kolom pertama yaitu dengan perintah sebagai berikut:
```
alter table biodata add column id(int11) first;
```
![waduh 4](https://user-images.githubusercontent.com/115526901/230830822-cc8e2aa9-02bd-4128-aa09-a9a3181011ca.png)

# 5. sisipkan sebuah kolom dengan nama phone (varchar 15) setelah kolom alamat.

untuk menambahkan kolom setelah kolom lain yaitu dengan perintah after

![waduh 5](https://user-images.githubusercontent.com/115526901/230831728-9f3b8c57-2f11-4412-9cff-bd0755dd1047.png)

# 6. ubah tipe data kolom id menjadi char(11).

untuk mengubah type data yaitu dengan perintah sebagai berikut:
```
alter table [nama_table] modify nama_field tipe_data_baru(ukuran);
```
![waduh 6](https://user-images.githubusercontent.com/115526901/230832559-bcae2426-e958-4e82-9b9f-0fc6b3e5b681.png)

# 7. ubah nama kolom phone menjadi hp(varchar20).

untuk mengubah kolom yaitu dengan perintah sebagai berikut:
```
ALTER TABLE [nama_tabel] CHANGE nama_field_lama nama_field_baru tipe_data(ukuran);
```
![waduh 7](https://user-images.githubusercontent.com/115526901/230832910-8b0bda68-464e-41eb-b53c-76f057961df7.png)

# 8. tambahkan kolom email setelah kolom hp 

![waduh 8](https://user-images.githubusercontent.com/115526901/230833400-5c9fc8d7-a414-409b-a59c-84a23769a718.png)

# 9. hapus kolom keterangan dari table.

untuk menghapus kolom dari dable yaitu dengan perintah sebagai berikut:
```
alter table [nama_table] drop_field;
```
![waduh 9](https://user-images.githubusercontent.com/115526901/230833755-cad46070-a62c-49f5-9e16-b5d61880748d.png)

# 10. ganti nama table menjadi data_mahasiswa.

untuk mengganti nama table yaitu dengan perintah sebagai berikut:
```
alter table [nama_table] rename [nama_table_baru]
```
![waduh 10](https://user-images.githubusercontent.com/115526901/230834130-5c16c3de-9a7a-443e-bae9-d7372734ae49.png)

# 11. ganti nama field id menjadi nim.

![waduh 11](https://user-images.githubusercontent.com/115526901/230834330-4c63b1cb-a5ff-44e1-a4ab-c64b5e3b4abc.png)

# 12. jadikan nim sebagai primary key.

untuk menambahkan index atau key, gunakan perintah sebagai berikut:
-tipe
-primary key
-unique key 
-fulltext
```
ALTER TABLE [nama_tabel] ADD [INDEX|PRIMARY KEY] (nama_field);
```
![waduh 12](https://user-images.githubusercontent.com/115526901/230835010-9d7dcfd1-71d7-4464-a46e-5b3f2803bf09.png)

# 13. jadikan kolom email sebagai

perintahnya sama seperti diatas, hanya saja diganti menjadi unique key.

![waduh 13](https://user-images.githubusercontent.com/115526901/230835722-a7185aea-a5c2-487c-80db-dff70e4437fd.png)

# evaluasi dan pertanyaan 

1. tulis semua printah-perintah SQL percobaan di pdf praktikum 1 beserta outputnya!

sql dll

* membuat database
```
create database latihan2
```
![waduh 2](https://user-images.githubusercontent.com/115526901/230840896-aac0e001-ab82-4054-b671-67d168123a5c.png)

* membuat table 
```
create biodata (nama varchar (15), alamat text)
```
![waduh 1](https://user-images.githubusercontent.com/115526901/230841347-bec1f074-0019-4927-8f1c-9ecd4847815d.png)

* menambah kolom 
```
alter table biodata add column keterangan text after alamat;
```
![waduh 3](https://user-images.githubusercontent.com/115526901/230841626-1af278d1-6209-4598-8ef3-6379e71e519f.png)

* menambah kolom diawal
```
alter table biodata add column id int first;
```
![waduh 4](https://user-images.githubusercontent.com/115526901/230842264-9beff864-bd36-4e84-849b-205aa080466f.png)
 
* mengubah nama kolom 
![waduh 7](https://user-images.githubusercontent.com/115526901/230842738-0e40971a-1a62-4888-b5a1-378606e5f80d.png)

* mengubah tipe data 
![waduh 6](https://user-images.githubusercontent.com/115526901/230842942-9441ea1b-69e3-4620-86ff-30af098b6cfe.png)

* menghapus kolom 
![waduh 9](https://user-images.githubusercontent.com/115526901/230843101-671efd9d-edbd-45fa-bcba-476c513db124.png)

2. apa maksud dari int(11)?
int(11) adalah nama tipe datanya yaitu integer dan memiliki panjang 11 karakter

3. ketika melihat struktur table dengan perintah desc, ada kolom null yang berisi yes dan no, apa maksudnya?
maksudnya yaitu untuk menjelaskan bahwa pada record yang harus diisi. sedangkan yes bisa tidak diisi










