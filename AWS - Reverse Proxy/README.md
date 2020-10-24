# REVERSE PROXY PADA SERVER PUBLIC

- Update dan upgrade OS menggunakan perintah `sudo apt update && sudo apt upgrade` lalu install nginx dengan perintah `sudo apt install nginx`

![text](1)
![text](2)

- Tes akses server public dari browser komputer lokal

![text](3)

- Menambahkan file bernama dumplay.conf pada directory `etc/nginx/sites-available` dan di isi seperti gambar berikut

![text](4)

- Hubungkan file dumplay.conf yang ada dalam directory `etc/nginx/sites-available` ke directory `etc/nginx/sites-enabled` menggunakan perintah `ln -s etc/nginx/sites-available/dumplay.conf etc/nginx/sites-enabled/dumplay.conf` agar tidak perlu mengganti file nginx.conf karena secara default sudah ada `include etc/nginx/sites-enabled/*`

![text](5)

- Tes akses website yang ada pada server private dari browser komputer lokal mengguakan ip server public

![text](6)