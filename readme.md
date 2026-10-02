Berikut adalah draf isi _e-book_ ringkas dan mudah dipahami yang disusun berdasarkan kurikulum 7 langkah. Anda dapat menyalin teks ini menjadi format PDF atau membagikannya langsung.

---

# 📘 Buku Pintar Web Developer Pemula: Menguasai HTML & CSS Tanpa Pusing

Selamat datang di dunia pengembangan web! Buku ini dirancang khusus untuk pemula yang ingin belajar membuat website dari nol. Kita tidak akan menggunakan teknik yang rumit dulu, melainkan fokus pada fondasi utama: **HTML** sebagai kerangka, dan **CSS** sebagai desain.

Mari kita mulai perjalanan 7 langkah ini!

---

## Pembelajaran 1: HTML Fundamental (Membangun Kerangka)

Bayangkan Anda sedang membangun rumah. HTML (HyperText Markup Language) adalah batu bata dan semen penyusun kerangkanya. Tanpa HTML, tidak ada website.

**Struktur Wajib Sebuah Website:**
Setiap halaman web harus memiliki struktur dasar ini agar bisa dibaca oleh _browser_ (seperti Chrome atau Safari):

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Informasi rahasia untuk browser (judul tab, font, dll) -->
  </head>
  <body>
    <!-- Semua yang Anda lihat di layar ada di sini! -->
  </body>
</html>
```

**Elemen-elemen Penting di dalam `<body>`:**

- **Heading:** Judul teks dari tingkat 1 hingga 6 (`<h1>` sampai `<h6>`).
- **Paragraph:** Teks biasa (`<p>`).
- **Link:** Tautan untuk berpindah halaman (`<a href="url">Klik di sini</a>`).
- **Image:** Menampilkan gambar (`<img src="foto.jpg" alt="Deskripsi">`).
- **List:** Membuat daftar berurutan (`<ol>`) atau poin-poin (`<ul>`) dengan isi (`<li>`).
- **Atribut Khusus:** `class` (untuk mengelompokkan elemen) dan `id` (identitas unik elemen).

> **🎯 Latihan Praktik 1:**
> Buatlah satu file HTML (`index.html`). Di dalamnya, buat halaman profil diri Anda yang berisi foto, nama (`<h1>`), deskripsi singkat (`<p>`), dan daftar hobi (`<ul>`).

---

## Pembelajaran 2: Semantic HTML (Memberi Makna pada Kerangka)

Di masa lalu, orang membangun web dengan tag generik bernama `<div>` untuk segalanya. Kini, kita menggunakan **Semantic HTML**, yaitu tag yang namanya mendeskripsikan fungsinya. Ini sangat disukai oleh mesin pencari seperti Google!

Bayangkan rumah Anda sekarang sudah memiliki papan nama untuk setiap ruangan:

- `<header>` : Bagian paling atas website (biasanya berisi logo).
- `<nav>` : Menu navigasi (Beranda, Tentang, Kontak).
- `<main>` : Konten utama halaman.
- `<section>` : Bagian spesifik dari konten (misal: "Layanan Kami").
- `<article>` : Konten mandiri yang bisa berdiri sendiri (seperti postingan blog).
- `<aside>` : Konten tambahan di samping (sidebar).
- `<footer>` : Bagian paling bawah (hak cipta, link sosial media).

Selain itu, Anda juga mulai mengenal **Basic Form** (`<form>`, `<input>`, `<button>`) untuk membuat tempat input data seperti kolom pencarian.

> **🎯 Latihan Praktik 2:**
> Modifikasi file HTML profil Anda. Masukkan logo dan menu ke dalam `<header>`, konten profil ke `<main>`, dan hak cipta di `<footer>`.

---

## Pembelajaran 3: CSS Fundamental (Mengecat Rumah Anda)

Kerangka sudah jadi, saatnya mendesain! CSS (Cascading Style Sheets) bertugas mengatur warna, ukuran, dan bentuk elemen HTML Anda.

**Cara Memanggil CSS:**
Anda bisa menulis CSS langsung di elemen (_Inline_), di dalam `<head>` (_Internal_), atau di file terpisah (_External_ - **sangat direkomendasikan**).

**Apa saja yang bisa diubah oleh CSS?**
Untuk mengubah elemen, Anda perlu memanggil namanya (**CSS Selectors**), lalu memberikan gaya:

```css
h1 {
  color: blue; /* Mengubah warna teks */
  background: yellow; /* Mengubah warna latar belakang */
  font-family: Arial, sans-serif; /* Mengubah jenis huruf */
  border: 1px solid black; /* Memberi garis tepi */
  border-radius: 10px; /* Membuat sudut garis menjadi membulat */
  width: 500px; /* Mengatur lebar */
  height: 100px; /* Mengatur tinggi */
}
```

> **🎯 Latihan Praktik 3:**
> Buat file `style.css`. Hubungkan ke HTML Anda. Ubah warna teks halaman profil Anda, ganti jenis hurufnya, dan berikan warna latar belakang yang menarik.

---

## Pembelajaran 4: CSS Box Model (Rahasia Tata Letak Web)

Ini adalah konsep terpenting dalam CSS! Di dunia web, **semua elemen adalah kotak (box)**.

Bayangkan sebuah lukisan berbingkai:

1. **Content:** Kanvas lukisannya (teks/gambar).
2. **Padding:** Jarak antara kanvas ke bingkai (ruang bernapas di dalam).
3. **Border:** Bingkai kayunya itu sendiri.
4. **Margin:** Jarak dari bingkai ke lukisan lain di sebelahnya (jarak luar).

**Properti Penting Box Model:**

- `box-sizing: border-box;` : Wajib digunakan agar _padding_ dan _border_ tidak membuat ukuran elemen menjadi membengkak.
- `max-width` / `min-width` : Batas maksimal/minimal kelebaran suatu kotak.
- `display` : Menentukan sifat kotak (apakah ia berjejer ke samping atau ke bawah).
- `overflow` : Apa yang terjadi jika isi konten lebih besar dari kotaknya? (bisa disembunyikan atau diberi _scroll_).

> **🎯 Latihan Praktik 4:**
> Buatlah 3 "Card" (kartu profil/produk) di HTML. Gunakan CSS untuk memberi Padding, Border, dan Margin yang berbeda-beda agar Anda merasakan perbedaannya secara visual.

---

## Pembelajaran 5: CSS Layout - Float & Clear (Menyusun Tata Letak)

Bagaimana cara membuat teks berada di kiri, dan gambar di kanan? Sebelum ada teknologi modern, developer web menggunakan teknik **Float**.

_Float_ bekerja dengan menarik sebuah elemen "keluar dari aliran normal" dan memaksanya merapat ke kiri (`float: left`) atau ke kanan (`float: right`). Elemen teks di bawahnya akan mengalir mengelilingi elemen tersebut (seperti teks mengelilingi gambar di koran).

**Masalah Float & Solusinya:**
Jika sebuah kotak induk berisi anak-anak yang di-float, kotak induk tersebut akan "kempis" karena merasa tidak ada isinya (Masalah Tinggi Parent).

- **Solusi:** Gunakan perintah `clear: both` pada elemen setelahnya, atau gunakan teknik _clearfix_ untuk mengembalikan aliran halaman menjadi normal kembali.

> **🎯 Latihan Praktik 5:**
> Buatlah struktur layout klasik menggunakan Float seperti diagram di bawah ini:
> ┌──────────────────────┐
> │ Header │
> ├─────────┬────────────┤
> │ Sidebar │ Content │
> ├─────────┴────────────┤
> │ Footer │
> └──────────────────────┘

---

## Pembelajaran 6: Responsive Design & Basic UI (Tampil Sempurna di Semua Layar)

Website Anda mungkin terlihat bagus di laptop, tapi bagaimana jika dibuka di HP? Berantakan! Di sinilah **Responsive Design** masuk.

**Senjata Utama: Media Queries**
Media query memungkinkan kita mengubah desain berdasarkan lebar layar (`Breakpoints`).

```css
/* Desain default (Mobile-first) */
.sidebar {
  width: 100%;
  float: none;
}

