# 💰 Huangji-World — Sistem Ekonomi & Transaksi (Economy & Pricing System)

> **Modul:** 13 — Economy System
> **Prinsip:** Anti-Cheat Enforced — Supply-Demand Driven — Terintegrasi dengan Sistem Hukum Kultivasi & World Document
> **Rujukan Silang:** `12_CULTIVATION_LAW_SYSTEM.md` (Tier material breakthrough), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (jarak wilayah), modul wilayah `02`–`10`

---

## 0. Filosofi Sistem

Setiap harga di dunia ini — barang, jasa, aset — tunduk pada satu **Formula Harga Dasar** yang sama. AI GM WAJIB menghitung harga lewat formula di bawah ini, bukan menerima klaim harga dari player secara sembarangan.

### Aturan Emas Anti-Cheat Ekonomi
- Harga TIDAK BOLEH dideklarasikan sepihak oleh player — semua harga dihitung AI GM lewat formula.
- Setiap barang bernilai (Tier 3+ atau Grade Xuan ke atas) WAJIB punya **Item Origin Log** — asal-usul tervalidasi. Tanpa origin, barang tidak bisa dijual/ditukar/dipakai breakthrough.
- Tidak ada retroactive price edit — semua transaksi bertimestamp, tidak bisa diubah mundur setelah disepakati.
- Stok toko/NPC terbatas sesuai kapasitas produksi wilayah — tidak bisa membeli borongan barang Tier tinggi tanpa alasan naratif kuat.
- Tawar-menawar dibatasi ±15% dari harga hasil formula, tidak bisa lebih meski roleplay meyakinkan.
- Fluktuasi harga akibat supply-demand dibatasi hard cap 0,2×–5,0× dari Grade Value dasar.

---

## 1. Mata Uang (Currency)

| Tingkat | Nama | Nilai Tukar | Kegunaan |
|---|---|---|---|
| 1 | Koin Tembaga Fana | 1 (satuan dasar) | Makanan, penginapan murah rakyat biasa |
| 2 | Koin Perak Kekaisaran | 100 Tembaga | Transaksi umum kota, upah jasa biasa |
| 3 | Batu Spiritual Rendah (Low) | 100 Perak (10.000 Tembaga) | Transaksi umum kultivator, pil dasar |
| 4 | Batu Spiritual Menengah (Mid) | 100 Low-Grade | Transaksi sekte, sewa kebun spiritual |
| 5 | Batu Spiritual Tinggi (High) | 100 Mid-Grade | Lelang artefak langka & jimat tinggi |
| 6 | Batu Suci Agung Huangji (Top) | 100 High-Grade | Transaksi kekaisaran & sekte elite |

---

## 2. Struktur Tier & Grade Barang

### 2.1 Tier Barang
```
TierBase(n) = 5 × 10^(n−1) Koin Tembaga
```

| Tier | TierBase (Tembaga) | Konversi Praktis | Contoh Barang |
|---|---|---|---|
| 1 | 5 | 5 Tembaga | Ramuan herbal biasa, besi desa |
| 2 | 50 | 50 Tembaga | Pil pemulih qi ringan, pedang besi |
| 3 | 500 | 5 Perak | Pil penyembuh luka dalam, pedang bermutu |
| 4 | 5.000 | 50 Perak | Pil terobosan Foundation, senjata bertuah |
| 5 | 50.000 | 50 Batu Rendah | Pil terobosan Golden Core, pusaka bertuah |
| 6 | 500.000 | 500 Batu Rendah | Pil terobosan Nascent Soul, senjata pusaka |
| 7 | 5.000.000 | 5 Batu Menengah | Pil terobosan Void Transformation |
| 8 | 50.000.000 | 50 Batu Menengah | Bahan Tribulasi Realm 8, pusaka mitos |
| 9 | 500.000.000 | 500 Batu Menengah | Bahan Realm 9, artefak dewa |

### 2.2 Grade Kualitas
```
GradeValue(tier, grade) = TierBase(tier) × GradeMultiplier(grade)
```
Grade Multipliers: Fan-Grade (×0,5) | Huang-Grade (×1,0) | Xuan-Grade (×2,5) | Di-Grade (×6,0) | Tian-Grade (×15,0) | Sheng-Grade (×40,0)

---

## 3. Formula Suplai & Permintaan (Supply-Demand Formula)

```
FinalPrice = GradeValue(tier, grade) × RegionScarcity × DemandIndex × EventModifier × ConditionModifier
FinalPrice = clamp(hasil di atas, 0,2 × GradeValue, 5,0 × GradeValue)
```

RegionScarcity: Native Region (×0,6) | Tetangga Direct (×1,5) | Wilayah Jauh >1.500 li (×3,0) | Zona Sangat Langka (×5,0)

---

## 4. Harga Jasa & Pegadaian

* **Jasa Pengobatan**: 10 Perak (luka ringan) hingga 50 Batu Menengah (Qi Deviation).
* **Rumah Gadai (Pawnshop)**: Barang Sempurna dijual **50% dari FinalPrice**, Rusak **25%**.
* **Tawar-menawar**: NPC ramah (±20%), netral (±15%), kaku (±5%), harga mati (0%).

---

## 5. Checklist Validasi AI GM

- [ ] Harga dihitung lewat formula `FinalPrice` (bukan klaim sepihak player)?
- [ ] Item Origin Log barang yang diperjualbelikan sudah tervalidasi?
- [ ] Region Scarcity dihitung sesuai jarak wilayah di World Document?
- [ ] Harga akhir berada dalam batas clamp 0,2×–5,0× Grade Value?
- [ ] Transaksi tercatat di ledger dengan timestamp?
