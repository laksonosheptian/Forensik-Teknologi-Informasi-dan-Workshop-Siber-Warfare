<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laporan Analisis Cyber Warfare</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            background: #f8f9fa;
        }

        .container {
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0,0,0,0.1);
        }

        header {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 20px;
            border-bottom: 3px solid #2c3e50;
        }

        h1 {
            color: #2c3e50;
            margin-bottom: 10px;
            font-size: 2.2em;
        }

        .subtitle {
            color: #7f8c8d;
            font-size: 1.1em;
            margin-bottom: 10px;
        }

        .author {
            color: #34495e;
            font-style: italic;
            font-weight: bold;
        }

        .section {
            margin-bottom: 50px;
        }

        h2 {
            color: #2c3e50;
            margin-bottom: 25px;
            padding-bottom: 10px;
            border-bottom: 2px solid #3498db;
            font-size: 1.8em;
        }

        h3 {
            color: #34495e;
            margin: 30px 0 20px 0;
            font-size: 1.4em;
        }

        h4 {
            color: #2c3e50;
            margin: 20px 0 15px 0;
            font-size: 1.2em;
        }

        .question {
            margin-bottom: 30px;
            padding: 20px;
            background: #f8f9fa;
            border-left: 5px solid #3498db;
            border-radius: 5px;
        }

        .question-text {
            font-weight: bold;
            margin-bottom: 15px;
            color: #2c3e50;
            font-size: 1.1em;
        }

        .answer {
            background: #e8f4f8;
            padding: 15px;
            border-radius: 5px;
            margin-top: 10px;
            border: 1px solid #bdc3c7;
        }

        .multiple-choice {
            margin: 15px 0;
        }

        .choice {
            padding: 10px;
            margin: 8px 0;
            background: white;
            border-radius: 4px;
            border-left: 4px solid #bdc3c7;
        }

        .choice.correct {
            background: #d4edda;
            border-left-color: #28a745;
            font-weight: bold;
        }

        .choice.incorrect {
            background: #f8d7da;
            border-left-color: #dc3545;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 25px 0;
            background: white;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        th, td {
            padding: 15px;
            text-align: left;
            border: 1px solid #ddd;
        }

        th {
            background: #34495e;
            color: white;
            font-weight: bold;
        }

        tr:nth-child(even) {
            background: #f8f9fa;
        }

        .scenario {
            background: #fff3cd;
            padding: 20px;
            margin: 20px 0;
            border-left: 5px solid #ffc107;
            border-radius: 5px;
        }

        .classification {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 25px;
            margin: 25px 0;
        }

        .cyber-crime, .cyber-warfare {
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        .cyber-crime {
            background: #f8d7da;
            border-left: 5px solid #dc3545;
        }

        .cyber-warfare {
            background: #d1ecf1;
            border-left: 5px solid #17a2b8;
        }

        ul {
            padding-left: 25px;
            margin: 15px 0;
        }

        li {
            margin: 8px 0;
            line-height: 1.5;
        }

        .diagram-placeholder {
            background: #f8f9fa;
            padding: 30px;
            margin: 25px 0;
            border-radius: 8px;
            border: 2px dashed #bdc3c7;
            text-align: center;
        }

        .conclusion {
            background: #d4edda;
            padding: 25px;
            border-radius: 8px;
            margin: 25px 0;
            border-left: 5px solid #28a745;
        }

        .phase-box {
            background: #e8f4f8;
            padding: 20px;
            margin: 15px 0;
            border-radius: 6px;
            border-left: 4px solid #3498db;
        }

        .mechanism-box {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin: 20px 0;
        }

        .mechanism {
            padding: 20px;
            border-radius: 6px;
            background: white;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }

        .mechanism-sabotage {
            border-left: 4px solid #dc3545;
        }

        .mechanism-deception {
            border-left: 4px solid #17a2b8;
        }

        .asset-box {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .asset {
            padding: 20px;
            border-radius: 6px;
            background: white;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            border-left: 4px solid #3498db;
        }

        .highlight {
            background: #fff3cd;
            padding: 2px 6px;
            border-radius: 3px;
            font-weight: bold;
        }

        footer {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            color: #7f8c8d;
            border-top: 1px solid #bdc3c7;
        }

        @media (max-width: 768px) {
            .classification, .mechanism-box {
                grid-template-columns: 1fr;
            }
            
            .container {
                padding: 20px;
            }
            
            .asset-box {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>Laporan Analisis Cyber Warfare</h1>
            <p class="subtitle">Minggu 1-2: Soal Latihan & Tugas Analisis</p>
            <p class="author">Dibuat oleh: Sertu Ttu Laksono Sheptian Yoga P</p>
        </header>

        <!-- Bagian A: Soal Latihan -->
        <div class="section">
            <h2>Bagian A: Soal Latihan Pilihan Ganda & Esai Singkat</h2>
            
            <!-- Soal 1 -->
            <div class="question">
                <div class="question-text">
                    1. Menurut definisi yang disajikan dalam materi, elemen paling fundamental yang membedakan Cyber Warfare dari bentuk serangan siber lainnya adalah...
                </div>
                <div class="multiple-choice">
                    <div class="choice incorrect">a. Penggunaan malware yang canggih</div>
                    <div class="choice correct">b. Aktornya adalah negara-bangsa (atau proksi-nya)</div>
                    <div class="choice incorrect">c. Menargetkan infrastruktur digital</div>
                    <div class="choice incorrect">d. Menyebabkan kerugian finansial yang besar</div>
                </div>
                <div class="answer">
                    <strong>Jawaban: b. Aktornya adalah negara-bangsa (atau proksi-nya)</strong>
                </div>
            </div>

            <!-- Soal 2 -->
            <div class="question">
                <div class="question-text">
                    2. Pengakuan Cyberspace sebagai domain peperangan kelima berarti bahwa...
                </div>
                <div class="multiple-choice">
                    <div class="choice incorrect">a. Perang hanya akan terjadi di dunia maya</div>
                    <div class="choice incorrect">b. Semua negara wajib memiliki angkatan siber</div>
                    <div class="choice correct">c. Aktivitas di ruang siber dapat dianggap setara dengan aksi militer di domain fisik</div>
                    <div class="choice incorrect">d. Hukum perang tidak berlaku di internet</div>
                </div>
                <div class="answer">
                    <strong>Jawaban: c. Aktivitas di ruang siber dapat dianggap setara dengan aksi militer di domain fisik</strong>
                </div>
            </div>

            <!-- Soal 3 -->
            <div class="question">
                <div class="question-text">
                    3. Serangan yang menargetkan persepsi manusia, seperti kampanye disinformasi dan operasi psikologis (PSYOP), terjadi pada lapisan Cyberspace yang mana?
                </div>
                <div class="answer">
                    <strong>Jawaban: c. Cognitive Layer</strong>
                </div>
            </div>

            <!-- Soal 4 -->
            <div class="question">
                <div class="question-text">
                    4. Peristiwa historis yang dianggap sebagai "titik balik" di mana serangan siber pertama kali berhasil melumpuhkan infrastruktur digital sebuah negara secara masif adalah...
                </div>
                <div class="answer">
                    <strong>Jawaban: c. Serangan Siber terhadap Estonia (2007)</strong>
                </div>
            </div>

            <!-- Soal 5 -->
            <div class="question">
                <div class="question-text">
                    5. Tindakan proaktif yang diambil di luar jaringan sendiri untuk memproyeksikan kekuatan dan mencapai tujuan militer, seperti melakukan spionase atau melancarkan serangan, diklasifikasikan sebagai...
                </div>
                <div class="answer">
                    <strong>Jawaban: b. Operasi Siber Ofensif (OCO)</strong>
                </div>
            </div>

            <!-- Esai Singkat -->
            <h3>Jawaban Esai Singkat</h3>
            
            <!-- Esai 6 -->
            <div class="question">
                <div class="question-text">
                    6. Jelaskan dua karakteristik unik dari Cyberspace sebagai domain peperangan dan mengapa karakteristik tersebut mengubah sifat konflik modern!
                </div>
                <div class="answer">
                    Dua karakteristik unik cyberspace adalah <span class="highlight">batas geografis yang kabur</span> (serangan dapat dilancarkan dari mana saja ke mana saja) dan <span class="highlight">tingkat anonimitas yang tinggi</span>. Hal ini mengubah sifat konflik karena membuat identifikasi pelaku menjadi sulit, mempercepat eskalasi, dan mengaburkan garis antara keadaan damai dan perang.
                </div>
            </div>

            <!-- Esai 7 -->
            <div class="question">
                <div class="question-text">
                    7. Apa perbedaan fundamental antara motivasi di balik Cyber Warfare dan Cyber Crime? Berikan satu contoh untuk masing-masing.
                </div>
                <div class="answer">
                    Perbedaan fundamentalnya terletak pada motivasinya: Cyber Warfare dimotivasi oleh <span class="highlight">tujuan geopolitik atau militer</span> suatu negara, sedangkan Cyber Crime dimotivasi oleh <span class="highlight">keuntungan finansial atau pribadi</span>.<br><br>
                    <strong>Contoh:</strong><br>
                    • <span class="highlight">Cyber Warfare</span>: Serangan Stuxnet untuk mengganggu program nuklir Iran<br>
                    • <span class="highlight">Cyber Crime</span>: Ransomware WannaCry yang meminta tebusan uang
                </div>
            </div>

            <!-- Esai 8 -->
            <div class="question">
                <div class="question-text">
                    8. Mengapa insiden Morris Worm pada tahun 1988 dianggap sebagai peristiwa penting dalam sejarah keamanan siber, meskipun tidak dirancang untuk tujuan jahat?
                </div>
                <div class="answer">
                    Morris Worm dianggap penting karena demonstrasi pertama bagaimana sebuah program dapat menyebar dengan cepat dan melumpuhkan sebagian besar internet awal, yang membuktikan kerentanan fundamental dalam jaringan terhubung dan memicu lahirnya bidang keamanan siber yang terorganisir.
                </div>
            </div>

            <!-- Esai 9 -->
            <div class="question">
                <div class="question-text">
                    9. Dalam konteks Operasi Siber Militer, apa yang dimaksud dengan Mission Assurance dan mengapa hal ini menjadi tujuan utama dari Operasi Siber Defensif (DCO)?
                </div>
                <div class="answer">
                    Mission Assurance adalah upaya untuk memastikan bahwa misi atau operasi kritis dapat terus berjalan meskipun terjadi serangan atau gangguan siber. Ini menjadi tujuan utama DCO karena fokusnya bergeser dari sekadar "melindungi jaringan" menjadi "menjamin kelangsungan fungsi operasional" yang vital.
                </div>
            </div>

            <!-- Esai 10 -->
            <div class="question">
                <div class="question-text">
                    10. Jelaskan mengapa serangan Stuxnet dianggap sebagai momen "melintasi Rubicon" dalam sejarah cyber warfare!
                </div>
                <div class="answer">
                    Stuxnet dianggap "melintasi Rubicon" karena ini adalah senjata siber pertama yang secara fisik merusak dan menghancurkan infrastruktur kritis di dunia nyata (pusat pemrosesan nuklir Iran), sehingga membuktikan bahwa serangan digital dapat memiliki konsekuensi fisik yang berbahaya seperti senjata konvensional.
                </div>
            </div>
        </div>

        <!-- Tugas 1: Analisis Komparatif -->
        <div class="section">
            <h2>Tugas 1: Analisis Komparatif – Cyber Warfare vs. Cyber Crime</h2>
            
            <div class="scenario">
                <h4>Insiden ALFA</h4>
                <p>Sebuah kelompok meretas sistem perbankan nasional dan berhasil mencuri dana nasabah senilai miliaran rupiah. Jejak digital menunjukkan mereka menggunakan ransomware yang dibeli dari pasar gelap dan beroperasi dari Eropa Timur.</p>
            </div>

            <div class="scenario">
                <h4>Insiden BETA</h4>
                <p>Sebuah fasilitas pengolahan air milik negara tiba-tiba mengalami malfungsi pada sistem kontrol industrinya (PLC), menyebabkan tekanan air yang tidak stabil. Analisis forensik menemukan malware kustom yang sangat canggih dan tidak pernah terlihat sebelumnya, yang tampaknya hanya menargetkan tipe PLC spesifik tersebut. Tidak ada permintaan tebusan. Insiden ini terjadi di tengah meningkatnya ketegangan diplomatik dengan negara tetangga.</p>
            </div>

            <h3>1. Analisis Komparatif Berdasarkan Kriteria</h3>
            
            <table>
                <thead>
                    <tr>
                        <th>Kriteria</th>
                        <th>Insiden ALFA</th>
                        <th>Insiden BETA</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><strong>Aktor</strong></td>
                        <td>Kelompok kriminal (kemungkinan dari Eropa Timur)</td>
                        <td>Negara bangsa (state-sponsored) dengan kemampuan tinggi</td>
                    </tr>
                    <tr>
                        <td><strong>Motivasi</strong></td>
                        <td>Keuntungan finansial (ekonomis)</td>
                        <td>Tujuan geopolitik/strategis</td>
                    </tr>
                    <tr>
                        <td><strong>Target</strong></td>
                        <td>Sistem perbankan (sektor finansial)</td>
                        <td>Infrastruktur kritis nasional (sistem pengolahan air)</td>
                    </tr>
                    <tr>
                        <td><strong>Metodologi</strong></td>
                        <td>Menggunakan ransomware komersial yang tersedia di pasar gelap</td>
                        <td>Malware kustom yang sangat canggih dan spesifik</td>
                    </tr>
                    <tr>
                        <td><strong>Tujuan Akhir</strong></td>
                        <td>Pencurian dana (kerugian ekonomi)</td>
                        <td>Gangguan operasional infrastruktur kritis (potensi destabilisasi)</td>
                    </tr>
                </tbody>
            </table>

            <h3>2. Klasifikasi dan Justifikasi</h3>
            
            <div class="classification">
                <div class="cyber-crime">
                    <h4>Insiden ALFA → Cyber Crime</h4>
                    <p><strong>Justifikasi:</strong></p>
                    <ul>
                        <li>Motif ekonomi murni (pencurian dana)</li>
                        <li>Menggunakan tools komersial yang tersedia umum</li>
                        <li>Target sektor finansial untuk keuntungan pribadi</li>
                        <li>Tidak ada indikasi tujuan politik atau militer</li>
                    </ul>
                </div>

                <div class="cyber-warfare">
                    <h4>Insiden BETA → Cyber Warfare</h4>
                    <p><strong>Justifikasi:</strong></p>
                    <ul>
                        <li>Target infrastruktur kritis nasional (strategis)</li>
                        <li>Malware kustom yang sangat spesifik menunjukkan sumber daya negara</li>
                        <li>Tidak ada permintaan tebusan - motif non-ekonomi</li>
                        <li>Terjadi dalam konteks ketegangan diplomatik (motif geopolitik)</li>
                    </ul>
                </div>
            </div>

            <h3>3. Diagram Visualisasi Perbedaan Fundamental</h3>
            
            <div class="diagram-placeholder">
                <h4>Diagram Perbandingan Insiden ALFA vs BETA</h4>
                <p><em>File gambar: gbr1.png</em></p>
            </div>

            <div class="conclusion">
                <h4>Kesimpulan Analisis</h4>
                <p>Insiden ALFA menunjukkan karakteristik <span class="highlight">kriminal siber klasik</span> dengan motif ekonomi, sementara Insiden BETA mengindikasikan operasi <span class="highlight">perang siber state-sponsored</span> yang bertujuan untuk mengganggu stabilitas nasional melalui target infrastruktur kritis. Perbedaan fundamental terletak pada <span class="highlight">aktor, motivasi, dan dampak strategis</span> dari masing-masing insiden.</p>
            </div>
        </div>

        <!-- Tugas 2: Anatomi Serangan Stuxnet -->
        <div class="section">
            <h2>Tugas 2: Studi Kasus – Anatomi Serangan Stuxnet</h2>
            
            <h3>1. Fase Utama Serangan Stuxnet</h3>
            
            <div class="phase-box">
                <h4>Fase 1: Infiltrasi Awal & Menjembatani Air Gap</h4>
                <ul>
                    <li>Stuxnet menyebar melalui removable drive (USB) yang terinfeksi</li>
                    <li>Memanfaatkan zero-day vulnerability dalam Windows untuk eksekusi otomatis</li>
                    <li>Menjembatani air gap dengan menginfeksi workstation yang tidak terhubung internet tetapi terhubung ke jaringan internal PLC</li>
                </ul>
            </div>
            
            <div class="phase-box">
                <h4>Fase 2: Eskalasi Hak Akses & Persebaran Lateral</h4>
                <ul>
                    <li>Mengeksploitasi zero-day vulnerability kedua untuk eskalasi privilege</li>
                    <li>Menyebar melalui jaringan internal menggunakan kredensial yang dicuri</li>
                    <li>Mencari sistem SCADA dan PLC target secara spesifik</li>
                </ul>
            </div>
            
            <div class="phase-box">
                <h4>Fase 3: Identifikasi & Verifikasi Target</h4>
                <ul>
                    <li>Memindai dan mengidentifikasi PLC Siemens S7-300/400 tertentu</li>
                    <li>Memverifikasi bahwa PLC tersebut mengontrol sentrifugal nuklir IR-1</li>
                    <li>Hanya mengaktifkan payload pada sistem yang memenuhi kriteria target</li>
                </ul>
            </div>
            
            <div class="phase-box">
                <h4>Fase 4: Sabotase Fisik & Penipuan</h4>
                <ul>
                    <li><strong>Sabotase Fisik:</strong> Memodifikasi kode PLC untuk mengubah kecepatan sentrifugal (mempercepat dan memperlambat di luar batas aman)</li>
                    <li><strong>Penipuan/Penyembunyian:</strong> Mengirim data normal palsu ke ruang kontrol untuk menyembunyikan kerusakan yang terjadi</li>
                </ul>
            </div>
            
            <div class="phase-box">
                <h4>Fase 5: Pemeliharaan Akses & Evasi</h4>
                <ul>
                    <li>Menginstal rootkit untuk menyembunyikan keberadaan malware</li>
                    <li>Mempertahankan akses untuk potensi serangan lanjutan</li>
                    <li>Membersihkan jejak untuk menghindari deteksi</li>
                </ul>
            </div>

            <h3>2. Mekanisme Kunci Efektivitas Stuxnet</h3>
            
            <div class="mechanism-box">
                <div class="mechanism mechanism-sabotage">
                    <h4>Mekanisme Sabotase Fisik</h4>
                    <p>Stuxnet secara spesifik memanipulasi kecepatan sentrifugal dengan pola akselerasi dan deselerasi ekstrem yang menyebabkan keausan mekanis cepat dan kerusakan fisik permanen pada peralatan nuklir, sambil tetap beroperasi dalam parameter yang tampak normal.</p>
                </div>
                
                <div class="mechanism mechanism-deception">
                    <h4>Mekanisme Penipuan/Penyembunyian</h4>
                    <p>Malware ini mengimplementasikan man-in-the-middle attack terhadap sistem monitoring dengan merekam data operasi normal dan memutar ulang data tersebut ke operator, sehingga kerusakan fisik yang terjadi tidak terdeteksi hingga benar-benar parah.</p>
                </div>
            </div>

            <h3>3. Diagram Alur Serangan Stuxnet</h3>
            
            <div class="diagram-placeholder">
                <h4>Diagram Rantai Serangan (Kill Chain) Stuxnet</h4>
                <p><em>File gambar: gbr2.png</em></p>
            </div>

            <div class="conclusion">
                <h4>Poin Kritis Keberhasilan Stuxnet</h4>
                <ul>
                    <li><strong>Multi-stage infiltration</strong> yang efektif menembus isolasi fisik</li>
                    <li><strong>Target specificity</strong> yang hanya mengaktifkan diri pada lingkungan tertentu</li>
                    <li><strong>Dual mechanism</strong> yang menggabungkan sabotase fisik dengan penipuan monitoring</li>
                    <li><strong>Persistence</strong> yang mempertahankan akses sambil menghindari deteksi</li>
                </ul>
            </div>
        </div>

        <!-- Tugas 3: Dampak Cyber Warfare Maritim -->
        <div class="section">
            <h2>Tugas 3: Dampak Cyber Warfare pada Pertahanan Maritim Indonesia</h2>
            
            <h3>1. Sistem/Aset Rentan dan Kritis</h3>
            
            <div class="asset-box">
                <div class="asset">
                    <h4>AIS (Automatic Identification System)</h4>
                    <p><strong>Fungsi:</strong> Sistem pelacakan dan identifikasi kapal otomatis</p>
                    <p><strong>Kerentanan:</strong> Data tidak terenkripsi, mudah dimanipulasi</p>
                    <p><strong>Kritisitas:</strong> Tinggi - menjadi dasar awareness maritim</p>
                </div>
                
                <div class="asset">
                    <h4>ECDIS (Electronic Chart Display and Information System)</h4>
                    <p><strong>Fungsi:</strong> Sistem navigasi digital dan pemetaan elektronik</p>
                    <p><strong>Kerentanan:</strong> Kerentanan pada update charts dan integrasi GPS</p>
                    <p><strong>Kritisitas:</strong> Vital - navigasi keselamatan pelayaran</p>
                </div>
                
                <div class="asset">
                    <h4>Port Management System (Terminal Operating System)</h4>
                    <p><strong>Fungsi:</strong> Mengelola operasional pelabuhan, crane, dan logistik</p>
                    <p><strong>Kerentanan:</strong> Terhubung ke jaringan administrasi pelabuhan</p>
                    <p><strong>Kritisitas:</strong> Strategis - mempengaruhi rantai pasok nasional</p>
                </div>
            </div>

            <h3>2. Skenario Serangan Siber Realistis</h3>
            
            <div class="scenario">
                <h4>Skenario 1: AIS Spoofing Attack</h4>
                <p><strong>Vektor Serangan:</strong> Injeksi data AIS palsu melalui transmitter ilegal</p>
                <p><strong>Konsekuensi:</strong> Kapal komersil dialihkan ke perairan berbahaya, tabrakan kapal, gangguan logistik nasional, kerugian ekonomi besar</p>
            </div>
            
            <div class="scenario">
                <h4>Skenario 2: ECDIS/GPS Spoofing</h4>
                <p><strong>Vektor Serangan:</strong> Manipulasi sinyal GPS dan corrupt data chart ECDIS</p>
                <p><strong>Konsekuensi:</strong> KRI dan kapal komersil tersesat, kandas di perairan dangkal, gangguan operasi patroli maritim, ancaman kedaulatan</p>
            </div>
            
            <div class="scenario">
                <h4>Skenario 3: Port System Ransomware</h4>
                <p><strong>Vektor Serangan:</strong> Spear-phishing ke admin pelabuhan + ransomware pada TOS</p>
                <p><strong>Konsekuensi:</strong> Pelabuhan utama lumpuh (Tanjung Priok, Surabaya), rantai pasok terputus, kerugian ekonomi $100-200 juta/hari</p>
            </div>

            <h3>3. Diagram Pemetaan Ancaman</h3>
            
            <div class="diagram-placeholder">
                <h4>Diagram Ancaman Siber pada Domain Maritim Indonesia</h4>
                <p>[Diagram akan ditambahkan sebagai file gambar terpisah]</p>
                <p><em>File gambar: gbr3.png</em></p>
            </div>

            <div class="conclusion">
                <h4>Analisis Dampak Strategis</h4>
                <p>Ancaman siber pada domain maritim Indonesia berpotensi menyebabkan:</p>
                <ul>
                    <li><strong>Krisis kedaulatan</strong> melalui manipulasi awareness maritim</li>
                    <li><strong>Kerugian ekonomi masif</strong> akibat gangguan rantai pasok</li>
                    <li><strong>Krisis energi</strong> jika pelabuhan minyak lumpuh</li>
                    <li><strong>Dampak geopolitik</strong> terhadap posisi Indonesia sebagai poros maritim dunia</li>
                </ul>
                
                <h4 style="margin-top: 20px;">Rekomendasi</h4>
                <ul>
                    <li>Implementasi cybersecurity framework khusus sektor maritim</li>
                    <li>Enkripsi dan autentikasi data AIS/ECDIS</li>
                    <li>Air-gapping sistem kritis pelabuhan</li>
                    <li>Latihan gabungan TNI AL-Badan Siber Nasional menghadapi serangan siber maritim</li>
                </ul>
            </div>
        </div>

        <footer>
            <p>© 2025 - Laporan Analisis Cyber Warfare | Sertu Ttu Laksono Sheptian Yoga P</p>
        </footer>
    </div>
</body>
</html>