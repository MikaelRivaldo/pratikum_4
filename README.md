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

`SELECT COUNT(*) AS jumlah_baris FROM pegawai;`

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

`SELECT AVG(gaji) AS rata_gaji FROM pegawai`

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

1.Tampilkan jumlah hewan yang dimiliki setiap owner.

2.Tampilkan jumlah hewan berdasarkan spesies.

3.Tampilkan jumlah hewan berdasarkan jenis kelamin.

4.Tampilkan jumlah hewan berdasarkan spesies dan jenis kelamin.

5.Tampilkan jumlah hewan berdasarkan spesis (cat dan dog saja) dan jenis kelamin.

6.Tampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui saja.

# Penyelesaian

1.Tampilkan jumlah hewan yang dimiliki setiap owner.

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT owner, COUNT(*) AS jumlah_hewan FROM hewan GROUP BY owner;`

hasilnya akan seperti ini :

![gambar jwbno1](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/25b66544-9973-44b8-853b-0a253cee5707)

2.Tampilkan jumlah hewan berdasarkan spesies.

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT species, COUNT(*) AS jumlah_hewan FROM hewan GROUP BY species;`

hasilnya akan seperti ini :

![gambar jwbno2](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/7e5b6166-f98f-4899-a66f-88615f5095bb)

3.Tampilkan jumlah hewan berdasarkan jenis kelamin

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT sex, COUNT(*) AS jumlah_hewan FROM hewan GROUP BY sex;`

hasilnya akan seperti ini :

![gambar jwbno3](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/7264f281-6f68-46d3-a1f1-03e3fab9bae0)

4.Tampilkan jumlah hewan berdasarkan spesies dan jenis kelamin.

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT species, sex, COUNT(*) AS jumlah_hewan FROM hewan GROUP BY species,sex;`

hasilnya akan seperti ini :

![gambar jwbno4](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/de00ed2c-b8f5-4f21-975e-e48d5a140b5d)


5.Tampilkan jumlah hewan berdasarkan spesis (cat dan dog saja) dan jenis kelamin.

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT species, sex, COUNT(*) AS jumlah_hewan FROM hewan WHERE species IN('Cat','Dog')GROUP BY species, sex;`

hasilnya akan seperti ini :

![gambar jwbno5](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/d5b105f8-b39d-4cf6-ad09-480a5f2294d3)

6.Tampilkan jumlah hewan berdasarkan jenis kelamin yang diketahui saja.

`JAWAB`

Untuk perintahnya bisa menggunkan perintah seperti ini  :

`SELECT sex, COUNT(*) AS jumlah_hewan FROM hewan WHERE sex IN('f','m')GROUP BY sex;`

hasilnya akan seperti ini :

![gambar jwbno6](https://github.com/MikaelRivaldo/pratikum_4/assets/115770247/85f63ffc-c71e-4154-bdf3-d05d2f7f2635)
