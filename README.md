# Lab4Web
# Laporan Praktikum 4: CSS Layout

## Langkah-Langkah Praktikum

### 1. Membuat Box Element dan CSS Float
* **Penjelasan**: Membuat file HTML dasar untuk mempelajari konsep *box element* menggunakan tag `<div>` serta menerapkan properti `float: left` agar kotak-kotak elemen dapat berjejer secara horizontal[cite: 31, 33].
* **Screenshot**:
<img width="1366" height="738" alt="Screenshot from 2026-10-12 10-33-10" src="https://github.com/user-attachments/assets/4122fd9f-afa4-4e28-9927-a581bac8beaa" />


### 2. Mengatur Clearfix Element
* **Penjelasan**: Menambahkan elemen `div4` dan menggunakan properti `clear: left` untuk mengatasi efek mengambang (*float*) dari elemen sebelumnya sehingga tata letak kembali normal ke bawah[cite: 34].
* **Screenshot**:
<img width="1366" height="738" alt="Screenshot from 2026-10-12 10-34-11" src="https://github.com/user-attachments/assets/683f7727-24ca-4e24-aebf-2a9316f1a78c" />


### 3. Membuat Kerangka Layout Sederhana (`home.html` & `style.css`)
* **Penjelasan**: Membangun kerangka layout web menggunakan elemen semantic HTML5 (`<header>`, `<nav>`, `<section>`, `<aside>`, `<footer>`) di dalam wadah kontainer utama berukuran `980px` yang dipusatkan dengan `margin: 0 auto`[cite: 32, 35, 36, 37].
* **Screenshot**:
<img width="1366" height="738" alt="Screenshot from 2026-10-12 10-35-23" src="https://github.com/user-attachments/assets/af99193b-503e-4269-b0cc-df8f453dc93f" />


### 4. Membuat Navigasi dan Hero Panel
* **Penjelasan**: Mengatur tampilan menu navigasi dengan latar belakang biru serta menyusun *Hero Panel* (bagian sambutan utama dengan judul, teks paragraf, dan tombol aksi "Learn more") menggunakan background abu-abu terang[cite: 38, 39].
* **Screenshot**:
<img width="1366" height="738" alt="Screenshot from 2026-10-12 10-42-08" src="https://github.com/user-attachments/assets/e6a37448-af4d-4210-ae40-eeebaee0ad6f" />


### 5. Mengatur Layout Main Content dan Sidebar Widget
* **Penjelasan**: Membagi area kontainer utama (`#wrapper`) menjadi dua kolom menggunakan properti float: area konten utama (`#main` dengan lebar 640px) di sebelah kiri dan area samping (`#sidebar` dengan lebar 260px) yang berisi kotak widget navigasi dan teks di sebelah kanan[cite: 39, 40].
* **Screenshot**:
<img width="1366" height="738" alt="Screenshot from 2026-10-12 11-11-05" src="https://github.com/user-attachments/assets/960a3e5d-303f-4110-8b07-312b62fe609f" />


### 6. Mengatur Footer
* **Penjelasan**: Menata bagian kaki halaman (`<footer>`) dengan latar belakang gelap (`#1d1d1d`) serta menyematkan properti `clear: both` agar posisinya selalu berada di bawah elemen yang menggunakan *float*[cite: 41].
* **Screenshot**:
<img width="1366" height="738" alt="Screenshot from 2026-10-12 11-11-23" src="https://github.com/user-attachments/assets/868c0b96-f55e-471a-b155-9b71c47d24c9" />


### 7. Menambahkan Kolom Konten Tiga Kotak (Boxes)
* **Penjelasan**: Menambahkan tiga kolom kotak berdampingan di dalam *main content* yang masing-masing berisi gambar ikon berbentuk lingkaran (`image-circle`), judul (*heading*), paragraf singkat, dan tombol detail[cite: 41, 42].
* **Screenshot**:
<img width="1366" height="738" alt="Screenshot from 2026-10-12 11-12-58" src="https://github.com/user-attachments/assets/21799f3e-d466-49ec-b3e2-055000f5107e" />


### 8. Menambahkan Konten Artikel Berformat Khusus
* **Penjelasan**: Membuat bagian artikel berita/fitur tambahan menggunakan tag `<article>` dan class `.entry`, lengkap dengan pengaturan posisi gambar di sebelah kiri dan kanan teks (`right-img`) serta garis pemisah (`divider`)[cite: 43, 44].
* **Screenshot**:
<img width="1366" height="738" alt="Screenshot from 2026-10-12 17-47-10" src="https://github.com/user-attachments/assets/c389e718-9be1-437d-a58a-8c5ea73f939a" />
*

---

## Jawaban Pertanyaan dan Tugas

### 1. Membuat Layout untuk Menu About (`about.html`)
  <!DOCTYPE html>
<html lang="en">
<head>
        <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Layout Sederhana</title>
            <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
    </div>
<header>
    <h1>Layout Sederhana</h1>
</header>
<nav>
    <a href="home.html">Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html"class="active">About</a>
    <a href="kontak.html">Kontak</a>
</nav>
<section id="hero">
    <h1>About Me</h1>
        <p>
        Saya Eirenetrian Bagus Prakoso mahasiswa Universitas Pelita Bangsa Program Studi 
        Teknik Informatika.
        Saat ini saya sedang mempelajari dasar-dasar pengembangan
        aplikasi web menggunakan HTML dan css.
        </p>
<section id="wrapper">
    <section id="main">
         <div class="row">
            <div class="box">
                <img src="/home/eren/Pictures/html.png" width="100" height="100" alt=""
                class="image-circle">
                <h3>HTML</h3>
                <p></p>
                <a href="#" class="btn btn-default">View detail</a>
            </div>
             <div class="row">
            <div class="box">
                <img src="/home/eren/Pictures/css.png" width="100" height="100" alt=""
                class="image-circle">
                <h3>CSS</h3>
                <p></p>
                <a href="#" class="btn btn-default">View detail</a>
            </div>
    </section>
    <aside id="sidebar"></aside>
<footer>
    <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
</body>
</html>
Tampilan di Browser :
               
### 2. Membuat Layout untuk Menu Comtact (`contact.html`)
<!DOCTYPE html>
<html lang="en">
<head>
        <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Layout Sederhana</title>
            <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
    </div>
<header>
    <h1>Layout Sederhana</h1>
</header>
<nav>
    <a href="home.html" >Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html">About</a>
    <a href="kontak.html"class="active">Kontak</a>
</nav>
<section id="hero">
    <h1>Hubungi Kami</h1>
    <p> <h3>Info Kontak</h3>
                <p><strong>Alamat:</strong><br>Jl. Inspeksi Kalimalang, Cikarang, Bekasi</p>
                <p><strong>Email:</strong><br>info@pelitabangsa.ac.id</p>
                <p><strong>Telepon:</strong><br>(021) 88375512</p>
            </div>                

                <h3>Jam Operasional</h3>
                <p>Senin - Jumat: 08:00 - 16:00 WIB</p>
                <p>Sabtu - Minggu: Libur</p></p>
</section>
<section id="wrapper">
    <section id="main"></section>
    <aside id="sidebar"></aside>
</section>
<footer>
    <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
</body>
</html>
Tampilan di Browser :
