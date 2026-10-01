# 🧪 Huangji-World — Sistem Alkimia, Tempa & Formasi Segel (Crafting System)

> **Modul:** 19 — Alchemy, Forging & Array System
> **Prinsip:** Anti-Cheat Enforced — Material & Recipe Dependent — Terintegrasi dengan Ekonomi & Gardening
> **Rujukan Silang:** `13_ECONOMY_SYSTEM.md`, `17_GARDENING_SYSTEM.md`, `16_BESTIARY.md`

---

## 0. Filosofi Sistem

Setiap proses peracikan Alkimia, penempaan senjata, dan ukiran Formasi Array membutuhkan ketersediaan bahan baku yang sah (tercatat di Item Origin Log) serta tungku/peralatan yang sesuai.

### Aturan Emas Anti-Cheat Crafting
- Pembuat produk wajib memiliki bahan baku yang sah sebelum meracik.
- Peluang keberhasilan dihitung AI GM dari formula tingkat keterampilan.
- Produk hasil crafting WAJIB dicatat di **Item Origin Log** sebelum bisa dijual atau digunakan.

---

## 🧪 1. Sistem Alkimia (Alchemy Crafting)

$$\text{Peluang Berhasil} = 50\% + (\text{Ranah Pemain} \times 10\%) + \text{Bonus Tungku} - (\text{Tier Pill} \times 15\%)$$

### Katalog Resep Pill Utama
| Tier Pill | Nama Pill Alkimia | Resep Bahan Wajib | Efek & Khasiat |
|---|---|---|---|
| **Tier 1** | **Pill Pemulih Qi Rendah** | 2x Rumput Embun Jiwa + 1x Batu Spiritual Rendah | Memulihkan 50 Poin Qi instan |
| **Tier 1** | **Pill Vitalitas Darah** | 2x Bunga Ginseng Merah + 1x Daging Beast | Memulihkan 40 Poin HP instan |
| **Tier 2** | **Pill Penawar Rawa** | 1x Bunga Teratai Hitam + 1x Lendir Katak | Menghentikan efek Poison & Imun 3 Turn |
| **Tier 3** | **Pill Breakthrough Inti Emas** | 1x Ginseng Lava + 1x Teratai Es + 2x Core Tier 3 | Syarat Utama Terobosan Ranah Golden Core |

---

## 🔨 2. Sistem Tempa Senjata & Zirah (Forging System)

* **Pedang Besi Qi Rendah (Tier 1)**: 2x Bijih Besi Tembaga + 1x Batu Spiritual Rendah. (Damage +15).
* **Zirah Sisik Ular Besi (Tier 2)**: 5x Sisik Besi Tembaga + 1x Kulit Serigala. (Defense +25, Imun Cut).

---

## ☯️ 3. Sistem Formasi Segel & Array (Array Creation)

| Nama Formasi Array | Konsumsi Qi & Bahan | Durasi Aktif | Efek Wilayah |
|---|---|---|---|
| **Array Pelindung Kebun** | 30 Qi + 2 Batu Spiritual Rendah | 30 Hari In-Game | Mencegah Hama Serangga & Pencuri mendekati kebun |
| **Array Pengumpul Qi** | 50 Qi + 5 Batu Spiritual Rendah | 7 Hari In-Game | Kecepatan Meditasi & Regenerasi Qi **+25%** |

---

## 4. Checklist Validasi AI GM

- [ ] Bahan baku pembuatan sudah terdaftar di Item Origin Log?
- [ ] Peluang keberhasilan dihitung dari formula resmi?
- [ ] Produk akhir dicatat di Item Origin Log?
