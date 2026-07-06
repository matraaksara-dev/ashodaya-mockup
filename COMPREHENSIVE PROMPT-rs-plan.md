"Pra-Rancangan/Skematik Desain (Preliminary/Schematic Design) yang dilengkapi dengan komponen Studi Kelayakan Awal (Preliminary Feasibility Study)"

# PROMPT UNTUK AI — RANCANGAN AWAL PROYEK RUMAH SAKIT
**Gunakan untuk Claude atau model dengan context window besar.**

Buatlah rancangan awal proyek rumah sakit yang sangat detail, komprehensif, dan profesional. Jangan hilangkan satu pun instruksi di bawah ini. Ikuti semua spesifikasi secara ketat.

---

## 0. PERAN, MODE EKSEKUSI, DAN FORMAT KELUARAN

### 0.1 Peran (Persona)
Bertindaklah sebagai **tim gabungan**, bukan satu penulis:
- **Principal Architect** — bertanggung jawab atas konsep massa bangunan, zoning, dan narasi desain.
- **Healthcare Planner (setara konsultan Siloam Group)** — bertanggung jawab atas kepatuhan terhadap standar Kemenkes, distribusi bed, dan alur klinis.
- **Quantity Surveyor / Estimator** — bertanggung jawab atas seluruh perhitungan luasan, validasi angka, dan tabel estimasi.
- **Brand & Interior Strategist** — bertanggung jawab atas penerapan Corporate Color Brand Template (Bagian 9) ke seluruh elemen desain fisik.
- **Editor Teknis** — memastikan seluruh dokumen konsisten, tidak ada kontradiksi angka, dan siap cetak sebagai proposal.

Tulis seolah kelima peran ini berkolaborasi, tetapi keluaran akhir tetap satu dokumen tunggal yang koheren.

### 0.2 Mode Eksekusi (Wajib — Jangan Lewati)
Karena volume dan detail yang diminta sangat besar, kerjakan dalam **tahapan berurutan**, dan **jangan memampatkan/generalisasi** demi menyingkat jawaban. Urutan wajib:

1. **Tahap Validasi Angka** — sebelum menulis narasi apa pun, buat *tabel validasi kuantitatif* yang membuktikan semua angka dalam Bagian 1 saling konsisten (lihat 0.4).
2. **Tahap Site Plan** — narasi + tabel zoning tapak, termasuk penegasan bahwa gedung rumah sakit dan gedung parkir adalah dua massa bangunan yang **terpisah**.
3. **Tahap Floor Plan per Lantai Rumah Sakit** — enam sub-bagian terpisah, satu per lantai, masing-masing dengan tabel ruangan dan tabel distribusi bed kumulatif.
4. **Tahap Gedung Parkir 5 Lantai & Unit Pengolahan Limbah** — termasuk akses masuk tengah, putaran tengah gedung parkir, dan alokasi lantai 1 untuk unit pengolahan limbah.
5. **Tahap Sirkulasi & Jalan Akses 7 Meter.**
6. **Tahap Ruang Terbuka Hijau (17m x 67m).**
7. **Tahap Konsep Desain, Narasi, dan Brand Application** — penerapan palet warna Bagian 9 ke tiap zona.
8. **Tahap Estimasi Luasan Total & Rekonsiliasi Lahan** — tabel akhir yang menjumlahkan seluruh komponen dan membandingkannya dengan luas lahan total 85m x 66m.
9. **Tahap Justifikasi Desain & Catatan Teknis.**
10. **Tahap Changelog & Lampiran.**

Jika keterbatasan panjang jawaban membuat seluruh tahapan tidak muat dalam satu respons, **nyatakan secara eksplisit di akhir jawaban tahap mana yang sudah selesai dan tahap mana yang masih tertunda**, lalu lanjutkan pada respons berikutnya — jangan diam-diam memotong isi tanpa pemberitahuan.

### 0.3 Format Dokumen Akhir (Wajib: Word/.docx)
Keluaran akhir harus disusun **sebagai dokumen Word (.docx) profesional**, bukan sekadar teks chat. Gunakan struktur berikut agar heading dapat dikonversi otomatis menjadi Table of Contents:

- **Cover Page**: Nama proyek "ASHODAYA HOSPITAL — Fajar Harapan", sub-judul "Rancangan Awal Proyek Rumah Sakit", lokasi proyek, tanggal dokumen, dan disclaimer "Dokumen Konsep Awal — Untuk Keperluan Presentasi Internal".
- **Daftar Isi (Table of Contents)** otomatis dari heading Level 1 & 2.
- **Heading Level 1** untuk tiap Bagian besar (1–9 seperti struktur di bawah, plus lampiran).
- **Heading Level 2/3** untuk sub-bagian (mis. per lantai, per palet warna).
- **Tabel** untuk semua data numerik (luasan, distribusi bed, palet warna, changelog) — jangan sajikan angka penting hanya dalam bentuk paragraf.
- **Header/footer**: nama proyek di header, nomor halaman di footer.
- Gunakan gaya penomoran konsisten (1.1, 1.2, dst.) mengikuti struktur prompt ini.
- Sisipkan placeholder eksplisit bertanda `[GAMBAR: deskripsi]` di titik-titik yang seharusnya diisi Site Plan, Floor Plan, dan render 3D, karena AI teks tidak dapat menghasilkan gambar arsitektural sungguhan — jangan berpura-pura menyisipkan gambar nyata.

### 0.4 Validasi Kuantitatif Wajib (Cross-Check)
Sebelum finalisasi, AI **wajib** membuat tabel yang membuktikan kombinasi berikut tidak saling bertentangan, dan menuliskan secara eksplisit jika ditemukan potensi konflik geometris (jangan disembunyikan atau dihaluskan):

