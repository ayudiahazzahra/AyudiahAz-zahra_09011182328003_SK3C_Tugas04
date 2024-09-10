### 1. Lihat peralatan I/O, character device, yang ada pada system komputer.

![2 1](https://github.com/user-attachments/assets/d0cf5f8a-2b03-4df6-b14e-bcf3fcb5f2a1)

# Perintah di terminal tersebut digunakan untuk mencari perangkat karakter dalam direktori `/dev` di sistem Linux. Pada perintah pertama, pengguna mencoba menggunakan `ls -l /dev | grep "/^c"`, namun ada kesalahan karena simbol `/` tidak diperlukan di depan ekspresi reguler. Perintah ini gagal karena format pencarian yang salah.Pada perintah kedua, kesalahan diperbaiki menjadi `ls -l /dev | grep "^c"`, yang berarti mencari semua file dalam direktori `/dev` yang ditampilkan oleh perintah `ls -l`, dan kemudian menggunakan `grep` untuk memfilter hasil yang barisnya diawali dengan huruf "c". Huruf "c" dalam output tersebut biasanya menandakan perangkat karakter (character devices) yang merupakan bagian dari sistem file perangkat di Linux.

### 2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori latihan5.

![2 2](https://github.com/user-attachments/assets/974869e8-353d-467f-a6ba-6e507ae8b9f2)

# Pada gambar tersebut, pengguna mencoba membuat direktori baru dengan perintah `mkdir`, namun terjadi kesalahan karena adanya opsi yang tidak valid, yaitu simbol `/`. Setelah memperbaiki kesalahan, pengguna akhirnya membuat direktori bernama `latihan5` menggunakan perintah `mkdir ~/latihan5`, yang berarti membuat direktori di dalam direktori home pengguna.Setelah itu, pengguna menggunakan perintah `cd ~/latihan5` untuk masuk ke direktori `latihan5`. Perintah `pwd` dijalankan untuk memastikan lokasi direktori saat ini, dan hasilnya menunjukkan bahwa pengguna berada di direktori `/home/ayudiah/latihan5`. Selanjutnya, pengguna membuat tiga subdirektori dengan nama `januari`, `februari`, dan `maret` menggunakan perintah `mkdir januari februari maret` di dalam direktori `latihan5`. Terakhir, perintah `ls` digunakan untuk melihat isi direktori, yang menampilkan ketiga direktori yang baru saja dibuat: `februari`, `januari`, dan `maret`.

### 3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret.

![2 3](https://github.com/user-attachments/assets/1c798544-b2c1-47c7-81bf-dbaab1f730b8)

# Pada gambar tersebut, pengguna membuat sebuah file teks menggunakan perintah `echo`. Dengan perintah `echo -e`, pengguna menambahkan baris baru (`\n`) dalam teks dan menulis informasi berupa nama, NIM, dan alamat ke dalam file bernama `dataku` di dalam direktori `januari`. Selanjutnya, pengguna menyalin file `dataku` dari direktori `januari` ke direktori `februari` menggunakan perintah `cp januari/dataku februari/`, dan kemudian juga menyalinnya ke direktori `maret` dengan perintah `cp januari/dataku maret/`. Setelah menyalin file, pengguna menggunakan perintah `ls` untuk melihat isi direktori `februari` dan `maret`. Hasilnya menunjukkan bahwa file `dataku` berhasil disalin ke kedua direktori tersebut, karena file tersebut muncul di dalam direktori `februari` dan `maret`.

### 4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write.

![2 4](https://github.com/user-attachments/assets/cfbdc37c-504f-4db2-b18c-bd73cf4d5988)

# Perintah `chmod go+w januari/dataku` digunakan untuk menambahkan izin tulis (write) bagi grup dan pengguna lain pada file atau direktori bernama "dataku" di dalam folder "januari", sedangkan perintah `ls -l januari/dataku` akan menampilkan detail informasi tentang file atau direktori tersebut, termasuk izin akses, pemilik, ukuran, dan waktu modifikasi terakhir.

### 5. Ubahlah ijin akses file dataku pada sub direktori pebruari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read

![2 5](https://github.com/user-attachments/assets/8510d32e-1c69-496b-97b3-9c9f2f6ada8e)

# Perintah `chmod 754 februari/dataku` digunakan untuk mengubah izin akses file atau direktori bernama "dataku" di dalam folder "februari". Izin akses ini berarti: Pemilik file memiliki izin penuh (membaca, menulis, dan mengeksekusi), Grup pengguna hanya bisa membaca dan mengeksekusi file, tetapi tidak bisa menulis, Pengguna lain hanya bisa membaca file tanpa izin eksekusi atau penulisan. Selanjutnya, perintah `ls -l februari/dataku` digunakan untuk menampilkan detail informasi dari file atau direktori "dataku" di folder "februari". Hasilnya akan menunjukkan izin akses, ukuran file, waktu modifikasi terakhir, dan nama pemilik file.


![2 6](https://github.com/user-attachments/assets/e85ad6f0-b02a-47d1-b7b4-1e83e96bce55)
![2 7](https://github.com/user-attachments/assets/d38eec72-3f38-43a2-8e79-f6f4ca46d34e)
![2 8](https://github.com/user-attachments/assets/5ac9d6ed-09e5-4a54-9b1f-bee19b98c1cc)
![2 9](https://github.com/user-attachments/assets/213cd756-ccdb-40d9-9735-6b383574076d)
![2 10](https://github.com/user-attachments/assets/9b708560-57e8-4c1f-9e09-c868c59abc8d)
