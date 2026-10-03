# 💰 Huangji-World — Sistem Ekonomi & Transaksi (Economy & Pricing System)

> **Modul:** 13 — Economy, Pricing & Valuation System
> **Prinsip:** Anti-Cheat Enforced — Supply-Demand Driven — Terintegrasi dengan Sistem Hukum Kultivasi & World Document
> **Rujukan Utama:** [`INDEX.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/INDEX.md?v=1)
> **Rujukan Silang:**
> - [`00_CORE_RULES_AI_GM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/00_CORE_RULES_AI_GM.md?v=1) (Aturan Wajib AI GM)
> - [`12_CULTIVATION_LAW_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/12_CULTIVATION_LAW_SYSTEM.md?v=1) (Tier Material Breakthrough)
> - [`14_VITALITY_HUNGER_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/14_VITALITY_HUNGER_SYSTEM.md?v=1) (Harga Makanan & Jasa Medis)
> - [`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1) (Nilai Artefak & Durability)
> - [`16_BESTIARY.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/16_BESTIARY.md?v=1) (Nilai Loot & Core Beast)
> - [`19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1) (Harga Hasil Crafting)
> - [`43_PAVILIUN_LELANG_SUCI_HUANGJI.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/43_PAVILIUN_LELANG_SUCI_HUANGJI.md?v=1) (Sistem Lelang)
> - Modul Wilayah `01`–`10` (Kekayaan & Soft-Cap Pasar)

---

## 📜 0. Filosofi & Aturan Emas Ekonomi

Ekonomi di Benua Huangji digerakkan oleh kelangkaan Batu Spiritual, Tael Giok, dan material esensi alam semesta. Setiap harga barang, jasa pengawalan, sewa lahan, pengobatan tabib, hingga transaksi di Rumah Gadai dan Pasar Gelap **wajib tunduk pada Formula Harga Akhir (*Final Pricing Formula*)**.

**AI GM WAJIB menghitung harga menggunakan formula resmi di bawah ini. AI GM dilarang keras menyetujui klaim harga buatan pemain secara sepihak.**

### 🛡️ Aturan Emas Anti-Cheat Ekonomi
1. **Formula Pricing Mutlak**: Harga barang dan jasa ditentukan oleh `FinalPrice(tier, grade, region, demand, event, condition)`. Roleplay tawar-menawar hanya dapat menggeser harga dalam batas marjin yang diizinkan (maksimal $\pm 15\%$).
2. **Item Origin Log (Bukti Kepemilikan)**: Setiap barang bernilai (Tier 2 / Grade Huang ke atas) **WAJIB** memiliki catatan asal-usul yang sah (hasil berburu, dibeli dari toko resmi, hadiah misi, atau dibuat via crafting). Barang tanpa Item Origin Log dianggap barang haram/curian dan dilarang diperjualbelikan di toko resmi.
3. **Penyimpanan Transaksi Bertimestamp**: Seluruh catatan keuangan (pemasukan & pengeluaran Tael/Batu Spiritual) wajib dicantumkan pada blok *Profil Karakter* di setiap turn narasi. Tidak ada retroactive edit (pengubahan catatan keuangan masa lalu).
4. **Kapasitas Stok Toko (Store Stock Floor)**: Toko NPC di setiap wilayah memiliki batas stok harian. Pemain tidak dapat memborong barang langka tanpa alasan naratif yang masuk akal.
5. **Hard-Cap Fluktuasi Harga**: Harga barang akibat kelangkaan wilayah atau event darurat dibatasi secara mutlak antara **$0,2\times$ hingga $5,0\times$** dari nilai Grade dasar.

---

## 🪙 1. Matriks Hirarki Mata Uang (Currency Exchange Hierarchy)

Sistem ekonomi Huangji-World menggunakan hirarki mata uang bertingkat, menghubungkan ekonomi masyarakat fana (*Mortal Economy*) hingga transaksi tingkat Kaisar (*Immortal Economy*). Di atas Tael Perak Kekaisaran, digunakan **Tael Giok Putih** sebagai jembatan sebelum Batu Spiritual:

```text
1 Tael Perak Kekaisaran       = 100 Tael Tembaga Fana
1 Tael Giok Putih Kekaisaran  = 100 Tael Perak Kekaisaran      = 10.000 Tael Tembaga
1 Batu Spiritual Rendah       = 100 Tael Giok Putih Kekaisaran = 1.000.000 Tael Tembaga
1 Batu Spiritual Menengah     = 100 Batu Spiritual Rendah
1 Batu Spiritual Tinggi       = 100 Batu Spiritual Menengah
1 Batu Suci Agung Huangji     = 100 Batu Spiritual Tinggi      = 1.000.000 Batu Rendah
```