| Komponen | Dimensi/Luasan Diberikan |
|---|---|
| Lahan keseluruhan | 85 m x 66 m |
| Bangunan Rumah Sakit | 64,3 m x 33,7 m = 2.166,91 m² |
| Gedung Parkir | 5 lantai, luas floor 43,5 m x 30 m = 1.305 m² per lantai |
| Unit Pengolahan Limbah (di dalam Gedung Parkir lantai 1) | 17,5 m x 8 m = 817 m² |
| Ruang terbuka hijau/fasilitas minor | 17 m x 67 m (bersih, di luar jalan keliling) |
| Jalan akses/keliling | lebar 7 m, dari entrance ke exit, termasuk ring road |

Catatan penting untuk validasi:
- **Gedung Rumah Sakit dan Gedung Parkir adalah dua bangunan yang terpisah** (tidak menyatu/tidak bertumpuk satu sama lain) — pastikan Site Plan dan seluruh narasi mencerminkan pemisahan ini secara konsisten.
- Gedung Parkir memiliki **akses masuk di posisi tengah bangunan** dan **jalur putaran (ramp/sirkulasi) di posisi tengah gedung parkir**.
- Lantai 1 Gedung Parkir dialokasikan untuk **Unit Pengolahan Limbah**, diletakkan di **bagian paling depan** dari massa Gedung Parkir tersebut.
- Lantai 2 sampai Lantai 4 Gedung Parkir digunakan sepenuhnya sebagai **area parkir**.
- Lantai 5 Gedung Parkir digunakan sepenuhnya sebagai **Kantin**.

Jika penjumlahan luas bangunan RS + parkir + unit pengolahan limbah + ruang hijau + jalan keliling tidak pas ke dalam 85 m x 66 m secara presisi, **AI wajib menyatakan hal ini secara terbuka sebagai catatan teknis** (bukan memaksakan angka agar terlihat konsisten), dan menawarkan 1-2 opsi penyesuaian tata letak yang realistis. Kejujuran teknis diutamakan di atas kerapian kosmetik dokumen.

### 0.5 Rubrik Kualitas (AI mengevaluasi keluarannya sendiri sebelum selesai)
Sebelum dianggap final, tiap tahap harus lulus kriteria berikut:
- [ ] Tidak ada angka yang bertentangan dengan Bagian 1.
- [ ] Total bed di seluruh lantai rumah sakit = tepat 150 (dibuktikan dengan tabel kumulatif per lantai).
- [ ] Semua 9 poliklinik pada Bagian 4 muncul di alokasi ruang — tidak lebih, tidak kurang.
- [ ] Semua 5 warna Brand Palette (Bagian 9) direferensikan minimal satu kali dalam konteks aplikasi fisik (bukan hanya di tabel warna).
- [ ] Gedung Rumah Sakit dan Gedung Parkir digambarkan sebagai dua massa bangunan terpisah, tidak menyatu.
- [ ] Unit Pengolahan Limbah tercatat berada di lantai 1 Gedung Parkir, bagian depan massa gedung parkir.
- [ ] Setiap keputusan desain utama disertai kalimat justifikasi yang merujuk standar Kemenkes atau Siloam.

---

## 1. DATA LAHAN DAN BANGUNAN

### 1.1 Lahan Keseluruhan
- Luas tanah keseluruhan: **85 m x 66 m**.

### 1.2 Rumah Sakit
- Luas bangunan Rumah Sakit: **64,3 m x 33,7 m = 2.166,91 m²**.
- Total lantai rumah sakit: **6 lantai**.**lt basement, lantai 1 (area penanganan, (IGD, srug, clean up, clean std, clean, ruang ok 1, ruang ok 2, ruang ganti, ruang dokter, dll)), lantai 2 rawat inap, lantai 3 rawat inap, lantai 4 rawat inap, lantai 5 rawat inap, lantai 6 Rooftop**
- Desain gedung rumah sakit **mengerucut ke atas** (tapering upwards).
- Ruang VIP berada di lantai atas (lantai tertinggi).
- Luasan ruang VIP: **3,45 m x 5,5 m** per kamar. (estimaikan dapat berapa kamar)
- Ruang Kelas 1, Kelas 2, dan Kelas 3: luasannya harus sesuai dengan standar peraturan yang berlaku di Indonesia (Kemenkes).
- **Total jumlah tempat tidur seluruh rumah sakit harus tepat 150 bed**, termasuk ruang VIP.
- Parkiran Dokter dan staf management, Koridor lift, tangga,Laundry, Dapur Khusus Rumah Sakit, dan gudang berada **di basement gedung rumah sakit**.
- Posisi bangunan rumah sakit berada di **TENGAH-DEPAN lahan** (center-front), menjadi focal point utama saat memasuki tapak dari jalan utama (Jalan Tentara Pelajar). Fasad depan rumah sakit menghadap langsung ke arah jalan masuk utama/akses publik.
- Parkiran Ambulan ada didepan IGD Gedung Rumah Sakit

### 1.3 Gedung Parkir
- **Gedung Parkir berdiri sebagai bangunan terpisah dari Gedung Rumah Sakit** (dua massa bangunan yang tidak menyatu).
- **Jumlah lantai: 4 lantai.**
- **Akses masuk Gedung Parkir berada di posisi tengah bangunan**, dengan **jalur putaran (ramp/sirkulasi) juga berada di posisi tengah Gedung Parkir**.
- **Luas floor Gedung Parkir: 43,5 m x 30 m = 1.305 m² per lantai.**
- **Lantai 1**: dialokasikan untuk **Unit Pengolahan Limbah**, diletakkan di **bagian paling depan** massa Gedung Parkir, dengan luasan **17,5 m x 8 m = 817 m²**.
- **Lantai 2 (37 mobil, 120 Motor) - 3 (37 mobil, 120 Motor)– Lantai 4 (37 mobil, 110 Motor) - lantai 5 (digunakan untuk kantin pengunjung dan umum)**: digunakan sepenuhnya sebagai **area parkir** kendaraan staf, pengunjung, dan ambulans/logistik rumah sakit.
- Unit Pengolahan Limbah berada di **lantai 1 Gedung Parkir, bagian belakang** tapak secara keseluruhan (mengacu pada orientasi Site Plan: Gedung Parkir berada di belakang, Gedung Rumah Sakit di depan).
- Desain atap Gedung Parkir pada lantai teratas dapat difungsikan sebagai rooftop parkir terbuka atau area hijau tambahan (opsional, sebutkan sebagai catatan desain).

