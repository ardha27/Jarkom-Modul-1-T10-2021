# Jarkom-Modul-1-T10-2021

PRAKTIKUM MODUL 1 JARINGAN KOMPUTER 2021

Anggota Kelompok IT07:<br>
Tri Rizki Yuliawan (05311940000024) <br>
Kevin Nathaniel (05311940000032) <br>
I Gde Ardha Semaranatha Gunasatwika (05311940000034) <br>

# Soal <a name="Soal"></a>

### 1. Sebutkan webserver yang digunakan pada "ichimarumaru.tech"!

Pencarian web server dilakukan dengan display filter `http.host contains "ichimarumaru.tech"`

<img src="screenshot/1.1.png">

Kemudian Follow TCP stream, maka kita bisa melihat web server yang digunakan, maka bisa dilihat web servernya adalah nginx/1.18.0 (Ubuntu)

<img src="screenshot/1.2.png">

### 2.Temukan paket dari web-web yang menggunakan basic authentication method!

Untuk filter website yang menggunakan basic authentication menggunakan command `http.authbasic` pada display filter

<img src="screenshot/2.1.png">

### 3.Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng!

Untuk mengetahui username dan password saat memasuki site maka kita akan mencarinya dengan display filter menggunakan command `http.host contains “ichimarumaru.tech`

<img src="screenshot/3.1.png">

Dari snapshot tersebut bisa dilihat credentialnya yaitu :
Username : kuncimenujulautan
Pwd : tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN
Jawaban pertanyaan : Putih hijau - Hijau - Putih Orange - Biru - Putih biru - orange - putih coklat - coklat

<img src="screenshot/3.2.png">

### 4.Temukan paket mysql yang mengandung perintah query select!

Melakukan display filter `Frame contains “SELECT”` dan akan didapatkan hasil sebagai berikut

<img src="screenshot/4.1.png">

### 5.Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari query insert pada table users dari file .pcap!

Untuk mendapatkan username dan password, digunakan display filter `mysql`. Karena data yang didapat sedikit, kami mengecek secara manual dan didapatkan sebagai berikut,

<img src="screenshot/5.1.png">

Lalu, terdapat soal sebagai berikut,

<img src="screenshot/5.2.png">

### 11. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!

Kita dapat menggunakan filter command : `src port 80`

<img src="screenshot/11.1.png">

### 12. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!

Kita dapat menggunakan filter command: `port 21`

<img src="screenshot/12.1.png">

Tidak terdapat lalu lintas data karena port 21 biasanya hanya digunakan pada saat mengakses FTP Server dan pada saat itu saya tidak mengakses FTP server sehingga tidak ada lalu lintas data.

### 13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!

Kita dapat menggunakan filter command: `dst port 443`

<img src="screenshot/13.1.png">

### 14. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke kemenag.go.id!

Untuk mengambil paket yang tujuannya ke kemenag.go.id, kita bisa menggunakan capture filter `dst host kemenag.go.id`

<img src="screenshot/14.1.png">

### 15. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

Untuk mencari ip, kami menggunakan command prompt, kemudian mengetikkan command ipconfig. Dari situ, kami menemukan bahwa ip kami adalah 192.168.43.13

<img src="screenshot/15.1.png">

Sehingga untuk mengambil paket yang berasal dari ip kami, dapat menggunakan capture filter: `ip src 192.168.43.13`

<img src="screenshot/15.2.png">
