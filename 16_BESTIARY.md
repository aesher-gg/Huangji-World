# 🐉 Huangji-World — Bestiary & Katalog Spesies Spirit (Monster, Spirit Beast, Sprite & Apex Guardians)

> **Modul:** 16 — Bestiary & Monster System
> **Prinsip:** Anti-Cheat Enforced — Habitat-Locked — Terintegrasi dengan Sistem HP, Combat, Taming, & Item Origin Log
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md` (aturan wajib), `12_CULTIVATION_LAW_SYSTEM.md` (Tingkat Ranah), `13_ECONOMY_SYSTEM.md` (Nilai Loot/Core), `15_COMBAT_SYSTEM.md` (Damage Formula), `18_TAMING_SYSTEM.md` (Penjinakan)

---

## 0. Filosofi Sistem

Dunia Huangji dihuni oleh berbagai bentuk kehidupan spiritual — mulai dari **Binatang Wild / Spirit Beast**, **Roh/Peri Esensi (*Sprite / Fairy / Spirit Manifestation*)**, hingga **Penjaga Purba Lintas Wilayah (*Apex Guardian Beasts*)**.

Setiap makhluk memiliki habitat resmi, batas stat fisik, peluang kemunculan (*Ambush Rate*), dan formula drop loot yang wajib divalidasi oleh AI GM. **Pemain dilarang mendatangkan monster di luar habitat resminya atau mengklaim loot tanpa mengalahkan monster tersebut dalam pertarungan naratif.**

### Aturan Emas Anti-Cheat Bestiary
1. **Statistik Terikat Formula**: HP dan Attack Power monster dihitung dari formula berbasis QiCap ranah setaranya.
2. **Kemunculan Berbasis Dadu GM**: Ambush dan kemunculan monster liar dipicu oleh `AmbushChance` yang dihitung oleh AI GM sesuai wilayah dan waktu.
3. **Loot Log Validation**: Loot hanya dianggap sah menjadi milik pemain setelah pertempuran selesai dan dicatat di *Item Origin Log* pada blok Profil Karakter.
4. **Sprite & Spirit Non-Fisik**: Roh Esensi (*Sprite*) membutuhkan teknik Jiwa atau Senjata Elemen untuk diserang (imun serangan fisik murni).

---

## 🎲 1. Formula Ambush & Formasi Encounter

```
AmbushChance = BaseChance (5%) × DangerModifier × TimeModifier × NoiseModifier
```

### 📊 Tabel Modifier Kemunculan Monster

| Faktor Lingkungan | Kategori Lingkungan / Kondisi | Modifier (`DangerModifier`) |
|---|---|:---:|
| **Area Pemukiman / Kota** | Dalam Ibu Kota Huangji / Kota Sekte Utama | **×0,1** (Hanya Beast Peliharaan) |
| **Jalan Utama / Jalur Dagang** | Jalur Kuda & Pos Penjagaan Kekaisaran | **×0,5** |
| **Hutan / Pegunungan Normal** | Pinggiran Hutan Kayu / Bukit Rendah | **×1,0** |
| **Zona Liar / Rawa / Gurun** | Hutan Purba / Rawa Kabut Miasma / Gurun Pasir | **×2,0** |
| **Zona Terlarang / Kawah Lahar**| Lembah Api Vulkanik / Kawah Lahar / Palung Laut | **×4,0** |

*Time & Noise Multiplier:*
- Siang Hari: `×1,0` | Malam Hari: `×2,0`
- Perjalanan Senyap (Stealth Check Berhasil): `×0,5` | Membuat Suara Bising / Pendarahan Luka: `×2,5`

---

## 💎 2. Sistem Drop Loot & Rarity Rate

```
LootDropRate = BaseDropRate(Rarity) × LuckModifier
```

| Tingkat Rarity | Base Drop Rate | Jenis Barang Drop & Material Kanon |
|:---:|:---:|---|
| **Umum (Common)** | **70% – 90%** | Daging spirit, kulit kasar, sisik biasa, taring, tulang, bulu unggas. |
| **Jarang (Rare)** | **20% – 40%** | Core Beast Tier 1–4, kelenjar racun murni, bulu kilat, darah segar. |
| **Langka (Epic)** | **5% – 15%** | Core Beast Tier 5–6, tanduk giok, esensi elemen murni, Kristal Roh. |
| **Legendaris (Apex / Boss)**| **100% (First Kill)** | Core Beast Tier 7–8, Sisik Naga, Esensi Roh Purba, Artefak Mitos. |

---

## 📖 3. Katalog Lengkap Makhluk & Spirit Beast per 10 Wilayah

---

### 🌿 3.1 Dataran Hijau Abadi (Verdant Qi Plains) — Elemen Kayu & Vitalitas

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Kelinci Qi Rumput Hijau** | 🐺 Wild Beast | Tier 0 (Fana) | 30 | 5 | Sangat Mudah (LV 1) | Kelinci pemakan herba liar. Sangat lincah melompat. | Daging Kelinci Fana (+10% Satiety) |
| **Ayam Hutan Spirit Kayu** | 🐺 Wild Beast | Tier 0 (Fana) | 40 | 8 | Sangat Mudah (LV 1) | Ayam liar bertanduk kayu kecil. Suka mematuk benih. | Daging Ayam Spirit, Bulu Warna-Warni |
| **Peri Bunga Embun (*Dew Sprite*)** | 🧚 Sprite / Roh | Tier 1 (Body Refining) | 80 | 12 | Sedang (LV 2) | **Imun Serangan Fisik**. Menyembuhkan luka herba +15 HP. | Esensi Bunga Embun (Bahan Pil Tier-1) |
| **Serigala Akar Hijau** | 🐺 Spirit Beast | Tier 2 (Qi Gathering) | 120 | 25 | Sedang (LV 2) | *Gigitan Akar Duri*: Menyergap dari balik semak belukar. | Kulit Serigala — Jarang: Core Beast Tier 1 |
| **Beruang Kayu Kuno** | 🐺 Spirit Beast | Tier 3 (Foundation) | 450 | 80 | Sulit (LV 3) | *Hantaman Batang Jati*: Memukul tanah, memicu Stun 1 turn. | Empedu Beruang — Jarang: Core Beast Tier 2 |

---

### ⚡ 3.2 Pegunungan Petir Guntur (Thunder Crest Range) — Elemen Petir & Logam

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Ular Besi Tembaga** | 🐺 Spirit Beast | Tier 2 (Qi Gathering) | 100 | 30 | Sedang (LV 2) | *Patukan Listrik*: Kulit tembaga keras, kebal tebasan biasa. | Sisik Tembaga — Jarang: Core Beast Tier 1 |
| **Roh Kilat Ungu (*Volt Sprite*)**| 🧚 Sprite / Roh | Tier 2 (Qi Gathering) | 90 | 35 | Sulit (LV 3) | Bola energi kilat liar. Serangan memicu efek *Paralysis*. | Percikan Esensi Petir (Bahan Tempa T2) |
| **Elang Kilat Ungu** | 🐺 Spirit Beast | Tier 3 (Foundation) | 380 | 95 | Sulit (LV 3) | Menukik dari puncak pegunungan dengan kecepatan suara. | Bulu Kilat Ungu — Jarang: Core Beast Tier 2 |
| **Macan Tutul Logam Guntur** | 🐺 Spirit Beast | Tier 4 (Golden Core) | 1.300 | 230 | Sangat Sulit (LV 4)| Cakar logam tajam, mampu melintasi medan tebing curam. | Kulit Macan Logam — Jarang: Core Beast Tier 3 |

---

### 🔥 3.3 Lembah Api Merah (Crimson Blaze Valley) — Elemen Api & Vulkanik

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Salamander Magma** | 🐺 Spirit Beast | Tier 3 (Foundation) | 400 | 85 | Sedang (LV 3) | *Semburan Lahar*: Menyemburkan cairan lahar memicu Burn. | Kulit Tahan Api — Jarang: Core Beast Tier 2 |
| **Sprite Api Vulkanik (*Lava Flame*)**| 🧚 Sprite / Roh | Tier 3 (Foundation) | 250 | 110 | Sulit (LV 3) | Elemen api hidup. Meledak saat HP menyentuh 0% (AoE Fire).| Esensi Api Merah (Bahan Alkimia T3) |
| **Kera Api Purba** | 🐺 Spirit Beast | Tier 4 (Golden Core) | 1.200 | 220 | Sangat Sulit (LV 4)| *Hujan Batu Lahar*: Melempar bongkahan batu membara. | Tangan Kera Api — Jarang: Core Beast Tier 3 |

---

### ❄️ 3.4 Danau Es Bintang (Frost Star Lake) — Elemen Es & Air Pembeku

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Ikan Perak Es** | 🐺 Wild Beast | Tier 0 (Fana) | 25 | 3 | Mudah (LV 1) | Ikan bersisik bening seperti kaca es. Lezat dimasak. | Daging Ikan Es (+15% Satiety) |
| **Hiu Es Kristal** | 🐺 Spirit Beast | Tier 3 (Foundation) | 420 | 90 | Sulit (LV 3) | *Tandukan Sirip Es*: Menembus perisai Qi, memicu Freeze. | Sirip Hiu Es — Jarang: Core Beast Tier 2 |
| **Roh Kristal Bintang (*Frost Sprite*)**|🧚 Sprite / Roh | Tier 3 (Foundation) | 280 | 85 | Sulit (LV 3) | Roh es mengapung. Menciptakan dinding es pembeku. | Esensi Es Kristal (Bahan Alkimia T3) |

---

### 💀 3.5 Tanah Gersang Tulang (Desolate Bone Wasteland) — Elemen Jiwa & Kegelapan

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Kalajengking Tulang Kelabu**| 🐛 Insect / Gu | Tier 3 (Foundation) | 360 | 75 | Sedang (LV 3) | *Sengatan Racun Jiwa*: Mengabaikan zirah fisik biasa. | Sengat Kalajengking — Jarang: Core Beast Tier 2 |
| **Sprite Jiwa Kelabu (*Soul Wisp*)**| 🧚 Sprite / Roh | Tier 3 (Foundation) | 200 | 95 | Tidak Bisa Dijinakkan| Arwah penasaran melayang. Menyerang langsung ke Dantian. | Esensi Jiwa Kelabu (Bahan Segel T3) |
| **Serigala Tulang Rangka** | 🗿 Undead Beast | Tier 4 (Golden Core) | 1.400 | 210 | Sangat Sulit (LV 4)| Serigala tanpa daging. **Imun racun dan perdarahan**. | Tulang Kuno — Jarang: Core Beast Tier 3 |

---

### 🏜️ 3.6 Gurun Pasir Emas (Golden Sand Desert) — Elemen Pasir & Tanah

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Kadal Pasir Gurun** | 🐺 Wild Beast | Tier 1 (Body Refining) | 70 | 15 | Mudah (LV 1) | Bersembunyi di dalam pasir panas. Menyergap kaki. | Daging Kadal, Kulit Pasir Kasar |
| **Cacing Pasir Raksasa** | 🐺 Spirit Beast | Tier 4 (Golden Core) | 1.500 | 250 | Sangat Sulit (LV 4)| *Pusaran Telan Pasir*: Memendam mangsa ke dalam tanah. | Kulit Cacing Gurun — Jarang: Core Beast Tier 3 |

---

### ☣️ 3.7 Rawa Kabut Racun (Shadow Mist Swamp) — Elemen Racun & Kabut

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Katak Teratai Hitam** | 🐺 Spirit Beast | Tier 3 (Foundation) | 390 | 80 | Sedang (LV 3) | *Lembatan Lidah Beracun*: Menyemprotkan lendir asam. | Lendir Katak — Jarang: Core Beast Tier 2 |
| **Sprite Kabut Miasma (*Poison Sprite*)**|🧚 Sprite / Roh| Tier 3 (Foundation) | 220 | 85 | Sulit (LV 3) | Kabut hijau hidup. Menghirupnya memicu efek *Poison*. | Kelenjar Miasma Murni (Bahan Racun T3) |

---

### 🏔️ 3.8 Puncak Langit Surgawi (Celestial Sky Peaks) — Elemen Angin Langit

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Burung Rajawali Angin Tajam**| 🐺 Spirit Beast | Tier 4 (Golden Core) | 1.100 | 210 | Sangat Sulit (LV 4)| *Tebasan Badai Angin*: Memotong pepohonan dengan bilah angin.| Bulu Angin Tajam — Jarang: Core Beast Tier 3 |
| **Sprite Angin Awan (*Sylph*)** | 🧚 Sprite / Roh | Tier 4 (Golden Core) | 800 | 240 | Ekstrem (LV 5) | Menari di atas awan. Kecepatan gerak +50% (Hard to hit). | Esensi Angin Langit (Bahan Alkimia T4) |

---

### 🌊 3.9 Kepulauan Palung Samudra (Oceanic Abyss Islands) — Elemen Samudra

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Mutiara Kerang Air** | 🐺 Wild Beast | Tier 1 (Body Refining) | 90 | 10 | Mudah (LV 1) | Kerang raksasa di dasar laut tipis. | Mutiara Air Biasa, Daging Kerang |
| **Gurita Palung Samudra** | 🐺 Spirit Beast | Tier 5 (Nascent Soul) | 3.800 | 450 | Ekstrem (LV 5) | *Cengkeraman Sembilan Tentakel*: Menenggelamkan kapal. | Tinta Gurita Murni — Jarang: Core Beast Tier 4 |

---

### 🗿 3.10 Apex Guardian & Makhluk Langka Lintas Wilayah

Makhluk legendaris ini menjelajahi perbatasan benua dan hanya muncul saat event besar atau gangguan ekosistem:

| Nama Makhluk | Kategori Makhluk | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan & Deskripsi Naratif | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Naga Kabut Purba Huangji**| 🗿 Apex Guardian | Tier 8 (Tribulation) | 350.000 | 45.000 | Mustahil (LV 10) | Penjaga perbatasan benua. Menguasai hukum hujan & petir. | **Sisik Naga Purba (100% First Kill)**, Core T8 |
| **Kirin Emas Kekaisaran** | 🗿 Apex Guardian | Tier 7 (Void Trans) | 120.000 | 18.000 | Mustahil (LV 9) | Makhluk pembawa keberuntungan Kekaisaran Huangji. | Tanduk Kirin Emas, Esensi Suci Huangji |
| **Burung Feniks Api Vulkanik**| 🗿 Apex Guardian | Tier 7 (Void Trans) | 110.000 | 19.500 | Mustahil (LV 9) | Bangkit kembali dari abu setiap kali HP menyentuh 0% (1x). | Bulu Feniks Api, Darah Suci Feniks |

---

## 🛡️ 4. Checklist Validasi AI GM

- [ ] Apakah HP dan Attack Power monster sesuai dengan tabel katalog di atas?
- [ ] Apakah jenis monster yang ditemui pemain sesuai dengan habitat wilayahnya?
- [ ] Apakah Sprite/Roh telah diberi karakteristik imun serangan fisik murni jika belum menggunakan senjata Qi/Elemen?
- [ ] Apakah loot drop telah dikalkulasikan berdasarkan Rarity dan dimasukkan ke *Item Origin Log* di Profil Karakter?
