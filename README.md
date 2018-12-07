# Docker - Orchestration using Docker Compose 
> By : Apriliana Puspitasari

> 163210008

> Komputerisasi Akuntansi

---

Sebelum menjalankan docker dari katacoda, saya mengerjakan praktikum mengenai docker untuk menginstal wordpress.
Pertama saya memastikan bahwa docker sudah ada dalam komputer, kemudian saya mengaktifkan cmd.exe untuk membuka
direktori docker.
1. Membuka cmd.exe masuk direktori docker toolbox. Kemudian ketik Docker version untuk mengetahui versi docker tersebut.

![1]()

> Docker version untuk mengetahui versi docker yang sedang kita gunakan.

![2]()

![3]()

![4]()

2. Kemudian membukan Docker Quickstart Terminal untuk mengetahui apakah docker sudah running atau belum, dan ketika 
sudah saya buka hasilnya seperti dibawah ini :

![5]()

3. Setelah itu saya membuka folder Docker Toolox di drive C lalu dalam folder Kitematic saya menjalankan Kitematic.exe 
untuk menggunakan docker melalui virtual machine.

![6]()

Tetapi setelah ditunggu Virtual machine dari docker tidak mau membuka, sehingga saya mencoba untuk menggunakan linux dalam
Virtual Box tetapi OS dalam Virtual Box tersebut tidak berjalan.

![7]()

Dan pembuatan wordpress dengan menggunakan docker gagal untuk dilanjutkan proses instalasinya. Setelah itu tugas yang
dikerjakan sebagai pengganti itu ada di [Orchestration using Docker Compose](https://www.katacoda.com/courses/docker/11)

**Step 1 - Defining First Container**

Mendefinisikan kontainer awal dengan pengaktifan property sebagai value nya.

![8]()

Membuat kontainer **web** dengan propery **build**

![9]()

**Step 2 - Defining Settings**

Menghubungkan beberapa kontainer dengan koneksi links ke **redis**. Redis sebagai database nya.

![10]() 

Sedangkan untuk koneksi ke port, menggunakan perintah :

![11]() 

Menambahkan port 3001 sebagai tambahan dari tugas yang harus dijalankan.

![12]() 

**Step 3 - Defining Second Container**

Pada Container yang pertama saya menggunakan container yang ada dalam dockerfile, untuk menggunakan container yang kedua saya menggunakan 
image dalam docker Hub. Dengan menggunakan nama container redis dan image redis.

![13]() 

**Step 4 - Docker Up**

Menjalankan aplikasi yang sudah dibuat sebelumnya.

![14]() 

![15]() 

![16]() 

**Step 5 - Docker Management**

Mengelola semua kontainer yang ada dalam docker.

Untuk melihat semua kontainer yang ada dengan menggunakan perintah dibawah ini :

![17]() 

Untuk mengakses semua pattern, dengan menggunakan perintah :

![18]() 

![19]() 

![20]() 

**Step 6 - Docker Scale**

Menentukan skala untuk kontainer yang sedang dijalankan, jika skala semakin besar maka akan memunculkan container tambahan.

![21]() 

Dapat mengembalikan skala yang seperti semula.

![22]() 

**Step 7 - Docker Stop**

Untuk menghentikan semua kontainer.

![23]() 

Untuk menghapus semua kontainer, gunakan perintah.

![24]() 

---