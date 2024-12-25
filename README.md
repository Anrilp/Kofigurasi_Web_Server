# Basic-networking

Submission  Proyek Membangun Web Server - Kelas Belajar Jaringan Komputer untuk Pemula

[Sertifikat Kompetensi Kelas Belajar Jaringan Komputer untuk Pemula](https://www.dicoding.com/certificates/JMZV46RLNXN9)

# Konfigurasi Reverse Proxy Server Menggunakan Nginx dan Apache2

Untuk menjalankan project ini, pastikan `Ubuntu` sudah terinstall pada komputer/laptop Anda.

---

Tata cara menjalankan project:

1. Open Ubuntu
2. Install nvm 

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash
```

3. Install Node.js versi v14.15.4 

```
nvm install v14.15.4
```

4. Install node modules

```
npm install
```

5. Jalankan project

```
npm run start
```

# Mengonfigurasi NGINX sebagai Reverse Proxy Server

1. Install nginx

```
sudo apt update
sudo apt-get install nginx -y
sudo service nginx status
```

2. Masukan code sesuai dengan folder Konfig

```
sudo nano /etc/nginx/sites-available/default
sudo service nginx restart
```
# Mengonfigurasi Apache2 sebagai Reverse Proxy Server

1. Install apache2

```
sudo apt update
sudo apt-get install apache2 -y
sudo service apache2 status
```

2. Install modul

```
sudo a2enmod proxy
sudo a2enmod proxy_http
sudo a2enmod headers
sudo a2enmod rewrite
```
3. Masukan code sesuai dengan folder Konfig

```
sudo nano /etc/apache2/sites-available/000-default.conf
sudo nano /etc/apache2/ports.conf
sudo service nginx restart
```
