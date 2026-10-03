# 🌱 Huangji-World — Sistem Pertanian Spiritual & Non-Spiritual (Gardening System)

> **Modul:** 17 — Gardening System
> **Prinsip:** Anti-Cheat Enforced — Time & Qi Irrigation Dependent — Terintegrasi dengan Alkimia, Ekonomi, & Vitalitas
> **Rujukan Silang:** `02_VERDANT_QI_PLAINS.md`, `13_ECONOMY_SYSTEM.md`, `14_VITALITY_HUNGER_SYSTEM.md`, `19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`

---

## 0. Filosofi & Aturan Emas Pertanian

Bercocok tanam di Benua Huangji tidak hanya dilakukan oleh para kultivator untuk menghasilkan bahan racikan pil alkimia, tetapi juga oleh masyarakat fana (Mortal) untuk memenuhi bahan pangan, obat-obatan herbal dasar, serta komoditas perdagangan. Baik tanaman fana (non-spiritual) maupun tanaman spiritual membutuhkan pengelolaan nutrisi tanah, penyiraman air/Qi secara berkala, dan perlindungan dari ancaman hama.

### 📜 Aturan Emas Anti-Cheat Gardening
1. **Tidak Ada Panen Instan**: Tanaman tumbuh berdasarkan giliran (*Turn*) atau durasi waktu dunia yang berlalu secara sah. Tidak boleh ada skenario skip waktu tanpa perhitungan waktu dunia yang konsisten.
2. **Konsumsi Qi & Air Tercatat**: Setiap tindakan penyiraman Qi murni atau perawatan tanaman WAJIB mencatat pengurangan Qi/Stamina pada log profil karakter.
3. **Penyimpanan Item Origin Log**: Semua hasil panen herba dan tanaman spiritual WAJIB dicatat di **Item Origin Log** (`[Nama Item | Grade | Sumber: Hasil Panen Petak X | Timestamp]`) sebelum dapat digunakan untuk alkimia atau dijual.
4. **Resiko Kematian Tanaman**: Tanaman yang tidak disiram selama lebih dari 2 kali durasi siklus penyiraman akan layu dan mati (kehilangan benih dan hasil panen).

---

## 🏔️ 1. Tingkatan Kelas Tanah (Soil Grades)

Kualitas tanah menentukan kecepatan tumbuh, tingkat keberhasilan panen, dan batasan tier tanaman yang dapat ditanam.

| Kode Kelas | Nama Kelas Tanah | Ciri & Syarat Unsur | Lokasi Dominan | Efek Kecepatan & Kualitas | Maks. Tier Tanaman |
|---|---|---|---|---|---|
| **G-0** | **Tanah Fana / Tandus** | Unsur hara rendah, tanpa Qi. | Desa Fana, Area Pinggiran | Tumbuh Normal (1x), Kualitas Standar. | Khusus Non-Spiritual (Tier 0) |
| **G-1** | **Tanah Subur Biasa** | Unsur hara tinggi, kaya humus. | Lembah Hijau, Dataran Rendah | Tumbuh Normal (1x), Hasil Panen +10%. | Tier 1 Spiritual / Non-Spiritual |
| **G-2** | **Tanah Qi Kayu Murni (Verdant Soil)** | Dialiri napas alam & Qi Kayu pekat. | Verdant Qi Plains, Kebun Sekte | Tumbuh **2x Lebih Cepat**, Kualitas +1 Grade. | Tier 1 – Tier 3 Spiritual |
| **G-3** | **Tanah Beku Es Bintang (Frost Soil)** | Dingin ekstrim, dipenuhi Qi Es Murni. | Pegunungan Es Bintang | Khusus Tanaman Elemen Es/Air. Tumbuh 1.5x Cepat. | Tier 1 – Tier 4 Spiritual |
| **G-4** | **Tanah Abu Vulkanik (Lava Soil)** | Hangat & kaya mineral panas. | Crimson Blaze Peaks | Khusus Tanaman Elemen Api/Bumi. Tumbuh 1.5x Cepat. | Tier 1 – Tier 4 Spiritual |
| **G-5** | **Tanah Petir Ungu (Thunder Soil)** | Mengandung energi konduktif kilat. | Thunder Crest Mountains | Khusus Tanaman Elemen Petir/Logam. Tumbuh 2x Cepat. | Tier 1 – Tier 5 Spiritual |
| **G-6** | **Tanah Suci Abadi (Huangji Holy Soil)** | Dialiri urat naga (*Dragon Vein*) Kekaisaran. | Puncak Surgawi, Istana Agung | Tumbuh **4x Lebih Cepat**, Kualitas Murni (+2 Grade). | Tier 1 – Tier 9 Spiritual |