### 💸 Tabel Hirarki & Peruntukan Pasar

| Tingkat | Nama Mata Uang | Nilai Konversi Dasar | Peruntukan & Jangkauan Pasar |
|:---:|---|:---:|---|
| **T1** | **Tael Tembaga Fana** | 1 Unit Base | Makanan rakyat biasa, roti kering, penginapan kelas bawah di desa. |
| **T2** | **Tael Perak Kekaisaran** | 100 Tael Tembaga | Peralatan besi biasa, obat herba pasar desa, sewa kuda, upah pekerja. |
| **T3** | **Tael Giok Putih Kekaisaran**| 100 Tael Perak | Bahan herbal berkualitas, peralatan dojo, transaksi pejabat & bangsawan. |
| **T4** | **Batu Spiritual Rendah (*Low*)** | 100 Tael Giok Putih | Transaksi dasar kultivator, pil Tier 1–2, herba spiritual, senjata Tier 1–2. |
| **T5** | **Batu Spiritual Menengah (*Mid*)**| 100 Low-Grade | Pil breakthrough Golden Core, senjata Tier 3–4, sewa kebun spiritual. |
| **T6** | **Batu Spiritual Tinggi (*High*)**| 100 Mid-Grade | Artefak tingkat Jiwa Nascent, material Tribulasi, lelang ibu kota. |
| **T7** | **Batu Suci Agung Huangji (*Top*)**| 100 High-Grade | Pusaka Tingkat Kaisar, transaksi antar-Sekte Elite, upeti Kekaisaran. |

---

## 📦 2. Struktur Tier Base Value & Grade Multiplier

Setiap barang dan material di Benua Huangji memiliki **Tier Material** (1–9) dan **Grade Kualitas** (Fan s/d Sheng).

$$\text{TierBase}(n) = 5 \times 10^{n-1} \text{ Tael Tembaga}$$
$$\text{GradeValue}(\text{Tier}, \text{Grade}) = \text{TierBase}(\text{Tier}) \times \text{GradeMultiplier}(\text{Grade})$$

---

### 📦 2.1 Tabel Tier Base Value (Harga Floor Standar)

| Tier Material | TierBase (Tael Tembaga) | Konversi Praktis Standar | Contoh Barang / Material Kanon |
|:---:|:---:|:---:|---|
| **Tier 1** | 5 Tael Tembaga | 5 Tael Tembaga | Herba Tempa Otot, Besi Desa, Kulit Serigala Liar. |
| **Tier 2** | 50 Tael Tembaga | 50 Tael Tembaga | Herba Embun Pagi, Pil Pemulihan Qi Dasar, Core Beast T1. |
| **Tier 3** | 500 Tael Tembaga | 5 Tael Perak | Kayu Suci Awan, Pil Pemulihan Darah T1, Core Beast T2. |
| **Tier 4** | 5.000 Tael Tembaga | 50 Tael Perak | Pasir Emas Murni, Pil Terobosan Inti Emas, Zirah Besi. |
| **Tier 5** | 50.000 Tael Tembaga | 5 Tael Giok Putih | Kristal Es Bintang, Pil Jiwa Nascent, Core Beast T4. |
| **Tier 6** | 500.000 Tael Tembaga | 50 Tael Giok Putih | Logam Petir Ungu, Pedang Pusaka Kelas Xuan, Formasi Segel T5. |
| **Tier 7** | 5.000.000 Tael Tembaga | 5 Batu Spiritual Rendah | Mutiara Samudra Purba, Pil Void Transformation, Zirah Naga. |
| **Tier 8** | 50.000.000 Tael Tembaga | 50 Batu Spiritual Rendah | Teratai Api Vulkanik Purba, Jimat Tribulasi Petir. |
| **Tier 9** | 500.000.000 Tael Tembaga | 500 Batu Spiritual Rendah | Esensi Tahta Emas Huangji, Artefak Tingkat Kaisar Abadi. |

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

## 🏷️ 3. Formula Harga Akhir Pasar (Final Pricing Formula)

Harga aktual suatu barang di toko NPC atau pasar bebas dihitung menggunakan formula berikut:

$$\text{FinalPrice} = \text{GradeValue}(\text{Tier}, \text{Grade}) \times \text{RegionScarcity} \times \text{DemandIndex} \times \text{EventModifier} \times \text{ConditionModifier}$$
$$\text{FinalPrice} = \text{Clamp}\left(\text{HasilKalkulasi}, 0,2 \times \text{GradeValue}, 5,0 \times \text{GradeValue}\right)$$

