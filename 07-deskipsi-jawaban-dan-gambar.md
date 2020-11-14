# Domain Name Server
Domain Name Server atau DNS adalah sebuah sistem yang menghubungkan Uniform Resource Locator (URL) dengan Internet Protocol Address (IP Address).

DNS digunakan untuk merubah alamat IP menjadi alamat domain name, hal ini mempermudah pengguna melakukan pencarian menggunakan domain name daripada alamat ip.
---
## Cara Kerja DNS
* DNS resolver melakukan pencarian alamat host pada file HOSTS. Jika alamat host yang dicari sudah ditemukan dan diberikan, maka proses selesai.
* DNS resolver melakukan pencarian alamat host pada file HOSTS. Jika alamat host yang dicari sudah ditemukan dan diberikan, maka proses selesai.
* DNS resolver melakukan pencarian pada data cache yang sudah dibuat oleh resolver untuk menyimpan hasil permintaan sebelumnya. Bila ada, kemudian disimpan dalam data cache lalu hasilnya diberikan dan selesai.
* DNS resolver melakukan pencarian pada alamat server DNS pertama yang telah ditentukan oleh pengguna.
* Server DNS ditugaskan untuk mencari nama domain pada cache-nya.
* Apabila nama domain yang dicari oleh server DNS tidak ditemukan, maka pencarian dilakukan dengan melihat file database (zones) yang dimiliki oleh server.
* Apabila masih tidak ditemukan, pencarian dilakukan dengan menghubungi server DNS lain yang masih terkait dengan server yang dimaksud. Jika sudah ditemukan kemudian disimpan dalam cache lalu hasilnya diberikan ke client (melalui web browser).

![Image of 01](/folder-images-jawaban-07/01.png)