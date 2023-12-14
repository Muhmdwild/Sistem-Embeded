# A. ESP32 Capacitive Touch Sensor
## 1. Touch Sensor
### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![Screenshot 2023-11-28 140859](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/934aed65-6ff5-4b63-81f5-5e0b3716e280)

### b. Source Code
Kode program : <a href="touch_sensor.ino">di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Pada praktikum 2, fokusnya adalah pada protokol komunikasi dan sensor. Protokol komunikasi mengatur aturan komunikasi antara entitas, sedangkan sensor mendeteksi sinyal fisik atau lingkungan. Pada percobaan A, ESP32 Capacitive Touch Sensor digunakan, menghasilkan output yang ditampilkan di serial monitor dan Serial Plotter. Saat sensor disentuh, nilai output menjadi 0, dan grafik pada Serial Plotter menurun. LED juga menyala saat sentuhan terdeteksi.


### d. Hasil Touch Sensor
https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/1c205697-cb69-4b96-b366-3a400768368e


## 2. Touch LED Menyala

### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![Screenshot 2023-11-28 140859](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/934aed65-6ff5-4b63-81f5-5e0b3716e280)


### b. Source Code
Kode program : <a href="https://github.com/AmaliaPrisca/SISTEMEMBEDDED/blob/master/Job%202/1.%20ESP32%20Capacitive%20Touch%20Sensor/A.%20%20ESP32%20Capacitive%20Touch%20Sensor/2._LED_menyala/2._LED_menyala.ino">klik di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Dalam percobaan ini akan membuka komunikasi serial dan menampilkan pesan "ESP32 Touch Test". Dalam loop utama, nilai kapasitansi sensor sentuh pada pin T0 (GPIO 4) terus-menerus dibaca. Jika nilai kapasitansi kurang dari 20, menunjukkan adanya sentuhan, dan hal ini menyebabkan LED pada pin 16 menyala; jika tidak, maka LED akan dimatikan. Program akan terus membaca nilai sensor dan mengendalikan LED berdasarkan deteksi sentuhan yang terus-menerus dilakukan.

### d. Hasil Touch LED Menyala
https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/82542dd6-39af-4bcc-9a12-c40b539fc93d


## 3. Touch LED Menyala Blink

### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![Screenshot 2023-11-28 140859](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/934aed65-6ff5-4b63-81f5-5e0b3716e280)

### b. Source Code
Kode program :<a href="https://github.com/AmaliaPrisca/SISTEMEMBEDDED/blob/master/Job%202/1.%20ESP32%20Capacitive%20Touch%20Sensor/A.%20%20ESP32%20Capacitive%20Touch%20Sensor/3._touch_blink/2._touch_blink.ino">klik di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Selanjutnya, dalam praktikum, jika sensor disentuh, LED akan menyala dengan efek berkedip. Program yang digunakan tetap serupa dengan sebelumnya, hanya ditambahkan perintah `digitalWrite(led, LOW); delay(500);`. Saat nilai kapasitansi kurang dari 20 (menandakan sentuhan terdeteksi), LED pada pin 16 akan berkedip dengan interval 500 ms menyala dan 500 ms mati. Ketika nilai kapasitansi lebih besar atau sama dengan 20 (tidak ada sentuhan terdeteksi), LED akan dimatikan.

### d. Hasil Touch LED Menyala Blink
https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/971fdc3f-0878-4bbe-bd74-6cb9f2be95e8



## 4. Touch Bertambah

### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![Screenshot 2023-11-28 140859](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/934aed65-6ff5-4b63-81f5-5e0b3716e280)


### b. Source Code
Kode program :<a href="https://github.com/AmaliaPrisca/SISTEMEMBEDDED/blob/master/Job%202/1.%20ESP32%20Capacitive%20Touch%20Sensor/A.%20%20ESP32%20Capacitive%20Touch%20Sensor/4._touch_angka_yang_akan_bertambah_setiap_kali_sensor_disentuh/3._touch_angka_yang_akan_bertambah_setiap_kali_sensor_disentuh.ino">klik di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Pada praktikum berikutnya, saat LED menyala, nilai angka akan ditampilkan di Serial Monitor dan akan bertambah setiap kali sensor disentuh. Program ini mencakup kondisi jika nilai kapasitansi kurang dari 20, di mana LED pada pin 16 dinyalakan, nilai hitungan (hitung) ditambah 1, dan kondisi LED (kondisi led) diatur ke LED menyala. Jika tidak, LED dimatikan dan kondisi LED diatur ke LED mati. Nilai hitungan kemudian dicetak ke serial monitor.

### d. Hasil Touch Bertambah
https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/50aa40fc-5b75-49fd-98eb-781210555396

## 5. Touch LED Menyala Running
### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![Screenshot 2023-11-28 140859](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/934aed65-6ff5-4b63-81f5-5e0b3716e280)


### b. Source Code
Kode program :<a href="https://github.com/AmaliaPrisca/SISTEMEMBEDDED/blob/master/Job%202/1.%20ESP32%20Capacitive%20Touch%20Sensor/A.%20%20ESP32%20Capacitive%20Touch%20Sensor/5._LED_menyala_menjadi_running_LED/4._LED_menyala_menjadi_running_LED.ino">klik di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Pada praktikum terakhir, dalam rangkaian terdapat 3 LED, dan saat sensor disentuh, LED akan menyala menjadi running LED yang bergerak dari kiri ke kanan, kemudian dari kanan ke kiri secara kontinyu. Program ini membuka komunikasi serial dan mencetak pesan "ESP32 Touch Test". Di dalam loop utama, nilai kapasitansi sensor sentuh pada pin T0 (GPIO 4) terus-menerus dibaca. Jika nilai kapasitansi kurang dari 20 (sentuhan terdeteksi), tiga LED (led, led2, led3) akan dinyalakan secara berurutan dengan interval 500 ms menyala dan 500 ms mati. Jika tidak ada sentuhan terdeteksi, semua LED akan dimatikan. Nilai hitungan kemudian dicetak ke serial monitor.

### d. Hasil Touch LED Menyala Running
https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/ca891a87-65d2-4008-acc4-7d1b7c7ab872
