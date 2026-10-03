# 🧪 Huangji-World — Sistem Alkimia, Tempa & Formasi Segel (Crafting System)

> **Modul:** 19 — Alchemy, Forging & Array System
> **Prinsip:** Anti-Cheat Enforced — Material & Recipe Dependent — Terintegrasi dengan Ekonomi, Gardening, & Bestiary
> **Rujukan Silang:** `13_ECONOMY_SYSTEM.md`, `17_GARDENING_SYSTEM.md`, `16_BESTIARY.md`, `12_CULTIVATION_LAW_SYSTEM.md`

---

## 0. Filosofi & Aturan Emas Crafting

Di Benua Huangji, pembuatan pil alkimia, penempaan senjata spiritual, dan pengukiran formasi segel (*Array Matrices*) adalah tiga profesi sekunder utama (*Support Professions*) yang menentukan kejayaan seorang kultivator maupun sekte. Setiap proses peracikan membutuhkan ketersediaan bahan baku yang sah (tercatat di **Item Origin Log**), peralatan/tungku yang sesuai, serta eksekusi manipulasi api/Qi secara presisi.

### 📜 Aturan Emas Anti-Cheat Crafting
1. **Verifikasi Bahan Baku (Item Origin Log Check)**: Pemain **WAJIB** memiliki bahan baku yang sah di inventory-nya sebelum memulai proses peracikan. Tidak ada pembuatan barang dari udara hampa.
2. **Resiko Ledakan Tungku (Cauldron Explosion)**: Kegagalan kritis (*Critical Failure*) saat meracik pil alkimia atau memformulasikan array memicu ledakan energi — memberikan Damage Fisik/Api sebesar 25% HP Max pada pengerajin dan menghancurkan seluruh bahan baku.
3. **Pencatatan Produk Akhir**: Seluruh hasil produksi (Pil, Senjata, Zirah, atau Bendera Array) WAJIB dicatat di **Item Origin Log** (`[Nama Produk | Grade/Kualitas | Pembuat: Nama Character | Timestamp]`) sebelum dapat digunakan, dipakai, atau dijual di pasar.

---

## 🧪 1. Sistem Alkimia (Alchemy Crafting System)

Alkimia adalah seni mengintegrasikan herba spiritual, inti beast, dan energi elemen bumi ke dalam wujud pil kental yang padat nutrisi dan Qi.

### 🔥 Tingkatan Tungku Alkimia (Cauldron Grades)

| Cauldron Grade | Nama Tungku Alkimia | Bahan / Asal-Usul | Bonus Peluang Sukses | Pengurangan Resiko Ledakan | Harga Pasar |
|---|---|---|---|---|---|
| **C-1** | **Tungku Tembikar Fana** | Tanah Liat Biasa | +0% | -0% | 100 Koin Perak |
| **C-2** | **Tungku Besi Qi Murni** | Besi Tempa + Serbuk Batu Spirit | +10% | -5% | 10 Batu Spiritual Rendah |
| **C-3** | **Tungku Perunggu Esens Jiwa** | Perunggu Kuno + Urat Api Vulkanik | +20% | -10% | 50 Batu Spiritual Rendah |
| **C-4** | **Tungku Api Giok Naga** | Giok Abadi + Inti Beast Tier 4 | +30% | -20% | 5 Batu Spiritual Menengah |
| **C-5** | **Tungku Suci Huangji Sovereign** | Logam Abadi + Nyala Api Jiwa Naga | +50% | -35% (Imun Ledakan T1-T4) | 50 Batu Spiritual Menengah / Artifact |

---

### 🎲 Formula Kalkulasi Sukses Alkimia & Purity Roll

Saat peracikan dimulai, AI GM melakukan kalkulasi berdasarkan formula:

$$\text{Peluang Berhasil (\%)} = 40\% + (\text{Ranah Pemain} \times 10\%) + \text{BonusTungku} + \text{BonusApiSpesial} - (\text{Tier Pil} \times 15\%)$$

