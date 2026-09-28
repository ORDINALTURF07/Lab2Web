# LAPORAN PRAKTIKUM 2

## HTML LANJUTAN

### Identitas Mahasiswa

* **Nama:** UGI INSAN MULYAWAN
* **NIM:** 312510268
* **Program Studi:** Teknik Informatika
* **Mata Kuliah:** Pemrograman Web
* **Praktikum:** Praktikum 2 — HTML Lanjutan

---

## Pengertian HTML

HTML (*HyperText Markup Language*) adalah bahasa markup yang digunakan untuk membuat struktur dan menyusun konten pada halaman web. HTML memungkinkan kita menampilkan berbagai elemen, seperti teks, tabel, formulir, tautan, gambar, audio, dan video.

Pada praktikum ini, materi yang dipelajari meliputi pembuatan tabel, form, radio button, checkbox, select, textarea, semantic HTML, multimedia, serta validasi form dasar.

## Langkah-Langkah Praktikum

### 1. Membuat Tabel Data Mahasiswa

**Tujuan:** Membuat tabel data mahasiswa menggunakan elemen HTML, seperti `table`, `tr`, `th`, dan `td`.

**CODING:**

```html
<!DOCTYPE html>
<html>
<head><title>HTML Lanjutan</title></head>
<body>
<h1>Data Mahasiswa</h1>
<table border="1">
    <tr><th>NIM</th><th>Nama</th><th>Program Studi</th></tr>
    <tr><td>31241001</td><td>Andi</td><td>Teknik Informatika</td></tr>
    <tr><td>31241002</td><td>Budi</td><td>Teknik Informatika</td></tr>
</table>
</body>
</html>
```

**Screenshot Codingan:**

![Codingan Langkah 1](images/codingan%201.png)

**Hasil Browser:**

![Hasil Browser Langkah 1](images/hasil-browser%201.png)

**Keterangan:**

Tabel digunakan untuk menampilkan data mahasiswa dalam bentuk baris dan kolom. Elemen `th` digunakan untuk judul kolom, sedangkan `td` digunakan untuk menampilkan data.

### 2. Mengembangkan Tabel dengan thead, tbody, dan tfoot

**Tujuan:** Membuat tabel yang memiliki bagian kepala, isi, dan kaki tabel.

**CODING:**

```html
<table border="1">
    <caption>Nilai Praktikum</caption>
    <thead>
        <tr><th>No</th><th>Nama</th><th>Nilai</th></tr>
    </thead>
    <tbody>
        <tr><td>1</td><td>Andi</td><td>85</td></tr>
        <tr><td>2</td><td>Budi</td><td>90</td></tr>
    </tbody>
    <tfoot>
        <tr><td colspan="2">Rata-rata</td><td>87.5</td></tr>
    </tfoot>
</table>
```

**Screenshot Codingan:**

![Codingan Langkah 2](images/codingan%202.png)

**Hasil Browser:**

![Hasil Browser Langkah 2](images/hasil-browser%202.png)

**Keterangan:**

Elemen `thead` digunakan untuk bagian kepala tabel, `tbody` untuk bagian isi tabel, dan `tfoot` untuk bagian kaki tabel. Atribut `colspan="2"` digunakan untuk menggabungkan dua kolom menjadi satu.

### 3. Membuat Form Registrasi Mahasiswa

**Tujuan:** Membuat formulir registrasi mahasiswa dengan input nama, email, password, dan tanggal lahir.

**CODING:**

```html
<h1>Form Registrasi Mahasiswa</h1>
<form>
    <label for="nama">Nama Lengkap</label><br>
    <input type="text" id="nama" name="nama"><br><br>

    <label for="email">Email</label><br>
    <input type="email" id="email" name="email"><br><br>

    <label for="password">Password</label><br>
    <input type="password" id="password" name="password"><br><br>

    <label for="tanggal">Tanggal Lahir</label><br>
    <input type="date" id="tanggal" name="tanggal"><br><br>

    <button type="submit">Daftar</button>
    <button type="reset">Reset</button>
</form>
```

