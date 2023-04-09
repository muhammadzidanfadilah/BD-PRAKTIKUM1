# PRAKTIKUM 1

# - Pertama tama kita membuat database latihan 1 seperti gambar di bawah ini

![gambar1](gambar/gambar1.png)

# - Melihat basis data yang ada di my sql

![gambar1](gambar/gambar2.png)

# - kemudian membuat tabel dengan menggunakan perintah di bawah ini nama dan alamat 

CREATE TABLE siswa (nama VARCHAR(100),alamat TEXT);

![gambar1](gambar/gambar3.png)

# - Menambahkan kolom keterangan dengan menggunakan perintah seperti di bawah ini beserta contoh nya 

ALTER TABLE siswa ADD COLUMN keterangan VARCHAR(15) AFTER alamat;

![gambar1](gambar/gambar4.png)

# - Kemudian kita akan mengubah nama kolom id(int 11) dengan menggunakan perintah dan contoh nya seperti di bawah ini

ALTER TABLE siswa ADD COLUMN id int(11) First;

![gambar1](gambar/gambar5.png)

# - Tambahkan sebuah kolom untuk id (varchar11)

ALTER TABLE siswa MODIFY COLUMN id varchar(11) after alamat;

![gambar1](gambar/gambar6.png)

# - Ubah tipe data kolom hp menjadi char(20)

ALTER TABLE siswa MODIFY COLUMN phone hp VARCHAR(20);

![gambar1](gambar/gambar7.png)

# - Mengubah nama kolom phone menjadi hp (varchar20)

ALTER TABLE siswa CHANGE COLUMN phone hp varchar(20);

![gambar1](gambar/gambar8.png)

# - Menambahkan kolom email setelah kolom hp

ALTER TABLE siswa ADD COLUMN email text after hp;

![gambar1](gambar/gambar9.png)

# - Hapus kolom keterangan dari tabel

ALTER TABLE siswa DROP keterangan;

![gambar1](gambar/gambar10.png)

# - Ganti nama tabel menjadi data_mahasiswa

ALTER TABLE siswa RENAME data_mahasiswa;

![gambar1](gambar/gambar11.png)

# - Mengubah kolom nim (11)

ALTER TABLE data_mahasiswa CHANGE COLUMN id nim varchar(11);

![gambar1](gambar/gambar12.png)

# - Menambahkan primary key dengan menggunakan perintah di bawah ini

ALTER TABLE siswa ADD PRIMARY KEY(nim);

![gambar1](gambar/gambar13.png)

# - Menambahkan constraint dengan menggunakan perintah di bawah ini

ALTER TABLE siswa ADD CONSTRAINT PK_siswa PRIMARY KEY(email);

![gambar1](gambar/gambar14.png)

- Pengertian dari int(11)
int (11) nunjukkan bahwa kolom memiliki tipe data bilangan bulat (integer) dengan ukuran 11 digit 

- Melihat struktur tabel dengan perintah desc dan ada kolom null berisi yes dan no apa itu?
Jika kolom "Null" adalah "YES", itu berarti kolom tersebut diizinkan untuk memiliki nilai NULL.

Jika kolom "Null" adalah "NO", maka kolom tersebut tidak diizinkan untuk memiliki nilai NULL