---

## 🧪 2. Pupuk Spiritual & Nutrisi Organik

Pemain dapat mengaplikasikan pupuk untuk mempercepat masa tanam atau meningkatkan kualitas hasil panen:

| Nama Pupuk / Nutrisi | Komposisi & Bahan | Efek Tumbuh | Kualitas Panen | Durasi Efek |
|---|---|---|---|---|
| **Pupuk Kompos Fana** | Kotoran Ternak & Daun Busuk | Memotong waktu tumbuh **1 Turn**. | Normal | 1 Siklus Tanam |
| **Pupuk Qi Kayu Rendah** | Serbuk Batu Spiritual + Sisa Herba Tier 1 | Memotong waktu tumbuh **2 Turn**. | Kualitas +5% | 1 Siklus Tanam |
| **Pupuk Cair Esens Spirit** | Ekstrak Darah Beast Tier 2–3 + Qi Murni | Memotong waktu tumbuh **50%**. | Potensi Hasil Panen ×2 | 1 Siklus Tanam |
| **Aroma Ginseng Abadi** | Abu Alkimia Pil Tier 4 + Air Murni | Memotong waktu tumbuh **75%**. | Kualitas Naik 1 Grade (Misal: Baik → Unggul) | 1 Siklus Tanam |
| **Pupuk Abadi Teratai Emas** | Konsentrat Urat Naga + Abu Pil Tier 6 | Memotong waktu tumbuh **90%** & Imun Hama. | Kualitas Murni / Sempurna | 2 Siklus Tanam |

---

## 🐛 3. Hama, Gangguan & Penyakit Tanaman

Pada setiap **3 Turn** sekali saat proses pertumbuhan, AI GM melakukan roll keberuntungan (*Check 1d20*) untuk menentukan apakah petak pertanian diserang gangguan:

| Hasil Roll (1d20) | Jenis Gangguan / Hama | Dampak Jika Dibiarkan | Cara Penanganan / Solusi |
|---|---|---|---|
| **1 – 3** | **Tikus Tanah Qi / Ulat Kayu Spirit** | Menggerogoti tanaman (-50% Hasil Panen / Turn). | Pembasmian Manual (Aksi Turn) / Pasang Perangkap Beast |
| **4 – 6** | **Jamur Pembusuk Akar (Akar Hitam)** | Tanaman mati dalam 2 Turn. | Penyiraman Air Garam Spirit / Aplikasi Pupuk Qi Kayu |
| **7 – 9** | **Kekeringan Qi (Air Lembab Habis)** | Pertumbuhan terhenti (*Stagnant*). | Injeksi Qi Air/Kayu (20 Qi per Petak) |
| **10 – 12** | **Belalang Merah Api** | Menurunkan Kualitas Panen sebesar 1 Grade. | Pengasapan Herbal / Array Pelindung Kebun |
| **13 – 20** | **Aman & Subur** | Tanaman tumbuh optimal tanpa hambatan. | Tidak perlu tindakan khusus. |

---

## 🌾 4. Katalog Tanaman Non-Spiritual (Tumbuhan Fana / Biasa)

Tanaman non-spiritual ditanam di tanah fana (G-0 atau G-1) oleh masyarakat biasa, petani, maupun kultivator yang ingin memproduksi bahan pangan, rempah, dan tekstil. Tanaman ini tidak membutuhkan penyiraman Qi murni, melainkan cukup disiram air biasa secara rutin.

