# 💰 13. Economy System — Huangji-World

> **Status File**: Modul Utama Sistem Ekonomi & Transaksi
> **Versi**: 3.0 (Huangji Core Edition)
> **Rujukan Silang**: `01_WORLD_OVERVIEW_AND_CAPITAL.md`, `10_ECONOMY_SYSTEM.md` (inggo-alvn reference), `ECONOMY_ORACLE.md`

---

## 🪙 1. Hirarki Mata Uang & Kurs Resmi

Di Benua Huangji, transaksi masyarakat terbagi menjadi dua ranah: **Ranah Fana (Mortal)** dan **Ranah Kultivator**.

### Tabel Konversi Mata Uang
| Mata Uang | Nilai Konversi | Pengguna & Kegunaan |
|---|---|---|
| **Koin Tembaga Fana** | Base Unit (1 Tembaga) | Rakyat biasa, makanan mortal, sewa rumah biasa |
| **Koin Perak Kekaisaran** | 1 Perak = 1.000 Tembaga | Pedagang menengah, pajak kota, penginapan umum |
| **Batu Spiritual Rendah (Low-Grade Spirit Stone)** | 1 Low = 100 Perak = 100.000 Tembaga | Mata uang standar kultivator, transaksi herba biasa |
| **Batu Spiritual Menengah (Mid-Grade Spirit Stone)** | 1 Mid = 100 Low-Grade | Pembelian resep pil, senjata spiritual, sewa kebun |
| **Batu Spiritual Tinggi (High-Grade Spirit Stone)** | 1 High = 100 Mid-Grade | Lelang artefak langka, pembayaran jimat tingkat tinggi |
| **Batu Suci Agung Huangji (Top-Grade Sovereign Stone)** | 1 Top = 100 High-Grade | Perdagangan antar-sekte besar & istana kekaisaran |

---

## 🏷️ 2. Katalog Harga Acuan Komoditas, Barang & Jasa

### A. Penginapan & Konsumsi Spiritual
* **Kamar Penginapan Mortal**: 5 Perak / malam.
* **Penginapan Spiritual Rendah (Pengumpul Qi)**: 2 Batu Spiritual Rendah / malam.
* **Penginapan Spiritual Elit (Inti Emas)**: 1 Batu Spiritual Menengah / malam.
* **Satu Porsi Daging Spirit Beast Rank 1**: 3 Batu Spiritual Rendah (Memulihkan 30% Satiety & +10 Qi).

### B. Herba & Hasil Gardening
* **Benih Rumput Embun Jiwa**: 1 Batu Spiritual Rendah / 5 benih.
* **Benih Bunga Ginseng Merah**: 3 Batu Spiritual Rendah / benih.
* **Pupuk Qi Kayu Murni**: 5 Batu Spiritual Rendah / kantong.
* **Herba Teratai Es Abadi (Matang)**: 5 Batu Spiritual Menengah / tangkai.

### C. Alkimia (Pill & Ramuan)
* **Pill Pemulih Qi Rendah (Tier 1)**: 5 Batu Spiritual Rendah / butir.
* **Pill Penawar Racun Rawa (Tier 1)**: 4 Batu Spiritual Rendah / butir.
* **Pill Pemulih Vitalitas Darah (Tier 2)**: 2 Batu Spiritual Menengah / butir.
* **Pill Breakthrough Inti Emas (Tier 3)**: 10 Batu Spiritual Tinggi / butir.

### D. Tempa & Peralatan
* **Pedang Besi Qi Rendah (Tier 1)**: 20 Batu Spiritual Rendah.
* **Zirah Sisik Ular Besi (Tier 2)**: 3 Batu Spiritual Menengah.
* **Tungku Alkimia Temba Purba (Tier 3)**: 15 Batu Spiritual Menengah.

### E. Jasa Khusus
* **Sewa Kebun Herbal Spiritual (1 Bulan)**: 50 Batu Spiritual Rendah.
* **Jasa Penjinakan Beast oleh Master**: 1 Batu Spiritual Menengah / ekor.
* **Biaya Pengiriman Surat Serikat Dagang**: 1 Batu Spiritual Rendah.

---

## 📜 3. Mekanisme Tawar-Menawar & Pegadaian (Pawnshop)

### Tawar-Menawar (Bargaining Check)
Pemain dapat menawar harga barang di pasar dengan *Persuasion Check* berbasis Wibawa/Insight:
* **Berhasil (Dadu $\ge 12$)**: Diskon harga **15% - 25%**.
* **Gagal (Dadu $< 12$)**: Harga tetap atau pedagang menolak melayani.

### Rumah Gadai (Pawnshop System)
Barang bekas atau jarahan pertarungan dapat dijual ke Rumah Gadai resmi Serikat Dagang Sembilan Bintang:
* **Harga Jual Normal**: **50% dari harga katalog**.
* **Barang Cacat / Rusak**: **25% dari harga katalog**.
