---
title: ThinkPad T14 Gen 1 Intel - Apakah Support Dual SSD NVME Storage ?
author: wakhid
date: 2023-05-24 12:32:00 -0500
categories: [Blogging, ThinkPad]
tags: [ThinkPad, Lenovo, Laptop]
---

Setelah melakukan pencarian di Google dan membaca informasi di Forum Lenovo, saya akhirnya mencoba sendiri untuk memastikan kompatibilitas dual storage pada ThinkPad T14 Gen 1 (Intel).

Saya membeli sebuah Storage NVMe Gen3 x2 yang juga kompatibel dengan seri ThinkPad sebelumnya, seperti T480 dan T480s.

Berikut adalah spesifikasi NVMe yang saya beli:

- Model: WD PC SN520
- Form Factor: M.2 2240 + 12MM = 2242
- Interface: PCIe Gen 3 x2
- Capacity: 256GB
- Sequential Read up to 1,700 MB/s
- Sequential Write up to 1,400 MB/s
- Endurance (TBW): 300 TBW

NVMe ini juga bisa digunakan pada Slot WWAN T480 dan T480s. Anda dapat membelinya di : [https://tokopedia.link/AlLLtG6O3zb](https://tokopedia.link/AlLLtG6O3zb)

![WD SN520 2242](/images/bukanai-com-thinkpad-t14-dual-storage-wwan-1.png)



## Proses Pemasangan NVME di ThinkPad T14 Gen 1

Pemasangan NVMe di Slot WWAN ThinkPad T14 Gen 1 sangat mudah. Saya hanya perlu membuka casing bawah laptop dan memasangnya di Slot WWAN yang tersedia. Slot tersebut bersebelahan dengan Slot NVMe utama.


![Slot WWAN ThinkPad T14 Gen 1](/images/bukanai-com-thinkpad-t14-dual-storage-wwan-2.png)


## NVME di Slot WWAN Terdeteksi
Setelah selesai dipasang, saya menghidupkan laptop dan setelah masuk ke sistem operasi Windows, NVMe di Slot WWAN berhasil terdeteksi dengan baik.

Setelah NVMe terdeteksi di Windows, saya mencoba memformat NVMe SN520 ini, dan prosesnya berjalan lancar tanpa kendala. NVMe ini siap digunakan untuk menyimpan data.


![Dual Storage ThinkPad T14 Gen 1](/images/bukanai-com-thinkpad-t14-dual-storage-wwan-3.png)

![Dual Storage ThinkPad T14 Gen 1](/images/bukanai-com-thinkpad-t14-dual-storage-wwan-4.png)


## Terdapat Beberapa Hal yang Perlu Diperhatikan
Meskipun semua tampak selesai, ada beberapa hal yang perlu diperhatikan. Meskipun tidak mengganggu, saya merasa penting untuk mencatatnya:

- NVMe di Slot WWAN hanya terdeteksi jika laptop dihidupkan setelah shutdown. 

    Jadi, setelah selesai bekerja dan melakukan shutdown, saat laptop dinyalakan kembali, NVMe di Slot WWAN akan terdeteksi dengan baik. 
    Namun, jika laptop di-restart, NVMe di Slot WWAN tidak akan terdeteksi. Solusinya, cukup lakukan shutdown dan nyalakan kembali laptop.


- NVMe di Slot WWAN tidak terdeteksi di sistem operasi Linux dan Hackintosh. 
    
    Saya menemukan masalah ini saat melakukan instalasi Linux (Ubuntu/Fedora) dan Hackintosh. Setelah proses instalasi selesai, NVMe di Slot WWAN tidak terdeteksi sama sekali.
    
- Saya belum sempat melakukan penelusuran lebih lanjut karena Saya harus segera menggunakan laptop ini untuk bekerja.

## Kesimpulan
Meskipun dual storage pada ThinkPad T14 Gen 1 (Intel) ini tidak sebaik di ThinkPad T480/T480s, akhirnya saya dapat mengetahui sejauh mana kompatibilitas dual storage pada laptop ini.

Bagi pengguna sistem operasi Windows, mungkin tidak perlu khawatir dengan masalah yang saya sebutkan di atas. Jadi, mempertimbangkan atau mencobanya adalah hal yang layak.


