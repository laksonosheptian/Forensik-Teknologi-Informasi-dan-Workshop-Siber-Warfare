Analisis Cyber Warfare
<div align="justify">
Repository ini berisi analisis komprehensif tentang cyber warfare, perbedaan dengan cyber crime, studi kasus Stuxnet, dan dampaknya pada pertahanan maritim Indonesia.

Bagian A: Soal Latihan Pilihan Ganda & Esai Singkat
I. Soal Pilihan Ganda
1. Elemen fundamental yang membedakan Cyber Warfare:

Jawaban: b. Aktornya adalah negara-bangsa (atau proksi-nya)

Aktor negara-bangsa merupakan pembeda utama karena melibatkan tujuan geopolitik dan militer

2. Pengakuan Cyberspace sebagai domain peperangan kelima:

Jawaban: c. Aktivitas di ruang siber dapat dianggap setara dengan aksi militer di domain fisik

Menempatkan operasi siber setara dengan operasi militer konvensional

3. Serangan yang menargetkan persepsi manusia:

Jawaban: c. Cognitive Layer

Berfokus pada persepsi, keyakinan, dan proses pengambilan keputusan manusia

4. Titik balik serangan siber pertama yang melumpuhkan infrastruktur digital:

Jawaban: c. Serangan Siber terhadap Estonia (2007)

Serangan DDoS masif yang melumpuhkan perbankan, media, dan layanan pemerintah

5. Tindakan proaktif di luar jaringan sendiri:

Jawaban: b. Operasi Siber Ofensif (OCO)

Melibatkan proyeksi kekuatan ofensif untuk mencapai tujuan militer

II. Jawaban Esai Singkat
6. Karakteristik unik Cyberspace:

Jawaban: Dua karakteristik unik cyberspace adalah batas geografis yang kabur (serangan dapat dilancarkan dari mana saja ke mana saja) dan tingkat anonimitas yang tinggi. Hal ini mengubah sifat konflik karena membuat identifikasi pelaku menjadi sulit, mempercepat eskalasi, dan mengaburkan garis antara keadaan damai dan perang.

7. Perbedaan fundamental Cyber Warfare vs Cyber Crime:

Jawaban: Perbedaan fundamentalnya terletak pada motivasinya: Cyber Warfare dimotivasi oleh tujuan geopolitik atau militer suatu negara, sedangkan Cyber Crime dimotivasi oleh keuntungan finansial atau pribadi.

Contoh: Cyber Warfare: Serangan Stuxnet untuk mengganggu program nuklir Iran. Cyber Crime: Ransomware WannaCry yang meminta tebusan uang.

8. Pentingnya insiden Morris Worm:

Jawaban: Morris Worm dianggap penting karena demonstrasi pertama bagaimana sebuah program dapat menyebar dengan cepat dan melumpuhkan sebagian besar internet awal, yang membuktikan kerentanan fundamental dalam jaringan terhubung dan memicu lahirnya bidang keamanan siber yang terorganisir.

9. Mission Assurance dalam Operasi Siber:

Jawaban: Mission Assurance adalah upaya untuk memastikan bahwa misi atau operasi kritis dapat terus berjalan meskipun terjadi serangan atau gangguan siber. Ini menjadi tujuan utama DCO karena fokusnya bergeser dari sekadar "melindungi jaringan" menjadi "menjamin kelangsungan fungsi operasional" yang vital.

10. Signifikansi serangan Stuxnet:

Jawaban: Stuxnet dianggap "melintasi Rubicon" karena ini adalah senjata siber pertama yang secara fisik merusak dan menghancurkan infrastruktur kritis di dunia nyata (pusat pemrosesan nuklir Iran), sehingga membuktikan bahwa serangan digital dapat memiliki konsekuensi fisik yang berbahaya seperti senjata konvensional.

</div>
Bagian B: Tugas Analisis dan Studi Kasus
Tugas 1: Analisis Komparatif – Cyber Warfare vs. Cyber Crime
<div align="justify">
Deskripsi Insiden:

Insiden ALFA: Kelompok meretas sistem perbankan nasional dan mencuri dana miliaran rupiah menggunakan ransomware dari pasar gelap, beroperasi dari Eropa Timur.

Insiden BETA: Fasilitas pengolahan air milik negara mengalami malfungsi sistem kontrol industri, ditemukan malware kustom sangat canggih yang hanya menargetkan PLC spesifik, tanpa permintaan tebusan, terjadi saat ketegangan diplomatik.

1. Analisis Komparatif Berdasarkan Kriteria:

Kriteria	Insiden ALFA	Insiden BETA
Aktor	Kelompok kriminal (Eropa Timur)	Negara bangsa (state-sponsored)
Motivasi	Keuntungan finansial	Tujuan geopolitik/strategis
Target	Sistem perbankan	Infrastruktur kritis nasional
Metodologi	Ransomware komersial	Malware kustom canggih
Tujuan Akhir	Pencurian dana	Destabilisasi nasional
2. Klasifikasi dan Justifikasi:

Insiden ALFA → Cyber Crime

Motif ekonomi murni (pencurian dana)

Menggunakan tools komersial yang tersedia umum

Target sektor finansial untuk keuntungan pribadi

Tidak ada indikasi tujuan politik atau militer

Insiden BETA → Cyber Warfare

Target infrastruktur kritis nasional (strategis)

Malware kustom yang sangat spesifik menunjukkan sumber daya negara

Tidak ada permintaan tebusan - motif non-ekonomi

Terjadi dalam konteks ketegangan diplomatik (motif geopolitik)

3. Diagram Visualisasi Perbedaan Fundamental:

<div align="center"> <img src="images/gbr1.png" width="600"> </div>
Kesimpulan Analisis:
Insiden ALFA menunjukkan karakteristik kriminal siber klasik dengan motif ekonomi, sementara Insiden BETA mengindikasikan operasi perang siber state-sponsored yang bertujuan untuk mengganggu stabilitas nasional melalui target infrastruktur kritis. Perbedaan fundamental terletak pada aktor, motivasi, dan dampak strategis dari masing-masing insiden.

</div>
Tugas 2: Studi Kasus Mendalam – Anatomi Serangan Stuxnet
<div align="justify">
1. Fase Utama Serangan Stuxnet:

Fase 1: Infiltrasi Awal & Menjembatani Air Gap

Stuxnet menyebar melalui removable drive (USB) yang terinfeksi

Memanfaatkan zero-day vulnerability dalam Windows untuk eksekusi otomatis

Menjembatani air gap dengan menginfeksi workstation yang terhubung ke jaringan internal PLC

Fase 2: Eskalasi Hak Akses & Persebaran Lateral

Mengeksploitasi zero-day vulnerability kedua untuk eskalasi privilege

Menyebar melalui jaringan internal menggunakan kredensial yang dicuri

Mencari sistem SCADA dan PLC target secara spesifik

Fase 3: Identifikasi & Verifikasi Target

Memindai dan mengidentifikasi PLC Siemens S7-300/400 tertentu

Memverifikasi bahwa PLC tersebut mengontrol sentrifugal nuklir IR-1

Hanya mengaktifkan payload pada sistem yang memenuhi kriteria target

Fase 4: Sabotase Fisik & Penipuan

Sabotase Fisik: Memodifikasi kode PLC untuk mengubah kecepatan sentrifugal

Penipuan/Penyembunyian: Mengirim data normal palsu ke ruang kontrol

Fase 5: Pemeliharaan Akses & Evasi

Menginstal rootkit untuk menyembunyikan keberadaan malware

Mempertahankan akses untuk potensi serangan lanjutan

Membersihkan jejak untuk menghindari deteksi

2. Mekanisme Kunci Efektivitas Stuxnet:

Mekanisme Sabotase Fisik:
Stuxnet memanipulasi kecepatan sentrifugal dengan pola akselerasi dan deselerasi ekstrem yang menyebabkan keausan mekanis cepat dan kerusakan fisik permanen.

Mekanisme Penipuan/Penyembunyian:
Mengimplementasikan man-in-the-middle attack dengan merekam data operasi normal dan memutar ulang data tersebut ke operator.

3. Diagram Alur Serangan Stuxnet:

<div align="center"> <img src="images/gbr2.png" width="600"> </div>
Poin Kritis Keberhasilan Stuxnet:

Multi-stage infiltration yang efektif menembus isolasi fisik

Target specificity yang hanya mengaktifkan diri pada lingkungan tertentu

Dual mechanism yang menggabungkan sabotase fisik dengan penipuan monitoring

Persistence yang mempertahankan akses sambil menghindari deteksi

</div>
Tugas 3: Analisis Kontekstual – Dampak Cyber Warfare pada Pertahanan Maritim Indonesia
<div align="justify">
1. Sistem/Aset Digital Paling Rentan dan Kritis:

a. AIS (Automatic Identification System)

Fungsi: Sistem pelacakan dan identifikasi kapal otomatis

Kerentanan: Data tidak terenkripsi, mudah dimanipulasi

Kritisitas: Tinggi - menjadi dasar awareness maritim

b. ECDIS (Electronic Chart Display and Information System)

Fungsi: Sistem navigasi digital dan pemetaan elektronik

Kerentanan: Kerentanan pada update charts dan integrasi GPS

Kritisitas: Vital - navigasi keselamatan pelayaran

c. Port Management System (Terminal Operating System)

Fungsi: Mengelola operasional pelabuhan, crane, dan logistik

Kerentanan: Terhubung ke jaringan administrasi pelabuhan

Kritisitas: Strategis - mempengaruhi rantai pasok nasional

2. Skenario Serangan Siber Realistis:

Skenario 1: AIS Spoofing Attack

Vektor Serangan: Injeksi data AIS palsu melalui transmitter ilegal

Konsekuensi: Kapal komersil dialihkan ke perairan berbahaya, tabrakan kapal, gangguan logistik nasional, kerugian ekonomi besar

Skenario 2: ECDIS/GPS Spoofing

Vektor Serangan: Manipulasi sinyal GPS dan corrupt data chart ECDIS

Konsekuensi: KRI dan kapal komersil tersesat, kandas di perairan dangkal, gangguan operasi patroli maritim, ancaman kedaulatan

Skenario 3: Port System Ransomware

Vektor Serangan: Spear-phishing ke admin pelabuhan + ransomware pada TOS

Konsekuensi: Pelabuhan utama lumpuh, rantai pasok terputus, kerugian ekonomi $100-200 juta/hari

3. Diagram Pemetaan Ancaman Siber Maritim:

<div align="center"> <img src="images/gbr3.png" width="600"> </div>
Analisis Dampak Strategis:
Ancaman siber pada domain maritim Indonesia berpotensi menyebabkan:

Krisis kedaulatan melalui manipulasi awareness maritim

Kerugian ekonomi masif akibat gangguan rantai pasok

Krisis energi jika pelabuhan minyak lumpuh

Dampak geopolitik terhadap posisi Indonesia sebagai poros maritim dunia

Rekomendasi:

Implementasi cybersecurity framework khusus sektor maritim

Enkripsi dan autentikasi data AIS/ECDIS

Air-gapping sistem kritis pelabuhan

Latihan gabungan TNI AL-Badan Siber Nasional menghadapi serangan siber maritim

</div>
<div align="center"> **Dibuat oleh: Sertu Ttu Laksono Sheptian Yoga P** </div>