| Nama Tanaman | Waktu Tumbuh | Penyiraman Air | Hasil Panen per Petak | Harga Jual Pasar (Biasa) | Nilai Satiety / Kegunaan Nyata |
|---|---|---|---|---|---|
| **Beras Padi Emas** | 3 Turn | 1x / Turn | 10 Kg Beras | 50 Koin Perunggu / Kg | Bahan Pangan Utama (+20% Satiety per Porsi Nasi) |
| **Gandum Lembah Hijau** | 3 Turn | 1x / Turn | 12 Kg Gandum | 40 Koin Perunggu / Kg | Bahan Roti & Mie (+15% Satiety per Porsi) |
| **Ubi Ungu Gunung** | 2 Turn | 1x / 2 Turn | 15 Kg Ubi | 30 Koin Perunggu / Kg | Makanan Tahan Lama (+25% Satiety per Ubi Rebus) |
| **Bawang Perak Fana** | 2 Turn | 1x / Turn | 5 Kg Bawang | 60 Koin Perunggu / Kg | Bumbu Masak & Dapur, Obat Batuk Ringan (+5 HP) |
| **Sawi Putih Embun** | 1 Turn | 1x / Turn | 8 Kg Sawi | 25 Koin Perunggu / Kg | Sayur Segar (+10% Satiety, Pemulihan Stamina +5) |
| **Cabai Merah Bara** | 2 Turn | 1x / Turn | 4 Kg Cabai | 80 Koin Perunggu / Kg | Bumbu Penghangat Tubuh (Menghilangkan Debuff Cold) |
| **Jahe Hutan Fana** | 3 Turn | 1x / 2 Turn | 6 Kg Jahe | 1 Koin Perak / Kg | Penawar Demam & Mual Ringan, Ramuan Penghangat |
| **Teh Daun Hijau** | 4 Turn | 1x / Turn | 3 Kg Daun Teh | 3 Koin Perak / Kg | Bahan Minuman Teh (+10 Stamina & FOKUS +1) |
| **Kapas Sutra Fana** | 5 Turn | 1x / Turn | 5 Kg Kapas | 2 Koin Perak / Kg | Bahan Baku Pakaian, Kain, Zirah Kain Biasa |
| **Kayu Manis Fana** | 6 Turn | 1x / 2 Turn | 4 Kg Kulit Kayu | 4 Koin Perak / Kg | Rempah Wangi, Pengawet Daging, Komoditas Dagang |

---

## 🌸 5. Katalog Tanaman Spiritual (Tumbuhan Qi & Herba Kultivasi)

Tanaman spiritual memerlukan penyiraman Qi murni dan jenis tanah khusus. Hasil panennya merupakan bahan baku utama Alkimia, pemulihan Qi/HP tingkat lanjut, serta konsumsi spiritual.

### 🟢 Tier 1 — Spiritual Herbs (Ranah Pembersihan Tubuh / Body Refining)

| Nama Tanaman | Waktu Tumbuh | Konsumsi Qi / Turn | Syarat Tanah | Hasil Panen & Kegunaan | Harga Pasar |
|---|---|---|---|---|---|
| **Rumput Embun Jiwa** | 3 Turn | 10 Qi | G-1 / G-2 | Bahan Utama Pil Pemulih Qi Rendah (Tier 1) | 50 Koin Perak |
| **Bunga Ginseng Merah** | 5 Turn | 20 Qi | G-2 (Verdant) | Bahan Pil Pemulih Vitalitas & Darah (Tier 1) | 1 Batu Spiritual Rendah |
| **Jamur Bayang Perak** | 4 Turn | 15 Qi | G-1 (Tepi Gua) | Bahan Pil Penyamar Aura & Racun Lemah | 80 Koin Perak |
| **Bunga Melati Embun** | 3 Turn | 12 Qi | G-1 / G-2 | Bahan Teh Spiritual (+50 Qi & +10% Satiety) | 60 Koin Perak |
| **Akar Serabut Qi** | 4 Turn | 18 Qi | G-2 (Verdant) | Bahan Dasar Salep Pemulih Memar & Luka Otot | 90 Koin Perak |

