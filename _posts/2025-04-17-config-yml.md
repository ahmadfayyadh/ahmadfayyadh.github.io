---
layout: posts
title: "Config YML"
date: 2025-04-17
---
Materi tentang Config YML

YAML (YAML Ain't Markup Language) adalah format data yang sering digunakan untuk konfigurasi aplikasi karena sintaksnya yang sederhana dan mudah dibaca manusia.

## Struktur Dasar YAML

- Menggunakan indentasi (spasi) untuk menandai level.
- Tidak menggunakan tanda kurung atau kurung kurawal.
- File biasanya memiliki ekstensi `.yml` atau `.yaml`.

## Contoh File config.yml

```yml
app:
  name: MyApplication
  version: 1.0.0
  debug: true

database:
  host: localhost
  port: 3306
  username: user
  password: pass123

logging:
  level: INFO
  path: /var/log/myapp.log
```

## Penjelasan

- `app`: Konfigurasi aplikasi.
- `database`: Konfigurasi database.
- `logging`: Pengaturan log.

## Catatan

- Pastikan indentasi konsisten (biasanya 2 atau 4 spasi).
- Hindari penggunaan tab.
- YAML sensitif terhadap format dan spasi.