### 1.4 Ruang Terbuka Hijau & Fasilitas Minor
- Lahan dialokasikan untuk fasilitas minor berikut:
  - Ruang terbuka hijau (taman, area duduk luar ruangan, healing garden).
  - Elemen lansekap pendukung konsep "healing environment" (mis. gazebo kecil, jalur pejalan kaki taman, kolam kecil/water feature, area tunggu keluarga pasien di luar ruangan).
  - Sisa lahan kosong yang dialokasikan sebagai ruang terbuka hijau/fasilitas minor memiliki luasan **17 m x 67 m**.
  - Luasan ini adalah luasan **bersih di luar jalan keliling** — jalan akses (lihat poin 1.5) sudah dihitung terpisah dan tidak termasuk dalam angka 17 m x 67 m ini.
  - area pemulihan pasien, parkir tambahan khusus mobil cukup 50 unit bisa digunakan sebagian areanya untuk parkir vip.

### 1.5 Jalan Akses / Sirkulasi Kendaraan
- **Lebar jalan akses adalah 7 meter**, berlaku mulai dari pintu masuk (entrance) hingga pintu keluar (exit), termasuk **jalan keliling (ring road) tapak**.
- Jalan keliling ini digunakan untuk sirkulasi kendaraan pengunjung, ambulans, dan logistik yang mengelilingi bangunan utama di dalam tapak.
- Pastikan lebar 7 meter ini cukup untuk dua jalur kendaraan berlawanan arah beserta ruang manuver ambulans di titik IGD.
- Jalur ini harus digambarkan secara jelas dalam Site Plan sebagai elemen sirkulasi utama, terpisah dari perhitungan luas bangunan dan ruang terbuka hijau.

---

## 2. LOKASI PROYEK

Rumah sakit berlokasi di **Jalan Tentara Pelajar, Kelurahan Bumijo, Kecamatan Jetis, Kota Yogyakarta, Daerah Istimewa Yogyakarta (Kode Pos: 55231)**.

Letak strategis:
- Utara Tugu Jogja: ±700 meter ke barat laut Monumen Tugu Yogyakarta.
- Barat Stasiun Tugu: sangat dekat dengan Stasiun Yogyakarta (waktu tempuh <5 menit).
- Area ring satu pariwisata Yogyakarta, dikelilingi hotel, losmen, dan kuliner lokal.
- Dekat dengan Koramil 01/Jetis, sekolah, dan instansi pemerintahan.

Gunakan konteks lokasi ini untuk memberi justifikasi mengapa posisi tengah-depan lahan (1.2) dan fasad menghadap jalan masuk itu strategis — kaitkan dengan visibilitas dari jalan raya, arus lalu lintas Tugu–Stasiun, dan citra publik rumah sakit sebagai landmark kawasan.

---

## 3. KONSEP DAN STANDARISASI

Rumah sakit ini dikelola oleh **SILOAM Management**. Lakukan riset internal mengenai standar operasional, desain, fasilitas, dan best practices Siloam Hospitals di Indonesia. Sesuaikan seluruh rancangan dengan:
- Standar rumah sakit Indonesia (Kementerian Kesehatan).
- Standar Siloam Hospitals.
- Peraturan bangunan, keselamatan, aksesibilitas, dan fasilitas kesehatan terkini.

Jika AI tidak memiliki akses real-time/pencarian untuk memverifikasi standar Siloam terkini, **nyatakan ini secara eksplisit sebagai asumsi berbasis pengetahuan umum industri rumah sakit swasta kelas menengah-atas di Indonesia**, bukan seolah-olah data internal resmi Siloam. Jangan mengarang klaim spesifik seolah dikutip dari dokumen resmi Siloam yang tidak dapat diverifikasi.

---

## 4. POLIKLINIK (Hanya yang disebutkan, jangan tambah)

- Poli Umum
- Poli Internis
- Poli Bedah
- Poli Kandungan
- Poli Anak
- Poli THT
- Poli Syaraf
- Poli Gigi
- Poli Mata

---

## 5. A. FASILITAS WAJIB

- IGD / UGD
- Ruang Observasi
- Ruang Rawat Inap (semua kelas)
- Kamar Mayat
- Basement
- Gedung Parkir 4 lantai (terpisah dari Gedung Rumah Sakit, lihat poin 1.3), termasuk Unit Pengolahan Limbah di lantai 1
- Ruang tunggu yang luas dan nyaman
- Semua fasilitas rumah sakit umum lainnya (laboratorium, radiologi, farmasi, ruang operasi, ICU, NICU, dll. sesuai kebutuhan standar)
- Ruang terbuka hijau dan fasilitas minor pendukung pada lahan 17 m x 67 m (lihat poin 1.4)

---

