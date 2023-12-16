# E. Two-Way Communication

## 1. Two-Way Communication 1

### a. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut
![rangkaian](https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/fb549940-0d36-44e0-93ab-ba3e43dcd991)

### b. Source Code
Kode program : <a href="1/2_way_comm_1">di sini</a>

### c. Hasil dan Pembahasan
Dalam implementasinya, pengembang harus memilih protokol komunikasi yang mendukung two-way communication, mengkonfigurasi jaringan untuk memastikan keterhubungan perangkat, dan menulis kode yang mendukung pembacaan data, pengiriman pesan, dan penanganan respons.

##### Hasil Cek
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/f97b1805-4b27-44e4-989e-5f2729a4c11c

##### Hasil Akhir
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/6f9fdaac-467c-4992-a39e-b8c78a8996e1

## 2. Two-Way Communication 2

### a. Source Code
Kode program : <a href="e. Two-Way Communication/2/2_way_comm_2/2_way_comm_2.ino">klik di sini</a>

### b. Hasil dan Pembahasan
Two-way communication pada ESP32 dapat diimplementasikan dengan menggunakan protokol MQTT. Misalnya, ESP32 sebagai pengirim mengirimkan data sensor ke topik tertentu di broker MQTT, dan ESP32 sebagai penerima berlangganan topik yang sama untuk menerima dan merespons data. Dengan demikian, ESP32 dapat saling berkomunikasi, memungkinkan pertukaran informasi dan kontrol aktif antar perangkat dalam konteks Internet of Things (IoT).

https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/7f876392-e9e7-4dc2-8685-fad7f17f0094