**Screenshot Codingan:**

![Codingan Langkah 3](images/codingan%203.png)

**Hasil Browser:**

![Hasil Browser Langkah 3](images/hasil-browser%203.png)

**Keterangan:**

Form digunakan untuk menerima input dari pengguna. Input `text` digunakan untuk nama, `email` untuk alamat email, `password` untuk kata sandi, dan `date` untuk tanggal lahir. Tombol Daftar digunakan untuk mengirim form, sedangkan tombol Reset digunakan untuk mengosongkan input.

### 4. Radio Button dan Checkbox

**Tujuan:** Membuat pilihan jenis kelamin menggunakan radio button dan pilihan keahlian menggunakan checkbox.

**CODING:**

```html
<h2>Jenis Kelamin</h2>
<input type="radio" id="laki" name="jk" value="L">
<label for="laki">Laki-laki</label>

<input type="radio" id="perempuan" name="jk" value="P">
<label for="perempuan">Perempuan</label>

<h2>Keahlian</h2>
<input type="checkbox" id="html" name="skill" value="HTML">
<label for="html">HTML</label>

<input type="checkbox" id="css" name="skill" value="CSS">
<label for="css">CSS</label>

<input type="checkbox" id="js" name="skill" value="JavaScript">
<label for="js">JavaScript</label>
```

**Screenshot Codingan:**

![Codingan Langkah 4](images/codingan%204.png)

**Hasil Browser:**

![Hasil Browser Langkah 4](images/hasil-browser%204.png)

**Keterangan:**

Radio button digunakan untuk memilih satu pilihan dalam kelompok yang sama. Checkbox digunakan untuk memilih satu atau beberapa pilihan sekaligus.

### 5. Select dan Textarea

**Tujuan:** Membuat pilihan program studi menggunakan select dan kolom alamat menggunakan textarea.

**CODING:**

```html
<label for="prodi">Program Studi</label>
<select id="prodi" name="prodi">
    <option value="">-- Pilih Prodi --</option>
    <option value="ti">Teknik Informatika</option>
    <option value="si">Sistem Informasi</option>
</select>

<br><br>

<label for="alamat">Alamat</label><br>
<textarea id="alamat" name="alamat" rows="5" cols="40"></textarea>
```

**Screenshot Codingan:**

![Codingan Langkah 5](images/codingan%205.png)

**Hasil Browser:**

![Hasil Browser Langkah 5](images/hasil-browser%205.png)

**Keterangan:**

Elemen `select` digunakan untuk menampilkan pilihan yang dapat dipilih oleh pengguna. Elemen `textarea` digunakan untuk memasukkan teks yang lebih panjang, seperti alamat.

### 6. Validasi Form Dasar

**Tujuan:** Menerapkan validasi form menggunakan atribut `required`, `minlength`, `min`, dan `max`.

**CODING:**

```html
<form>
    <label for="nama">Nama</label>
    <input type="text" id="nama" name="nama"
           required minlength="3">

    <label for="email">Email</label>
    <input type="email" id="email" name="email" required>

    <label for="umur">Umur</label>
    <input type="number" id="umur" name="umur"
           min="17" max="60" required>

    <button type="submit">Kirim</button>
</form>
```

**Screenshot Codingan:**

![Codingan Langkah 6](images/codingan%206.png)

**Hasil Browser:**

![Hasil Browser Langkah 6](images/hasil-browser%206.png)

**Keterangan:**

Atribut `required` membuat input wajib diisi. Atribut `minlength="3"` menentukan panjang minimal teks sebanyak tiga karakter. Atribut `min="17"` dan `max="60"` membatasi nilai umur dari 17 sampai 60. Browser akan menampilkan pesan validasi jika input tidak memenuhi ketentuan.

### 7. Membuat Halaman Semantic HTML

**Tujuan:** Menyusun struktur halaman web menggunakan elemen semantic HTML.

**CODING:**

