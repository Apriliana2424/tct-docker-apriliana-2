# Docker - Orchestration using Docker Compose 
> By : Apriliana Puspitasari

> 163210008

> Komputerisasi Akuntansi

---

Sebelum menjalankan docker dari katacoda, saya mengerjakan praktikum mengenai docker untuk menginstal wordpress.
Pertama saya memastikan bahwa docker sudah ada dalam komputer, kemudian saya mengaktifkan cmd.exe untuk membuka
direktori docker.
1. Membuka cmd.exe masuk direktori docker toolbox. Kemudian ketik Docker version untuk mengetahui versi docker tersebut.

![1](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/1.jpg)

> Docker version untuk mengetahui versi docker yang sedang kita gunakan.

![2](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/2.png)

![3](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/3.png)

![4](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/4.png)

2. Kemudian membukan Docker Quickstart Terminal untuk mengetahui apakah docker sudah running atau belum, dan ketika 
sudah saya buka hasilnya seperti dibawah ini :

![5](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/5.png)

3. Setelah itu saya membuka folder Docker Toolox di drive C lalu dalam folder Kitematic saya menjalankan Kitematic.exe 
untuk menggunakan docker melalui virtual machine.

![6](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/6.png)

Tetapi setelah ditunggu Virtual machine dari docker tidak mau membuka, sehingga saya mencoba untuk menggunakan linux dalam
Virtual Box tetapi OS dalam Virtual Box tersebut tidak berjalan.

![7](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/7.png)

Dan pembuatan wordpress dengan menggunakan docker gagal untuk dilanjutkan proses instalasinya. Setelah itu tugas yang
dikerjakan sebagai pengganti itu ada di [Orchestration using Docker Compose](https://www.katacoda.com/courses/docker/11)

**Step 1 - Defining First Container**

Mendefinisikan kontainer awal dengan pengaktifan property sebagai value nya.

![8](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/8.png)

Membuat kontainer **web** dengan propery **build**

![9](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/9.png)

**Step 2 - Defining Settings**

Menghubungkan beberapa kontainer dengan koneksi links ke **redis**. Redis sebagai database nya.

![10](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/10.png) 

Sedangkan untuk koneksi ke port, menggunakan perintah :

![11](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/11.png) 

Menambahkan port 3001 sebagai tambahan dari tugas yang harus dijalankan.

![12](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/12.png) 

**Step 3 - Defining Second Container**

Pada Container yang pertama saya menggunakan container yang ada dalam dockerfile, untuk menggunakan container yang kedua saya menggunakan 
image dalam docker Hub. Dengan menggunakan nama container redis dan image redis.

![13](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/13.png) 

**Step 4 - Docker Up**

Menjalankan aplikasi yang sudah dibuat sebelumnya.

![14](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/14.png) 

![15](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/15.png) 

![16](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/16.png) 

**Step 5 - Docker Management**

Mengelola semua kontainer yang ada dalam docker.

Untuk melihat semua kontainer yang ada dengan menggunakan perintah dibawah ini :

![17](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/17.png) 

Untuk mengakses semua pattern, dengan menggunakan perintah :

![18](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/18.png) 

![19](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/19.png) 

![20](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/20.png) 

**Step 6 - Docker Scale**

Menentukan skala untuk kontainer yang sedang dijalankan, jika skala semakin besar maka akan memunculkan container tambahan.

![21](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/21.png) 

Dapat mengembalikan skala yang seperti semula.

![22](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/22.png) 

**Step 7 - Docker Stop**

Untuk menghentikan semua kontainer.

![23](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/23.png) 

Untuk menghapus semua kontainer, gunakan perintah.

![24](https://github.com/Apriliana2424/tct-docker-apriliana-2/blob/master/images/24.png) 

---