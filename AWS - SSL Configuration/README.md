# MENAMBAHKAN SSL LET'S ENCRYPT

- Menginstal aplikasi certbot dengan beberapa perintah berikut pada server public

```
sudo add-apt repository ppa:certbot/certbot
sudo apt-get update
sudo apt-get install python-certbot-nginx
```

- Setelah itu menjalankan perintah `sudo certbot --nginx -d elga.instructype.com` untuk mengaktifkan let's encrypt dengan bantuan certbot

![text](asset/1.png)

![text](asset/2.png)

- Check settingan nginx yang ada pada file dumplay.conf dalam directory `etc/nginx/sites-available`

![text](asset/3.png)