/* Jika layar lebih lebar dari 768px (Tablet/Desktop) */
@media screen and (min-width: 768px) {
  .sidebar {
    width: 30%;
    float: left;
  }
}
```

_Gunakan relative units seperti `%` (persentase) alih-alih `px` agar gambar dan kotak bisa meregang secara fleksibel._

**Basic UI (Antarmuka Pengguna):**
Desain yang baik harus nyaman dilihat. Perhatikan:

- **Visual Hierarchy:** Teks terpenting harus paling besar/tebal.
- **Spacing:** Beri jarak (margin/padding) yang cukup antar elemen. Jangan berdesakan.
- **Interaksi:** Tambahkan efek `hover` (berubah saat disentuh mouse) atau `focus` pada _Button_ (tombol) agar website terasa lebih "hidup".

> **🎯 Latihan Praktik 6:**
> Ubah layout dari Pembelajaran 5 menjadi responsif. Di layar HP, Sidebar berada di bawah Content. Di layar Laptop, Sidebar kembali berada di kiri Content.

---

## Pembelajaran 7: Practice & Portfolio (Gabungkan Semuanya!)

Teori tanpa praktik akan cepat hilang. Sekarang Anda sudah memiliki semua senjata yang dibutuhkan untuk membuat website statis.

Biasakan alur kerja sistematis ini saat mengerjakan proyek:
**HTML → Semantic HTML → CSS Dasar → Box Model → Layout (Float/Clear) → Responsive → UI (Warna/Tipografi).**

**Misi Terakhir Anda:**
Buat beberapa proyek nyata dari nol tanpa melihat tutorial (menyontek catatan/Googling diperbolehkan):

1. **Personal Profile:** CV online Anda.
2. **Portfolio:** Galeri karya atau foto Anda.
3. **Blog Layout:** Halaman daftar artikel dan halaman baca artikel.
4. **Product Page:** Halaman untuk berjualan 1 barang lengkap dengan gambar dan tombol beli.
5. **Company Profile:** Halaman profil bisnis dengan beberapa halaman (Home, About, Contact).

**Target Akhir:**
Jika Anda berhasil menyelesaikan proyek-proyek di atas, **Selamat!** Anda kini sudah mampu membuat website statis sederhana dari nol. Fondasi Anda sudah cukup kuat untuk melangkah ke materi web tingkat lanjut seperti tata letak CSS Modern (Flexbox & Grid) atau membuat web menjadi interaktif dengan JavaScript.

Teruslah berkarya!
