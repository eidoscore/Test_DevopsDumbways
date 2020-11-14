## Perbedaan Docker dan VMWare
---

VMWare Virtual Machine | Docker Container
---------------------- | ----------------
Berat | Ringan
Performa | Performa maksimum tergantung pada hardware fisik
Virtualisasi pada level hardware | Virtualisasi pada level OS
Waktu start up dalam hitungan menit | Waktu start up dalam hitungan detik
Terisolasi penuh pada level hardware sehingga lebih aman | Terisolasi pada level proses
---
## Kenapa Harus VMWare

karena Resource hardware yang eksklusif sehingga tidak terganggu jika ada apps yang lain tiba-tiba membutuhkan resource yang tinggi, security yang tinggi dan jauh lebih baik dari Docker

## Kenapa Harus Docker
Waktu yang dibutuhkan untuk mengemas dan memasang app dalam container lebih cepat bila dibandingkan dengan VM, Mengurangi Resource, fleksible dan scalable, serta mempermudah ketika melakukan migrasi karna aplokasi dan depency sudah dikemas dalam kontainer serta ringan.