* **Tingkat Kemurnian Pil (Purity Level)** (*1d100 Roll jika Sukses*):
  - **1 – 40 (Low Grade / Kotor)**: Efek Pil 70%, Menimbulkan +5% Impurity Toxicity pada Meridian.
  - **41 – 80 (Mid Grade / Standar)**: Efek Pil 100%, Efek samping normal.
  - **81 – 98 (High Grade / Murni)**: Efek Pil 130%, Tanpa Efek Samping (+0% Impurity).
  - **99 – 100 (Perfect / Pills Pattern / Pola Awan)**: Efek Pil **200%**, Memberikan Buff Permanen +10 Qi Cap.

---

### 📜 Katalog Resep Pil Alkimia Utama (Tiers 1 – 9)

| Tier Pil | Nama Pil Alkimia | Resep Bahan Wajib (Item Origin) | Efek Utama & Khasiat Nyata | Harga Pasar |
|---|---|---|---|---|
| **Tier 1** | **Pil Pemulih Qi Rendah** | 2x Rumput Embun Jiwa + 1x Batu Spirit Rendah | Memulihkan **50 Poin Qi** instan. | 1 Batu Spiritual Rendah |
| **Tier 1** | **Pil Vitalitas Darah** | 2x Bunga Ginseng Merah + 1x Daging Beast T1 | Memulihkan **40 Poin HP** instan. | 1 Batu Spiritual Rendah |
| **Tier 2** | **Pil Penawar Rawa Racun** | 1x Bunga Teratai Hitam + 1x Lendir Katak Racun | Menghentikan efek Poison & Imun Racun selama 3 Turn. | 4 Batu Spiritual Rendah |
| **Tier 2** | **Pil Es Bintang Penenang** | 2x Teratai Es Bintang + 1x Air Murni | Menghilangkan Debuff Burn & Meredam Qi Deviation -20. | 5 Batu Spiritual Rendah |
| **Tier 3** | **Pil Terobosan Inti Emas** | 1x Ginseng Lava + 1x Teratai Es + 2x Core T3 | Syarat Utama Terobosan ke Ranah Golden Core (+30% Success).| 30 Batu Spiritual Rendah |
| **Tier 3** | **Pil Tempa Tulang Besi** | 2x Buah Kristal Besi + 1x Darah Beast T3 | Meningkatkan Defense Murni +25 selama 10 Turn. | 25 Batu Spiritual Rendah |
| **Tier 4** | **Pil Jiwa Nascent Abadi** | 1x Teratai Jiwa Emas + 1x Buah Darah Naga T4 | Syarat Terobosan ke Ranah Nascent Soul (+25% Success). | 2 Batu Spiritual Menengah |
| **Tier 5** | **Pil Seribu Tahun Umur** | 1x Ginseng Ungu Seribu Tahun + 1x Core T5 | Memperpanjang Umur Karakter +50 Tahun In-Game. | 10 Batu Spiritual Menengah |
| **Tier 6 – 9**| **Pil Kaisar Abadi Huangji** | 1x Buah Abadi Huangji + 1x Esens Dragon Vein | Memulihkan seluruh HP/Qi & Syarat Terobosan Sovereign. | Tak Ternilai / Lelang Istana |

---

## 🔨 2. Sistem Tempa Senjata & Zirah (Forging System)

Penempaan adalah proses mengolah bijih logam, kristal mineral, dan bagian tubuh Spirit Beast (tulang, sisik, tanduk) menjadi peralatan tempur bernilai tinggi.

### ⚒️ Bahan Baku Bijih & Logam Tempa

| Grade Logam | Nama Bijih Mineral | Lokasi Tambang Utama | Digunakan Untuk | Price / Kg |
|---|---|---|---|---|
| **M-1** | **Besi Besi Tembaga Fana** | Tambang Dataran Lembah | Senjata & Zirah Tier 1 | 50 Koin Perak |
| **M-2** | **Baja Qi Kayu Murni** | Verdant Qi Plains | Senjata & Zirah Tier 2 | 3 Batu Spiritual Rendah |
| **M-3** | **Perak Es Bintang** | Pegunungan Es Bintang | Senjata Fleksibel & Zirah Ringan Tier 3 | 15 Batu Spiritual Rendah |
| **M-4** | **Tembaga Merah Lava** | Crimson Blaze Peaks | Senjata Elemen Api Tier 4 | 1 Batu Spiritual Menengah |
| **M-5** | **Besi Petir Ungu** | Thunder Crest Mountains | Senjata Konduktor Petir Tier 5 | 5 Batu Spiritual Menengah |
| **M-6** | **Emas Abadi Sovereign** | Puncak Surgawi | Artifact Imperial & Zirah Abadi Tier 6–9 | 50 Batu Spiritual Menengah |

