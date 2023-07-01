---
title:  "Pengalaman Baru Mengenai Pengaturan Sleep State pada ThinkPad untuk Linux dan Windows"
author: wakhid
date: 2023-06-28 12:32:00 -0500
categories: [Blogging, ThinkPad, Review, Linux, Windows]
tags: [ThinkPad, Laptop, Linux, Windows]
---

Saya menggunakan ThinkPad T14 Gen 1 (Intel) untuk bekerja dan saya menginstall Linux Ubuntu pada laptop ini. Namun saya mendapati kejadian yang janggal pada laptop saat laptop dalam mode sleep. Persentase baterai laptop berkurang meski laptop dalam keadaan sleep. Awalnya saya mengira ada yang salah dengan konfigurasi power di Ubuntu, hingga akhirnya saya menemukan konfigurasi baru dari Lenovo yang belum pernah saya termukan pada seri ThinkPad sebelumnya.

## Akar Permasalahan: Persentase baterai laptop berkurang meski laptop dalam keadaan sleep di Linux.
Setelah menyiapkan beberapa hal yang saya butuhkan untuk pekerjaan, saya menutup laptop dan tidur. Saat itu, baterai masih sekitar 95%. Namun, ketika saya membuka laptop keesokan paginya, saya sangat terkejut karena baterainya hanya tersisa 10%. 


## Proses Pengecekan
Saya baru mengetahui bahwa ThinkPad terbaru memiliki pengaturan "sleep state" di BIOS untuk pengaturan Linux dan Windows.

Laptop saya dikirimkan oleh Lenovo dengan Windows 10, sehingga pengaturan awalnya juga disetel ke "Windows". 
Saya melakukan semua pengaturan keamanan yang diperlukan di BIOS saat pertama kali menghidupkannya, tetapi melewatkan pengaturan "sleep state".

## Proses Perbaikan
Mengubah pengaturan Sleep State menjadi Linux.

**Di BIOS: Config ➜ Power ➜ Sleep State ➜ "Linux" / "Windows 10"**

Dengan mngubah pengaturan Sleep State menjadi Linux, laptop menjadi normal. 


![ThinkPad T14 BIOS Sleep State](https://storage.bukanai.com/images/bukanai-com-pengalaman-pengaturan-sleep-state-thinkpad-linux-windows-1.png)


## Kesimpulan
Sekilas informasi yang saya dapatkan, mode Sleep State Windows adalah Modern Standby yang cara kerjannya belum/tidak cocok dengan Linux.
Sehingga pada laptop yang menggunakan OS Linux dengan pengaturan Sleep State Windows maka mengakibatkan proses sleep tidak bekerja dengan baik.

Kemudian saya mencoba menggunakan OS Windows, saya mendapati pengaturan Sleep State Linux juga bisa meng-handle mode sleep di OS Windows.


## Referensi
- [Modern Standby vs S3](https://learn.microsoft.com/en-us/windows-hardware/design/device-experiences/modern-standby-vs-s3)
- [P14s gen2 BIOS 1.36 has S3 sleep state option](https://forums.lenovo.com/t5/ThinkPad-P-and-W-Series-Mobile-Workstations/P14s-gen2-BIOS-1-36-has-S3-sleep-state-option/m-p/5087053)


