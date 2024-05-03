# BASIS-P8
# 1. Tampilkan semua isi/record tabel!
SELECT * FROM mahasiswa;
![1](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/2238969c-1ccd-426b-8f2f-2457d677bc73)

# 2. Ubah data tanggal lahir mahasiswa yang bernama Ari menjadi: 1979-08-31!
UPDATE mahasiswa SET tanggal_lahir = '1979-08-31'WHERE nama = 'Ari Santoso';
![3](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/9ea21b95-3913-45a6-aa05-dfc2404fe64d)

# 3. Tampilkan satu baris / record data yang telah diubah tadi yaitu record dengan nama Ari saja!
SELECT * FROM mahasiswa WHERE nama = 'Ari Santoso';
![3](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/9ea21b95-3913-45a6-aa05-dfc2404fe64d)

# 4. Hapus Mahasiswa yang bernama Dina!
DELETE FROM mahasiswa WHERE nama = 'Dina Marlina';

![4](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/86c35ddc-558b-4e84-986e-48fb35a28d1b)

# 5. Tampilkan record atau data yang tanggal kelahirannya lebih dari atau sama dengan 1996-1-2!
SELECT * FROM mahasiswa WHERE tanggal_lahir >= '1996-01-02';

![5](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/d5edf95e-ddea-45d3-acaa-29be8856bd09)
# 6. Tampilkan semua Mahasiswa yang berasal dari Bekasi dan berjenis kelamin perempuan!
SELECT * FROM mahasiswa WHERE kota = 'Bekasi' AND jenis_kelamin = 'Perempuan';

![6](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/546b0988-c508-4dbb-99d0-d912c10b3bdd)
# 7. Tampilkan semua Mahasiswa yang berasal dari Bekasi dengan kelamin laki-laki atau Mahasiswa yang berumur lebih dari 22 tahun dengan kelamin wanita!
SELECT * FROM mahasiswa WHERE (kota = 'Bekasi' AND jenis_kelamin = 'Laki-laki') OR (YEAR(CURRENT_DATE) - YEAR(tanggal_lahir) > 22 AND jenis_kelamin = 'Perempuan');

![7](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/41a19e69-bc2d-4b6c-ba84-a94826084721)
# 8. Tampilkan data nama dan alamat mahasiswa saja dari tabel tersebut
SELECT nama,kota FROM mahasiswa;

![8](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/770df059-b48d-4286-aa44-62ccd2f807c5)
# 9. Tampilkan data mahasiswa terurut berdasarkan nama
SELECT * FROM mahasiswa ORDER BY nama;

![9](https://github.com/MUHAMMADRIZKYEFENDI/BASIS-P8/assets/168548623/7908ea72-5858-42fc-addd-ce8aa8f5f32c)

Apa bedanya penggunaan BETWEEN dan penggunaan operator >=
dan <= ? 
jawab : Secara singkat:

- BETWEEN digunakan untuk menentukan apakah sebuah nilai berada dalam rentang tertentu, termasuk kedua batas rentang.
- Operator >= (lebih besar atau sama dengan) digunakan untuk memeriksa apakah nilai lebih besar dari atau sama dengan nilai tertentu.
- Operator <= (kurang dari atau sama dengan) digunakan untuk memeriksa apakah nilai kurang dari atau sama dengan nilai tertentu.

Jadi, perbedaan utama adalah BETWEEN mencakup kedua batas rentang, sedangkan operator >= dan <= memeriksa apakah nilai lebih besar dari atau kurang dari batas tersebut.

Berikan kesimpulan anda!
jawab : tugas ini di berikan supaya kita bisa memahami tentang ddl dan databases serta oprator operator di dalam nya.
