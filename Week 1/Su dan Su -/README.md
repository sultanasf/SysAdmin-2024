# Command "su" dan "su -"

## Command su

![alt](./assets/Screenshot%202024-02-26%20051803.png)
su merupakan singkatan dari substitute user adalah command Linux yang digunakan untuk berganti user pada saat sesi login. Pada umumnya su sering disalah artikan sebagai singkatan dari super user.
Dikarenakan memang command tersebut bisa digunakan untuk mendapatkan privilege superuser. Ketika su diexecute tanpa username, maka otomatis akan menjadi superuser setelah memasukkan root password yang benar. Setelahnya, pengguna akan memasuki default environment root seperti pada contoh diatas

Dengan menjalankan command su, pengguna akan dipindahkan ke akun lain yang diinginkan. Dan jika tidak menyebutkan akun yg dituju, maka pengguna diarahkan ke akun root secara default seperti yang sudah dijelaskan sebelumnya.
su melakukan switch akun yang digunakan tanpa menjalankan login shell, dan variabel environment yang terdapat pada current user tidak akan berubah.

## Command su -

![alt](./assets/Screenshot%202024-02-26%20051829.png)
Tidak seperti command su, command su - akan memindahkan pengguna ke akun yang dituju sekaligus mengganti values pada environment variabel ke values yang terdapat pada current working environment. Dan semua environment variable yang menjadi milik main user akan dihapus.
su - merupakan cara terbaik yg digunakan untuk mengkonfigurasi environment variable secara total. Selain itu, command su -l dan su -login memiliki kegunaan atau behaviour yang sama dengan su -.

## Kesimpulan

Singkatnya, command su digunakan untuk berpindah akun dengan tetap mempertahankan current user environment variables. Sedangkan command su - mengexecute login shell untuk berganti akun dan secara umum merubah environment variables yang terdapat pada current user.
