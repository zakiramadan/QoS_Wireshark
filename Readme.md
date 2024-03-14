# Pengukuran Parameter QoS (Quality Of Service) : Throughput, Delay, Jitter, Packet Loss

Wireshark adalah perangkat lunak analisis jaringan yang memungkinkan pengguna untuk menangkap, memantau, dan menganalisis lalu lintas data dalam jaringan komputer secara detail, sehingga memungkinkan pengguna untuk memecahkan masalah jaringan, memantau kinerja, dan menganalisis keamanan jaringan dengan mudah.

### Langkah-Langkah Menjalankan

Untuk mendapatkan parameter waktu di Wireshark, terlebih dahulu menonton youtube atau bermain game online. Disini saya menonton youtube kira-kira selama 10 menit untuk mendapatkan parameter waktu.

1. Buka Wireshark dan pilih wifi lalu buka youtube dan tonton sampai waktu yang ditentukan.

![1  Buka Wireshark dan pilih wifi](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/89900b92-523c-4175-9533-48a8c3c1b00f)

2. Buka Wireshark dan pilih wifi lalu buka youtube dan tonton sampai waktu yang ditentukan.

![2  Data parameter](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/443017ba-92ff-4d79-820f-fca9b3f0fa26)

3. Lalu kita akan mengukur Throughput, untuk melihat time span dan bytes kita harus pergi ke statistics lalu Capture File Properties.

![3  Pilih Capture File Properties](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/9281bb69-5a4c-4143-84c0-469d7aa82f19)

4. Lalu, catat time span dan bytes, dan cari maka nanti hasilnya akan sama dengan Avarage bits/s.

![4  time span dan bytes](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/19e3e068-c989-4438-8eb9-b425f68bf45e)

5. Kita cari dengan rumus seperti dibawah ini.

![5  Rumus Throughput](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/907a3b7e-60c8-4b76-8d24-e90898089faf)

6. Sekarang kita akan melihat 'Packet Loss' dengan cara ketik pada wireshark `tcp.analysis.lost_segment' maka data packet loss akan keluar kemudian kalian hitung untuk menghitung rata-rata dari packet loss.

![6  tcp analysis lost_segment](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/81ddab85-e942-4130-ba63-36777391adc2)

7. Untuk melihat keseluruhan packet kalian pergi ke statistic dan lihat jumlah packet disana.

![packets](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/2d150e83-6180-4dc4-acb2-e5462252831b)

8. lalu hitung packet loss dengan rumus seperti dibawah ini

![packtess loss](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/5b7033fc-460d-470c-b238-0e5561cc5d49)

9. kita akan menghitung Delay, dengan cara kita ketik di wireshark tcp maka data-data akan terfilter. Lalu pilih File pilih Export Packet Dissections dan pilih As CSV agar mempermudah menghitung delay.

![export ke excel](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/5e4c6149-e2e1-4059-a814-057d2be4887e)

10. Oke, selanjutnya kita akan menghitung Jitter, kita harus membuat Delay1, Delay2 dan Jitter Delay1 kita ambil dari nilai Delay waktu yang pertama dikurangi dengan Delay waktu kedua, Delay2 kita ambil dari nilai Delay waktu yang kedua, dan Jitter hasil dari Delay2 dikurang Delay1.
    
![8  Export Packet Dissections dan pilih As CSV](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/eb2c9c7d-39cb-423f-ae67-45dc07848610)


12. Untuk mencari Total Jitter kita jumlahkan seluruh Jitter, dan untuk mencari Rata-rata Jitter dengan cara Total Delay dibagi dengan Paket Diterima.

![Terakhir](https://github.com/zakiramadan/QoS_Wireshark/assets/126186033/f12292f7-a188-42d2-afc1-cce2c9c1bd2c)
