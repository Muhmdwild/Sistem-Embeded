# C. Menggunakan Switch Node

### a. Rangkaian dan Flowchart

Rangkaian pada percobaan ini adalah sebagai berikut

![Screenshot 2023-11-28 211139](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/eaf94b49-91cf-4d8d-bd0a-386ea0a687c1)
<br>
![5C](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/2acea72e-8699-4434-b423-f8447617eda9)



### b. Hasil dan Pembahasan

<p align="justify">Percobaan C membahas penggunaan Switch Node dalam Node-RED. Langkah pertamanya adalah membuat flow dan mengonfigurasi Inject Node. Angka 28 dimasukkan sebagai Payload pada Inject Node 1, sedangkan angka 27 dimasukkan pada Inject Node 2. Konfigurasi Switch Node dilakukan sesuai instruksi pada jobsheet, kemudian program di-deploy dan hasilnya didokumentasikan.
Pada saat menguji alur (flow), data yang disertakan dari sensor gerak atau nilai yang disimulasikan dari Inject Node dialirkan ke node-node yang sesuai berdasarkan kondisi yang telah ditentukan pada Switch Node. Switch Node memungkinkan pengguna untuk memilih rute data yang berbeda berdasarkan kondisi atau nilai tertentu yang diuji dari pesan yang mengalir. Ini memberikan kemampuan untuk mengarahkan atau memproses data secara khusus sesuai kebutuhan. Sebagai contoh, dengan konfigurasi Switch Node, jika pesan memiliki nilai "true", data akan dialirkan ke node berikutnya; sedangkan jika nilai pesan adalah "false", data tersebut akan dialirkan ke node lain atau bisa diabaikan.

![1](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/c58102cf-50b7-40cb-9dee-ddb424832a64)
