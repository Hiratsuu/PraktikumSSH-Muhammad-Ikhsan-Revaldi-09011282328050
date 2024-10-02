### Nama: Muhammad Ikhsan Revaldi
### NIM: 09011282328060
### Kelas: SK3C
# Melakukan setup dan menguhubungkan ke pc lain melalui SSH pada linux

1. Melakukan persiapan untuk menginstal layanan SSH pada linux dengan cara melakukan upgrade dan update pada semua paket apt ke versi terbaru dengan tujuan memastikan instalasi openssh dari repository terbarukan untuk mendapat package yang lebih termutakhir
![System update and upgrade](https://github.com/Hiratsuu/PraktikumSSH-Muhammad-Ikhsan-Revaldi-09011282328050/blob/main/SSH/1.png?raw=true)

2. Lalu setelah itu kita lakukan penginstalan layanan SSH nya dengan command **Sudo apt install openssh-server**
![Installing OpenSSH server](https://github.com/Hiratsuu/PraktikumSSH-Muhammad-Ikhsan-Revaldi-09011282328050/blob/main/SSH/2.png?raw=true)

3. Berikutnya kita aktifkan layanan SSH dengan command **sudo systemctl enable --now ssh**
![SSH service installation details](https://github.com/Hiratsuu/PraktikumSSH-Muhammad-Ikhsan-Revaldi-09011282328050/blob/main/SSH/3.png?raw=true)
lalu kita cek apakah layanan SSH tersebut sudah aktif atau belum dengan command systemctl status ssh.
![Configuring and starting SSH service](https://github.com/Hiratsuu/PraktikumSSH-Muhammad-Ikhsan-Revaldi-09011282328050/blob/main/SSH/3.1.png?raw=true)

4. Sebelum menghubungkan ke server melalui SSH, kita perlu memeriksa firewall untuk memastikan apakah sudah dikonfigurasi dengan benar dengan command **sudo ufw status**. jika firewall memiliki status inactive maka kita bisa memberi izin koneksi SSH dengan command **sudo ufw allow ssh**
![Checking SSH status and allowing through firewall](https://github.com/Hiratsuu/PraktikumSSH-Muhammad-Ikhsan-Revaldi-09011282328050/blob/main/SSH/4.png?raw=true)

5. pada bagian ini, kita sudah bisa menghubungkan server kita ke device lain dengan menggunakan command **ssh username@IP_address** (perlu diketahui kita perlu mengetahui alamat ip dan nama pengguna si device tujuan kita). Kali ini saya mencoba untuk menghubungan device teman saya.
![Connect to the server](https://github.com/Hiratsuu/PraktikumSSH-Muhammad-Ikhsan-Revaldi-09011282328050/blob/main/SSH/5.png?raw=true)
setelah berhasil terhubung ke device lain maka kita bisa mengaksesnya pada pc kita dan juga kita bisa melihat spesifikasi si device yang kita hubungkan tadi dan masih banyak hal juga yang bisa kita lakukan setelah menghubungkannya.