## 5. B. LIST ALKES 
,Quantity,Satuan,Keterangan,Merek,Jenis,Satuan (Rp),Jumlah (Rp)
,,,POLI UMUM,,,,
1,1,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,81084000
2,1,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,22759000
3,2,Pcs,Stethoscope,Littmann,Classic III,7250000,14500000
4,1,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,10221000
5,1,Unit,Ultrasonic Nebulizers,Dummy,Nebulizer VVT,4869000,4869000
6,1,Pcs,Adult Weight Scale Digital,Gerlink,GL ANTRO-02,4294000,4294000
7,3,Pcs,Tongue Spatula,Jenco,"Mayo Tongue Depressor, 16/22 mm, 17 cm",2435000,7305000
8,1,Pcs,Reflex Hammer,Jenco,"Taylor Percussion Hammer, 20 cm",984000,984000
9,1,Set,Combination Diagnostic Set in,MARPLUS,SET 79,61254000,61254000
10,1,Pcs,Baby Scale,Gerlink,GL ANTRO-01,6259000,6259000
11,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
12,1,Set,Laryngoscope,Medtromed,FO Macintosh Laryngoscope 4 Blade,21063000,21063000
13,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
,,,POLI INTERNIS,,,,
14,2,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,162168000
15,2,Pcs,Stethoscope,Littmann,Classic III,7250000,14500000
16,2,Pcs,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,20442000
17,2,Pcs,Reflex Hammer,Jenco,"Taylor Percussion Hammer, 20 cm",2435000,4870000
18,2,Pcs,Tongue Spatula,Jenco,"Mayo Tongue Depressor, 16/22 mm, 17 cm",984000,1968000
19,2,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,45518000
20,1,Unit,ECG 12 Channel with full,Medtromed,MD-ECG12CH With Trolley,225312000,225312000
21,1,Unit,Suction Pump Drainage,Medtromed,MD-02 MSP,155174000,155174000
22,1,Unit,Manual Resuscitation Silicone,GEA,Manual PVC Set,434000,434000
23,1,Set,Combination Diagnostic Set in,MARPLUS,SET 79,61254000,61254000
24,1,Set,Laryngoscope,Medtromed,FO Macintosh Laryngoscope 4 Blade,21063000,21063000
25,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
26,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
,,,POLI BEDAH,,,,
27,2,Unit,Operating Table,BES,BES Luxury OTE-001,1624148000,3248296000
28,2,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,45518000
29,2,Pcs,Stethoscope,Littmann,Classic III,7250000,14500000
30,2,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,20442000
31,1,Set,Electrosurgical unit Medium 350 ,Doctanz,400 watts,144927000,144927000
32,1,Set,Circumcision Set,Medtromed,Various,51477000,51477000
33,1,Pcs,Alat Pembuka Gips,Jenco,Jenco as manual plaster saw set,119479000,119479000
34,2,Set,Minor Surgey Set,Medtromed,Various,101939000,203878000
35,1,Set,Large Suture Instrument Set,Medtromed,Tontara,37221000,37221000
36,1,Pcs,Bandage Instrument Set,Mar Plus,Various,11144000,11144000
37,1,Unit,Suction Pump Drainage,Medtromed,MD-02 MSP,155174000,155174000
38,1,Unit,Mobile Operating Lamp,Medtromed,MD-578 LED with bateray,351458000,351458000
39,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
40,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
41,2,Unit,Anesthesin Ventilator,AXCENT,APUS X3 High end,3647446000,7294892000
,,,POLI PARU-PARU,,,,
42,1,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,81084000
43,1,Pcs,Stethoscope,Littmann,Classic III,7250000,7250000
44,1,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,10221000
45,2,Pcs,Tongue Spatula,Jenco,"Mayo Tongue Depressor, 16/22 mm, 17 cm",984000,1968000
46,1,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,22759000
47,1,Set,Thoractomy Instrument Set,Jenco,Jenco as thoracotomy set,3393187000,3393187000
48,1,Unit,Suction Pump Drainage,Medtromed,MD-02 MSP,155174000,155174000
49,1,Set,Bronchoscope consisting of,Gerlink,GL ECS-01 VAR94,6434521000,6434521000
50,1,Unit,Ultrasonic Nebulizers,Dummy,Nebulizer VVT,4869000,4869000
51,1,Unit,X-Ray Unit/C-arm Mobile x-Ray,GMM,CHORUS with Survey and Dose Meter,6904692000,6904692000
52,1,Unit,Spirometer Portable,Sibelmed-Spain,DatospirAURA T,73718000,73718000
53,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
,,,POLI JANTUNG,,,,
54,1,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,81084000
55,1,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,22759000
56,1,Pcs,Stethoscope,Littmann,Classic III,7250000,7250000
57,1,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,10221000
58,1,Unit,ECG multi channel with monitor,KALTECH,KAL-U90,208196000,208196000
59,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
,,,POLI KANDUNGAN,,,,
60,1,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,81084000
61,1,Pcs,Stethoscope,Littmann,Classic III,7250000,7250000
62,2,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,20442000
63,1,Set,Fetal Doppler,KALTECH,KFM-1,158703000,158703000
64,1,Unit,Gynaecological Examination Table,Megal,MAGYN-01,45328000,45328000
65,1,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,22759000
66,1,Unit,CGT,Batos,BT-350,37825000,37825000
67,1,Unit,Gynaecological Examination,Jenco,jenco as examination material health set,88247000,88247000
68,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
69,1,Unit,Gynaecological Chair with foot plate,Medtromed,MD-02 GE,135701000,135701000
70,1,Unit,Timbangan dg tinggi badan,Gerlink,GL ANTRO STD 01,3932000,3932000
71,1,Unit,Ultrasonography (USG),GE,Volusion P8BT-22,1942949000,1942949000
72,1,Set,Vaginal Spechulum,Jenco,Grove Vaginal Specula Fig 2.95 X 35 mm,3801000,3801000
73,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
74,10,Unit,Ranjang Bayi/box baby,Megal,MABAB-02,36363000,363630000
,,,POLI ANAK,, ,,
75,2,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,162168000
76,2,Pcs,Baby Scale,Gerlink,GL ANTRO-01,6259000,12518000
77,2,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,20442000
78,2,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,45518000
79,1,Unit,ECG 12 Channel with full,Medtromed,MD-ECG12CH With Trolley,225312000,225312000
80,1,Set,Lumbar Function Instrumen Set,Mar Plus,Large Fragment Instrumen Set 1.1,905091000,905091000
81,1,Set,Infanct Resuscitation Set Silicone,GEA,Neo-1,30074000,30074000
82,1,Set,Combination Diagnostic Set in,MARPLUS,SET 79,61254000,61254000
83,1,Unit,Ultrasonic Nebulizers,Dummy,Nebulizer VVT,4869000,4869000
84,2,Pcs,Stethoscope,Littmann,Classic III,7250000,14500000
85,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
86,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
87,1,Unit,Suction Pump Drainage,Medtromed,MD-02 MSP,155174000,155174000
,,,POLI THT,,,,
88,1,Unit,ENT In Unit and Chair,OPTOMIC,Otosmart,1105628000,1105628000
89,1,Unit,ENT Chair,OPTOMIC,OP-54,386486000,386486000
90,1,Set,ENT Instrument Chair,OPTOMIC,Otosmart,729254000,729254000
91,1,Set,Head Lamp Suspection/portable,OPTOMIC,OP-HL 150,95049000,95049000
92,1,Set,Head Lamp with condition table,OPTOMIC,CP-LFS,61925000,61925000
93,1,Unit,Audiometer,Sibelmed-Spain,Sibelsound 400 ACM Plus,218898000,218898000
94,1,Unit,Sound Proof Room + 2 buah kursi,Various,Various,730228000,730228000
95,1,Unit,Otoscope,OPTOMIC,Ruget Telescope,151657000,151657000
96,1,Pcs,Stethoscope,Littmann,Classic III,7250000,7250000
97,1,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,10221000
98,1,Set,Sinusscope,OPTOMIC,Ruget Telescope,151657000,151657000
99,1,Set,Nasopharyngolaryngoscopy,Gerlink,GL ECS-01 VAR27,4758649000,4758649000
100,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
101,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
,,,POLI SARAF,,,,
102,1,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,81084000
103,1,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,22759000
104,1,Set,Lumbar Function Instrumen Set,Mar Plus,Large Fragment Instrumen Set 1.1,905091000,905091000
105,1,Pcs,Stethoscope,Littmann,Classic III,7250000,7250000
106,1,Pcs,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,10221000
107,1,Pcs,Reflex Hammer,Jenco,"Taylor Percussion Hammer, 20 cm",984000,984000
108,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
109,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
,,,POLI GIGI,,,,
110,1,Unit,Dental Unit Electric,SS ITALO,Simple & Smart,490470000,490470000
111,1,Set,Extracing Forceps for Child,Saffa marwa,Flat Handle FC,1520000,1520000
112,1,Set,Extracing Forceps for Adult,Saffa marwa,Flat Handle FA,2570000,2570000
113,2,Set,Dental Instrument Set,Gerlink,Dental set,1148100000,2296200000
114,1,Unit,Dental Autociave / dry head,Runda,Dental Autociave MAX-88,58419000,58419000
115,1,Unit,Dental panaromic Set,Triden,Multifov 11 X 14,7922968000,7922968000
,,,POLI BEDAH NON BEDAH,,,,
116,8,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,648672000
117,6,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,136554000
118,2,Unit,Infusion Pomp,Medtromed,MD-IPS 10,69615000,139230000
119,2,Unit,Sytenge Pump,Medtromed,MD-SPS 10,69372000,138744000
120,2,Unit,ECG 3/6/12 Channel,Medtromed,MD-ECG12CH With Trolley,265073000,530146000
121,2,Unit,Patient Strecher/Transport,Medtromed,MD-01 STD,126062000,252124000
122,4,Pcs,Stethoscope,Littmann,Classic III,7250000,29000000
123,6,Unit,Suction Pump,Medtromed,MD-02 STD,182557000,1095342000
124,2,Unit,Oksigen Teraphy 6 m,-,Tabung Oksigen,4508000,9016000
125,3,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,30663000
126,1,Unit,Laboratory Refrigerator,KALTECH,KLR-R038,623128000,623128000
127,2,Unit,Spirometer Portable,Sibelmed-Spain,DatospirAURA T,73718000,147436000
128,2,Unit,Emergency Troley,Megal,MAET-01,33956000,67912000
129,1,Pcs,Adult Weight Scale Digital,Gerlink,GL ANTRO-02,4294000,4294000
130,1,Pcs,Baby Scale,Gerlink,GL ANTRO-01,6259000,6259000
131,1,Unit,Bedside Monitor,Medtromed,MD-PM90 5 Parameter with Trolley,209332000,209332000
132,1,Unit,Manual Defribilator biphasic; ECG Pacemeter R,Medtromed,PACER,705376000,705376000
133,1,Unit,Mobile Operating Lamp,Medtromed,MD-578 LED with bateray,351458000,351458000
134,1,Unit,Adult Resuscitator Silicone,ENDO,RESQ-BAG Manual Resuscitator,6811000,6811000
135,1,Unit,Infant Resuscitator Silicone,Serenity,Manual Resuscitator for Infant ,1522000,1522000
136,1,Set,Adult Instubation,Serenity,Instubation set-RC Surg/Well,40538000,40538000
137,1,Set,Infant Instubation,Serenity,Instubation Child Indtrument Set,92232000,92232000
138,1,Unit,Medical Emergency Kit Adult,Jenco,Jenco As Emergency room set,149355000,149355000
139,1,Unit,Medical Emergency Kit Infant,Jenco,Jenco As Mate. & Neonatus Emerg. set,139567000,139567000
140,1,Unit,Operating Table,BES,BES Luxury OTE-001,1624148000,1624148000
141,1,Set,Electrosurgical unit Medium 350 ,Doctanz,400 watts,144927000,144927000
142,1,Unit,Suction Pump Drainage,Medtromed,MD-02 MSP,155174000,155174000
143,1,Set,Basic Instrument Set,Mar Plus,MAJOR BASIC SET 1-3,249556000,249556000
144,1,Set,Large Suture Instrument Set,Medtromed,Tontara,37221000,37221000
145,1,Set,Veno Section instrument set,Mar Plus,VENO SECTION,35017000,35017000
146,1,Set,Trancheostormy Instrumen Set,Mar Plus,Trancheostormy Instrumen Set 1.2,59777000,59777000
147,1,Pcs,Bandage Instrument Set,Mar Plus,Bandage Set,11144000,11144000
148,1,Set,Minor Surgey Set,Medtromed,Various,101939000,101939000
149,1,Set,Dilatation and Curettage,Mar Plus,Dilatation and Curettage Set,57904000,57904000
150,1,Unit,Embryiotormy Instrument Set,AS Medizitechnik,Various,177429000,177429000
151,1,Unit,Anasthesy Apparatus,-,Medical Anasthesia Machine AM831,346815000,346815000
152,1,Unit,Bed Screen SS,Onemed,4 Bidang Stainless - Plus Kain,3043000,3043000
153,1,Set,Combination Diagnostic Set in,MARPLUS,SET 79,61254000,61254000
154,1,Pcs,Tongue Spatula,Jenco,"Mayo Tongue Depressor, 16/22 mm, 17 cm",984000,984000
,,,OBSERVATION,,,,
155,1,Unit,Examination Table + Tangga SS,Medtromed,MD-02 ET,81084000,81084000
156,1,Pcs,Stethoscope,Littmann,Classic III,7250000,7250000
157,1,Unit,Sphygmomanometer Mobile,Medtromed,Adult/Child,10221000,10221000
158,1,Pcs,Reflex Hammer,Jenco,"Taylor Percussion Hammer, 20 cm",984000,984000
159,1,Pcs,Tongue Spatula,Jenco,"Mayo Tongue Depressor, 16/22 mm, 17 cm",984000,984000
160,1,Unit,Halogen Examination Lamp,Medtromed,MD-07 LED,22759000,22759000
161,1,Unit,ECG 8 Channel with fullinterpretive,KALTECH,KEC-03,225312000,225312000
162,1,Unit,Suction Pump Drainage,Medtromed,MD-02 MSP,155174000,155174000
163,1,Unit,Manual Resuscitation Silicone,ENDO,RESQ-BAG Manual Resuscitator,6811000,6811000
,,,EMERGENCY SURGERY,,,,
164,5,Unit,Kamar Operasi,Operamed,Mayor Standart + Full Equipment & Timbal,8519320000,42596600000
165,2,Unit,Caterisasi Jantung,GE,GE Innova IGS 5 Premium,55547213000,111094426000
166,1,Unit,Laparoscopy,Gerlink,GL ECS-01 VAR49,14187469000,14187469000
167,1,Unit,CT scan 64 Slice,GE,Revolution Maxima,28965688000,28965688000
168,1,Unit,MRI,GE,Signa Prime,73832045000,73832045000
169,1,Unit,Hemidialisasi,Toray,TR-8000,769173000,769173000
,,,,,,,337417478000

