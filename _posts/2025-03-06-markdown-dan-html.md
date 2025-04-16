---
 layout: Belajar Markdown & HTML
 title: "Belajar Markdown & HTML"
 date: 2025-03-06
 ---
 

 Materi tentang Markdown dan HTML
 
 Pada pertemuan ini, kami belajar menulis konten menggunakan **Markdown**, yaitu format penulisan yang lebih simpel dibanding HTML.
 # 📘 Belajar Markdown dan HTML
 
 Beberapa hal yang kami pelajari:
 ## 📝 Apa Itu Markdown?
 
 - Heading (`#`), list, link, dan emphasis (**tebal**, _miring_)
 - Perbandingan penulisan Markdown vs HTML
 - Struktur dasar file `.md` di Jekyll
 - Bagaimana Markdown di-render otomatis menjadi HTML oleh Jekyll
 **Markdown** adalah bahasa markup ringan yang digunakan untuk memformat teks dengan cara yang mudah dibaca dan ditulis.
 
 Markdown banyak digunakan untuk:
 - README file di GitHub
 - Dokumentasi
 - Blog berbasis Jekyll atau Hugo
 
 ---
 
 ### 📌 Contoh Penulisan Markdown
 
 #### 1. Heading
 
 
 # Judul H1
 ## Subjudul H2
 ### Sub-subjudul H3 
 
 
 #### 2. Teks
 
 
 **Tebal**  
 _Miring_  
 ~~Coret~~  
 `Code`
 
 
 #### 3. List
 
 
 - Item 1
 - Item 2
   - Sub-item
 
 1. Pertama
 2. Kedua
 
 
 #### 4. Link dan Gambar
 
 
 [Klik Link Ini](https://m-zakifahrezi.github.io/OnlyJack.com/)
 
 ![Gambar](/assets/images/coding.png)
 
 
 #### 5. Code Block
 
 Markdown sering dianggap sebagai alternatif dari HTML karena kemudahan penggunaannya. Beberapa perbandingan antara keduanya adalah:
 
 HTML: Memerlukan lebih banyak tag dan atribut untuk mendefinisikan elemen-elemen di halaman, seperti <h1>, <ul>, <ol>, <li>, <a>, <strong>, dan sebagainya. Walaupun sangat fleksibel, HTML bisa menjadi lebih rumit untuk penulisan konten yang sederhana.
 
 Markdown: Menyederhanakan proses penulisan dengan menggunakan karakter-karakter tertentu, seperti # untuk heading dan - untuk daftar, sehingga membuatnya lebih cepat dan lebih mudah digunakan.
 <h1>Hello World</h1>
 
 3. Struktur Dasar File .md di Jekyll
    Dalam proyek Jekyll, file Markdown memiliki ekstensi .md dan digunakan untuk menulis konten. Jekyll akan secara otomatis mengonversi file Markdown menjadi HTML saat diproses. Struktur dasar file .md di Jekyll adalah sebagai berikut:
 
 Setiap file Markdown di Jekyll dimulai dengan bagian Front Matter yang berisi metadata seperti judul, tanggal, dan layout. Ini biasanya diawali dengan tanda ---.
 
 Setelah bagian Front Matter, konten utama ditulis menggunakan sintaks Markdown yang kemudian akan diterjemahkan menjadi HTML oleh Jekyll.
 ---
 
 ## 🌐 Apa Itu HTML?
 
 **HTML (HyperText Markup Language)** adalah bahasa standar untuk membuat dan menyusun halaman web.
 
 HTML digunakan untuk:
 - Struktur konten halaman web
 - Menampilkan teks, gambar, link, video, dan elemen lainnya
 
 ---
 
 ### 📌 Struktur Dasar HTML
 
 
 <!DOCTYPE html>
 <html>
   <head>
     <title>Judul Halaman</title>
   </head>
   <body>
     <h1>Halo Dunia</h1>
     <p>Ini paragraf pertama saya.</p>
     <a href="https://www.instagram.com/zkyy.frezy?igsh=MXB3N21zbm44ZjdwNw==">Kunjungi media sosial saya</a>
   </body>
 </html>
 
 
 ---
 
 ### 🧩 Elemen HTML Umum
 
 | Tag              | Fungsi               |
 |------------------|----------------------|
 | `<h1>` - `<h6>`  | Heading              |
 | `<p>`            | Paragraf             |
 | `<a>`            | Link                 |
 | `<img>`          | Gambar               |
 | `<ul>`, `<ol>`, `<li>` | Daftar        |
 | `<div>`          | Container umum       |
 | `<span>`         | Inline container     |
 | `<br>`           | Baris baru           |
 
 ---
 
 ## 🤝 Markdown vs HTML
 
 | Markdown               | HTML                              |
 |------------------------|-----------------------------------|
 | Lebih mudah dibaca     | Lebih fleksibel dan powerful      |
 | Ringkas dan cepat      | Cocok untuk kontrol penuh layout  |
 | Sering dipakai di GitHub | Digunakan di semua halaman web |
 
 ---
 
 ## ✅ Kesimpulan
 
 - **Markdown** cocok untuk menulis teks dengan format sederhana seperti dokumentasi, catatan, dan blog post.
 - **HTML** memberikan kontrol penuh atas struktur dan tampilan halaman web.
 - Keduanya saling melengkapi: Markdown cepat dan simpel, HTML fleksibel dan lengkap.
 - Belajar keduanya akan sangat membantu saat membuat konten web atau proyek open source.
 
 Markdown membuat penulisan konten lebih cepat dan nyaman.
 > 💡 Mulailah dari Markdown, lalu perdalam HTML untuk kontrol yang lebih menyeluruh! 🚀