---

### 🗺️ 3.1 Tabel Region Scarcity Multiplier (Kelangkaan Wilayah)

Harga barang melambung jika dijual jauh dari wilayah asalnya:

| Kategori Lokasi Barang | Multiplier (`RegionScarcity`) | Contoh Kasus Naratif |
|---|:---:|---|
| **Wilayah Asal (Native Region)** | **×0,6** | Membeli Herba Kayu Vitalitas langsung di Dataran Hijau Abadi ([`02`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/02_VERDANT_QI_PLAINS.md?v=1)). |
| **Wilayah Berdampingan Direct** | **×1,2** | Membeli Herba Kayu Vitalitas di Ibu Kota Huangji ([`01`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/01_WORLD_OVERVIEW_AND_CAPITAL.md?v=1)) atau Lembah Api ([`04`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/04_CRIMSON_BLAZE_VALLEY.md?v=1)).|
| **Wilayah Jauh (> 1.500 Li)** | **×2,5** | Membeli Herba Kayu Vitalitas di Gurun Pasir Emas ([`07`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/07_GOLDEN_SAND_DESERT.md?v=1)) atau Danau Es ([`05`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/05_FROST_STAR_LAKE.md?v=1)). |
| **Zona Terisolasi / Ekstrem** | **×4,0** | Membeli Esensi Es Kristal di dalam kawah lahar Lembah Api Merah ([`04`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/04_CRIMSON_BLAZE_VALLEY.md?v=1)). |

---

### 📈 3.2 Tabel Demand, Event, & Condition Multiplier

- **Demand Index**:
  - Normal: `×1,0`
  - Tinggi (Masa Perang / Turnamen): `×1,5`
  - Krisis Kelangkaan Ekstrem: `×3,0`
- **Event Modifier**:
  - Standar / Tanpa Event: `×1,0`
  - Event Festival / Diskon: `×0,8`
  - Event Darurat Perang / Bencana: `×2,0`
- **Condition Modifier**:
  - Baru / Sempurna: `×1,0`
  - Bekas / Aus: `×0,7`
  - Rusak Parah (Butuh Perbaikan): `×0,3`

---

## 🏛️ 4. Tarif Jasa, Sewa, & Pegadaian (Service & Pawnshop System)

### 🏥 4.1 Tabel Tarif Jasa Layanan Standar

| Jenis Jasa / Layanan | Biaya Standar | Catatan & Penyedia Resmi |
|---|:---:|---|
| **Penginapan Biasa (Kamar Fana)** | 2 Tael Perak / Malam | Penginapan umum di kota/desa. |
| **Kamar Meditasi Qi Pekat** | 1 Tael Giok Putih / Hari | Mengakselerasi regen Qi +50% (Sekte/Kota Besar). |
| **Pengobatan Tabib (Luka Ringan)** | 10 Tael Perak | Memulihkan luka fisik biasa (Balai Tabib Pengembara [`37`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/37_BALAI_TABIB_PENGEMBARA_HUANGJI.md?v=1)). |
| **Pengobatan Tabib (Qi Deviation / Organ)**| 50 Batu Spiritual Rendah | Penanganan trauma Dantian oleh Tabib Ahli. |
| **Penyewaan Kebun Spiritual T1** | 5 Tael Giok Putih / Bulan | Lahan tanam herba spiritual ([`17_GARDENING_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/17_GARDENING_SYSTEM.md?v=1)). |
| **Biaya Identifikasi Intel / Berita** | 2–20 Tael Giok Putih | Pembelian informasi di Paviliun Seribu Bisik ([`35`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/35_PAVILIUN_SERIBU_BISIK.md?v=1)). |
| **Kontrak Pembunuhan Bayaran** | 10–500 Batu Spiritual Rendah | Tergantung realm target di Perkumpulan Pisau Sunyi ([`33`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/33_PERKUMPULAN_PISAU_SUNYI_HUANGJI.md?v=1)). |

---

### 🏪 4.2 Sistem Pegadaian & Penjualan Barang (Pawnshop System)

Saat pemain menjual barang ke NPC Toko, Rumah Gadai Giok Sejuk ([`36_RUMAH_GADAI_GIOK_SEJUK.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/36_RUMAH_GADAI_GIOK_SEJUK.md?v=1)), atau Pedagang Kaki Lima:

- **Penjualan Barang Sempurna (Item Origin Log Sah)**: NPC membeli seharga **50% dari `FinalPrice`**.
- **Penjualan Barang Cacat / Bekas**: NPC membeli seharga **25% dari `FinalPrice`**.
- **Penjualan Barang Tanpa Origin Log (Gadai Gelap)**: NPC membeli seharga **15% dari `FinalPrice`** (Risiko dilaporkan ke penjaga kota).

