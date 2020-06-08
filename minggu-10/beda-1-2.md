# TUGAS

## Perbedaan antara versi 1.x.x dengan versi 2.x.x
---
* InfluxDB versi 1.x.x
Pada InfluxDB 1.x adalah komponen basis data time source seri terbuka TICK Stack (Telegraf, InfluxDB, Chronograf, Kapacitor).

Kelebihan InfluxDB 1.x.x
1. Performa tinggi
InfluxDB adalah penyimpanan data berkinerja tinggi yang ditulis khusus untuk data deret waktu. Hal ini memungkinkan untuk konsumsi throughput tinggi, kompresi, dan permintaan waktu-nyata. InfluxDB sepenuhnya ditulis dalam Go dan mengkompilasi ke dalam biner tunggal tanpa ketergantungan eksternal. Ini memberikan kemampuan menulis dan permintaan dengan antarmuka baris perintah, API HTTP bawaan, satu set perpustakaan klien (misalnya, Go, Java, dan JavaScript) dan plugin untuk format data umum seperti Telegraf, Graphite, Collectd, dan OpenTSDB .

2. Query seperti SQL
InfluxDB bekerja dengan InfluxQL, bahasa query seperti SQL untuk berinteraksi dengan data. Itu telah dibuat dengan penuh kasih sayang untuk merasa akrab bagi mereka yang datang dari SQL lain atau lingkungan seperti SQL sambil juga menyediakan fitur khusus untuk menyimpan dan menganalisis data deret waktu. InfluxQL mendukung ekspresi reguler, ekspresi aritmatika, dan fungsi spesifik seri waktu untuk mempercepat pemrosesan data.

3. Downsampling dan penyimpanan data
InfluxDB dapat menangani jutaan titik data per detik. Bekerja dengan banyak data dalam jangka waktu lama dapat menyebabkan masalah penyimpanan. InfluxDB secara otomatis memadatkan data untuk meminimalkan ruang penyimpanan Anda. Selain itu, Anda dapat dengan mudah menurunkan sampel data; menyimpan data mentah berpresisi tinggi untuk waktu yang terbatas dan menyimpan data yang diringkas dengan presisi lebih rendah untuk waktu yang lebih lama atau hingga akhir waktu. InfluxDB memiliki dua fitur yang membantu untuk mengotomatiskan proses downsampling dan kedaluwarsa data - Kebijakan Permintaan dan Retensi Berkesinambungan. 

* InfluxDB versi 2.x.x (Beta)
Saat ini dalam versi beta, InfluxDB 2.0 menggabungkan semua yang Anda butuhkan dalam platform deret waktu ke dalam satu biner.

InfluxDB 2.0 Beta ini mencakup perangkat tambahan berikut:
1. Pelengkapan otomatis fluks editor - Editor skrip Flux di peramban sekarang memiliki kemampuan untuk melengkapi nama tag sekaligus nilai pengukuran di dalam filter. Juga, mengklik kanan pada editor Flux memunculkan jendela konteks yang memungkinkan Anda untuk dengan cepat memformat skrip Anda dan melompat ke referensi dalam skrip yang lebih besar. Ini tersedia di mana pun Anda mengedit skrip Flux.
2. Influx Command Line Improments - Alat baris perintah influx telah ditingkatkan untuk menghormati variabel lingkungan bersama dengan perintah influx config baru. Ini akan membantu pengguna bermigrasi ke konfigurasi baru.
3. Diupgrade ke Flux v0.66.1 - Flux telah diperbarui ke versi terbaru yang mencakup banyak perbaikan bersama dengan fungsi alignTime baru yang akan menyelaraskan banyak seri ke waktu mulai yang umum. 

Kelebihan dari versi 2.x.x :
1. Waktu yang lebih cepat untuk mengagumkan
InfluxDB sekarang mencakup semua yang dibutuhkan dalam satu biner - visualisasi, dasbor, kueri, tugas, peringatan. Tersedia di bawah lisensi MIT dalam sumber terbuka atau di InfluxDB Cloud sebagai platform deret waktu elastis sebagai penawaran layanan, ia menawarkan evolusi terbesar dari platform sejak penciptaan InfluxDB.

2. Wawasan dan analisis mendalam
InfluxDB sekarang termasuk Flux, bahasa yang kuat yang memungkinkan pengembang untuk melihat dari waktu ke waktu. Flux adalah bahasa pemrosesan data generasi keempat yang dioptimalkan untuk analisis deret waktu.

3. Dukungan perpustakaan klien
InfluxDB 2.0 sekarang termasuk perpustakaan klien yang kuat dalam bahasa populer seperti Go, Java, PHP dan Python. Ini memungkinkan adopsi InfluxDB lebih cepat di seluruh organisasi pengembangan dan waktu lebih cepat untuk memasukkan aplikasi ke dalam produksi. 