# Pembuatan Web Server pada ElementaryOS menggunakan Apache

untuk membuat web server sederhana pada laptop kali ini saya menggunakan apache2 pada sistem operasi linux Elementary, berikut langkah-langkahnya

step pertama buka terminal, ketikan command :
> sudo apt-get update
> sudo apt-get install apache2

buat direktori pada folder /home/eidoscore/www
>mkdir /home/eidoscore/www

edit file hosts
> vi /etc/hosts

lalu tambahkan ip dan address berikut, setelah itu simpan.

![Image of 01](/folder-images-jawaban-08/01.png)

buat file config baru dan copy semua : 
> cp /etc/apache2/sites-available/000-default.conf /etc/apache2/sites-available/dumbways-khaerulanwar.xyz.conf

buka file yg baru copy tadi.
> vi /etc/apache2/sites-available/dumbways-khaerulanwar.xyz.conf

kemudian rubah syntax seperti berikut :

>ServerName dumbways-khaerulanwar.xyz
>DocumentRoot /home/eidoscore/www


![Image of 01](/folder-images-jawaban-08/02.png)

kemudian disable config lama dan enable config baru kemudian restart
>sudo a2dissite 000-default.conf
>sudo a2ensite hackdx.md.conf
>sudo systemctl reload apache2

Update Config Apache terbaru agar tidak forbidden :

> vi /etc/apache2/apache2.conf

tambahkan baris berikut ke bagian akhir : 
><Directory /home/eidoscore/www>
>        Options Indexes FollowSymLinks
>        AllowOverride None
>        Require all granted
></Directory>

kemudian restart services apache2
> sudo systemctl reload apache2