---

## 🤝 5. Batas Tawar-Menawar (Bargaining Cap)

Pemain dapat melakukan roleplay tawar-menawar (*bargaining*) dengan NPC pedagang. Batas diskon atau kenaikan harga jual ditentukan oleh sikap NPC:

- **NPC Ramah / Sahabat Faksi**: Maksimal Diskon **-20%**.
- **NPC Netral / Pedagang Pasar**: Maksimal Diskon **-15%**.
- **NPC Kaku / Pelit**: Maksimal Diskon **-5%**.
- **NPC Bermusuhan / Pasar Gelap**: **0% Diskon** (Harga Naik +30%).

---

## 📜 6. Sistem Item Origin Log & Transaksi (Ledger Rules)

Setiap barang bernilai Tier 2 / Grade Huang ke atas WAJIB dicatat pada **Item Origin Log** di sheet karakter sebelum dapat ditransaksikan atau digunakan untuk breakthrough:

```text
[Item Origin Log — Transaksi Pasar]
- Nama Barang: Pil Pemulihan Darah T2 (Grade: Xuan) ×1
- Sumber: Dibeli di Rumah Gadai Giok Sejuk (Ibu Kota Huangji)
- Biaya: 25 Tael Giok Putih
- Timestamp: Tahun 1, Bulan 4, Hari 10
```

---

## 🗺️ 7. Integrasi 10 Wilayah & Soft-Cap Kekayaan Regional

Setiap wilayah geografis di Benua Huangji memiliki kapasitas likuiditas pasar (*Regional Wealth Soft-Cap*):

| Wilayah Geografis | Kekayaan Regional Soft-Cap | Karakteristik Pasar & Komoditas Utama |
|:---|:---:|:---|
| **01. Ibu Kota Agung Huangji** | **± 950 Juta Tael** | Pusat lelang kekaisaran, likuiditas tertinggi, barang mewah. |
| **02. Dataran Hijau Abadi** | **± 380 Juta Tael** | Pasar herba spiritual, hasil panen pertanian, kayu jati purba. |
| **03. Pegunungan Petir Guntur**| **± 290 Juta Tael** | Tambang bijih tembaga, besi, dan logam petir ungu. |
| **04. Lembah Api Merah** | **± 310 Juta Tael** | Pasar tungku alkimia, batu obsidian panas, dan bahan peluncur lahar. |
| **05. Danau Es Bintang** | **± 250 Juta Tael** | Komoditas ikan perak es, kristal bintang, dan sutra pembeku. |
| **06. Tanah Gersang Tulang** | **± 180 Juta Tael** | Pasar gelap bahan rangka, kristal jiwa, dan senjata kuno. |
| **07. Gurun Pasir Emas** | **± 150 Juta Tael** | Komoditas kurma emas, kulit cacing pasir, dan oasis jualan. |
| **08. Rawa Kabut Racun** | **± 210 Juta Tael** | Komoditas racun miasma, lendir katak, dan penawar racun. |
| **09. Puncak Langit Surgawi** | **± 270 Juta Tael** | Bulu elang surgawi, batu angin, dan jimat pergerakan. |
| **10. Kepulauan Palung Samudra**| **± 410 Juta Tael** | Mutiara air murni, sirip hiu purba, dan minyak laut dalam. |

---

## 🛡️ 8. Checklist Validasi & Anti-Cheat AI GM

Sebelum mengesahkan transaksi ekonomi, jual-beli, atau tawar-menawar, AI GM **wajib** memeriksa checklist berikut:

- [ ] Apakah harga barang dihitung menggunakan `FinalPrice` dengan `GradeValue`, `RegionScarcity`, dan `DemandIndex` yang tepat?
- [ ] Apakah harga berada dalam batas clamp aman $0,2\times$ hingga $5,0\times$ dari `GradeValue`?
- [ ] Apakah barang bernilai Tier 2+ yang dijual pemain memiliki **Item Origin Log** yang tervalidasi?
- [ ] Apakah pengeluaran dan pemasukan Tael / Batu Spiritual telah dicatat secara akurat di sheet *Profil Karakter*?
- [ ] Apakah batas diskon tawar-menawar tidak melampaui marjin sikap NPC (maksimal -20%)?
- [ ] Apakah konversi mata uang mengikuti hirarki resmi (Tael Tembaga $\rightarrow$ Tael Perak $\rightarrow$ Tael Giok Putih $\rightarrow$ Batu Spiritual Rendah)?
