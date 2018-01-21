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

## 1.3 Membuat POU \(Program Organization Unit\)

Langkah-langkah untuk membuat POU pada software SoMachine V4.1 adalah sebagai berikut ini :

1. Klik kanan pada menu Application kemudian pilih Add Object lalu pilih POU  
   ![](/assets/2018-01-21_204349.png)

2. Berikan nama pada POU yang dibuat. Pada contoh kali ini diberi nama Program\_1. Kemudian pilih bahasa perograman yang digunakan pada menu Implementation Language. Pada kali ini akan digunakan bahasa Ladder Logic Diagram \(LD\). Setelah itu lanjutkan dengan menekan tombol ADD. Layar editor Ladder Logic Diagram akan terbuka  
   ![](/assets/2018-01-21_204429.png)  
   ![](/assets/2018-01-21_204443.png)

3. Tambahkan simbol contact NO dan coil pada Ladder Diagram Editor dengan cara memilih simbol pada menu berikut ini  
   ![](/assets/2018-01-21_204519.png)![](/assets/2018-01-21_204537.png)

4. Berikan variabel pada contact NO dan coil yang telah dibuat. Cara memberikan variabel dapat dilakukan dengan cara mengklik tanda tanya, kemudian pilih tombol "..."   
   ![](/assets/2018-01-21_204558.png)

5. Pada window Input Assistant pilihlah variabel yang telah dibuat tadi yaitu variabel TOMBOL. Kemudian klik OK  
   ![](/assets/2018-01-21_204623.png)

6. Lakukan hal yang sama pada coil dengan memilih variabel LAMPU. Sehingga program akhir Anda menjadi seperti berikut ini  
   ![](/assets/2018-01-21_204650.png)

7. Masukkan program POU yang telah dibuat pada MAST task. Caranya dengan melakukan drag and drop POU ke area MAST   
   ![](/assets/2018-01-21_221546.png)

8. Lakukan kompilasi program untuk memastikan tidak ada error pada program. Caranya dengan menekan menu Build atau menekan tombol keyboard F11  
   ![](/assets/2018-01-21_220250.png)

9. Pastikan tidak ada error pada status hasil kompilasi di pojok kiri bawah  
   ![](/assets/2018-01-21_220625.png)

## 1.4 Melakukan Simulasi Program

Langkah-langkah untuk melakukan simulasi program yang telah dibuat adalah sebagai berikut :

1. Klik kanan pada menu Application kemudian pilih Add Object dan Visualization
   ![](/assets/2018-01-21_220754.png)

2. Buatlah nama khusus untuk melakukan simulasi. Pada contoh kali ini bernama Simulasi\_Program\_1. Lanjutkan dengan menekan tombol Add. Selanjutnya window Visualization editor akan muncul.
   ![](/assets/2018-01-21_220834.png)  
   ![](/assets/2018-01-21_220852.png)

3. Tambahkan komponen Push Switch pada Visualization editor. Caranya dengan melakukan drag and drop komponen Push Switch pada Toolbox sebelah kanan ke Visualization Editor.
   ![](/assets/2018-01-21_220917.png)  
   ![](/assets/2018-01-21_220947.png)

4. Berikan nama variabel pada komponen Push Switch dengan cara mengklik komponen terlebih dahulu, lalu merubah properties Variable.
   ![](/assets/2018-01-21_221019.png)

5. Pilih variabel TOMBOL untuk mensimulasikan komponen Push Switch
   ![](/assets/2018-01-21_221031.png)

6. Tambahkan komponen Lamp ke Visualization Editor dan berikan nama variabel LAMPU
   ![](/assets/2018-01-21_221057.png)

7. Aktifkan menu simulasi dengan cara memilih menu Online kemudian pilih Simulation
   ![](/assets/2018-01-21_221320.png)

8. Lakukan login ke Device Simulator dengan cara memilih menu Login atau menekan tombol keyboard ALT + F8
   ![](/assets/2018-01-21_221215.png)

9. Jika muncul window untuk memilih controller, maka lakukan klik pada CODESYS Controller
   ![](/assets/2018-01-21_221240.png)

10. Akan muncul pesan Warning. Lanjutkan dengan menekan kombinasi ALT + F pada keyboard 
    ![](/assets/2018-01-21_221248.png)

11. Lanjutkan proses Login jika muncul window konfirmasi
    ![](/assets/2018-01-21_221348.png)

12. Pilih Yes jika muncul Window yang meminta konfirmasi proses download program
    ![](/assets/2018-01-21_221401.png)

13. Setelah proses download program berhasil, akan muncul status di bagian bawah bahwa kondisi controller dalam keadaan STOP. Aktifkan controller dengan cara menekan menu Run.
    ![](/assets/2018-01-21_221423.png)

14. Setelah controller dalam mode running, program POU yang telah Anda dapat dimonitor kondisinya menjadi seperti berikut ini
    ![](/assets/2018-01-21_221703.png)

15. Lakukan ujicoba dengan menekan tombol pada window Visualization Editor kemudian perhatikan nyala lampu. Lampu akan menyala jika tombol ditekan. Untuk mematikan lampu tekan sekali lagi pada tombol.
    ![](/assets/2018-01-21_221739.png)

## 1.5 Melakukan Simulasi Program ???



