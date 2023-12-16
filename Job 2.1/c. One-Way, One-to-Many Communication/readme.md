# C. One-Way, One-to-Many Communication

## 1. Mengirim Pesan yang Sama Ke Beberapa Board ESP32

### a. Source Code
Kode program : <a href="1. Mengirim Pesan yang Sama Ke Beberapa Board ESP32/4_ESP_collab/4_ESP_collab.ino">di sini</a>

### b. Hasil dan Pembahasan
Dalam percobaan ini program dibuat untuk mengirim pesan yang sama pada beberapa board. One-Way, One-to-Many Communication untuk mengirim pesan yang sama ke beberapa Board ESP32 melibatkan konfigurasi jaringan yang sama, pemilihan protokol komunikasi seperti MQTT atau UDP, pengaturan pengirim untuk mengirim pesan ke alamat yang dapat diakses oleh semua ESP32 penerima, konfigurasi penerima untuk menerima pesan tersebut, dan penulisan kode menggunakan Arduino IDE atau platform ESP32. Selain itu, aspek keamanan harus diperhatikan, dan manajemen kesalahan harus diimplementasikan untuk meningkatkan kehandalan komunikasi. Keseluruhan proses ini memungkinkan pengiriman efisien pesan yang sama ke beberapa Board ESP32 secara bersamaan.

##### Hasil Receiver
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/a4852418-d7b9-46d5-9fa0-6df5678a5266

##### Hasil Sender Fail
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/8ff971f2-046b-4b32-b670-79127b9f748d

##### Hasil Sender Success
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/cb26cb28-2c3f-40d1-a970-82885dc443ac

## 2. Mengirim Pesan yang Berbeda Ke Beberapa Board ESP32

### a. Source Code
Kode program : <a href="2. Mengirim Pesan yang Berbeda Ke Beberapa Board ESP32/4_ESP_collab_beda_pesan/4_ESP_collab_beda_pesan.ino">klik di sini</a>

### b. Hasil dan Pembahasan
Dalam percobaan ini program dibuat untuk untuk mengirim pesan yang berbeda pada beberapa board. Pengaturan pengirim untuk mengirim pesan dengan informasi atau instruksi yang sesuai dengan kebutuhan perangkat penerima tertentu, serta penulisan kode yang memungkinkan ESP32 penerima untuk menangani pesan sesuai dengan topiknya. 

##### Hasil Data 1
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/6e4820c9-fd23-4b9a-ae54-b2cc97273e68

##### Hasil Data 2
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/32755734-cbbb-4e5f-b18b-621f8092549f

##### Hasil Data 3
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/05aff98b-dce6-427c-ae0f-26c47c5ee560

##### Hasil Sender
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/04a4183a-6690-44ca-9f03-bbc25db73dea