## 6. KONSEP DESAIN & NARASI

- **Lobi utama rumah sakit** harus terinspirasi dari desain lobi hotel eksklusif: mewah, nyaman, menenangkan, modern, dan elegan.
- Konsep keseluruhan: **"Meletakkan seluruh kesedihan di belakang"**. Bagian depan (lobi dan area publik) dirancang untuk menjaga mentalitas pengunjung dan pasien agar merasa bahagia, tenang, dan penuh harapan saat pertama kali masuk.
- Desain arsitektur secara keseluruhan harus elegan, modern, humanis, dan sesuai dengan karakter kota Yogyakarta.
- Gedung mengerucut ke atas dengan penempatan ruang VIP di lantai tertinggi.
- Dengan posisi rumah sakit di tengah-depan lahan, fasad utama dan lobi harus dirancang agar langsung terlihat dan menjadi orientasi utama pengunjung sejak dari jalan masuk (Jalan Tentara Pelajar), memperkuat kesan "gerbang harapan" sesuai konsep narasi Ashodaya.
- Rujuk kembali secara eksplisit ke tabel palet warna Bagian 9 (nama warna dan HEX code-nya) setiap kali sebuah ruang atau zona dideskripsikan (lobi, ruang anak, ruang tunggu, VIP, dsb.) — jangan hanya menyebut "warna hangat" atau "warna menenangkan" secara generik.

