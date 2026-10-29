# Praktikum 6: DOM dan Event JavaScript - Pemrograman Web
Repository ini dibuat untuk menyelesaikan tugas Praktikum 6 Pemrograman Web.
 
## Identitas Mahasiswa
 
| Keterangan      | Data                 |
| --------------- | -------------------- |
| **Nama**        | Lia Mulyati          |
| **Kelas**       | I251D                |
| **NIM**         | 312510167            |
| **Mata Kuliah** | Pemrograman Web      |
| **Dosen**       | Agung Nugroho, S.Kom., M.Kom. |
 
---
## Tujuan Praktikum
 
- Mahasiswa mampu memahami konsep DOM (Document Object Model) sebagai struktur dokumen HTML yang dapat diubah oleh JavaScript.
- Mahasiswa mampu memilih elemen HTML menggunakan `getElementById()`, `querySelector()`, dan `querySelectorAll()`.
- Mahasiswa mampu menangani event (`click`, `input`, `submit`) menggunakan `addEventListener()`.
- Mahasiswa mampu mengubah teks, class, dan gaya CSS secara dinamis menggunakan `textContent` dan `classList`.
- Mahasiswa mampu membuat validasi form sederhana menggunakan `preventDefault()`.
- Mahasiswa mampu membuat aplikasi interaktif sederhana (To-do List dan Form Pendaftaran Workshop).
---

# Struktur File Proyek

![img36](img/img36.png)

# Pertanyaan Evaluasi 
1. Apa yang dimaksud dengan DOM dan apa manfaatnya?

DOM (Document Object Model) adalah representasi struktur halaman HTML yang dapat diakses dan dimanipulasi menggunakan JavaScript. Manfaatnya adalah memungkinkan JavaScript mengubah teks, gaya, atribut, serta menambahkan atau menghapus elemen HTML secara dinamis.

2. Apa perbedaan getElementById(), querySelector(), dan querySelectorAll()?

- getElementById() → memilih satu elemen berdasarkan ID.
- querySelector() → memilih elemen pertama yang sesuai  dengan selector CSS.
- querySelectorAll() → memilih semua elemen yang sesuai dengan selector CSS.

3. Apa fungsi addEventListener() dan sebutkan tiga contoh event?

- click → ketika elemen diklik.
- input → ketika isi input berubah.
- submit → ketika form dikirim.

4. Mengapa event.preventDefault() digunakan pada event submit form?

Digunakan untuk mencegah perilaku bawaan form, yaitu mengirim atau me-refresh halaman. Dengan begitu, JavaScript dapat melakukan validasi terlebih dahulu dan menampilkan pesan kepada pengguna.

5. Apa perbedaan textContent dan innerHTML dari sisi penggunaan dan keamanan?

textContent → digunakan untuk mengubah atau mengambil teks biasa dan lebih aman karena tidak memproses HTML.
innerHTML → digunakan jika ingin memasukkan atau mengubah struktur HTML, tetapi harus lebih hati-hati karena HTML yang tidak terpercaya dapat menimbulkan risiko keamanan.

6. Bagaimana classList.toggle() membantu mengubah tampilan elemen?

classList.toggle() digunakan untuk menambahkan class jika belum ada dan menghapusnya jika sudah ada. Dengan begitu, tampilan elemen dapat diubah secara interaktif menggunakan CSS. Contohnya pada praktikum, highlight dan teks-besar dapat dinyalakan atau dimatikan dengan tombol.

7. Sebutkan minimal tiga skenario pengujian validasi form.

- Semua input dikosongkan → muncul pesan "Nama wajib diisi."
- Email diisi dengan format yang salah → muncul pesan "Masukkan email yang valid."
- Usia diisi kurang dari 17 tahun → muncul pesan "Usia harus berupa bilangan bulat 17–100."
- Semua data diisi dengan benar → muncul pesan bahwa validasi berhasil.

# Langkah Kerja Praktikum 

# Latihan 1 mengubah teks dengna DOM
Pilih elemen HTML berdasarkan id dan ubah kontennya.

JavaScript digunakan untuk mengambil elemen HTML berdasarkan id, kemudian mengubah teksnya menggunakan DOM.

 ![img1](<img/img 1.png>)