---

### 🗡️ Recipe Tempa Peralatan Utama

1. **Pedang Besi Qi Rendah (Tier 1)**:
   - *Bahan*: 2x Besi Tembaga + 1x Batu Spiritual Rendah.
   - *Stat*: Damage Fisik +15, Ketahanan (*Durability*) 100/100.
2. **Zirah Sisik Ular Besi (Tier 2)**:
   - *Bahan*: 5x Sisik Ular Besi + 2x Leather Serigala + 2x Batu Spiritual Rendah.
   - *Stat*: Defense +25, Imun Efek *Cut/Bleed* dari serangan fisik Tier 1.
3. **Tombak Petir Ungu (Tier 3)**:
   - *Bahan*: 3x Besi Petir Ungu + 1x Tanduk Beast Petir T3 + 10x Batu Spiritual Rendah.
   - *Stat*: Damage Fisik +60, +20 Damage Elemen Petir (Peluang 25% Paralysis 1 Turn).
4. **Perisai Abu Vulkanik (Tier 4)**:
   - *Bahan*: 4x Tembaga Merah Lava + 1x Tempurung Penyu Vulkanik T4.
   - *Stat*: Defense +120, Memantulkan 20% Damage Api kembali ke penyerang.

---

## ☯️ 3. Sistem Formasi Segel & Array (Array Creation System)

Formasi Segel (*Array*) adalah penyusunan garis geometri spiritual menggunakan Bendera Segel (*Array Flags*) dan Batu Spiritual untuk mengendalikan energi alam di suatu wilayah.

### 🚩 Komponen Penyusun Array
- **Bendera Segel (Array Flags)**: Dibuat dari kain sutra spiritual dan tinta esens beast.
- **Batu Penggerak (Core Energy)**: Membutuhkan Batu Spiritual sebagai bahan bakar aktif.

---

### 🌌 Katalog Formasi Array Utama

| Nama Formasi Array | Konsumsi Bahan & Qi | Durasi Aktif | Jangkauan Area | Efek Wilayah & Mekanik Khusus |
|---|---|---|---|---|
| **Array Pelindung Kebun** | 30 Qi + 2 Batu Spirit Rendah + 4x Bendera Kayu | 30 Hari In-Game | 1 Petak Kebun | Mencegah serangan hama serangga & pencuri (Hama Roll Imun). |
| **Array Pengumpul Qi** | 50 Qi + 5 Batu Spirit Rendah + 4x Bendera Giok | 7 Hari In-Game | Ruang Meditasi | Kecepatan Regenerasi Qi **+25%** & Meditasi EXP +20%. |
| **Array Ilusi Bayangan Malam**| 80 Qi + 10 Batu Spirit Rendah + 6x Bendera Bayang| 3 Hari In-Game | Lingkup 15 Meter | Menyembunyikan keberadaan kamp/pemain dari penglihatan NPC/Beast. |
| **Array Jebakan Petir Ungu**| 120 Qi + 20 Batu Spirit Rendah + 8x Bendera Petir| 1x Pakai (Trigger) | Lingkup 10 Meter | Memicu 150 Damage Elemen Petir & Stun 2 Turn pada musuh yang melangkah. |
| **Array Pertahanan Istana**| 500 Qi + 2 Batu Spirit Menengah + 12x Bendera Emas| 30 Hari In-Game | Seluruh Kompleks | Menghasilkan Qi Barrier sebesar **1.000 Point HP** melingkupi area. |

---

## 📝 4. Checklist Validasi AI GM untuk Crafting

- [ ] Apakah seluruh bahan baku yang dibutuhkan terverifikasi ada di **Item Origin Log** / Inventory pemain?
- [ ] Apakah kelas tungku / tempat penempaan / bendera array sesuai dengan syarat resep?
- [ ] Apakah kalkulasi rumus peluang sukses dan roll purity / kegagalan dicantumkan secara terbuka?
- [ ] Jika terjadi kegagalan kritis, apakah resiko ledakan tungku (*Cauldron Explosion*) diterapkan?
- [ ] Apakah produk akhir hasil produksi telah dicatat dengan lengkap di **Item Origin Log**?
