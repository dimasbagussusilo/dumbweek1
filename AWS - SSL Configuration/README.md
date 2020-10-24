# MENAMBAHKAN SSL LET'S ENCRYPT

- Menginstal aplikasi certbot dengan beberapa perintah berikut pada server public

```
sudo add-apt repository ppa:certbot/certbot
sudo apt-get update
sudo apt-get install python-certbot-nginx
```

setelah itu menjalankan perintah `sudo certbot --nginx -d elga.instructype.com` untuk mengaktifkan let's encrypt dengan bantuan certbot

![text](https://github.com/frostmarry/dumbweek1/tree/master/AWS%20-%20SSL%20Configuration/asset/1.png)
![text](https://github.com/frostmarry/dumbweek1/tree/master/AWS%20-%20SSL%20Configuration/asset/2.jpg)

- Check settingan nginx yang ada pada file dumplay.conf dalam directory `etc/nginx/sites-available`

![text](https://github.com/frostmarry/dumbweek1/tree/master/AWS%20-%20SSL%20Configuration/asset/3.jpg)
