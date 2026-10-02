# 💰 Huangji-World — Sistem Ekonomi & Transaksi (Economy & Pricing System)

> **Modul:** 13 — Economy, Pricing & Valuation System
> **Prinsip:** Anti-Cheat Enforced — Supply-Demand Driven — Terintegrasi dengan Sistem Hukum Kultivasi & World Document
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md` (aturan wajib), `12_CULTIVATION_LAW_SYSTEM.md` (Tier material breakthrough), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (Pusat Pasar Kekaisaran), `19_ALCHEMY_FORGING_ARRAY_SYSTEM.md` (Harga Hasil Crafting), modul wilayah `02`–`10`

---

## 0. Filosofi Sistem

Ekonomi di Benua Huangji digerakkan oleh kelangkaan Batu Spiritual dan material esensi alam semesta. Setiap harga barang, jasa, sewa lahan, hingga transaksi di Rumah Gadai dan Pasar Gelap **wajib tunduk pada Formula Harga Dasar (Final Pricing Formula)**.

**AI GM WAJIB menghitung harga menggunakan formula resmi di bawah ini. AI GM dilarang keras menyetujui klaim harga buatan pemain secara sepihak.**

### Aturan Emas Anti-Cheat Ekonomi
1. **Formula Pricing Mutlak**: Harga barang/jasa ditentukan oleh `FinalPrice(tier, grade, region, demand)`. Roleplay tawar-menawar hanya bisa menggeser harga dalam batas marjin yang diizinkan (maksimal ±15%).
2. **Item Origin Log (Bukti Kepemilikan)**: Setiap barang bernilai (Tier 2/Grade Huang ke atas) **WAJIB** memiliki catatan asal-usul yang sah (hasil berburu, dibeli dari toko resmi, hadiah misi, atau dibuat via crafting). Barang tanpa Item Origin Log dianggap barang haram/curian dan tidak bisa dijual di toko resmi.
3. **Penyimpanan Transaksi Bertimestamp**: Seluruh catatan keuangan (pemasukan/pengeluaran Batu Spiritual) wajib dicantumkan pada blok *Profil Karakter* di setiap turn narasi. Tidak ada retroactive edit (pengubahan catatan keuangan masa lalu).
4. **Kapasitas Stok Toko (Store Stock Floor)**: Toko NPC di wilayah memiliki batas stok harian. Pemain tidak dapat borong barang langka tanpa alasan naratif yang masuk akal.
5. **Hard-Cap Fluktuasi Harga**: Harga barang akibat kelangkaan wilayah atau event darurat dibatasi secara mutlak antara **`0,2×` hingga `5,0×`** dari nilai Grade dasar.

---

## 1. Matriks Mata Uang (Currency Exchange System)

Sistem ekonomi Huangji-World menggunakan hirarki mata uang bertingkat, menghubungkan ekonomi rakyat fana (*Mortal Economy*) hingga transaksi tingkat Kaisar (*Immortal Economy*).

```
1 Koin Perak            = 100 Koin Tembaga
1 Batu Spiritual Rendah  = 100 Koin Perak       = 10.000 Koin Tembaga
1 Batu Spiritual Menengah= 100 Batu Rendah      = 10.000 Koin Perak
1 Batu Spiritual Tinggi  = 100 Batu Menengah    = 10.000 Batu Rendah
1 Batu Suci Huangji      = 100 Batu Tinggi      = 1.000.000 Batu Rendah
```

### 💸 Tabel Hirarki & Kegunaan Mata Uang

| Tingkat | Nama Mata Uang | Nilai Konversi Dasar | Peruntukan & Jangkauan Pasar |
|:---:|---|:---:|---|
| **T1** | **Koin Tembaga Fana** | 1 Unit Base | Makanan rakyat biasa, roti kering, penginapan kelas bawah di desa. |
| **T2** | **Koin Perak Kekaisaran** | 100 Tembaga | Peralatan besi biasa, obat herba pasar desa, sewa kuda, upah pekerja. |
| **T3** | **Batu Spiritual Rendah (Low-Grade)** | 100 Perak | Transaksi dasar kultivator, pil Tier 1–2, herba spiritual, senjata Tier 1. |
| **T4** | **Batu Spiritual Menengah (Mid-Grade)**| 100 Low-Grade | Pil breakthrough Golden Core, senjata Tier 3–4, sewa kebun spiritual. |
| **T5** | **Batu Spiritual Tinggi (High-Grade)** | 100 Mid-Grade | Artefak tingkat Jiwa Nascent, material Tribulasi, lelang ibu kota. |
| **T6** | **Batu Suci Agung Huangji (Top-Grade)**| 100 High-Grade | Pusaka Tingkat Kaisar, transaksi antar-Sekte Elite, upeti Kekaisaran. |

---

## 2. Structure Tier, Grade, & Value Base

Setiap barang dan material di Benua Huangji memiliki **Tier Material** (1–9) dan **Grade Kualitas** (Fan s/d Sheng).

```
TierBase(n) = 5 × 10^(n−1) Koin Tembaga
GradeValue(tier, grade) = TierBase(tier) × GradeMultiplier(grade)
```

---

### 📦 2.1 Tabel Tier Base Value (Harga Floor)

| Tier Material | TierBase (Tembaga) | Konversi Praktis Standar | Contoh Barang / Material Kanon |
|:---:|:---:|:---:|---|
| **Tier 1** | 5 Tembaga | 5 Koin Tembaga | Herba Tempa Otot, Besi Desa, Kulit Serigala Liar. |
| **Tier 2** | 50 Tembaga | 50 Koin Tembaga | Herba Embun Pagi, Pil Pemulihan Qi Dasar, Core Beast T1. |
| **Tier 3** | 500 Tembaga | 5 Koin Perak | Kayu Suci Awan, Pil Fondasi Jiwa, Core Beast T2. |
| **Tier 4** | 5.000 Tembaga | 50 Koin Perak | Pasir Emas Murni, Pil Terobosan Inti Emas, Zirah Besi Tempa. |
| **Tier 5** | 50.000 Tembaga | 5 Batu Spiritual Rendah | Kristal Es Bintang, Pil Jiwa Nascent, Core Beast T4. |
| **Tier 6** | 500.000 Tembaga | 50 Batu Spiritual Rendah | Logam Petir Ungu, Pedang Pusaka Kelas Xuan, Formasi Segel T5. |
| **Tier 7** | 5.000.000 Tembaga | 5 Batu Spiritual Menengah | Mutiara Samudra Purba, Pil Void Transformation, Zirah Naga. |
| **Tier 8** | 50.000.000 Tembaga | 50 Batu Spiritual Menengah | Teratai Api Vulkanik Purba, Jimat Tribulasi Petir. |
| **Tier 9** | 500.000.000 Tembaga | 500 Batu Spiritual Menengah | Esensi Tahta Emas Huangji, Artefak Tingkat Kaisar Abadi. |

---

### 💎 2.2 Tabel Grade Multiplier Kualitas

| Grade Kualitas | Pengali Grade (`GradeMultiplier`) | Ciri Fisik & Kemurnian Barang |
|:---:|:---:|---|
| **Fan-Grade (Kasar)** | **×0,5** | Kualitas cacat, banyak kotoran esensi, daya tahan rendah. |
| **Huang-Grade (Kuning)** | **×1,0** | Kualitas standar pasar umum, kemurnian 60%–70%. |
| **Xuan-Grade (Misterius)**| **×2,5** | Kualitas halus, diproses ahli alkimia/penempa resmi, kemurnian 80%–89%. |
| **Di-Grade (Bumi)** | **×6,0** | Kualitas unggul, memancarkan aura Qi pekat, kemurnian 90%–95%. |
| **Tian-Grade (Langit)** | **×15,0** | Kualitas sempurna, tanpa cacat, kemurnian 99%+. |
| **Sheng-Grade (Suci)** | **×40,0** | Kualitas legendaris, memiliki roh artefak/esensi murni alam. |

---

## 3. Formula Harga Akhir Pasar (Final Pricing Formula)

Harga aktual suatu barang di toko atau pasar bebas dihitung menggunakan formula berikut:

```
FinalPrice = GradeValue(tier, grade) × RegionScarcity × DemandIndex × ConditionModifier
FinalPrice = clamp(hasil_kalkulasi, 0,2 × GradeValue, 5,0 × GradeValue)
```

---

### 🗺️ 3.1 Tabel Region Scarcity Multiplier (Kelangkaan Wilayah)

Harga barang melambung jika dijual jauh dari wilayah asalnya:

| Kategori Lokasi Barang | Multiplier (`RegionScarcity`) | Contoh Kasus Naratif |
|---|:---:|---|
| **Wilayah Asal (Native Region)** | **×0,6** | Membeli Herba Kayu Vitalitas langsung di Dataran Hijau Abadi (`02`). |
| **Wilayah Berdampingan Direct** | **×1,2** | Membeli Herba Kayu Vitalitas di Ibu Kota Huangji (`01`) atau Lembah Api (`04`).|
| **Wilayah Jauh (> 1.500 Li)** | **×2,5** | Membeli Herba Kayu Vitalitas di Gurun Pasir Emas (`07`) atau Danau Es (`05`). |
| **Zona Terisolasi / Ekstrem** | **×4,0** | Membeli Esensi Es Kristal di dalam kawah lahar Lembah Api Merah (`04`). |

---

### 📈 3.2 Tabel Demand & Condition Multiplier

* **Demand Index**:
  * Normal: `×1,0`
  * Tinggi (Masa Perang / Turnamen): `×1,5`
  * Krisis Kelangkaan Ekstrem: `×3,0`
* **Condition Modifier**:
  * Baru / Sempurna: `×1,0`
  * Bekas / Aus: `×0,7`
  * Rusak Parah (Butuh Perbaikan): `×0,3`

---

## 🏛️ 4. Tarif Jasa, Sewa, & Pegadaian (Service & Pawnshop System)

### 🏥 4.1 Tabel Tarif Jasa Layanan Standar

| Jenis Jasa / Layanan | Biaya Standar | Catatan & Penyedia Resmi |
|---|:---:|---|
| **Penginapan Biasa (Kamar Fana)** | 2 Koin Perak / Malam | Penginapan umum di kota/desa. |
| **Kamar Meditasi Qi Pekat** | 1 Batu Spiritual Rendah / Hari | Mengakselerasi regen Qi +50% (Sekte/Kota Besar). |
| **Pengobatan Tabib (Luka Ringan)** | 10 Koin Perak | Memulihkan luka fisik biasa (Balai Tabib Pengembara `37`). |
| **Pengobatan Tabib (Qi Deviation / Organ)**| 50 Batu Spiritual Menengah | Penanganan trauma Dantian oleh Tabib Ahli. |
| **Penyewaan Kebun Spiritual T1** | 5 Batu Spiritual Rendah / Bulan | Lahan tanam herba spiritual (`17_GARDENING_SYSTEM.md`). |
| **Biaya Identifikasi Intel / Berita** | 2–20 Batu Spiritual Rendah | Pembelian informasi di Paviliun Seribu Bisik (`35`). |
| **Kontrak Pembunuhan Bayaran** | 10–500 Batu Spiritual Rendah | Tergantung realm target di Perkumpulan Pisau Sunyi (`33`). |

---

### 🏪 4.2 Sistem Pegadaian & Penjualan Barang (Pawnshop System)

Saat pemain menjual barang ke NPC Toko, Rumah Gadai Giok Sejuk (`36`), atau Pedagang Kaki Lima:

* **Penjualan Barang Sempurna (Item Origin Log Sah)**: NPC membeli seharga **50% dari `FinalPrice`**.
* **Penjualan Barang Cacat / Bekas**: NPC membeli seharga **25% dari `FinalPrice`**.
* **Penjualan Barang Tanpa Origin Log (Gadai Gelap)**: NPC membeli seharga **15% dari `FinalPrice`** (Risiko dilaporkan ke penjaga kota).

---

## 🤝 5. Batas Tawar-Menawar (Bargaining Cap)

Pemain dapat melakukan roleplay tawar-menawar (*bargaining*) dengan NPC pedagang. Batas diskon atau kenaikan harga jual ditentukan oleh sikap NPC:

* **NPC Ramah / Sahabat Faksi**: Maksimal Diskon **−20%**.
* **NPC Netral / Pedagang Pasar**: Maksimal Diskon **−15%**.
* **NPC Kaku / Pelit**: Maksimal Diskon **−5%**.
* **NPC Bermusuhan / Pasar Gelap**: **0% Diskon** (Harga Naik +30%).

---

## 🛡️ 6. Checklist Validasi AI GM (Wajib Diperiksa Setiap Transaksi)

- [ ] Apakah harga barang dihitung memakai `FinalPrice` dengan `GradeValue`, `RegionScarcity`, dan `DemandIndex` yang tepat?
- [ ] Apakah harga berada dalam batas aman clamp `0,2×` hingga `5,0×` dari `GradeValue`?
- [ ] Apakah barang bernilai Tier 2+ yang dijual pemain memiliki **Item Origin Log** yang tervalidasi?
- [ ] Apakah pengurangan atau penambahan Batu Spiritual / Koin Perak sudah dicatat dengan benar di *Profil Karakter*?
- [ ] Apakah batas diskon tawar-menawar tidak melebihi marjin sikap NPC (maksimal −20%)?
