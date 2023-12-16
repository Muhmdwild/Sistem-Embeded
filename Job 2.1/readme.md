# JOBSHEET 2.1 - JARINGAN SENSOR NIRKABEL MENGGUNAKAN ESP-NOW
## Tujuan
1) Mahasiswa dapat memahami konsep topologi jaringan sensor nirkabel berbasis ESPNOW.
2) Mahasiswa dapat melakukan konfigurasi berbagai topologi ESP-NOW.
3) Mahasiswa dapat menganalisis dan menentukan topologi ESP-NOW,sesuai dengan
studi kasus proyek.


## Dasar Teori
<p align="justify">ESP-NOW adalah protokol yang dikembangkan oleh Espressif, yang memungkinkan banyak perangkat untuk berkomunikasi satu sama lain tanpa menggunakan Wi-Fi. Protokol ini mirip dengan konektivitas nirkabel 2.4GHz berdaya rendah. Pendifinisian alamat (MAC Address) pada masing-masing ESP32 diperlukan pada awal konfigurasi. Setelah konfigurasi alamat selesai dilakukan, jaringan peer-to-peer akan terbentuk dan perangkat tidak perlu melakukan handshaking kembali ketika akan berkomunikasi. Hal ini memunjukkan bahwa setelah perangkat ESP32 saling terpasang satu sama lain, koneksi akan tetap ada. Dengan kata lain, 
jika tiba-tiba salah satu ESP32 kehilangan daya atau diatur ulang, ketika restart, secara otomatis akan terhubung ke pasangan ESP32 yang telah terdefinisi alamatnya untuk melanjutkan komunikasi.
  
ESP-NOW mempunyai fitur sebagai berikut.          
a. Komunikasi unicast yang terenkripsi maupun tidak terenkripsi.         
b. Perpaduan komunikasi data yang terenkripsi maupun yang tidak terenkripsi pada perangkat yang berada pada topologi peer-to-peer.        
c. Payload (ukuran) data yang dapat dikirm mencapai 250 byte.              
d. Terdapat fungsi callback yang dapat menginformasikan data berhasil terkirim maupun gagal dikirim.

Selain itu, ESP-NOW mempunyai batasan sebagai berikut.            
a. Jumlah maksimal perangkat yang dapat berkomunikasi dalam mode station dengan data terenkripsi adalah 10 unit (6 dalam mode SoftAP atau SoftAP+Station).        
b. Untuk komunikasi tidak terenkripsi, jumlah maksimal perangkat adalah 20 unit, termasuk dengan yang terenkripsi. 

ESP-NOW mempunyai 2 tipe jaringan, yaitu One-Way Communication dan Two-Way Communication. One-Way Communication terbagi menjadi Point-to-Point, One-to-Many Communication dan Many-to-One Communication. Sementara Two-Way Communication terbagi menjadi Point-to-Point dan Mesh Communication</p>


**Sub-job** pada jobsheet ini, antara lain:
1. Memperoleh MAC Address ESP32 Receiver
2. ESP-NOW One-Way Point-to-Point Communication
3. One-Way, One-to-Many Communication 
4. One-Way, Many-to-One Communication
5. Two-Way Communication

## Alat dan Bahan
**Alat dan bahan** yang digunakan dalam jobsheet ini, antara lain:
1) ESP32
2) Breadboard
3) Kabel jumper
4) Resistor 10K Ohm


> [!NOTE]  
> *Buka folder-folder subjob untuk melihat laporan percobaan*
