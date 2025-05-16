---
layout: posts
title: "Membuat Layout Menggunakan SASS/SCSS"
date: 2025-05-07
---
Materi tentang Membuat Layout Menggunakan SASS/SCSS

## Pengantar SASS/SCSS

SASS (Syntactically Awesome Stylesheets) adalah preprocessor CSS yang menambahkan fitur seperti variabel, nesting, mixin, inheritance, dan lainnya. SCSS (Sassy CSS) adalah sintaks SASS yang lebih mirip CSS.

Dengan SASS/SCSS, pengembangan layout website menjadi lebih modular, efisien, dan mudah di-maintain.

## Keuntungan Menggunakan SASS/SCSS untuk Layout

- **Modular**: Memisahkan layout ke dalam file partials.
- **Variabel**: Mempermudah pengaturan ukuran, warna, dll.
- **Nesting**: Struktur CSS lebih rapi mengikuti HTML.
- **Mixins**: Membuat template reusable untuk grid, flexbox, dll.
- **Functions**: Membuat perhitungan otomatis (misal, grid width).

---

## Struktur Folder Layout SCSS

```bash
├── scss/
│   ├── base/
│   ├── components/
│   ├── layout/
│   ├── pages/
│   └── main.scss
```

- **base/**: Reset, typography, dan global styles.
- **components/**: Button, card, alert, dll.
- **layout/**: Header, footer, sidebar, grid.
- **pages/**: Style khusus halaman.
- **main.scss**: File utama yang meng-import semua.

---

## Contoh Layout SCSS

### 1. Variabel

```scss
// _variables.scss
$primary-color: #3498db;
$spacing-unit: 16px;
```

### 2. Grid System dengan Mixin

```scss
// _grid.scss
@mixin row {
  display: flex;
  flex-wrap: wrap;
  margin-right: -$spacing-unit;
  margin-left: -$spacing-unit;
}

@mixin col($size) {
  flex: 0 0 percentage($size / 12);
  max-width: percentage($size / 12);
  padding-right: $spacing-unit;
  padding-left: $spacing-unit;
}
```

### 3. Layout Header & Footer

```scss
// _header.scss
.header {
  background: $primary-color;
  padding: $spacing-unit;
  color: white;
}

// _footer.scss
.footer {
  background: darken($primary-color, 10%);
  padding: $spacing-unit;
  color: white;
}
```

### 4. Menggunakan di `main.scss`

```scss
@import 'variables';
@import 'layout/grid';
@import 'layout/header';
@import 'layout/footer';
```

---

## Contoh HTML Layout

```html
<body>
  <header class="header">Header</header>
  <div class="container">
    <div class="row">
      <div class="col-8">Content</div>
      <div class="col-4">Sidebar</div>
    </div>
  </div>
  <footer class="footer">Footer</footer>
</body>
```

---

## Kompilasi SASS ke CSS

```bash
sass scss/main.scss css/main.css --watch
```

---

## Tips Layout dengan SCSS

- Gunakan **variabel untuk spacing, warna, breakpoints**.
- Gunakan **mixin untuk grid atau flexbox** agar DRY (Don't Repeat Yourself).
- **Organisasi file SCSS dengan rapi**, gunakan partial dan import.
- Manfaatkan **functions SASS untuk kalkulasi dinamis (misal kolom grid)**.

---
