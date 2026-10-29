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
<img width="127" height="158" alt="img36" src="https://github.com/user-attachments/assets/68908736-a344-415a-b458-9092efe8655d" />

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

 <img width="394" height="95" alt="img 1" src="https://github.com/user-attachments/assets/654f10f9-7d2e-4686-936f-6e66ca446b49" />


Teks pada halaman berubah sesuai perintah JavaScript.
    hasil di browsernya.
<img width="223" height="122" alt="img2" src="https://github.com/user-attachments/assets/f2f722b0-630a-49fd-894f-bc0edf8b48b6" />

    hasil perubahannya.
<img width="290" height="140" alt="img3" src="https://github.com/user-attachments/assets/887e7b3c-728e-4a02-a21e-afddb90a9951" />

 # Latihan 2 Event click
Saat tombol diklik, ubah teks paragraf dan tampilkan waktu saat tindakan dilakukan. 
 <img width="515" height="65" alt="img4" src="https://github.com/user-attachments/assets/ff8d7b86-3b05-4390-a5d4-f3c76870032d" />


 # Latihan 3 mengubah kelas dan gaya CSS
Tambahkan aturan CSS berikut ke style.css dan buat paragraf id teksGaya serta tombol id tombolGaya. 

 <img width="260" height="148" alt="img5" src="https://github.com/user-attachments/assets/6cf949ea-6db9-4975-9869-01c6f9f2e650" />

 <img width="386" height="109" alt="img6" src="https://github.com/user-attachments/assets/54645d18-6aa1-4fe1-b4ba-659749e25612" />

 Menggunakan classList.toggle() untuk menambahkan atau menghapus class CSS pada sebuah elemen.

# Latihan 4 Event input dan penghitung karakter
Buat input teks dan indikator jumlah karakter yang diperbarui saat pengguna mengetik. 

Event input digunakan untuk mendeteksi perubahan isi input setiap kali pengguna mengetik.

<img width="378" height="58" alt="img7" src="https://github.com/user-attachments/assets/01b6db69-707d-4b98-a1c8-add7147481f5" />

<img width="399" height="89" alt="img8" src="https://github.com/user-attachments/assets/45070ea1-1d7f-4f0a-8371-e67219f50eb2" />

 
Jumlah karakter langsung bertambah atau berkurang sesuai teks yang dimasukkan.
 hasil browsernya.

<img width="230" height="53" alt="img9" src="https://github.com/user-attachments/assets/8427a8c9-8ceb-476b-9f37-2b7dc0b4f068" />

# Latihan 5 Validasi form pendaftaran
Buat form nama, email, dan usia. Program menampilkan pesan jika input tidak sesuai.
<img width="461" height="243" alt="img10" src="https://github.com/user-attachments/assets/227ca707-4f9f-4102-b947-99fbca20915d" />


JavaScript memeriksa nama, email, dan usia sebelum data dianggap valid.
<img width="545" height="431" alt="img11" src="https://github.com/user-attachments/assets/ec9ac996-b68c-4373-a25b-4386bf2e4b6b" />

Uji minimal lima kondisi: 

hasil browsernya.
semua kosong, 
<img width="262" height="233" alt="img122" src="https://github.com/user-attachments/assets/6d67d57b-2481-4578-9066-8a6db4bbfc9f" />

nama kosong,
<img width="229" height="228" alt="img13" src="https://github.com/user-attachments/assets/4dcb2c22-4a94-4ae7-bb99-606d6c51835f" />

email tidak valid,

<img width="241" height="234" alt="img14" src="https://github.com/user-attachments/assets/8a4ff236-233e-47f6-8677-20e4637fd236" />

usia di bawah 17,
<img width="235" height="238" alt="img15" src="https://github.com/user-attachments/assets/8cf877d2-417d-45ef-bec1-9b710e71497c" />

dan semua input valid. 
<img width="241" height="234" alt="img16" src="https://github.com/user-attachments/assets/d8abc687-aeb6-4c65-9a5b-116edd271ec7" />


Program menampilkan pesan kesalahan jika data tidak sesuai dan pesan berhasil jika semua data benar. Pengujian dilakukan dengan beberapa kondisi input.

# Latihan 6 Daftar Tugas Sederhana To-Do-List
Buat aplikasi kecil untuk menambahkan tugas dan menandai tugas selesai.
<img width="388" height="177" alt="img17" src="https://github.com/user-attachments/assets/3ffdf475-0211-499c-a540-c4623feee50f" />

