# B. Mengakses Sensor DHT 11 (Single Wire/BUS)
## 1. DHT Single Wire
### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut
</br>
![Screenshot 2023-11-28 150136](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/4fda8a34-ec2f-4278-a6c5-e5d72c44b2b2)



### b. Source Code
Kode program : <a href="https://github.com/AmaliaPrisca/SISTEMEMBEDDED/blob/master/Job%202/2.%20DHT/B.%20Mengakses%20Sensor%20DHT%2011%20(Single%20Wire%20%20BUS)/DHT_1/DHT_1.ino">di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Percobaan B, dilakukan akses terhadap Sensor DHT 11 (Single Wire / BUS) di mana jika suhu ruangan mencapai 30 derajat Celsius, ESP32 akan menyalakan LED Merah dan buzzer secara beep (blink). Jika suhu berada di bawah 30 derajat, ESP32 akan mematikan buzzer dan menyalakan LED dalam bentuk running LED, mirip dengan yang dilakukan pada Percobaan A. 
Cara kerja program dimulai dengan membuka komunikasi serial dan mencetak pesan "DHT11 Embedded System Test". Di dalam loop utama, program membaca nilai suhu dan kelembaban dari sensor DHT. Jika pembacaan gagal, program akan mencetak pesan kesalahan. Selanjutnya, program menghitung dan menampilkan indeks panas. Berdasarkan nilai suhu, program mengontrol LED dan buzzer. Jika suhu lebih dari 36°C, LED Merah (LEDM) dan buzzer akan menyala dengan interval 500 ms menyala dan 500 ms mati. Sedangkan jika suhu tidak lebih dari 36°C, LED Hijau (LEDH), LED Kuning (LEDK), LED Merah (LEDM), dan LED Biru (LEDB) akan menyala berurutan dengan interval 500 ms menyala dan 500 ms mati.

### d. Hasil DHT 11 Single Wire
https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/5beb9e32-0912-4202-b449-3ecae31e1e6d
