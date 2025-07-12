---
layout: post
title: "Langkah-Langkah Membuat Project Jekyll"
---

Jekyll adalah generator situs statis yang populer, sering digunakan untuk membuat blog atau website sederhana.
Jekyll memungkinkan Anda untuk membuat situs web dengan mudah menggunakan Markdown, Liquid, dan HTML.
Jekyll sangat cocok untuk proyek-programan, dokumentasi, atau blog pribadi.
Jekyll juga merupakan platform yang digunakan oleh GitHub Pages, sehingga Anda bisa langsung meng-host situs Jekyll Anda di GitHub. 
Berikut adalah langkah-langkah dasar untuk membuat project Jekyll:

## 1. **Persiapan Awal**
### a. Instalasi Ruby
Jekyll dibangun dengan Ruby, jadi pastikan Ruby sudah terpasang.
- Windows: Instal lewat [RubyInstaller](https://rubyinstaller.org/)
- MacOS / Linux: Biasanya sudah tersedia, atau bisa pakai brew / apt.

### b. **Instalasi Bundler dan Jekyll**
Buka terminal dan jalankan perintah berikut:
```bash
gem install jekyll bundler
```

## 2. **Membuat Project Jekyll Baru**
Buka terminal, lalu navigasikan ke direktori tempat Anda ingin membuat project. Jalankan perintah:
```bash
jekyll new nama_project
cd nama_project
```
Ini akan membuat folder baru dengan struktur dasar Jekyll.

## 3. **Menjalankan Server Lokal**
Untuk melihat website Anda secara lokal, jalankan perintah berikut:
```bash
bundle exec jekyll serve
```
Atau jika tidak menggunakan bundler:
```bash
jekyll serve
```
Lalu buka browser dan akses `http://localhost:4000` untuk melihat hasilnya.

## 4. **Struktur Folder Penting**

| Folder / File             | Fungsi                                        |
| ------------------------- | --------------------------------------------- |
| `_config.yml`             | Konfigurasi utama website                     |
| `_posts/`                 | Berisi artikel/postingan (format: YYYY-MM-DD) |
| `_layouts/`               | Template dasar halaman                        |
| `_includes/`              | Potongan HTML yang bisa disisipkan            |
| `index.md` / `index.html` | Halaman utama                                 |

## 5. **Menambah Postingan Baru**
Untuk menambah postingan baru, buat file baru di dalam folder `_posts/` dengan format nama `YYYY-MM-DD-judul-postingan.md`. Contoh:
```markdown
---
layout: post
title: "Judul Postingan"
date: 2025-04-20
---
Ini adalah isi dari postingan baru Anda.
```

## 6. **Menyesuaikan Tema (Opsional)**
Anda bisa mengubah tema dengan mengedit file `_config.yml` atau mengganti layout di dalam folder `_layouts/`. Anda juga bisa menambahkan CSS di folder `assets/css/` untuk mengubah tampilan.
Ganti tema default di `_config.yml`:
```yaml
theme: minima
```
Untuk tema lain, cek [https://jekyllthemes.io](https://jekyllthemes.io) atau [GitHub](https://github.com).

## 7. **Build ke HTML Statis (untuk deploy)**
Setelah selesai mengembangkan, Anda bisa membangun project Jekyll menjadi HTML statis dengan perintah:
```bash
bundle exec jekyll build
```
Atau jika tidak menggunakan bundler:
```bash
jekyll build
```
Ini akan menghasilkan folder `_site/` yang berisi semua file HTML yang siap untuk di-deploy ke server.