---

## 7. TUGAS AI

Buatlah rancangan awal lengkap yang mencakup, **masing-masing sebagai bagian terstruktur dengan heading dan tabel sendiri**:

1. **Site Plan** lengkap dengan:
   - Penempatan gedung rumah sakit di tengah-depan lahan.
   - Penempatan Gedung Parkir 5 lantai sebagai bangunan **terpisah**, di bagian belakang tapak, dengan akses masuk dan jalur putaran di posisi tengah gedung parkir.
   - Jalan keliling selebar 7 meter dari pintu masuk sampai pintu keluar.
   - Area ruang terbuka hijau/fasilitas minor seluas 17 m x 67 m (di luar jalan keliling).
   - Sirkulasi kendaraan, pejalan kaki, dan akses ambulans.
   - Landscaping dan akses keluar-masuk tapak.
   - `[GAMBAR: Site Plan skematik top-view tapak 85m x 66m]`
2. **Floor Plan** per lantai rumah sakit (6 lantai), **setiap lantai sebagai sub-bagian terpisah**, dengan:
   - Tabel distribusi ruangan per lantai.
   - Tabel distribusi bed per lantai + **tabel kumulatif** yang membuktikan total = 150 bed.
   - `[GAMBAR: Floor Plan Lantai X]` untuk tiap lantai.
