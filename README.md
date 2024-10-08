# Lab2Web
1. Membuat Dokumen HTML
Pada langkah pertama, Anda diminta untuk membuat dokumen HTML yang mendefinisikan struktur dasar halaman web. Berikut adalah penjelasannya:
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CSS Dasar</title>
</head>
<body>
<header>
<h1>CSS Internal dan <i>Inline CSS</i></h1>
</header>
<nav>
<a href="lab2_css_dasar.html">CSS Dasar</a>
<a href="lab2_css_eksternal.html">CSS Eksternal</a>
<a href="lab1_tag_dasar.html">HTML Dasar</a>
</nav>
<!-- CSS ID Selector -->
<div id="intro">
<h1>Hello World</h1>
<p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</p>
<!-- CSS Class Selector -->
<a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
</div>
</body>
</html>

![Screenshot 2024-10-08 040217](https://github.com/user-attachments/assets/b44b0d85-c042-4b5a-91b8-ec3fb4684245)

Penjelasan: Dokumen HTML ini memuat elemen-elemen seperti header, nav, dan div yang digunakan untuk mengelola struktur halaman. Teks “CSS Internal dan Inline CSS” ditampilkan sebagai judul halaman, dan terdapat tautan navigasi ke beberapa halaman lain.

2. Mendeklarasikan CSS Internal
Tambahkan CSS internal pada bagian <head> dokumen HTML. Berikut adalah kode CSS yang dimasukkan untuk mengatur gaya elemen pada halaman.

<head>
<title>CSS Dasar</title>
<style>
body {
font-family:'Open Sans', sans-serif;
}
header {
min-height: 80px;
border-bottom:1px solid #77CCEF;
}
h1 {
font-size: 24px;
color: #0F189F;
text-align: center;
padding: 20px 10px;
}
h1 i {
color:#6d6a6b;
}
</style>
</head>

![Screenshot 2024-10-08 040305](https://github.com/user-attachments/assets/2216b8b5-68ff-47c2-b1f0-ba085ba701f4)

Penjelasan: CSS internal ini memberikan gaya pada elemen-elemen seperti body, header, dan h1. Misalnya, font pada seluruh halaman diatur menjadi Open Sans, dan h1 memiliki ukuran font 24px, berwarna biru, dan berada di tengah.

3. Menambahkan Inline CSS
Tambahkan inline CSS pada tag <p> untuk memberikan gaya tambahan langsung pada elemen tersebut. Berikut contohnya:

<p style="text-align: center; color: #ccd8e4;">
  
![image](https://github.com/user-attachments/assets/5daa023e-c8ff-4d58-be72-77b6b5fbd0d2)

Penjelasan: Inline CSS ini memberikan gaya langsung pada elemen <p>, dengan teks diatur agar rata tengah dan berwarna biru muda (#ccd8e4).

4. Membuat CSS Eksternal
Langkah berikutnya adalah membuat file CSS eksternal bernama style_eksternal.css. Berikut adalah kode CSS yang dimasukkan ke dalam file tersebut:

nav {
  background: #20A759;
  color: #fff;
  padding: 10px;
}
nav a {
  color: #fff;
  text-decoration: none;
  padding: 10px 20px;
}
nav .active,
nav a:hover {
  background: #0B6B3A;
}

Setelah membuat file CSS eksternal, tambahkan tautan ke file tersebut di bagian <head> dokumen HTML:

<head>
  <!-- menyisipkan css eksternal -->
  <link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>

![Screenshot 2024-10-08 041927](https://github.com/user-attachments/assets/ff897ab7-3d75-445f-8aca-9f7d1d11ecb8)

Penjelasan: Dengan menyimpan gaya CSS di file terpisah (style_eksternal.css), Anda memisahkan pengaturan tampilan dari konten HTML. Kode CSS ini memberikan warna hijau pada latar belakang navigasi (nav), mengubah warna teks menjadi putih, dan memberikan efek hover pada tautan.

5. Menambahkan CSS Selector
CSS selector digunakan untuk memilih elemen HTML berdasarkan ID atau class. Berikut adalah tambahan kode untuk ID dan Class Selector pada file style_eksternal.css:

/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}

![Screenshot 2024-10-08 042026](https://github.com/user-attachments/assets/2eb57fd5-fae1-44b0-b7a6-5c93a11130d9)

Penjelasan: Kode ini memberikan gaya khusus untuk elemen-elemen berdasarkan ID. Elemen dengan ID merah memiliki teks berwarna merah, rata-tengah diatur rata tengah dengan ukuran font 12pt, dan serif menggunakan font sans-serif.
