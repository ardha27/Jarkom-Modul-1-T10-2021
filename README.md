# Jarkom-Modul-1-T10-2021
PRAKTIKUM MODUL 1 JARINGAN KOMPUTER 2021

Anggota Kelompok IT07:<br>
Tri Rizki Yuliawan (05311940000024) <br>
Kevin Nathaniel (05311940000032) <br>
I Gde Ardha Semaranatha Gunasatwika (05311940000034) <br>

# Soal <a name="Soal"></a>

### 1. Sebutkan webserver yang digunakan pada "ichimarumaru.tech"! 
Pencarian web server dilakukan dengan display filter `http.host contains "ichimarumaru.tech"`

Kemudian Follow TCP stream, maka kita bisa melihat web server yang digunakan, maka bisa dilihat web servernya adalah nginx/1.18.0 (Ubuntu)

### 2.Temukan paket dari web-web yang menggunakan basic authentication method!
Untuk filter website yang menggunakan basic authentication menggunakan command `http.authbasic` pada display filter

### 3.Ikuti perintah di basic.ichimarumaru.tech! Username dan password bisa didapatkan dari file .pcapng!
Untuk mengetahui username dan password saat memasuki site maka kita akan mencarinya dengan display filter menggunakan command `http.host contains “ichimarumaru.tech`

Dari snapshot tersebut bisa dilihat credentialnya yaitu :
Username : kuncimenujulautan
Pwd :  tQKEJFbgNGC1NCZlWAOjhyCOm6o3xEbPkJhTciZN
Jawaban pertanyaan : Putih hijau - Hijau - Putih Orange - Biru - Putih biru - orange - putih coklat - coklat

### 4.Temukan paket mysql yang mengandung perintah query select!
Melakukan display filter `Frame contains “SELECT”` dan akan didapatkan hasil sebagai berikut

### 5.Login ke portal.ichimarumaru.tech kemudian ikuti perintahnya! Username dan password bisa didapat dari query insert pada table users dari file .pcap!
Untuk mendapatkan username dan password, digunakan display filter `mysql`. Karena data yang didapat sedikit, kami mengecek secara manual dan didapatkan sebagai berikut,

Lalu, terdapat soal sebagai berikut,
