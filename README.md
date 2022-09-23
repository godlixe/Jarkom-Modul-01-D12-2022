# D12

### 1. Soal 1
Sebutkan web server yang digunakan pada "monta.if.its.ac.id"! 

#### Jawaban
Cara untuk mendapatkan web server yang digunakan pada situs di atas adalah dengan meng-capture paket-paket terlebih dahulu, mengakses monta.if.its.ac.id, stop capture, lalu pada display filter kita gunakan filter “tcp contains monta” sehingga didapat seperti gambar di bawah. 
![](pic/pic10.png)

### 2. Soal 2
Ishaq sedang bingung mencari topik ta untuk semester ini , lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id” , judul TA apa yang dibuka oleh ishaq ?

#### Jawaban
Kita akan mencari detail link yang diakses oleh Ishaq sehingga pada display filter kita menerapkan filter “http.request.uri contains "detail"” sehingga didapat hasil seperti di bawah.
![](pic/pic11.png)

Klik pada hasil capture paket untuk melihat detailnya didapat link yang diakses adalah http://monta.if.its.ac.id/index.php/topik/detailTopik/194. 
![](pic/pic12.png)

Ketika link tersebut diakses, muncul judul ta yang dibuka oleh Ishaq adalah “Topik Tugas Akhir”.
![](pic/pic13.png)

### 3. Soal 3
Filter sehingga wireshark hanya menampilkan paket yang menuju port 80! 

#### Jawaban
Menggunakan display filter tcp.dstport == 80
![](pic/pic14.png)

### 4. Soal 4
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!

#### Jawaban

Menggunakan display filter `tcp.srcport == 21`

### 5. Soal 5
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!

#### Jawaban

Menggunakan display filter `tcp.srcport == 443`

### 6. Soal 6
Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id
#### Jawaban

Menggunakan display filter `tcp.srcport == 443`

### 7. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

Buka cmd dan tuliskan ` ipconfig ` 
![](pic/pic1.png)

Selanjutnya pilih IPv4 sesuai dengan source yang mau ditangkap, saya memilih wi-fi
![](pic/pic2.png)

Selanjutnya memasukkan argument ke capture filter wireshark, yaitu ` ip src (ip anda) `
![](pic/pic3.png)

Berikut adalah hasilnya
![](pic/pic4.png)


### 8. Soal 8
Buka file ` soal8-10.pcapng ` dan tulis argumen ` tcp ` ke dalam display filter
![](pic/pic5.png)

Kemudian klik kanan pada salah satu packet dan pilih follow -> tcp stream
![](pic/pic6.png)

Hasilnya adalah sebagai berikut
![](pic/pic7.png)

![](pic/pic8.png)

![](pic/pic9.png)

### 9. Soal 9

### 10. Soal 10
