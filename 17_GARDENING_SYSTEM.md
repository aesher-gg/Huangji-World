# 🌱 Huangji-World — Sistem Pertanian Spiritual (Gardening System)

> **Modul:** 17 — Gardening System
> **Prinsip:** Anti-Cheat Enforced — Time & Qi Irrigation Dependent — Terintegrasi dengan Alkimia & Ekonomi
> **Rujukan Silang:** `02_VERDANT_QI_PLAINS.md`, `13_ECONOMY_SYSTEM.md`, `19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`

---

## 0. Filosofi Sistem

Bercocok tanam herba spiritual di Benua Huangji membutuhkan pengelolaan nutrisi tanah, penyiraman Qi secara rutin, dan perlindungan dari hama. Hasil panen tidak dapat didapatkan secara instan tanpa proses giliran yang sah.

### Aturan Emas Anti-Cheat Gardening
- Tanaman tidak dapat dipanen secara instan tanpa melewati waktu tunggu Turn yang ditentukan.
- Setiap penyiraman membutuhkan konsumsi Qi murni yang dicatat di log karakter.
- Hasil panen herba WAJIB dicatat di **Item Origin Log** sebelum bisa diracik menjadi pil Alkimia atau dijual.

---

## 🪴 1. Tahapan Pertanian Spiritual (5 Steps)

1. **Kualitas Tanah (Soil Grade)**:
   - *Tanah Biasa*: Tumbuh normal (1x).
   - *Tanah Qi Kayu Murni (Verdant Soil)*: Tumbuh **2x lebih cepat**, kualitas +1 Tier.
2. **Penanaman Benih (Seeding)**: Benih dibeli dari pasar atau ditemukan di hutan.
3. **Penyiraman & Injeksi Qi (Qi Irrigation)**: Injeksi 10–50 Qi per turn untuk menjaga nutrisi.
4. **Pupuk Spiritual (Spiritual Fertilizer)**:
   - *Pupuk Qi Kayu Rendah*: Memotong waktu tumbuh **2 Turn**.
   - *Pupuk Abadi Teratai Emas*: Memotong waktu tumbuh **50%** & imun hama.
5. **Penanganan Hama (Pest Control)**: Peluang 15% diserang Tikus Tanah Qi / Hama Serangga setiap 3 Turn.

---

## 🌸 2. Katalog Tanaman Spiritual Utama

| Nama Tanaman | Waktu Tumbuh (Turn) | Konsumsi Qi / Turn | Syarat Tanah | Hasil Panen & Kegunaan |
|---|---|---|---|---|
| **Rumput Embun Jiwa** | 3 Turn | 10 Qi | Biasa / Verdant | Bahan Utama Pill Pemulih Qi Rendah (Tier 1) |
| **Bunga Ginseng Merah** | 5 Turn | 20 Qi | Verdant Soil | Bahan Pill Pemulih Vitalitas & Darah (Tier 1) |
| **Teratai Es Bintang** | 8 Turn | 40 Qi | Cold Soil | Bahan Pill Penawar Burn & Freeze (Tier 2) |
| **Buah Spirit Emas** | 10 Turn | 50 Qi | Verdant Soil | Makanan Spiritual (+100% Satiety & +150 Qi) |
| **Ginseng Lava Vulkanik** | 12 Turn | 60 Qi | Volcanic Soil | Bahan Utama Pill Breakthrough Inti Emas (Tier 3) |
| **Akar Kayu Abadi** | 15 Turn | 80 Qi | Verdant Soil | Bahan Utama Pill Pemulih Organ Dalam (Tier 3) |

---

## 3. Checklist Validasi AI GM

- [ ] Waktu tumbuh tanaman dihitung sesuai Turn yang berlalu?
- [ ] Konsumsi Qi penyiraman dicatat di log karakter?
- [ ] Hasil panen terdaftar di Item Origin Log sebelum diracik?
