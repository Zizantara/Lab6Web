🌐 Praktikum 6: Twitter Bootstrap

Mata Kuliah: Pemrograman Web 1
Nama: Zizantara Arzeva Cakra Kahana
NIM: 312410398
Kelas: TI.24.A.3
Dosen: Agung Nugroho, S.Kom., M.Kom.

🎯 Tujuan Praktikum

Mahasiswa memahami konsep CSS Framework.

Mahasiswa memahami apa itu Twitter Bootstrap dan cara menggunakannya.

Mahasiswa mampu menerapkan Bootstrap Grid System untuk membuat layout responsif.

Mahasiswa dapat menggunakan komponen dasar Bootstrap seperti Navbar, Button, Card, dan Form.

Mahasiswa mampu merefaktor layout web sederhana menggunakan Bootstrap.

🧠 Dasar Teori

Bootstrap adalah framework CSS yang dikembangkan oleh Twitter untuk mempercepat pembuatan tampilan web yang responsif.
Framework ini menyediakan sistem grid 12 kolom, serta berbagai komponen siap pakai seperti navbar, tombol, form, dan card.

Beberapa konsep penting:

`.container` dan `.container-fluid` untuk pembungkus layout.

`.row` untuk baris dalam grid.

`.col-md-*` untuk kolom dengan ukuran berbeda berdasarkan perangkat.

`.navbar`, `.card`, `.btn`, dan `.form-control` adalah komponen utama yang mempermudah styling HTML.

⚙️ Persiapan

Buat folder proyek baru dengan nama lab6_bootstrap.

Unduh atau sertakan Bootstrap CDN pada setiap file HTML.

Buat tiga file halaman utama:

`home.html`

`about.html`

`kontak.html`

Semua file dihubungkan melalui Navbar Bootstrap.

🧩 1. Refactor Layout Praktikum 4
Sebelum

Layout sebelumnya menggunakan CSS manual dengan float, clear, dan margin.

Sesudah

Refactor layout menggunakan Bootstrap Grid System.

Kode:

File: `home.html`
```
<div class="container my-4">
  <div class="row">
    <div class="col-md-8">
      <div class="card">
        <div class="card-body">
          <h3 class="card-title">Selamat Datang</h3>
          <p class="card-text">Ini adalah layout web sederhana dengan Bootstrap.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4">
      <div class="card">
        <div class="card-header bg-primary text-white">Widget</div>
        <div class="card-body">
          <ul class="list-unstyled">
            <li><a href="#">Widget Link 1</a></li>
            <li><a href="#">Widget Link 2</a></li>
            <li><a href="#">Widget Link 3</a></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</div>
```
Komponen yang digunakan:

`.container`, `.row`, `.col-md-*`

`.card`, `.btn`, `.navbar`

📸 Screenshot hasil:

<img src="/hasil/home.png">

🧾 2. Refactor Form Praktikum 5

Formulir dari Praktikum 5 diubah agar rapi menggunakan class Bootstrap.

File: `kontak.html`
```
<form>
  <div class="mb-3">
    <label for="nama" class="form-label">Nama</label>
    <input type="text" class="form-control" id="nama" placeholder="Masukkan nama anda">
  </div>
  <div class="mb-3">
    <label for="email" class="form-label">Email</label>
    <input type="email" class="form-control" id="email" placeholder="Masukkan email anda">
  </div>
  <div class="mb-3">
    <label for="pesan" class="form-label">Pesan</label>
    <textarea class="form-control" id="pesan" rows="4" placeholder="Tulis pesan anda di sini..."></textarea>
  </div>
  <button type="submit" class="btn btn-primary">Kirim</button>
</form>
```

Komponen yang digunakan:

`.form-label`

`.form-control`

`.btn`

`.mb-3`

📸 Screenshot hasil:

<img src="/hasil/kontakl.png">

💼 3. Tugas: Halaman Portfolio Sederhana

File: `about.html`
Berisi section “Tentang Saya” dan section “Portfolio Saya”.
```
<div class="container my-5">
  <div class="row align-items-center">
    <div class="col-md-4">
      <img src="https://dummyimage.com/300x300/ccc/fff" class="img-fluid rounded-circle shadow" alt="Foto Saya">
    </div>
    <div class="col-md-8">
      <h2>Tentang Saya</h2>
      <p>Saya mahasiswa Universitas Pelita Bangsa yang sedang belajar pemrograman web.</p>
    </div>
  </div>

  <h3 class="mt-5">Portfolio Saya</h3>
  <div class="row">
    <div class="col-md-4">
      <div class="card">
        <img src="https://dummyimage.com/400x250/007bff/fff" class="card-img-top">
        <div class="card-body">
          <h5 class="card-title">Proyek 1</h5>
          <p class="card-text">Aplikasi manajemen inventaris berbasis web.</p>
        </div>
      </div>
    </div>
  </div>
</div>
```

Komponen yang digunakan:

`.img-fluid`

`.row dan .col-md-*`

`.card`

`.container`

📸 Screenshot hasil:

<img src="/hasil/about.png">

🌍 4. Navigasi Antar Halaman

Semua halaman dihubungkan melalui Navbar Bootstrap:
```
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="home.html">Layout Sederhana</a>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link active" href="home.html">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="about.html">About</a></li>
        <li class="nav-item"><a class="nav-link" href="kontak.html">Kontak</a></li>
      </ul>
    </div>
  </div>
</nav>
```

🧱 5. Struktur Folder
lab6_bootstrap/
│
├── home.html
├── about.html
├── kontak.html
└── README.md

✅ Kesimpulan

Dengan menggunakan Bootstrap, layout web menjadi lebih rapi dan responsif.

Tidak perlu lagi menulis banyak kode CSS manual.

Komponen seperti card, navbar, dan form sangat membantu mempercepat pembuatan tampilan.

Bootstrap Grid System menggantikan penggunaan float dan clear.

📚 Referensi

Dokumentasi Resmi Bootstrap 5

Modul Praktikum Pemrograman Web 1 — Universitas Pelita Bangsa
