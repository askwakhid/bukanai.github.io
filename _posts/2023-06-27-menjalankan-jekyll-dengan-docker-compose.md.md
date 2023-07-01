---
title: Menjalankan Jekyll dengan Docker Compose untuk Pengembangan Lokal yang Efisien
author: wakhid
date: 2023-06-27 12:32:00 -0500
categories: [Blogging, Docker, Jekyll]
tags: [Jekyll, Docker]
---
Di postingan kali ini, saya akan berbagi cara menjalankan Jekyll menggunakan Docker Compose untuk pengembangan situs web statis secara lokal. Dengan menggunakan Docker Compose, kita dapat mempercepat dan menyederhanakan proses pengembangan Jekyll di laptop kita.

Jekyll adalah alat yang populer untuk membangun situs web statis dengan menggunakan Markdown dan templating. Namun, instalasi dan konfigurasi Jekyll di mesin lokal dapat memakan waktu dan kompleksitas. Dalam hal ini, Docker Compose adalah solusi yang efisien untuk menjalankan Jekyll di dalam kontainer Docker dengan mudah.

### Persyaratan Awal
Sebelum memulai, pastikan Anda telah memenuhi persyaratan berikut:
1. Docker: Pastikan Anda telah menginstal Docker di sistem operasi Anda. Untuk informasi lebih lanjut tentang cara menginstal Docker, kunjungi [dokumentasi resmi Docker](https://docs.docker.com/get-docker/).
2. Docker Compose: Pastikan Anda telah menginstal Docker Compose. Untuk panduan instalasi, silakan lihat [dokumentasi Docker Compose](https://docs.docker.com/compose/install/).

### Langkah-langkah

#### Langkah 1: Membuat File Konfigurasi `docker-compose.yml`
1. Buka terminal atau command prompt dan arahkan ke direktori proyek Jekyll Anda.
2. Buat file baru bernama `docker-compose.yml` di direktori tersebut.

    ```bash
    $ touch docker-compose.yml
    ```

3. Buka file `docker-compose.yml` dengan editor teks favorit Anda.

#### Langkah 2: Konfigurasi Docker Compose
4. Di dalam file `docker-compose.yml`, tambahkan konfigurasi berikut:

    ```yaml
    version: '3'
    services:
      jekyll:
        image: jekyll/jekyll:latest
        volumes:
          - .:/srv/jekyll
        ports:
          - 4000:4000
        command: jekyll serve --watch --force_polling
    ```

    Penjelasan:
    - Versi Docker Compose yang digunakan adalah `3`.
    - Kami menggunakan image Docker resmi `jekyll/jekyll:latest`, yang merupakan versi Jekyll yang akan digunakan. Pastikan untuk mengganti versi ini jika diperlukan.
    - Volume dihubungkan antara direktori proyek saat ini dan direktori `/srv/jekyll` di dalam kontainer Jekyll. Ini memungkinkan perubahan yang dilakukan pada proyek di luar kontainer dapat langsung dilihat di dalam kontainer Jekyll.
    - Port 4000 dari kontainer dihubungkan ke localhost, sehingga Anda dapat mengakses situs Jekyll melalui `http://localhost:4000`.
    - Perintah `jekyll serve --watch --force_polling` dijalankan di dalam kontainer untuk menjalankan server Jekyll dengan mode pemantauan perubahan dan memaksa polling perubahan file.

#### Langkah 3: Menjalankan Kontainer Jekyll
5. Simpan perubahan pada file `docker-compose.yml`.
6. Di terminal atau command prompt, arahkan ke direktori proyek Jekyll.
7. Jalankan perintah berikut untuk memulai kontainer Jekyll:

    ```bash
    $ docker-compose up
    ```

    Docker Compose akan membaca file konfigurasi `docker-compose.yml` dan menjalankan kontainer Jekyll sesuai pengaturan yang telah didefinisikan.

8. Buka browser dan akses situs Jekyll melalui `http://localhost:4000`. Anda sekarang dapat melihat situs Jekyll dan melakukan perubahan pada proyek secara real-time.

### Kesimpulan
Dengan menggunakan Docker Compose, Anda dapat menjalankan Jekyll dengan mudah dan efisien di lingkungan lokal Anda. Penggunaan Docker Compose membebaskan Anda dari konfigurasi dan instalasi manual, sehingga Anda dapat fokus pada pengembangan situs web statis Anda.

---