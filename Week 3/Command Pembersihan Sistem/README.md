# 8.6: Cleaning The System

### 8.6.1 Disk Space Information

Berikut merupakan beberapa command atau tools yang bisa digunakan untuk mengecek ruang pada disk. <br>

#### Command `$ df -h`

Command ini digunakan untuk **mengetahui penggunaan kapasitas disk** pada setiap *mount point* (drive dan partisi) pada siste. <br>
<div align="center">
    <img src="./assets/1.png">
    <p><strong>Gambar 1:</strong> command df -h</p>
</div>

#### Command `$ du` dan `$ sort`

Digunakan untuk **mengecek seberapa *bulky* direktori** yang terdapat pada sistem dalam satuan megabyte. <br>
<div align="center">
    <img src="./assets/2.png">
    <p><strong>Gambar 2:</strong> command du & sort</p>
</div>

#### NCDU

Merupakan software *disk analyzer* dalam mode konsol. Sebelum dapat menggunakan software ini harus menginstall terlebih dahulu dengan command `$ sudo apt update && sudo apt install ncdu` lalu ketikkan command `$ ncdu` untuk membukanya. <br>
<div align="center">
    <img src="./assets/3.png">
    <p><strong>Gambar 3:</strong> ncdu</p>
</div>

#### Baobab

Sama seperti NCDU, bedanya Baobab merupakan GUI dan terintegrasi dengan GNOME. Instalasinya sama seperti NCDU dengan mengetikkan command `$ sudo apt update && sudo apt install baobab` lalu command `$ baobab` digunakan untuk menjalankan software tersebut. <br>
<div align="center">
    <img src="./assets/4.png">
    <p><strong>Gambar 4:</strong> Baobab</p>
</div>

### 8.6.2 Cleaning The Packages

Berikut merupakan beberapa command atau tools yang bisa digunakan untuk melakukan pembersihan package. <br>

#### Command `$ apt clean`

Command yang berfungsi untuk **membersihkan cache** dari package yang terinstall pada sistem.<br>
<div align="center">
    <img src="./assets/5.png">
    <p><strong>Gambar 5:</strong> apt clean</p>
</div>

#### Command `$ apt autoremove --purge`

Berfungsi untuk **menghapus package beserta file confignya** dari sistem. <br>
<div align="center">
    <img src="./assets/6.png">
    <p><strong>Gambar 6:</strong> apt autoremove --purge</p>
</div>

#### Command `$ apt list` dan `$ apt remove`

Berfungsi untuk **menghapus package obsolete** dari sistem. <br>
<div align="center">
    <img src="./assets/7.png">
    <p><strong>Gambar 7:</strong> apt list dan `$ apt remove`</p>
</div>

#### Deborphan

Selain `$ apt remove`, kita juga bisa menginstall Deborphan yang berfungsi untuk **menghapus *orphaned* package** dari sistem. <br>
<div align="center">
    <img src="./assets/8.png">
    <img src="./assets/9.png">
    <p><strong>Gambar 8 & 9:</strong> deborphan</p>
</div>

### 8.6.3 Emptying The Trash Bins

Berikut merupakan beberapa command atau tools yang bisa digunakan untuk membersihkan trash bin. Trash bin terdiri dari beberapa tipe, seperti **user wastebasket** milik pengguna biasa dan **administrator wastebasket** milik penguna root. <br>

#### The User Wastebasket

Berikut command untuk membersihkan trash bin milik user. <br>
<div align="center">
    <img src="./assets/10.png">
    <p><strong>Gambar 10:</strong> user trashbin</p>
</div>

#### The Root Wastebasket

Berikut command untuk membersihkan trash bin milik user root. <br>
<div align="center">
    <img src="./assets/11.png">
    <p><strong>Gambar 11:</strong> root user trashbin</p>
</div>

### 8.6.4 Purging Application Caches

Beberapa aplikasi menggunakan direktori cache untuk menyimpan file grafis dan beberapa informasi lainnya supaya bisa berjalan lebih cepat. Biasanya cache tidak memakan banyak ruang disk, tetapi jika direktori cache tersebut menjadi terlalu besar maka bisa dihapus untuk menyisakan ruang disk.<br>

#### Command

Berikut adalah command untuk menghapus file cache.<br>
<div align="center">
    <img src="./assets/12.png">
    <p><strong>Gambar 12:</strong> cache</p>
</div>

### 8.6.5 Purging The Thumbnails

Thumbnails merupakan representasi dari file grafis seperti gambar atau video yang disimpan pada suatu direktori untuk digunakan ulang. Hal ini dapat menimbulkan masalah ketika user menghapus suatu file grafis, dikarenakan file thumbnailsnya yang masih tersimpan dan dapat memakan ruang disk hanya untuk menyimpan file obsolete.<br>

#### Command

Berikut adalah command untuk menghapus file thumbnails.<br>
<div align="center">
    <img src="./assets/13.png">
    <p><strong>Gambar 13:</strong> thumbnails</p>
</div>

> Terima Kasih