---

### 🔵 Tier 2 — Spiritual Herbs (Ranah Pengumpulan Qi / Qi Gathering)

| Nama Tanaman | Waktu Tumbuh | Konsumsi Qi / Turn | Syarat Tanah | Hasil Panen & Kegunaan | Harga Pasar |
|---|---|---|---|---|---|
| **Teratai Es Bintang** | 8 Turn | 40 Qi | G-3 (Frost Soil) | Bahan Pil Penawar Burn & Freeze, Pil Suci Es | 5 Batu Spiritual Rendah |
| **Buah Spirit Emas** | 10 Turn | 50 Qi | G-2 (Verdant) | Makanan Spiritual (+100% Satiety & +150 Qi) | 8 Batu Spiritual Rendah |
| **Bunga Giok Hijau** | 7 Turn | 35 Qi | G-2 (Verdant) | Bahan Pil Pembersih Meridian & Racun Tier 2 | 4 Batu Spiritual Rendah |
| **Bambu Petir Ungu** | 9 Turn | 45 Qi | G-5 (Thunder) | Bahan Jimat Petir & Gagang Senjata Tier 2 | 6 Batu Spiritual Rendah |
| **Daun Angin Bintang** | 6 Turn | 30 Qi | G-2 (Verdant) | Bahan Pil Peningkat Kecepatan (Agility Boost) | 3 Batu Spiritual Rendah |

---

### 🟣 Tier 3 — Spiritual Herbs (Ranah Fondasi Jiwa / Foundation Establishment)

| Nama Tanaman | Waktu Tumbuh | Konsumsi Qi / Turn | Syarat Tanah | Hasil Panen & Kegunaan | Harga Pasar |
|---|---|---|---|---|---|
| **Ginseng Lava Vulkanik** | 12 Turn | 60 Qi | G-4 (Lava Soil) | Bahan Utama Pil Breakthrough Fondasi Jiwa / Inti Emas | 25 Batu Spiritual Rendah |
| **Akar Kayu Abadi** | 15 Turn | 80 Qi | G-2 (Verdant) | Bahan Utama Pil Pemulih Organ Dalam & Trauma | 35 Batu Spiritual Rendah |
| **Bunga Roh Rembulan** | 10 Turn | 50 Qi | G-2 (Malam Hari) | Bahan Pil Peningkat Jiwa Spiritual & Meredam Qi Deviation | 20 Batu Spiritual Rendah |
| **Buah Kristal Besi** | 14 Turn | 70 Qi | G-5 (Thunder) | Bahan Pil Tempa Tulang Besi (+Def Murni) | 30 Batu Spiritual Rendah |
| **Rumput Racun Kalajengking**| 11 Turn | 55 Qi | G-1 / G-2 | Bahan Racun Paralis Mematikan Tier 3 | 18 Batu Spiritual Rendah |

---

### 🟠 Tier 4 – Tier 5 — Advanced Spiritual Herbs (Ranah Inti Emas & Jiwa Nascent)

| Nama Tanaman | Tier | Waktu Tumbuh | Konsumsi Qi / Turn | Syarat Tanah | Hasil Panen & Kegunaan | Harga Pasar |
|---|---|---|---|---|---|---|
| **Buah Darah Naga Tanah** | Tier 4 | 20 Turn | 120 Qi | G-2 / G-4 | Bahan Pil Penguat Sumsum Naga (+100 HP Permanent) | 1 Batu Spiritual Menengah |
| **Teratai Jiwa Emas** | Tier 4 | 18 Turn | 100 Qi | G-6 (Holy Soil) | Bahan Pil Breakthrough Inti Emas & Pelindung Jiwa | 80 Batu Spiritual Rendah |
| **Ginseng Ungu Seribu Tahun**| Tier 5 | 30 Turn | 250 Qi | G-6 (Holy Soil) | Bahan Pil Breakthrough Jiwa Nascent & Umur +50 Tahun | 5 Batu Spiritual Menengah |
| **Jamur Es Jiwa Murni** | Tier 5 | 25 Turn | 200 Qi | G-3 (Frost Soil) | Bahan Pil Pembersih Karma Buruk & Penawar Racun Jiwa | 4 Batu Spiritual Menengah |