<img width="469" height="422" alt="img18" src="https://github.com/user-attachments/assets/8fe5cd6e-8852-4c42-921e-a94b7b7e9f38" />


<img width="392" height="203" alt="img19" src="https://github.com/user-attachments/assets/2d22eda9-5a36-45f1-8bd5-b12363d94b59" />


<img width="260" height="121" alt="img20" src="https://github.com/user-attachments/assets/84f0826e-3d7d-4688-a290-cc3a91b5600a" />


Membuat daftar tugas yang dapat ditambahkan dan ditandai sebagai selesai menggunakan JavaScript dan DOM.

hasil browsernya.

<img width="198" height="137" alt="img21" src="https://github.com/user-attachments/assets/97a38624-b9fe-4fcd-890f-772f4aa3fb47" />

Tugas baru muncul di daftar dan tombol Tandai selesai dapat mengubah status tugas.

# Mini Project Form Pendaftaran Workshop

Kembangkan halaman pendaftaran workshop dengan minimal tiga fungsi interaktif. 

Validasi nama, email, dan pilihan sesi. 
<img width="563" height="357" alt="img22" src="https://github.com/user-attachments/assets/57e09ff3-9466-415a-8cab-185e73f7ec92" />

<img width="503" height="278" alt="img23" src="https://github.com/user-attachments/assets/b434ca21-9375-4c14-bd91-32d7dfd0df65" />

<img width="421" height="203" alt="img24" src="https://github.com/user-attachments/assets/74daca37-416e-4aea-9a74-ba2daaf1221a" />


Penghitung karakter atau ringkasan input secara langsung.
 <img width="536" height="290" alt="img25" src="https://github.com/user-attachments/assets/71ec97ab-4215-494b-b12f-28d1c5dfa2d4" />

<img width="439" height="330" alt="img26" src="https://github.com/user-attachments/assets/bee200cc-1a0c-40a6-8388-05328d74091d" />

 Pesan kesalahan dan pesan sukses yang tampil pada halaman. 

 Pesan Berhasil 
 
<img width="239" height="233" alt="img27" src="https://github.com/user-attachments/assets/4a5bd06c-7915-4b86-9207-f52c0df8b027" />

 Pesan Kesalahan
 <img width="218" height="224" alt="img28" src="https://github.com/user-attachments/assets/ed663841-41d7-4e87-83d2-8b4e94eb1ca8" />

 Tombol reset atau hapus input. 
 <img width="466" height="89" alt="img29" src="https://github.com/user-attachments/assets/1c04492e-84da-4fd2-872a-d32bff1b94c4" />

<img width="226" height="50" alt="img30" src="https://github.com/user-attachments/assets/92f91907-589d-4b33-9275-c00eb22888de" />


 Gunakan addEventListener() untuk event input, change, click, atau submit. 
 
<img width="437" height="266" alt="img31" src="https://github.com/user-attachments/assets/b9d9016e-889b-4aeb-b1dd-d4f0ce741b6e" />

 Mengembangkan form workshop dengan beberapa fitur interaktif, seperti validasi nama, email, pilihan sesi, penghitung karakter, pesan berhasil/gagal, dan tombol reset.

 # Eksperimen Mandiri
 Tambahkan tombol untuk menghapus satu item dari To-do List. 
 <img width="344" height="206" alt="img32" src="https://github.com/user-attachments/assets/022a11d7-319e-450e-b9d7-a2e50b285911" />
<img width="344" height="206" alt="img32" src="https://github.com/user-attachments/assets/4d0e0dec-049f-4cfc-a930-0b0868ce43ba" />


hasil browsernya.
<img width="278" height="59" alt="img34" src="https://github.com/user-attachments/assets/48ca2441-f876-45d3-b293-4beaf67626ec" />


<img width="179" height="41" alt="img35" src="https://github.com/user-attachments/assets/14cb48ba-24cc-478a-aa3f-40214a44c93a" />

Ketika tombol Hapus diklik, tugas yang dipilih langsung hilang dari daftar.

# Kesimpulan 
Praktikum ini mempelajari cara menggunakan DOM dan Event Handling untuk membuat halaman web yang lebih interaktif. JavaScript dapat mengubah isi halaman, merespons tindakan pengguna, melakukan validasi, serta menambah dan menghapus elemen secara dinamis.
