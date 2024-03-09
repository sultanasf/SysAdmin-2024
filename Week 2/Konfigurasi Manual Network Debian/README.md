# Mengubah IP DHCP ke IP Manual Pada Debian

### 1. Cek IP Address Awal

Untuk melakukan cek IP bisa menggunakan command `$ ip addr` pada terminal Debian. Bisa dilihat pada gambar bahwa device saya mendapatkan ip **10.0.2.15** dari DHCP. <br>
<div align="center">
    <img src="./assets/1.png">
    <p><strong>Gambar 1:</strong>Initial IP Address</p>
</div>

### 2. Cek IP Gateway

Selanjutnya adalah cek gateway terlebih dahulu menggunakan command `$ sudo route -n` pada terminal Debian, pastikan menggunakan user dengan privilege *root* atau *superuser*. Alamat gateway tertera pada gambar adalah **10.0.2.2** <br>
<div align="center">
    <img src="./assets/2.png">
    <p><strong>Gambar 2:</strong>IP Gateway</p>
</div>

### 3. Konfigurasi IP Manual Pada Wired Network

Konfigurasi IP Manual melalui *Wired Network* dengan detail sebagai berikut:
<ul>
    <li>IPv4 Method: Manual</li>
    <li>Address: 10.0.2.17</li>
    <li>Netmask: 255.255.255.0</li>
    <li>Gateway: 10.0.2.0</li>
    <li>DNS: Google (8.8.8.8)</li>
</ul>
<div align="center">
    <img src="./assets/3.png">
    <p><strong>Gambar 3:</strong>Manual IP Config</p>
</div>

### 4. Cek IP Address Manual

Setelah mengkonfigurasi IP secara manual, restart *Wired Network* lalu cek ulang menggunakan command `$ ip addr` pada terminal Debian. Bisa terlihat pada gambar bahwa IP telah berganti ke **10.0.2.17** <br>
<div align="center">
    <img src="./assets/4.png">
    <p><strong>Gambar 4:</strong>Modified IP Address</p>
</div>

> Terima Kasih.