```html
<!DOCTYPE html>
<html>
<head><title>Portal Mahasiswa</title></head>
<body>
<header><h1>Portal Mahasiswa</h1></header>
<nav>
    <a href="#">Beranda</a>
    <a href="#">Profil</a>
    <a href="#">Kontak</a>
</nav>
<main>
    <section>
        <h2>Informasi Akademik</h2>
        <article>
            <h3>Praktikum HTML Lanjutan</h3>
            <p>Mahasiswa mempelajari tabel, form, semantic HTML,
            multimedia, dan validasi.</p>
        </article>
    </section>
    <aside>Informasi tambahan mahasiswa.</aside>
</main>
<footer><p>&copy; 2026 Teknik Informatika</p></footer>
</body>
</html>
```

**Screenshot Codingan:**

![Codingan Langkah 7](images/codingan%207.png)

**Hasil Browser:**

![Hasil Browser Langkah 7](images/hasil-browser%207.png)

**Keterangan:**

Semantic HTML menggunakan elemen yang memiliki makna tertentu. `header` merupakan kepala halaman, `nav` untuk navigasi, `main` untuk konten utama, `section` untuk kelompok konten, `article` untuk konten mandiri, `aside` untuk informasi tambahan, dan `footer` untuk bagian bawah halaman.

### 8. Menambahkan Multimedia

**Tujuan:** Menampilkan audio dan video pada halaman web menggunakan HTML.

**Struktur Folder:**

```text
praktikum-2-html-lanjutan/
├── index.html
└── media/
    ├── audio.mp3
    └── video.mp4
```

**CODING:**

```html
<h2>Audio</h2>
<audio controls>
    <source src="media/audio.mp3" type="audio/mpeg">
    Browser tidak mendukung audio.
</audio>

<h2>Video</h2>
<video controls width="480">
    <source src="media/gojo.mp4" type="gojo/mp4">
    Browser tidak mendukung video.
</video>
```

**Screenshot Codingan:**

![Codingan Langkah 8](images/codingan%208.png)

**Hasil Browser:**

![Hasil Browser Langkah 8](images/hasil-browser%208.png)

**Keterangan:**

Elemen `audio` digunakan untuk menampilkan pemutar audio, sedangkan `video` digunakan untuk menampilkan pemutar video. Atribut `controls` menampilkan kontrol pemutaran. File multimedia harus disimpan sesuai dengan lokasi yang ditentukan pada atribut `src`.

### 9. Proyek Mini — Form Biodata Mahasiswa

**Tujuan:** Menggabungkan materi tabel, form, semantic HTML, dan validasi dasar dalam satu halaman biodata mahasiswa.

**CODING:**

```html
<!DOCTYPE html>
<html>
<head><title>Biodata Mahasiswa</title></head>
<body>
<header><h1>Biodata Mahasiswa</h1></header>
<nav>
    <a href="index.html">Beranda</a>
    <a href="#biodata">Biodata</a>
    <a href="#form">Form</a>
</nav>
<main>
<section id="biodata">
    <h2>Data Mahasiswa</h2>
    <table border="1">
        <tr><th>Data</th><th>Keterangan</th></tr>
        <tr><td>NIM</td><td>31241001</td></tr>
        <tr><td>Nama</td><td>Nama Mahasiswa</td></tr>
        <tr><td>Program Studi</td><td>Teknik Informatika</td></tr>
    </table>
</section>
<section id="form">
    <h2>Form Biodata</h2>
    <form>
        <label for="nama">Nama</label>
        <input type="text" id="nama" name="nama" required>
        <br><br>

        <label for="email">Email</label>
        <input type="email" id="email" name="email" required>
        <br><br>

        <label for="prodi">Program Studi</label>
        <select id="prodi" name="prodi" required>
            <option value="">-- Pilih --</option>
            <option value="ti">Teknik Informatika</option>
            <option value="si">Sistem Informasi</option>
        </select>
        <br><br>

        <label for="alamat">Alamat</label><br>
        <textarea id="alamat" name="alamat" required></textarea>
        <br><br>

        <button type="submit">Simpan</button>
        <button type="reset">Reset</button>
    </form>
</section>
</main>
<footer><p>&copy; 2026 Teknik Informatika</p></footer>
</body>
</html>
```

