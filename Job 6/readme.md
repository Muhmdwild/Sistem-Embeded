# JOBSHEET 6 -  TRANSMISI DATA MENGGUNAKAN MESSAGE QUEUING TELEMETRY TRANSPORT (MQTT) PROTOCOL
## Tujuan
1) Mahasiswa dapat memahami alur kerja, kegunaan dan manfaat protokol MQTT.
2) Mahasiswa dapat memahami dan mengimplementasikan protokol MQTT 
pada sistem IoT untuk monitoring dan kendali.


## Dasar Teori
<p align="justify">MQTT (Message Queuing Telemetry Transport) adalah protokol komunikasi lightweight yang beroperasi di atas stack TCP/IP. Dirancang untuk komunikasi Machine-to-Machine (M2M), bersifat open source, dan memiliki overhead protokol rendah, menghasilkan konsumsi daya yang kecil. MQTT dapat beroperasi pada latency tinggi dan bandwidth rendah.

<p align="justify">Protokol ini bekerja pada lapisan aplikasi dalam standar OSI dan menggunakan model publish/subscribe. Publisher mengirim data, subscriber menerima, dan broker sebagai perantara yang meneruskan pesan dari publisher ke subscriber. Dengan metode publish/subscribe, antara publisher dan subscriber bersifat loosely coupled, tidak tergantung satu sama lain dalam hal tempat, waktu, dan sinkronisasi.

<p align="justify">Keuntungan lainnya termasuk space decoupling, di mana broker memfasilitasi komunikasi tanpa perlu pengetahuan letak atau keberadaan satu sama lain. Time decoupling memungkinkan publisher dan subscriber tidak harus terkoneksi secara bersamaan, memungkinkan subscriber menerima data yang tertunda ketika kembali terhubung. Synchronization decoupling menciptakan kondisi di mana pengaturan event tidak saling mengganggu di sebuah node. MQTT juga mendukung transfer berbagai jenis data, seperti binary, text, XML, dan JSON, serta menerapkan teknik kompresi data untuk efisiensi energi.</p>

**Sub-job** pada jobsheet ini, antara lain:
##### A. Koneksi MTTQ Broker
##### B. Menerima Data JSON Melalui Protokol MQTT
##### C. Mengirim Dummy Data untuk Simulasi I/O Menggunakan Hardware


## Alat dan Bahan
**Alat dan bahan** yang digunakan dalam jobsheet ini, antara lain:
1) ESP32
2) Breadboard
3) Kabel jumper
4) Potensiometer
5) Sensor DHT11
6) LED
7) Multimeter
8) Resistor 1K Ohm


> [!NOTE]  
> *Buka folder-folder subjob untuk melihat laporan percobaan*