3. **Floor Plan Gedung Parkir** (5 lantai), dengan:
   - Lantai 1: Unit Pengolahan Limbah (17,5 m x 8 m = 817 m²), diletakkan paling depan massa Gedung Parkir.
   - Lantai 2–4: area parkir.
   - Lantai 5: Kantin Umum.
   - Penjelasan akses masuk tengah dan jalur putaran tengah.
   - `[GAMBAR: Floor Plan Gedung Parkir per lantai]`
4. **Desain 3D konseptual** dan perspektif utama (terutama lobi, fasad depan yang menghadap jalan masuk, dan ruang VIP) — dalam bentuk deskripsi naratif detail + placeholder gambar, bukan gambar sungguhan.
5. **Zoning** dan alur pasien, pengunjung, staf, dan logistik yang optimal — termasuk alur dari Gedung Parkir menuju Gedung Rumah Sakit (mengingat keduanya terpisah). Sajikan sebagai diagram alur tekstual (mis. daftar bertahap atau tabel alur) yang bisa dikonversi jadi diagram di Word.
6. **Estimasi luasan** setiap bagian utama: rumah sakit, Gedung Parkir (termasuk Unit Pengolahan Limbah), jalan keliling (7m), dan ruang terbuka hijau/fasilitas minor (17m x 67m) — dalam satu **tabel rekonsiliasi akhir** yang totalnya dibandingkan terhadap luas lahan 85m x 66m (lihat 0.4).
7. **Justifikasi desain** berdasarkan standar Siloam, regulasi Indonesia, dan konsep narasi yang diminta — termasuk alasan penempatan rumah sakit di tengah-depan, pemisahan Gedung Parkir dari Gedung Rumah Sakit, dan penempatan Unit Pengolahan Limbah di lantai 1 Gedung Parkir bagian depan. Setiap justifikasi minimal 2-3 kalimat, bukan satu baris generik.
8. **Rekomendasi material, pencahayaan, dan suasana** yang mendukung healing environment, termasuk untuk area ruang terbuka hijau — kaitkan eksplisit dengan palet warna Bagian 9 (mis. material apa yang mewakili "Warm Stone", pencahayaan apa yang mendukung nuansa "Dawn Gold").

Buatlah output yang sangat detail, profesional, terstruktur, dan siap digunakan sebagai dasar presentasi proposal proyek dan **siap dikonversi menjadi dokumen Word (.docx)** sesuai format Bagian 0.3. Gunakan pendekatan arsitektur kesehatan kelas dunia namun tetap kontekstual dengan Yogyakarta.

Sertakan juga catatan teknis mengenai:
- Distribusi bed (150 bed total).
- Perhitungan lebar jalan 7 meter dan dampaknya terhadap sirkulasi tapak.
- Perhitungan luas Gedung Parkir 5 lantai dan Unit Pengolahan Limbah di lantai 1.
- Alasan setiap keputusan desain utama.

---

## 8. RINGKASAN DATA UTAMA

| No | Item | Ketentuan |
|----|------|-----------|
| 1 | Luas Lahan Keseluruhan | 85 m x 66 m |
| 2 | Luas Bangunan Rumah Sakit | 64,3 m x 33,7 m = 2.166,91 m² |
| 3 | Jumlah Lantai Rumah Sakit | 6 lantai |
| 4 | Posisi Rumah Sakit | Tengah-depan lahan, fasad menghadap Jalan Tentara Pelajar |
| 5 | Gedung Parkir | 5 lantai, terpisah dari Gedung Rumah Sakit |
| 6 | Akses & Putaran Gedung Parkir | Akses masuk di tengah bangunan, jalur putaran di tengah gedung parkir |
| 7 | Luas Floor Gedung Parkir | 43,5 m x 30 m = 1.305 m² per lantai |
| 8 | Unit Pengolahan Limbah | Lantai 1 Gedung Parkir, bagian depan massa gedung parkir, 17,5 m x 8 m = 817 m² |
| 9 | Lantai 2–4 Gedung Parkir | Area parkir |
| 10 | Lantai 5 Gedung Parkir | Kantin Umum |
| 11 | Jalan Akses/Keliling | Lebar 7 meter, dari entrance ke exit, termasuk ring road |
| 12 | Ruang Terbuka Hijau/Fasilitas Minor | 17 m x 67 m (bersih, di luar jalan keliling) |
| 13 | Total Tempat Tidur | 150 bed |

---

## 9. CORPORATE COLOR BRAND TEMPLATE

### ASHODAYA HOSPITAL — "Fajar Harapan"
**Brand Identity System for Siloam-Managed Hospital**

#### 9.1 Brand Color Philosophy

Berangkat dari filosofi nama Ashodaya (आशोदय) — gabungan dari *Asha* (Harapan) dan *Udaya* (Terbit/Fajar) — palet warna dirancang untuk membangkitkan sensasi fajar yang menenangkan: gelap perlahan berubah menjadi terang, dingin berubah menjadi hangat, dan harapan baru muncul.

| Warna | Kode | Filosofi |
|---|---|---|
| Dawn Gold | #F5A623 | Warna pertama matahari terbit — melambangkan harapan, optimisme, dan kehangatan |
| Twilight Blue | #1A2A4A | Langit sebelum fajar — melambangkan ketenangan, kepercayaan, dan profesionalisme medis |
| Healing Sage | #8BA88E | Warna alam yang menenangkan — melambangkan kesembuhan, pertumbuhan, dan keseimbangan |
| Pure Dawn | #FDF8F0 | Cahaya pertama yang murni — melambangkan kebersihan, kesucian, dan awal yang baru |
| Warm Stone | #D4C5A9 | Sentuhan bumi yang hangat — melambangkan stabilitas, kenyamanan, dan keakraban |

#### 9.2 Primary Color Palette

