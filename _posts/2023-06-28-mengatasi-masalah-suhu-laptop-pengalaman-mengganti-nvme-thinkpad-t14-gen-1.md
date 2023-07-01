---
title:  "Review ThinkPad T14 Gen 1 : NVME Juga Memberikan Dampak Kepada Temperatur Laptop"
author: wakhid
date: 2023-06-28 12:32:00 -0500
categories: [Blogging, Thinkpad, Review]
tags: [ThinkPad, Laptop, NVME]
---

Beberapa waktu lalu, saya melakukan upgrade NVME dari NVME Toshiba XG6 KXG6AZNV256G 256GB ke WD SN720 512GB, dengan tujuan mendapatkan kapasitas yang lebih tinggi. Namun, saya menghadapi masalah suhu yang tinggi pada laptop ThinkPad T14 Gen 1 (Intel).

## Akar Permasalahan: Suhu tinggi pada palmrest kiri laptop
Saya menghadapi masalah suhu yang tinggi pada laptop ThinkPad T14 Gen 1 (Intel) yang hanya terjadi pada palmrest kiri laptop saja, kondisi ini diperparah saat proses charging. 

Selama proses charging, suhu bagian palmrest kiri laptop juga semakin meningkat. Hal ini terkait dengan letak port charger usb-c, NVME slot, dan WWAN Slot yang berada di bagian tersebut.

Situasi ini membuat saya merasa bingung, karena meskipun laptop tidak sedang digunakan, palmrest kiri tetap terasa panas. Bahkan, kipas CPU tidak berputar karena suhu CPU masih rendah.

## Proses Pengecekan
Saya menyadari bahwa masalah ini mungkin terkait dengan NVME (Non-Volatile Memory Express) WD SN720 yang saya gunakan. Entah karena karakteristik NVME tersebut atau ada masalah pada perangkat NVME itu sendiri, suhu laptop tetap tinggi meskipun dalam kondisi idle dengan suhu NVME minimal 45°C dan dapat mencapai 70°C saat digunakan secara intensif.

Kemungkinan karena laptop ini tipis, sehingga slot NVME dan bagian aluminium chassis di bawah keyboard nyaris bersentuhan langsung. Terdapat pembatas berupa thermal pad yang sangat tipis, yang menyebabkan panas yang dihasilkan oleh NVME menyebar ke bagian laptop di bawah keyboard. Mungkin inilah salah satu faktor penyebaran panas di laptop ini.

![Temperatur WDSN720 Saat Digunakan](/images/bukanai-com-mengatasi-masalah-suhu-laptop-pengalaman-mengganti-nvme-thinkpad-t14-1.png)
![Temperatur WDSN720 Saat Idle](/images/bukanai-com-mengatasi-masalah-suhu-laptop-pengalaman-mengganti-nvme-thinkpad-t14-2.png)


## Proses Perbaikan
Setelah melakukan evaluasi lebih lanjut, saya memutuskan untuk mengganti NVME dengan merek PNY CS1031 256GB yang sebetulnya adalah NVME milik laptop ThinkPad saya lainnya. **Hasilnya, suhu laptop kembali normal**. 

Saya tidak memenggunakan lagi NVME Toshiba XG6 KXG6AZNV256G 256GB karena NVME tersebut sudah digunakan oleh orang lain.

![Temperatur PNY Saat Digunakan](/images/bukanai-com-mengatasi-masalah-suhu-laptop-pengalaman-mengganti-nvme-thinkpad-t14-3.png)


## Kesimpulan
Dalam kesimpulannya, pengalaman saya menghadapi masalah suhu yang tinggi pada laptop Lenovo ThinkPad T14 memberikan pelajaran berharga. Saya belajar bahwa selain menjaga kebersihan kipas dan mengganti pasta termal secara berkala, pemeriksaan terhadap suhu NVME juga penting dalam mendiagnosis dan mengatasi masalah panas pada laptop. Setiap pengguna laptop perlu memperhatikan faktor-faktor ini agar laptop dapat berfungsi optimal dan suhu tetap terjaga dalam batas yang aman.

## Disclaimer
Perlu dicatat bahwa tulisan ini bukan merupakan promosi untuk merek PNY, tetapi hanya kebetulan NVME tersebut berhasil mengatasi masalah suhu pada laptop saya. Saya terbuka untuk mencoba merek NVME lain jika diperlukan. Pengalaman ini menunjukkan bahwa selain mengganti pasta termal dan membersihkan kipas, memeriksa suhu NVME juga penting dalam mengatasi masalah panas pada laptop.