**Screenshot Codingan:**

![Codingan Langkah 9](images/codingan%209.png)

**Hasil Browser:**

![Hasil Browser Langkah 9](images/hasil-browser%209.png)

**Keterangan:**

Proyek mini ini menggabungkan tabel data mahasiswa, navigasi, form biodata, pilihan program studi, textarea, serta validasi input wajib. Halaman juga menggunakan elemen semantic HTML untuk menyusun struktur konten.

---

1. Apa fungsi <table>, <tr>, <th>, dan <td>?

Jawaban:
<table> berfungsi untuk membuat struktur tabel pada halaman HTML.
<tr> (Table Row) berfungsi untuk membuat baris pada tabel.
<th> (Table Header) berfungsi untuk membuat sel judul atau kepala kolom tabel.
<td> (Table Data) berfungsi untuk membuat sel yang berisi data pada tabel.

Contohnya, pada tabel data mahasiswa, elemen <table> digunakan sebagai wadah tabel, <tr> untuk membuat baris, <th> untuk judul kolom, dan <td> untuk menampilkan data mahasiswa.

2. Apa perbedaan <th> dan <td>?

**Jawaban:**

Perbedaan <th> dan <td> terletak pada fungsi penggunaannya. Elemen <th> digunakan untuk menampilkan judul atau kepala kolom tabel, sedangkan <td> digunakan untuk menampilkan isi atau data pada tabel.
Secara default, teks dalam <th> biasanya ditampilkan tebal dan rata tengah oleh browser. Sementara itu, teks dalam <td> biasanya ditampilkan dengan format normal dan rata kiri.

3. Apa fungsi atribut colspan pada tabel HTML?

**Jawaban:**

Atribut colspan berfungsi untuk menggabungkan dua atau lebih kolom menjadi satu sel secara horizontal pada tabel HTML.

Contohnya, atribut colspan="2" digunakan untuk menggabungkan dua kolom menjadi satu sel. Atribut ini dapat digunakan untuk membuat bagian keterangan atau rata-rata pada tabel agar terlihat lebih rapi.

4. Apa fungsi elemen <form> dalam HTML?

**Jawaban:**

Elemen <form> berfungsi untuk membuat formulir yang digunakan untuk menerima dan mengumpulkan input dari pengguna. Form dapat berisi berbagai jenis input, seperti nama, email, password, tanggal lahir, pilihan, dan alamat.

Data yang dimasukkan dapat dikirim menggunakan tombol submit untuk diproses lebih lanjut. Contohnya, form registrasi mahasiswa digunakan untuk memasukkan data mahasiswa, seperti nama lengkap, email, password, dan tanggal lahir.

5. Apa perbedaan radio button dan checkbox?

**Jawaban:**

Radio button digunakan untuk memilih satu pilihan dari beberapa pilihan dalam kelompok yang sama. Contohnya, memilih satu jenis kelamin.

Sementara itu, checkbox digunakan untuk memilih satu atau beberapa pilihan sekaligus. Contohnya, memilih beberapa keahlian seperti HTML, CSS, dan JavaScript.

Dengan demikian, radio button digunakan ketika hanya satu pilihan yang diperbolehkan, sedangkan checkbox digunakan ketika pengguna boleh memilih lebih dari satu pilihan.

6. Mengapa elemen <label> sebaiknya dihubungkan dengan id input menggunakan atribut for?

**Jawaban:**

Elemen <label> sebaiknya dihubungkan dengan id input menggunakan atribut for agar keterangan input terhubung dengan elemen yang sesuai.

Contohnya, jika <label for="nama"> dihubungkan dengan <input id="nama">, pengguna dapat mengeklik tulisan label untuk memfokuskan input tersebut. Hubungan ini juga membantu teknologi pembaca layar mengenali keterangan dari input, sehingga formulir lebih mudah diakses.

7. Apa perbedaan <textarea> dengan <input type="text">?

**Jawaban:**