| Role | Color Name | HEX | RGB | CMYK | Usage |
|---|---|---|---|---|---|
| Primary 1 | Dawn Gold | #F5A623 | 245, 166, 35 | 0, 32, 86, 4 | Logo utama, CTA buttons, aksen |
| Primary 2 | Twilight Blue | #1A2A4A | 26, 42, 74 | 65, 43, 0, 71 | Logo, header, footer, teks utama |
| Primary 3 | Pure Dawn | #FDF8F0 | 253, 248, 240 | 0, 2, 5, 1 | Latar belakang, white space |

#### 9.3 Secondary Color Palette

| Role | Color Name | HEX | RGB | Usage |
|---|---|---|---|---|
| Secondary 1 | Healing Sage | #8BA88E | 139, 168, 142 | Aksen ruang hijau, elemen dekoratif |
| Secondary 2 | Warm Stone | #D4C5A9 | 212, 197, 169 | Elemen kayu, tekstur, material alami |
| Secondary 3 | Soft Coral | #E8836B | 232, 131, 107 | Aksen hangat untuk ruang anak & ibu |
| Secondary 4 | Misty Lavender | #B8B0C9 | 184, 176, 201 | Aksen ruang meditasi & ruang tunggu |

#### 9.4 Neutral Color Palette

| Role | Color Name | HEX | Usage |
|---|---|---|---|
| Neutral 1 | Pure White | #FFFFFF | Latar, spasi, elemen bersih |
| Neutral 2 | Soft Grey | #F5F5F5 | Latar sekunder, card backgrounds |
| Neutral 3 | Mid Grey | #9E9E9E | Teks sekunder, border |
| Neutral 4 | Deep Charcoal | #2D2D2D | Teks utama, elemen grafis |

---

## LAMPIRAN A — CHECKLIST PENYERAHAN DOKUMEN AKHIR

Sebelum menyatakan dokumen selesai, pastikan file .docx akhir memuat:

- [ ] Cover page dengan judul, lokasi, dan tanggal.
- [ ] Daftar isi otomatis.
- [ ] Bagian 1–9 lengkap sesuai struktur di atas, tanpa ada bagian yang hilang atau disingkat.
- [ ] Semua tabel numerik (luasan, bed, warna, ringkasan data) tersaji sebagai tabel Word, bukan paragraf.
- [ ] Gedung Rumah Sakit dan Gedung Parkir tergambar sebagai dua massa bangunan terpisah.
- [ ] Unit Pengolahan Limbah tercatat berada di lantai 1 Gedung Parkir bagian depan massa gedung parkir.
- [ ] Placeholder gambar `[GAMBAR: ...]` ditandai jelas di semua titik yang butuh visual arsitektural nyata.
- [ ] Catatan asumsi yang tidak dapat diverifikasi dicantumkan secara transparan, bukan disamarkan sebagai fakta pasti.
- [ ] Rekonsiliasi luas lahan (Bagian 0.4) menunjukkan hasil perhitungan apa adanya, termasuk jika ditemukan ketidaksesuaian geometris.

---

## LAMPIRAN B — CATATAN UNTUK AI EKSEKUTOR

Jika sebuah AI (termasuk Claude) menerima prompt ini dan menyadari bahwa cakupannya terlalu besar untuk satu respons tunggal:
1. Prioritaskan menyelesaikan **Bagian 1 (validasi angka) dan Bagian 7 poin 1-3 (Site Plan + Floor Plan Rumah Sakit + Floor Plan Gedung Parkir)** terlebih dahulu, karena ini adalah inti teknis proyek.
2. Sampaikan secara eksplisit kepada pengguna bagian mana yang sudah selesai dan bagian mana yang perlu diminta secara terpisah pada percakapan lanjutan (mis. "Lanjutkan ke Bagian 8-9").
3. Jangan mengorbankan akurasi angka demi mengejar kelengkapan seluruh dokumen dalam satu jawaban.


## DATA tambahan

Data tambahan Ringkasan RAB :
NO.,URAIAN,(Rp.),(Rp.)
1,Persiapan Lahan dan Pematangan Lahan,,2,000,000,000
2,Perencanaan, Pengawasan Perizinan-Perizinan,,5,000,000,000
3,Pekerjaan Konstruksi dan Arsitektur,,145,154,800,000
3a,Lt.Bsmt,46,577,200,000,
3b,Lt.1,26,648,900,000,
3c,Lt.2,19,927,800,000,
3d,Lt.3,16,289,700,000,
3e,Lt.4,16,289,700,000,
3f,Lt.5,16,289,700,000,
3g,Lt.6,3,131,800,000,
4,Pekerjaan Mekanikal, Elektrikal, Lift dan Genset,,5,900,000,000
5,Pekerjaan Interior dan Peralatan,,5,000,000,000
6,Peralatan Medis Kedokteran,,160,000,000,000
7,Pengelolahan Air Kotor dan Hidrant,,1,500,000,000
8,Pengelolahan Air Bersih dan Oksigen,,2,300,000,000
9,Pengelolahan (IPAL) Air Limbah RS,,5,500,000,000
10,Pengelolahan (IPAL) dan Limbah B3,,3,600,000,000
11,Instalasi Gas Medis Beserta Peralatan,,4,000,000,000
12,Pekerjaan Eksternal, Parkir dan Landscape,,4,500,000,000
13,Jaringan Informasi dan Telekomunikasi,,7,200,000,000
14,Biaya Operasional Awal Rumah Sakit (2 Tahun),,60,000,000,000
15,Kendaraan Ambulan dan Operasional,,5,300,000,000
16,Laundry, Kitchen, & Kitchen Set,,3,000,000,000
,Jumlah,,419,954,800,000
,PPn ,11%,46,195,028,000
,Jumlah Total,,466,149,828,000
,Jumlah Total Pembulatan,, Rp 466,149,828,000  