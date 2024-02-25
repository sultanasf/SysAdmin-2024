# Instalasi Debian pada Virtual Box

## Persiapan Tools

1. Iso File Debian
![alt text](./assets/image.png)
2. Virtual Box
![alt text](./assets/image-1.png)

## Setup Virtual Machine

1. Buka Virtual Box
![alt](./assets/Screenshot%202024-02-19%20090432.png)
*Tampilan awal virtual box*
2. New Virtual Machine
![alt](./assets/Screenshot%202024-02-19%20093418.png)
*Klik new, arahkan ISO image ke direktori penyimpanan ISO yang sudah di download, check list pada "Skip Unattended Installation"*
3. Spesifikasi Hardware
![alt](./assets/Screenshot%202024-02-19%20091123.png)
*Disini virtual machine saya nantinya akan memiliki 4GB Memory serta 2-Core CPU*
4. Alokasi Storage
![alt](./assets/Screenshot%202024-02-19%20091246.png)
*Untuk penyimpanan, buat virtual hard disk dengan space 25GB untuk virtual machine saya*
5. Summary
![alt](./assets/Screenshot%202024-02-19%20091343.png)
*Cek kembali, apabila sudah benar klik finish*
6. Virtual Machine telah dibuat
![alt](./assets/Screenshot%202024-02-19%20093700.png)

## Setup Debian

1. Pilih bahasa
![alt](./assets/Screenshot%202024-02-19%20093850.png)
2. Setup lokasi
![alt](./assets/Screenshot%202024-02-19%20093922.png)
![alt](./assets/Screenshot%202024-02-19%20093940.png)
![alt](./assets/Screenshot%202024-02-19%20094003.png)
*Pilih other->asia->indonesia*
3. Setup locales
![alt](./assets/Screenshot%202024-02-19%20094038.png)
*Pilih United States*
4. Setup Keyboard
![alt](./assets/Screenshot%202024-02-19%20094114.png)
*Pilih american english untuk keymap, lalu klik continue*
5. Setup network
![alt](./assets/Screenshot%202024-02-19%20094236.png)
*Masukkan "SysAdmin-NRP" sebagai hostname*
![alt](./assets/Screenshot%202024-02-19%20094253.png)
*Domain name kosongkan, lalu klik continue*
6. Setup root dan user
![alt](./assets/Screenshot%202024-02-19%20094319.png)
*Masukkan pasword untuk akses root*
![alt](./assets/Screenshot%202024-02-19%20094414.png)
*Masukkan fullname untuk digunakan sebagai user baru(non-root)*
![alt](./assets/Screenshot%202024-02-19%20094433.png)
*Masukkan username untuk user yang telah dibuat*
![alt](./assets/Screenshot%202024-02-19%20094451.png)
*Masukkan password yang digunakan untuk akses user tadi*
7. Konfigurasi jam
![alt](./assets/Screenshot%202024-02-19%20094507.png)
*Pilih western untuk WIB*
8. Format Partisi
![alt](./assets/Screenshot%202024-02-19%20095609.png)
*Buat partisi dari alokasi storage tadi untuk / ,/storage, dan swap area*
9. Setup package manager
![alt](./assets/Screenshot%202024-02-19%20095829.png)
![alt](./assets/Screenshot%202024-02-19%20095843.png)
*Gunakan kebo.pens sebagai package manager*
10. Software selection
![alt](./assets/Screenshot%202024-02-19%20100601.png)
*Pilih software untuk di install*
11. Boot GRUB
![alt](./assets/Screenshot%202024-02-19%20111459.png)
*Saat pertama kali Machine dijalankan(booting), akan muncul GRUB untuk bisa masuk ke OS yang ada*
