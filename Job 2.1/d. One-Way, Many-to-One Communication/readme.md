# A. One-Way, Many-to-One Communication

## 1. One Way Many To One

### a. Source Code
Kode program : <a href="/one_way_many_to_one/one_way_many_to_one.ino">di sini</a>

### b. Hasil dan Pembahasan
Dalam percobaan ini program dibuat untuk dapat mengirimkan pesan dari beberapa ESP32 menuju satu ESP32. Langkah-langkah implementasinya melibatkan konfigurasi jaringan, pemilihan protokol komunikasi seperti MQTT atau UDP, serta penulisan kode untuk memungkinkan ESP32 penerima menerima data dari beberapa perangkat pengirim. Keuntungan dari pendekatan ini termasuk efisiensi dalam mengelola data dari beberapa sumber, sementara tantangan utamanya adalah memastikan koordinasi yang baik antara perangkat pengirim dan penerima serta manajemen sumber daya pada ESP32 pusat.

##### Hasil Receiver
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/f3f6511b-7b9e-4cb6-88f1-ddd8416dea6f

##### Hasil Sender
https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/34af09a9-fafc-4e10-a83f-b5a122daff6d