Elemen <textarea> digunakan untuk memasukkan teks yang panjang dan dapat terdiri dari beberapa baris, seperti alamat, deskripsi, atau komentar.

Sementara itu, <input type="text"> digunakan untuk memasukkan teks dalam satu baris, seperti nama, kota, atau data singkat lainnya.
Jadi, <textarea> lebih sesuai untuk teks panjang, sedangkan <input type="text"> lebih sesuai untuk teks singkat.

8. Apa fungsi semantic HTML seperti <header>, <nav>, <main>, <section>, <article>, <aside>, dan <footer>?

**Jawaban:**

Semantic HTML berfungsi untuk menyusun struktur halaman web menggunakan elemen yang memiliki makna dan tujuan yang jelas. Berikut fungsi masing-masing elemen:
<header> Menampilkan bagian kepala halaman atau bagian tertentu, seperti judul dan pengantar.
<nav> Menampung tautan navigasi untuk berpindah ke halaman atau bagian lain.
<main> Menampung konten utama halaman web.
<section> Mengelompokkan konten yang memiliki tema atau pembahasan yang sama.
<article> Menampung konten mandiri, seperti artikel atau berita.
<aside> Menampilkan informasi tambahan yang berkaitan dengan konten utama.
<footer> Menampilkan bagian penutup halaman, seperti informasi hak cipta.

Penggunaan semantic HTML membuat struktur kode lebih terorganisasi, mudah dibaca, dan membantu browser serta teknologi bantu memahami bagian-bagian halaman web.

9. Apa fungsi atribut required, min, max, dan minlength?

**Jawaban:**

Atribut-atribut tersebut digunakan untuk melakukan validasi dasar pada input HTML.

required berfungsi untuk mewajibkan pengguna mengisi suatu input sebelum form dapat dikirim.

min berfungsi untuk menentukan nilai minimum yang diperbolehkan pada input yang mendukung batas nilai, seperti angka dan tanggal.

max berfungsi untuk menentukan nilai maksimum yang diperbolehkan pada input yang mendukung batas nilai.

minlength berfungsi untuk menentukan jumlah karakter minimum yang harus dimasukkan pada input teks.

Contohnya, min="17" dan max="60" pada input umur menetapkan rentang umur 17 sampai 60. Sementara itu, minlength="3" mengharuskan teks memiliki minimal tiga karakter.

Atribut tersebut membantu mengurangi kesalahan pengisian data sebelum formulir dikirim.

10. Apa perbedaan elemen <audio> dan <video>?

**Jawaban:**

Elemen <audio> digunakan untuk menampilkan dan memutar berkas audio, seperti musik atau rekaman suara. Sementara itu, elemen <video> digunakan untuk menampilkan dan memutar berkas video yang umumnya terdiri dari gambar bergerak dan dapat disertai suara.

Keduanya dapat menggunakan atribut controls untuk menampilkan kontrol pemutaran, seperti tombol play, pause, dan pengaturan volume. Elemen <video> juga dapat menggunakan atribut width untuk mengatur lebar tampilan video.

Jadi, <audio> digunakan untuk media suara, sedangkan <video> digunakan untuk media gambar bergerak yang dapat disertai suara.

## Kesimpulan

Berdasarkan praktikum HTML Lanjutan, dapat disimpulkan bahwa HTML dapat digunakan untuk membuat halaman web yang memiliki struktur dan konten yang lebih lengkap. Melalui praktikum ini, mahasiswa mempelajari cara membuat tabel, formulir, radio button, checkbox, select, textarea, semantic HTML, serta menambahkan elemen multimedia.

Selain itu, penggunaan atribut validasi dasar dapat membantu memastikan bahwa data yang dimasukkan oleh pengguna sesuai dengan ketentuan. Seluruh materi tersebut diterapkan dalam proyek mini berupa halaman biodata mahasiswa.

## Dokumentasi

Seluruh screenshot codingan dan hasil browser disimpan dalam folder `screenshots`. Dokumentasi ini digunakan sebagai bukti pengerjaan setiap langkah praktikum.