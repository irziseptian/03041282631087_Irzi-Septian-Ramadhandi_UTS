Kelompok C – Instrumentasi  
[Monitoring Level Tangki] 
Project ini dibuat untuk memantau ketinggian air dalam tangki berdasarkan nilai persentase. Program Phyton ini 
akan mengelompokkan setiap data level tangki menjadi tiga status, yaitu LOW, NORMAL, dan HIGH. 
Tujuannya, pengguna dapat mengetahui kondisi level tangki, jumlah data pada setiap kategori, serta nilai rata
rata, maksimum, dan minimum. 
1. Input – Process - Output 
A. Input 
15 data level tangki yang telah diberikan dalam soal, 5 data tambahan, total data sebanyak 20 data. 
Cat: Satuan data menggunakan persentase (%). 
B. Process 
Memasukkan 20 data level, Memeriksa setiap data menggunakan perulangan. Menentukan status berdasarkan 
nilai level ,Menghitung jumlah setiap kategori ,Menghitung nilai rata-rata ,Menentukan nilai maksimum dan 
minimum ,Melakukan pengujian menggunakan 8 test case. 
C. Output 
Nomor atau urutan data ,Status LOW, NORMAL, atau HIGH ,Jumlah data pada setiap kategori ,Total 
keseluruhan data ,Nilai rata-rata ,Nilai maksimum dan minimum 
2. Daftar function yang dibuat beserta tujuan, parameter, dan return. 
a. rata_rata(data) 
Tujuan: Menghitung nilai rata-rata dari seluruh data. 
 Parameter: data (daftar nilai). 
 Return: Hasil rata-rata. 
b. kategori_status(status) 
Tujuan: Menentukan kategori berdasarkan nilai persentase. 
 Parameter: status (nilai persentase). 
 Return: Kategori "HIGH", "NORMAL", atau "LOW". 
Ketentuannya: 
 HIGH: nilai lebih dari 80. 
 NORMAL: nilai 30 sampai 80. 
 LOW: nilai kurang dari 30. 
c. 
hitung_kategori(data) 
Tujuan: Menghitung jumlah data pada setiap kategori. 
 Parameter: data (daftar nilai). 
 Return: Dictionary berisi jumlah HIGH, NORMAL, dan LOW. 
3. Penjelasan Singkat Penggunaan Decision Dan Loop  
A . Decision (Percabangan) 
Decision menggunakan if, elif, dan else pada function kategori_status() untuk menentukan kategori nilai 
berdasarkan kondisi: 
 HIGH jika nilai lebih dari 80. 
 NORMAL jika nilai 30–80. 
 LOW jika nilai kurang dari 30. 
B . Loop (Perulangan) 
Loop menggunakan for untuk mengulang dan memproses seluruh data. Perulangan digunakan untuk: 
 Menjumlahkan seluruh nilai untuk menghitung rata-rata. 
 Menghitung jumlah data berdasarkan kategori HIGH, NORMAL, dan LOW. 
 Menampilkan setiap data beserta nomor urut dan kategorinya. 
4. Contoh output program
===== MONITORING LEVEL TANGKI =====
01. Nilai = 18% -> LOW
02. Nilai = 25% -> LOW
03. Nilai = 33% -> NORMAL
04. Nilai = 41% -> NORMAL
05. Nilai = 55% -> NORMAL
06. Nilai = 62% -> NORMAL
07. Nilai = 76% -> NORMAL
08. Nilai = 84% -> HIGH
09. Nilai = 91% -> HIGH
10. Nilai = 47% -> NORMAL
11. Nilai = 29% -> LOW
12. Nilai = 38% -> NORMAL
13. Nilai = 70% -> NORMAL
14. Nilai = 82% -> HIGH
15. Nilai = 15% -> LOW
16. Nilai = 12% -> LOW
17. Nilai = 30% -> NORMAL
18. Nilai = 50% -> NORMAL
19. Nilai = 80% -> NORMAL
20. Nilai = 95% -> HIGH
===== RINGKASAN =====
Total data : 20
LOW        : 5
NORMAL     : 11
HIGH       : 4
Rata-rata : 51.65 %
Maksimum  : 95 %
Minimum   : 12 %

===== TESTING =====
1. Nilai = 29% -> LOW
2. Nilai = 30% -> NORMAL
3. Nilai = 31% -> NORMAL
4. Nilai = 79% -> NORMAL
5. Nilai = 80% -> NORMAL
6. Nilai = 81% -> HIGH
7. Nilai = 18% -> LOW
8. Nilai = 91% -> HIGH
===== SELESAI =====
6. Lima data tambahan yang dipilih sendiri dan alasan singkat mengapa data 
tersebut masih relevan 
No. Data Tambahan 
Alasan 
16 
12% 
Mewakili kondisi level sangat rendah. 
17 
30% 
Menguji batas awal kategori NORMAL. 
18 
50% 
Mewakili kondisi level normal. 
19 
80% 
Menguji batas akhir kategori NORMAL. 
20 
95% 
Mewakili kondisi level tinggi. 
7. Pernyataan penggunaan AI bila digunakan. 
Github-Copilot digunakan untuk merapihkan kode serta menghilangkan kemungkinan typo0
