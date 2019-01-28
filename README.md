APA ITU GIT ?
•	Git adalah salah satu sistem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.

•	Pengontrol versi bertugas mencatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.

•	Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja.

MEMBUAT REPOSITORY LOCAL

klik kanan pada dekstop tersebut, dan pilih menu Git Bash, sehingga muncul git bash commad

•	Buat direktory project praktikum pertama dengan nama latihan1

•	Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya •	masuk kedalam direktori tersebut dengan perintah cd (change directory)

![mkdir01](https://user-images.githubusercontent.com/46733431/51816686-52eddf00-22fa-11e9-9c46-d6a82d5d75ec.png)

Jalankan perintah git init, untuk membuat repository local.

•	Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git

•	Pada direktori tersebut, semua perubahan pada working directory akan disimpan. 

![git init](https://user-images.githubusercontent.com/46733431/51816771-c0017480-22fa-11e9-939c-c0cbba1091ca.png)

Menambahkan File baru pada repository

•	Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

•	disini kita akan coba buat satu file bernama README.md (text file)

$ echo “#Latihan 1” >> README.md

•	File README.md berhasil dibuat.

•	Untuk menambahkan file yang baru saja dibuat tersebut gunakan perintah git add.

$ git add README.md

•	File README.md berhasil ditambahkan.

![echo](https://user-images.githubusercontent.com/46733431/51816959-6ea5b500-22fb-11e9-8dce-76924ab464cb.png)

Commit (Menyimpan perubahan ke database)

•	Untuk menyimpan perubahan yang ada kedalam database repository local, gunakan perintah git commit -m “komentar commit”

$ git commit -m “File pertama saya”

•	Perubahan berhasil disimpan.

![commit](https://user-images.githubusercontent.com/46733431/51817108-fd1a3680-22fb-11e9-8215-261780301e40.png)

Membuat repository server

• masuk ke github.com lalu login

• lalu buat repositorynya 

•	Isi nama repositorynya, misal: latihan01.

•	lalu klik tombol Create repository

![111](https://user-images.githubusercontent.com/46733431/51817217-5f733700-22fc-11e9-84d9-692a1b888345.png)

![2222](https://user-images.githubusercontent.com/46733431/51817251-8598d700-22fc-11e9-81e1-ecf365d7b04c.png)

Menambahkan Remote Repository

•	Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

•	Untuk menambahkan remote repository server, gunakan perintah Menambahkan Remote Repository

•	Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.

•	Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url] 

![remote](https://user-images.githubusercontent.com/46733431/51817315-c690eb80-22fc-11e9-9496-ddd29e6430ef.png)

•	Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.

$ git push -u origin master

•	Perintah ini akan meminta memasukkan username dan password pada akun github.com 

![push](https://user-images.githubusercontent.com/46733431/51817392-1c659380-22fd-11e9-870c-fcc5645afd56.png)

Melihat hasilnya pada server repository

Buka laman github.com, arahkan pada repositorynya , maka perubahan akan terlihat pada laman tersebut.

![asdasdas](https://user-images.githubusercontent.com/46733431/51817453-62baf280-22fd-11e9-9168-169de9ac136e.png)