---

### 🔴 Tier 6 – Tier 9 — Sovereign & Immortal Herbs (Ranah Formasi Roh hingga Huangji Sovereign)

| Nama Tanaman | Tier | Waktu Tumbuh | Konsumsi Qi / Turn | Syarat Tanah | Hasil Panen & Kegunaan | Harga Pasar |
|---|---|---|---|---|---|---|
| **Teratai Sembilan Warna** | Tier 6 | 50 Turn | 500 Qi | G-6 (Holy Soil) | Bahan Utama Pil Rekonstruksi Tubuh Abadi | 20 Batu Spiritual Menengah |
| **Buah Hukum Kehampaan** | Tier 7 | 80 Turn | 1.200 Qi | G-6 (Holy Soil) | Bahan Pil Pemahaman Law Origin (+1 Tier Law) | 2 Batu Spiritual Tinggi |
| **Teratai Tribulasi Surgawi**| Tier 8 | 120 Turn | 3.000 Qi | G-6 (Holy Soil) | Meredam Damage Petir Tribulasi Surgawi sebesar 50% | 10 Batu Spiritual Tinggi |
| **Buah Abadi Huangji** | Tier 9 | 200 Turn | 8.000 Qi | G-6 (Holy Soil) | Bahan Utama Pil Kaisar Abadi (Penguasa Dunia) | Tak Ternilai / Lelang Istana |

---

## 💧 6. Mekanik Penyiraman Qi & Injeksi Elemen

1. **Penyiraman Standar (Qi Murni)**:
   - Pemain menguras poin Qi sesuai angka pada tabel tanaman.
   - Jika Qi tidak disiram dalam 1 Turn, pertumbuhan tanaman tertunda 1 Turn.
   - Jika Qi tidak disiram selama **3 Turn berturut-turut**, tanaman layu dan mati.

2. **Injeksi Elemen Spesifik (Resonansi Elemen)**:
   - Jika elemen Qi pemain cocok dengan elemen alami tanaman (misal: Pemain Elemen Api menyiram *Ginseng Lava Vulkanik*):
     - Waktu tumbuh dipotong **20%**.
     - Kualitas hasil panen meningkat menjadi Grade Unggul (*High Grade*).

---

## 🧺 7. Mekanik Panen & Catatan Log (Item Origin Log)

Saat tanaman mencapai siklus panen penuh:
1. Pemain melakukan tindakan **[Aksi: Memanen Kebun Petak X]**.
2. AI GM menghitung jumlah hasil panen berdasarkan keberadaan pupuk dan kelas tanah.
3. **Pencatatan Wajib**: AI GM mencantumkan entri hasil panen ke dalam profil/inventory pemain dalam format:
   ```text
   [Nama Item] (Grade: [Biasa/Unggul/Murni]) × [Jumlah] | Origin: Hasil Pertanian Petak [X] di [Lokasi] | Timestamp: Tahun X, Bulan Y
   ```

---

## 📝 8. Checklist Validasi AI GM untuk Pertanian

- [ ] Apakah jenis tanah di lokasi tempat menanam mendukung Tier tanaman yang ditanam?
- [ ] Apakah konsumsi Qi / Air penyiraman per Turn telah dipotong dari profil pemain secara akurat?
- [ ] Apakah durasi waktu tumbuh (*Turn*) telah dihitung secara sah tanpa ada skenario skip instan?
- [ ] Apakah roll keberuntungan hama/penyakit (*1d20*) dilakukan setiap 3 Turn?
- [ ] Apakah hasil panen telah dicatat dengan lengkap di **Item Origin Log**?
