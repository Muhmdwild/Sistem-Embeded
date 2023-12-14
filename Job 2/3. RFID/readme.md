# C. Mengakses Sensor RFID (SPI Communication)
## 1. Sensor RFID
### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut
![Screenshot 2023-11-28 150701](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/3d1cba70-1a64-45ac-8bea-30f2455db8da)

### b. Source Code
Kode program : <a href="https://github.com/AmaliaPrisca/SISTEMEMBEDDED/blob/master/Job%202/3.%20RFID/C.%20Mengakses%20Sensor%20RFID%20(SPI%20Communication)/RFID_1/RFID_1.ino">di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">pada Percobaan C, dilakukan akses terhadap Sensor RFID dengan menggunakan metode komunikasi SPI (Serial Peripheral Interface). Apabila Tag RFID yang telah terbaca sebelumnya digunakan untuk akses, berbagai tindakan akan dilakukan. Jika Tag RFID didekatkan pada Reader, LED Hijau akan menyala, servo motor akan bergerak ke arah kanan (kemudian kembali ke posisi semula setelah 3 detik), dan pesan "Akses Diterima, Silahkan Masuk" akan ditampilkan di Serial Monitor. Sebaliknya, jika Tag RFID tidak dikenali, LED Merah akan menyala, servo tidak akan bergerak, dan pesan "Akses Ditolak" akan muncul di Serial Monitor. Kemudian, menggunakan Tag RFID lain untuk melakukan percobaan yang sama.
Dalam loop utama program, dilakukan pengecekan apakah ada kartu baru yang tersedia. Jika ya, program akan membaca Unique ID (UID) dari kartu tersebut dan memeriksa apakah UID tersebut sesuai dengan yang diizinkan. Jika sesuai, akses akan diizinkan, servo motor akan bergerak ke posisi tertentu, dan LED hijau akan menyala. Namun, jika tidak sesuai, akses akan ditolak dan LED merah akan menyala.

### d. Hasil DHT 11 Single Wire
https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/7a5ba800-6ccd-4e39-858b-2dc423c6d227
