# Pengukuran Parameter QoS (Quality Of Service) : Throughput, Delay, Jitter, Packet Loss

Wireshark adalah perangkat lunak analisis jaringan yang memungkinkan pengguna untuk menangkap, memantau, dan menganalisis lalu lintas data dalam jaringan komputer secara detail, sehingga memungkinkan pengguna untuk memecahkan masalah jaringan, memantau kinerja, dan menganalisis keamanan jaringan dengan mudah.

### Langkah-Langkah Menjalankan

Untuk mendapatkan parameter waktu di Wireshark, terlebih dahulu menonton youtube atau bermain game online. Disini saya menonton youtube kira-kira selama 10 menit untuk mendapatkan parameter waktu.

1. Buka Wireshark dan pilih wifi lalu buka youtube dan tonton sampai waktu yang ditentukan.

![App Screenshot](/Image/1.%20Buka%20Wireshark%20dan%20pilih%20wifi.png)

2. Buka Wireshark dan pilih wifi lalu buka youtube dan tonton sampai waktu yang ditentukan.

![App Screenshot](/Image/2.%20Data%20parameter.png)

3. Lalu kita akan mengukur Throughput, untuk melihat time span dan bytes kita harus pergi ke statistics lalu Capture File Properties.

![App Screenshot](/Image/3.%20Pilih%20Capture%20File%20Properties.jpg)

4. Lalu, catat time span dan bytes, dan cari maka nanti hasilnya akan sama dengan Avarage bits/s.

![App Screenshot](/Image/4.%20time%20span%20dan%20bytes.png)

5. Kita cari dengan rumus seperti dibawah ini.

![App Screenshot](/Image/5.%20Rumus%20Throughput.png)

6. Sekarang kita akan melihat 'Packet Loss' dengan cara ketik pada wireshark `tcp.analysis.lost_segment' maka data packet loss akan keluar kemudian kalian hitung untuk menghitung rata-rata dari packet loss.

![App Screenshot](/Image/6.%20tcp.analysis.lost_segment.png)

7. Untuk melihat keseluruhan packet kalian pergi ke statistic dan lihat jumlah packet disana.

![App Screenshot](/Image/packets.png)

8. lalu hitung packet loss dengan rumus seperti dibawah ini

![App Screenshot](/Image/packtess%20loss.png)

9. kita akan menghitung Delay, dengan cara kita ketik di wireshark tcp maka data-data akan terfilter. Lalu pilih File pilih Export Packet Dissections dan pilih As CSV agar mempermudah menghitung delay.

![App Screenshot](/Image/export%20ke%20excel.jpg)

10. Oke, selanjutnya kita akan menghitung Jitter, kita harus membuat Delay1, Delay2 dan Jitter Delay1 kita ambil dari nilai Delay waktu yang pertama dikurangi dengan Delay waktu kedua, Delay2 kita ambil dari nilai Delay waktu yang kedua, dan Jitter hasil dari Delay2 dikurang Delay1.

11. Untuk mencari Total Jitter kita jumlahkan seluruh Jitter, dan untuk mencari Rata-rata Jitter dengan cara Total Delay dibagi dengan Paket Diterima.

![App Screenshot](/Image/Terakhir.png)
