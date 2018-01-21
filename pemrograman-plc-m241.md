# 1. Pemrograman PLC M241 Menggunakan Software SoMachine V4.1

## 1.1 Membuat Project Baru

Langkah-langkah untuk membuat project baru menggunakan software SoMachine V4.1 adalah sebagai berikut :

1. Buka software SoMachine V4.1 pada computer Anda, kemudian klik menu New Project untuk membuat project baru  
   ![](/assets/2018-01-21_190657.png)

2. Pilih menu Empty Project untuk membuat project kosong dari awal  
   ![](/assets/2018-01-21_190729.png)

3. Beri nama project yang akan dibuat, kemudian klik menu Create Project untuk meng-generate project  
   ![](/assets/2018-01-21_190811.png)

4. Klik menu Manage Device untuk melakukan konfigurasi perangkat controller yang akan digunakan pada project yang telah dibuat  
   ![](/assets/2018-01-21_190824.png)

5. Pilih jenis PLC yang sesuai, pada kali ini akan digunakan PLC dengan seri M241CE40R. Lakukan pencarian pada bagian Logic Controller lalu pilih tipe PLC M241 dan pilih seri PLC yang sesuai  
   ![](/assets/2018-01-21_190854.png)

6. Klik tombol arah ke kanan untuk menggunakan PLC seri tersebut pada project yang telah dibuat, kemudian klik OK untuk melanjutkan ke tahap berikutnya  
   ![](/assets/2018-01-21_190904.png)  
   ![](/assets/2018-01-21_190932.png)

7. Klik Open Configuration untuk membuka project yang telah Anda buat  
   ![](/assets/2018-01-21_190941.png)

8. Simpan project yang telah dibuat pada direktori khusus dengan cara memilih menu Save pada pojok kiri atas, sesuaikan nama file-nya dengan nama project yang telah dibuat diawal  
   ![](/assets/2018-01-21_191137.png)![](/assets/2018-01-21_191213.png)

9. Menu Device digunakan untuk melakukan konfigurasi terhadap modul perangkat keras yang ada pada PLC seperti modul input, modul output, modul komunikasi dan modul lainnya  
   ![](/assets/2018-01-21_191251.png)

10. Menu Application digunakan untuk melakukan konfigurasi terhadap perangkat lunak pada PLC seperti variabel dan program  
    ![](/assets/2018-01-21_191314.png)

## 1.2 Mendeklarasikan Variabel Pada GVL \(Global Variable List\)

Langkah-langkah untuk mendeklarasikan variabel pada software SoMachine V4.1 adalah sebagai berikut :

1. Klik dua kali pada menu GVL 
   ![](/assets/2018-01-21_201132.png)

2. Akan muncul layar kosong yang berisi text editor yang dapat digunakan untuk mendeklarasikan variabel dengan cara texttual \(diketik\). Pada kali ini deklarasi variabel akan dilakukan melalui tabular \(menggunakan tabel\). Pilih menu tabular agar text editor berubah manjadi sebuah tabel
   ![](/assets/2018-01-21_201208.png)![](/assets/2018-01-21_201256.png)

3. Variabel bisa dideklarasikan dengan cara melakukan klik kanan pada editor tabular, kemudian pilih menu Insert
   ![](/assets/2018-01-21_201423.png)

4. Tulislah nama variabel yang akan dideklarasikan. Pada contoh kali ini akan dideklarasikan variabel dengan nama TOMBOL dan tipe data BOOL \(boolean\). Buatlah variabel lainnya dengan nama LAMPU dan SUHU dengan tipe data BOOL
   ![](/assets/2018-01-21_201452.png)

5. Secara default tipe data yang dideklarasikan adalah tipe boolean. Jika tipe data ini ingin dirubah ke bentuk lain, caranya adalah dengan mengklik dua kali pada kolom Data type kemudian memilih menu "&gt;"
   ![](/assets/2018-01-21_201548.png)

6. Kemudian pilih tipe data yang diinginkan. Pada contoh kali ini variabel SUHU akan diganti tipe datanya menjadi INT \(integer\)
   ![](/assets/2018-01-21_201608.png)

7. Anda dapat memastikan tipe datanya telah berubah dengan melihat langsung pada editor tabular
   ![](/assets/2018-01-21_201620.png)

8. Anda juga dapat melihat source code program untuk deklarasi variabel secara textual dengan mengklik kembali menu textual
   ![](/assets/2018-01-21_201641.png)

## 1.3 Membuat Program

## 1.4 Men-download Program ke PLC

## 1.5 Melakukan Simulasi Program



