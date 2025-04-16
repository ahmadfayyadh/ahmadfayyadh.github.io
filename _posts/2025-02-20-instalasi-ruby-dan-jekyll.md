---
 layout: post
 title: "Instalasi Ruby dan Jekyll"
 date: 2025-02-20
 ---


 Materi tentang Instalasi Ruby dan Jekyll

 ## Instalasi Ruby dan Jekyll
 # 📘 Panduan Instalasi Jekyll dan Ruby
 
 Pada pertemuan pertama mata kuliah Workshop Web Dasar, kami mempelajari bagaimana cara menginstal **Ruby** dan **Jekyll**, dua komponen penting yang digunakan untuk membangun website statis menggunakan framework Jekyll.
 ## 💎 Apa Itu Ruby & Jekyll?
 
 ### Apa itu Ruby dan Jekyll?
 
 - **Ruby** adalah bahasa pemrograman yang digunakan oleh Jekyll.
 - **Jekyll** adalah static site generator, yaitu alat yang mengubah file teks biasa (Markdown, HTML) menjadi website statis yang bisa langsung di-hosting, misalnya di GitHub Pages.
 - **Ruby** adalah bahasa pemrograman yang digunakan Jekyll.
 - **Jekyll** adalah static site generator berbasis Ruby, populer untuk membuat blog atau dokumentasi (seperti GitHub Pages).
 
 ---
 
 ### Langkah-langkah yang kami lakukan:
 
 1. **Mengunduh dan Menginstal Ruby**
 ## 🔧 Persiapan Awal
 
    Kami mengunjungi situs [https://rubyinstaller.org](https://rubyinstaller.org) untuk pengguna Windows, lalu menginstal Ruby versi terbaru. Untuk pengguna macOS dan Linux, Ruby biasanya sudah tersedia atau dapat diinstal menggunakan terminal.
 ### 1. Install Ruby
 
 2. **Mengecek Ruby di terminal**
 #### ▶ Windows
 
    Setelah instalasi, kami membuka terminal atau command prompt dan mengetik: "ruby -v;"
    untuk memastikan Ruby sudah terinstal dengan benar.
 1. Download dari: [https://rubyinstaller.org](https://rubyinstaller.org)
 2. Pilih versi **Ruby + DevKit**, contoh: `Ruby 3.1.4-1 (x64)`
 3. Setelah instalasi:
    - Centang opsi “Run `ridk install`”
    - Pilih semua komponen (1, 2, dan 3)
 
 3. **Menginstal Bundler dan Jekyll**
 #### ▶ macOS
 
 Dengan Ruby yang sudah terpasang, kami menjalankan perintah berikut: "gem install bundler jekyll"
 Perintah ini akan menginstal Jekyll dan Bundler ke dalam sistem, yang dibutuhkan untuk membuat dan mengelola proyek Jekyll.
 Install via Homebrew:
 
 4. **Membuat Proyek Jekyll Baru**
 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
 brew install ruby
 
 Setelah instalasi selesai, kami membuat project baru dengan: "jekyll new my-website"
 #### ▶ Linux
 
 Ini akan menghasilkan struktur folder Jekyll lengkap di dalam folder `my-website`.
 sudo apt update
 sudo apt install ruby-full build-essential zlib1g-dev
 Tambahkan RubyGems ke PATH:
 echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
 echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
 echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
 source ~/.bashrc
 
 5. **Menjalankan Server Lokal**
 🌟 Instalasi Jekyll
 Setelah Ruby terinstal, jalankan:
 gem install jekyll bundler
 
 Kami masuk ke dalam folder proyek dengan: "cd my-website"
 🚀 Membuat dan Menjalankan Proyek Jekyll
 
 Lalu menjalankan website lokal menggunakan: "jekyll serve"
 1. Membuat proyek baru:
    jekyll new nama-proyek
    cd nama-proyek
 
 Setelah itu, kami membuka browser dan mengakses:
 http://localhost:4000
 2. Menjalankan server lokal:
    bundle exec jekyll serve
    Buka di browser:
    http://localhost:4000
 
 Di situ, kami bisa melihat website statis Jekyll pertama kami berjalan dengan baik.
 🧪 Cek Versi
 ruby -v # versi Ruby
 jekyll -v # versi Jekyll
 
 ---
 
 ### Kesimpulan
 ## ✅ Kesimpulan
 
 Instalasi Jekyll membutuhkan beberapa langkah utama, yaitu:
 
 1. **Menginstal Ruby** – sebagai fondasi karena Jekyll dibangun dengan Ruby.
 2. **Menginstal Jekyll dan Bundler** – menggunakan perintah `gem install`.
 3. **Membuat dan menjalankan proyek Jekyll** – dengan `jekyll new` dan `bundle exec jekyll serve`.
 
 Instalasi Ruby dan Jekyll merupakan langkah awal yang sangat penting sebelum membangun website. Kami jadi memahami bahwa meskipun Jekyll adalah alat sederhana, ia memiliki struktur dan alur kerja yang profesional — dimulai dari pengaturan lingkungan kerja, hingga memulai proyek dan melihat hasilnya secara lokal di browser.
 Dengan mengikuti langkah-langkah ini, kamu sudah siap membangun situs statis menggunakan Jekyll di berbagai sistem operasi (Windows, macOS, atau Linux). Pastikan kamu juga melakukan pengecekan versi dan menyesuaikan jika menggunakan layanan seperti GitHub Pages.
 
 Ini adalah awal dari perjalanan kami sebagai pengembang web.
 > Selamat berkarya dengan Jekyll! 🚀