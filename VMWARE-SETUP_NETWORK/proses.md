# KONFIGURASI VM AGAR DAPAT TERHUBUNG KE JARINGAN INTERNET

1. ubah adapter dari NAT ke Bridged Adapter kemudian pilih hardware komputer lokal yang terhubung ke internet (dalam kasus saya wlp2s0)

![8](https://github.com/frostmarry/dumbweek1/blob/master/asset/8.png)

2. kemudian saat proses instalasi network connection ubah ip dari DHCP ke STATIC dan masukkan ip secara manual

![8.1](https://github.com/frostmarry/dumbweek1/blob/master/asset/8.1.png)

3. setelah proses instalasi selesai cek ip menggunakan perintah `ifconfig` dan cek ping ke google untuk memastikan server sudah terhubung ke internet

![8.2](https://github.com/frostmarry/dumbweek1/blob/master/asset/8.2.png)

