# D12

1.
2.
3.
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
[](pic/pic1)

Selanjutnya pilih IPv4 sesuai dengan source yang mau ditangkap, saya memilih wi-fi
[](pic/pic2)

Selanjutnya memasukkan argument ke capture filter wireshark, yaitu ` ip src (ip anda) `
[](pic/pic3)

Berikut adalah hasilnya
[](pic/pic4)

8.
9.
10.
