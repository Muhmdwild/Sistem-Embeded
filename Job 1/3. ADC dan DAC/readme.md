# C. ADC (Analog to Digital Converter) dan DAC (Digital to Analog Converter)

## 1. ADC dan DAC | Membaca Nilai Analog dari Potensiometer

### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![5](https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/724ff1b9-da4c-481d-a303-d9f6f9638d49)
<br>
![1](https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/f3beb30c-2af2-4a0f-9526-125e220fa4be)



### b. Source Code
Kode program : <a href="ADC%20dan%20DAC/ADC%20dan%20DAC/ADC_1/ADC_1.ino">klik di sini</a>

### c. Hasil dan Pembahasan
Dalam fungsi setup(), program menginisialisasi komunikasi serial dengan Serial.begin(115200) dan memberikan jeda waktu selama 1 detik menggunakan delay(1000). Pada fungsi loop(), beberapa langkah utama dijalankan. Pertama, program membaca nilai analog dari potensiometer menggunakan fungsi analogRead(potPin) dan menyimpannya dalam variabel potValue. Selanjutnya, nilai potensiometer tersebut ditampilkan di Serial Monitor dengan menggunakan Serial.println(potValue). Terdapat juga delay sebesar 500 ms menggunakan delay(500) agar nilai potensiometer tidak berubah terlalu cepat, memudahkan pemantauan melalui Serial Monitor.

https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/dcc24334-893e-4070-9eb1-0a76d5e29306


## 2. ADC dan DAC | Mengatur Kecerahan LED Menggunakan Potensiometer

### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![5](https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/724ff1b9-da4c-481d-a303-d9f6f9638d49)
<br>
![2](https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/1fc8e52d-35da-408d-8010-c51f6ff6d060)


### b. Source Code
Kode program : <a href="ADC%20dan%20DAC/ADC%20dan%20DAC/ADC_2/ADC_2.ino">klik di sini</a>

### c. Hasil dan Pembahasan
Dalam fungsi setup(), program menginisialisasi komunikasi serial dengan baudrate 115200 dan melakukan konfigurasi modul PWM untuk mengontrol LED. Pengaturan PWM melibatkan menetapkan frekuensi (freq), channel PWM (ledChannel), dan resolusi (resolution). Setelahnya, program menghubungkan saluran PWM ke pin output analog yang terhubung ke LED. Pada fungsi loop(), program membaca nilai analog dari potensiometer menggunakan analogRead(analogInPin) dan menyimpannya dalam variabel sensorValue. Nilai ini kemudian di-mapping dengan fungsi map() dari rentang nilai analog (0 hingga 4095) ke rentang nilai PWM (0 hingga 255). Nilai tersebut digunakan untuk mengatur kecerahan LED melalui fungsi analogWrite(analogOutPin, outputValue).

https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/1828ddeb-e15e-47ad-8057-c33fad4722f9


