# Tugas pratikum_4

# Tugas Pratikum (1)

1.Tampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000 !

2.Tampilkan pegawai yang tunjangannya NULL!

3..Tampilkan pegawai yang tunjangannya tidak NULL!

4.Tampilkan/hitung jumlah baris/record tabel pegawai!

5.Tampilkan/hitung jumlah total gaji di tabel pegawai!

6.Tampilkan/hitung rata-rata gaji pegawai!

7.Tampilkan gaji terkecil!

8.Tampilkan gaji terbesar!


![gambar1](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/7f7a0162-ba08-40c0-890f-535b74b47507)


`Untuk menulis perintah sql bisa ke menu seperti dibawah ini : `

![gambar menu menampilkan](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/a4ea21ca-ed58-41b1-868c-bdbce979658d)


# Penyelesaian

1.Tampilkan pegawai yang gajinya bukan 2.000.000 dan 1.250.000 !

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT * FROM pegawai WHERE gajih NOT IN (2000000, 1250000);`

hasilnya akan seperti ini :

![gambar jawaban no1](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/0cb432bc-c432-464b-bbdb-e54b70535222)


2.Tampilkan pegawai yang tunjangannya NULL!

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT * FROM pegawai WHERE tunjangan IS NULL;`

hasilnya akan seperti ini :

![gambar jawaban no2](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/ab39858f-753c-4227-a789-121215befbac)

3.Tampilkan pegawai yang tunjangannya tidak NULL!

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT * FROM pegawai WHERE tunjangan IS NOT NULL;`

 hasilnya akan seperti ini :

![gambar jawaban no3](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/84671f5f-a175-48e7-866f-2aba119d00c0)

4.Tampilkan/hitung jumlah baris/record tabel pegawai!

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT COUNT(*) AS jumlah_baris FROM tb_pegawai;`

hasilnya akan seperti ini :

![gambar jawaban no4](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/1aa41e1c-0651-48c3-bdc2-4eae4b598a40)

5.Tampilkan/hitung jumlah total gaji di tabel pegawai!

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT SUM(gaji) AS total_gaji FROM pegawai;`

hasilnya akan seperti ini :

![gambar jawaban no5](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/f85ac4d1-e069-4fed-b17b-5ec9a2a0a24e)]

6.Tampilkan/hitung rata-rata gaji pegawai!

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT AVG(gaji) AS rata_gaji FROM tb_pegawai`

hasilnya akan seperti ini :

![gambar jawaban no6](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/30e6fa55-530d-4caf-948c-96d3288559b9)

7.Tampilkan gaji terkecil!

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT MIN(gaji) AS gaji_terkecil FROM pegawai;`

hasilnya akan seperti ini :

![gambar jawaban no7](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/7e567935-3f0b-4dba-b701-26aa3d3c5e73)

8.Tampilkan gaji terbesar!

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT MAX(gaji) AS gaji_terbesar FROM pegawai;`

hasilnya akan seperti ini :

![gambar jawban no8](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/fb27e507-9cb5-49d8-b1c3-8b657ac22f95)



# Tugas Pratikum (2)

