<h1>Laporan pengerjaan studi kasus penggunaan docker UTS TCC </h1>

<h3>A. Pengerjaan Getting started di dokcerhub</h3>

1. Langkah pertama untuk menggunakan docker adalah dengan melakukan instalasi docker desktop, ataupun docker toolbox apabila requirements untuk docker desktop tidak terpenuhi.

2. Ketika instalasi sudah selesai kita dapat mengeceknya melalui cmd ataupun docker qucikstart(terminal docker) dengan menggunakan perintah "docker --version"

![versidocker](/UTS-TCC/versidocker.jpg)

3. Selanjutnya kita melakukan clone/pull terhadap repository git yang didalamnya terdapat beberapa image docker(disediakan didalam fitur getting started dockerhub)

4. Setelah proses clone selesai, saya memilih untuk menggunakan image docker dengan nama halloween2019, dengan saya memilih image docker tersebut maka saya masuk kedalam direktori image docker tersebut.didalam direktori kita dapat menggunakan perintah build untuk menjalankan isi dari DockerFile image halloween2019

![build](/UTS-TCC/build-halloween.jpg)

5. Setelah sukes melakukan build kita menggunakan perintah "docker run" yang dimana perintah run docker pertama-tama membuat layer container yang dapat ditulis di atas image yang ditentukan, dan kemudian memulainya dengan menggunakan perintah yang ditentukan.

![hasilrunhalloween](/UTS-TCC/output.jpg)

6. Pada saat menggunakan perintah "run" kita menyelipkan shorthand -t yang dimana berguna seperti membuat container tersebut memiliki sesi koneksi terminal(ketika selesai run tidak akan berhenti kecuali menggunakan perintah untuk berhenti)

7. Karena hal tersebut kita dapat menghentikan container tersebut menggunakan perintah kill atau stop, pada proses ini saya menggunakan perintah kill, dan setelah dicek container tersebut sudah tidak berjalan lagi.

![matikancontainer](/UTS-TCC/stopcontainter.jpg)

<h3>B. Pembuatan DockerFile, dan Push ke repo dockerhub</h3>

1. Pertama saya membuat folder untuk dockerFile yang ingin dibuat.

2. Lalu didalam dockerFilenya saya menggunakan base image dari ubuntu, dan meletakkan perintah untuk menampilkan pesan dari cmd.

![buat](/UTS-TCC/buatdockerfile.jpg)

3. Setelah selesai membuat docker file saya melakukan build image melalui docker quickstart terminal, dan setelah selesai build saya melakukan cek menggunakan perintah "docker images".

![buildimage](/UTS-TCC/buildockersaya.jpg)

4. Setelah itu saya melakukan run terhadap image tersebut, dan hasilnya sesuai dengan isi yang saya buat didalam dockerFile-nya yaitu menampilkan pesan di cmd.

![runimage](/UTS-TCC/hasilrunimagesaya.jpg)

5. Lalu untuk persiapan push dikarenakan kita harus mendownload image yang kita buat menjadi lokal maka saya melakukan commit didocker, dan membuat nama dan tag baru untuk image lokal-nya.

![localimage](/UTS-TCC/commitdocker.jpg)

6. Setelah mendowload image yang saya buat ke lokal, saya menggunakan perintah docker push untuk melakukan push ke repo di akun dockerhub saya

![imagepush](/UTS-TCC/dockerpush.jpg)

7. Setelah sukses kita dapat melakukan cek dengan menghapus image lokal dan pull dari repo online, tetapi saya tidak melakukan itu karena hanya buang waktu.

8. Dan akhirnya hasil push dari image lokal saya dapat dilihat di akun dockerhub saya.

![dockerrepo](/UTS-TCC/dockerhubrepo.jpg)