Teks pada halaman berubah sesuai perintah JavaScript.
    hasil di browsernya.
 ![img2](ig/img2.png)

    hasil perubahannya.
 ![img3](img/img3.png)

 # Latihan 2 Event click
Saat tombol diklik, ubah teks paragraf dan tampilkan waktu saat tindakan dilakukan. 
 ![img4](img/img4.png)

 # Latihan 3 mengubah kelas dan gaya CSS
Tambahkan aturan CSS berikut ke style.css dan buat paragraf id teksGaya serta tombol id tombolGaya. 

 ![img5](img/img5.png)

 ![img6](img/img6.png)

 Menggunakan classList.toggle() untuk menambahkan atau menghapus class CSS pada sebuah elemen.

# Latihan 4 Event input dan penghitung karakter
Buat input teks dan indikator jumlah karakter yang diperbarui saat pengguna mengetik. 

Event input digunakan untuk mendeteksi perubahan isi input setiap kali pengguna mengetik.

 ![img7](img/img7.png)

 ![img8](img/img8.png)

Jumlah karakter langsung bertambah atau berkurang sesuai teks yang dimasukkan.
 hasil browsernya.
![img9](img/img9.png)

# Latihan 5 Validasi form pendaftaran
Buat form nama, email, dan usia. Program menampilkan pesan jika input tidak sesuai.
![img10](img/img10.png)

JavaScript memeriksa nama, email, dan usia sebelum data dianggap valid.
![img11](img/img11.png)

Uji minimal lima kondisi: 

hasil browsernya.
semua kosong, 
![img12](img/img122.png)

nama kosong,
![img13](image.png)

email tidak valid,
![img14](img/img14.png) 

usia di bawah 17,
![img15](img/img15.png)

dan semua input valid. 
![img16](img/img16.png)

Program menampilkan pesan kesalahan jika data tidak sesuai dan pesan berhasil jika semua data benar. Pengujian dilakukan dengan beberapa kondisi input.

# Latihan 6 Daftar Tugas Sederhana To-Do-List
Buat aplikasi kecil untuk menambahkan tugas dan menandai tugas selesai.
![img17](img/img17.png)

![img18](img/img18.png)

![img19](img/img19.png)

![img20](img/img20.png)

Membuat daftar tugas yang dapat ditambahkan dan ditandai sebagai selesai menggunakan JavaScript dan DOM.

hasil browsernya.
![img21](img/img21.png)

Tugas baru muncul di daftar dan tombol Tandai selesai dapat mengubah status tugas.

# Mini Project Form Pendaftaran Workshop

Kembangkan halaman pendaftaran workshop dengan minimal tiga fungsi interaktif. 

Validasi nama, email, dan pilihan sesi. 
![img22](img/img22.png)

![img23](img/img23.png)

![img24](img/img24.png)

Penghitung karakter atau ringkasan input secara langsung.
 ![img25](image-1.png)

 ![img26](img/img26.png)

 Pesan kesalahan dan pesan sukses yang tampil pada halaman. 

 Pesan Berhasil 
 ![img27](img/img27.png)

 Pesan Kesalahan
 ![img28](img/img28.png)

 Tombol reset atau hapus input. 
 ![img29](image-2.png)

 ![img30](img/img30.png)

 Gunakan addEventListener() untuk event input, change, click, atau submit. 
 ![img31](img/img31.png)

 Mengembangkan form workshop dengan beberapa fitur interaktif, seperti validasi nama, email, pilihan sesi, penghitung karakter, pesan berhasil/gagal, dan tombol reset.

 # Eksperimen Mandiri
 Tambahkan tombol untuk menghapus satu item dari To-do List. 
 ![img32](img/img32.png)

 ![img33](img/img33.png)

hasil browsernya.
![img34](img/img34.png)

![img35](img/img35.png)

Ketika tombol Hapus diklik, tugas yang dipilih langsung hilang dari daftar.

# Kesimpulan 
Praktikum ini mempelajari cara menggunakan DOM dan Event Handling untuk membuat halaman web yang lebih interaktif. JavaScript dapat mengubah isi halaman, merespons tindakan pengguna, melakukan validasi, serta menambah dan menghapus elemen secara dinamis.