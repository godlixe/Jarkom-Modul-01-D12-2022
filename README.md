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

Menggunakan capture filter `src port 21`
![](pic/pic15.png)

### 5. Soal 5
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!

#### Jawaban

Menggunakan capture filter `src port 443`
![](pic/pic16.png)

### 6. Soal 6
Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id

#### Jawaban

Menggunakan display filter `http contains lipi.go.id`
![](pic/pic17.png)

### 7. Soal 7
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

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
Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama “flag.txt”.

Dari percakapan bisa diambil bahwa file dikirim melalui port 9002. Memasukkan argumen ke dalam display filter tcp.port == 9002
![](pic/pic18.png)

Kemudian klik kanan dari salah satu packet, follow -> tcp stream akan didapatkan sebagai berikut
![](pic/pic19.png)

Kemudian pilih show data as raw dan save file dengan [nama kelompok].des3 (D12.des3)

Setelah disimpan dengan format raw, file kemudian didecode melalui openssl sebagai berikut 
![](pic/pic20.png)

### 10. Soal 10
Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!
JaRkOm2022{8uK4N_CtF_k0k_h3h3h3}
![](pic/pic21.png)

## Kendala Yang Dialami
1. saat mendecode file hasil dari wireshark
![](pic/pic22.png)
