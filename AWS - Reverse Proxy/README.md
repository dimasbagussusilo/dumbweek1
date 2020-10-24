# REVERSE PROXY PADA SERVER PUBLIC

- Update dan upgrade OS menggunakan perintah `sudo apt update && sudo apt upgrade` lalu install nginx dengan perintah `sudo apt install nginx`

![text](https://github.com/frostmarry/dumbweek1/blob/master/AWS%20-%20Reverse%20Proxy/asset/1.png)
![text](https://github.com/frostmarry/dumbweek1/blob/master/AWS%20-%20Reverse%20Proxy/asset/2.png)

- Tes akses server public dari browser komputer lokal

![text](https://github.com/frostmarry/dumbweek1/blob/master/AWS%20-%20Reverse%20Proxy/asset/3.png)

- Menambahkan file bernama dumplay.conf pada directory `etc/nginx/sites-available` dan di isi seperti gambar berikut

![text](https://github.com/frostmarry/dumbweek1/blob/master/AWS%20-%20Reverse%20Proxy/asset/4.png)

- Hubungkan file dumplay.conf yang ada dalam directory `etc/nginx/sites-available` ke directory `etc/nginx/sites-enabled` menggunakan perintah `ln -s etc/nginx/sites-available/dumplay.conf etc/nginx/sites-enabled/dumplay.conf` agar tidak perlu mengganti file nginx.conf karena secara default sudah ada `include etc/nginx/sites-enabled/*`

![text](https://github.com/frostmarry/dumbweek1/blob/master/AWS%20-%20Reverse%20Proxy/asset/5.png)

- Tes akses website yang ada pada server private dari browser komputer lokal mengguakan ip server public

![text](https://github.com/frostmarry/dumbweek1/blob/master/AWS%20-%20Reverse%20Proxy/asset/6.png)