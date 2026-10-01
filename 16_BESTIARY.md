# 🐉 16. Bestiary — Huangji-World

> **Status File**: Modul Utama Katalog Spirit Beast & Monster
> **Versi**: 3.0 (Huangji Core Edition)
> **Rujukan Silang**: `01` s/d `10` (modul wilayah), `12_CULTIVATION_LAW_SYSTEM.md`, `15_COMBAT_SYSTEM.md`, `18_TAMING_SYSTEM.md`

---

## 🎲 1. Mekanisme Ambush & Formasi Encounter

Peluang disergap Spirit Beast / Monster liar saat menjelajah area luar kota dihitung menggunakan formula:

$$\text{AmbushChance} = 5\% \times \text{DangerModifier} \times \text{TimeModifier}$$

| Modifier | Nilai |
|---|---|
| **DangerModifier — Area Pemukiman / Jalan Utama** | ×0,5 |
| **DangerModifier — Wilayah Hutan / Pegunungan Normal** | ×1,0 |
| **DangerModifier — Zona Liar / Rawa / Gurun Liar** | ×2,0 |
| **DangerModifier — Zona Terlarang / Kawah / Palung Dalam** | ×4,0 |
| **TimeModifier — Siang Hari** | ×1,0 |
| **TimeModifier — Malam Hari** | ×2,0 (Mayoritas monster Yin & Pemangsa lebih aktif) |

---

## 💎 2. Sistem Drop Loot

$$\text{LootDropRate} = \text{BaseDropRate}(\text{Rarity})$$

| Rarity Loot | Base Drop Rate | Contoh Barang Drop |
|---|---|---|
| **Umum (Common)** | 70% – 90% | Daging spirit, sisik biasa, taring, cakar, cangkang |
| **Jarang (Rare)** | 20% – 40% | Core Beast Tier 1–4, kelenjar racun murni, bulu kilat |
| **Legendaris (Boss / Ancient Guardian)** | 5% – 15% (100% First Kill) | Core Beast Tier 5–8, pusaka purba, darah naga |

---

## 📖 3. Katalog Monster & Spirit Beast per 10 Wilayah

---

### 🌿 1. Dataran Hijau Abadi (Verdant Qi Plains)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Serigala Akar Hijau** | 🐺 Spirit Beast | Tier 2, Awal (Qi Gathering) | 120 | 25 | Bergerak lincah di semak-semak. Menyergap dengan *Gigitan Akar Duri* (Damage 25 & Root 1 Turn). | Umum: Kulit Serigala, Taring Duri — Jarang: Core Beast Tier 1 |
| **Beruang Kayu Kuno** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 450 | 80 | Tubuh keras bagaikan kayu jati purba. Menyapu lawan dengan *Hantaman Batang Jati* (Damage 80 & Stun 1 Turn). | Umum: Empedu Beruang Kayu, Daging Spirit Rank 2 — Jarang: Core Beast Tier 2 |
| **Kera Duri Belukar** | 🐺 Spirit Beast | Tier 2, Mid (Qi Gathering) | 150 | 32 | Bersarang di pohon tua, melontarkan buah duri beracun dari jarak jauh. | Umum: Bulu Duri Hijau — Jarang: Buah Duri Spirit (Tier 1) |
| **Piton Bambu Hijau** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 600 | 110 | Menyamar di antara dahan bambu, melilit target dan meremukkan perisai Qi. | Umum: Sisik Bambu Hijau — Jarang: Kelenjar Bisa Bambu (Tier 2) |
| **Rusa Embun Suci** | 🐺 Spirit Beast (Langka) | Tier 4, Awal (Golden Core) | 1.800 | 220 | Makhluk anggun pemancar aura vitalitas. Menyembuhkan luka sekitar saat terancam. | Umum: Tanduk Embun Suci — Legendaris: Core Beast Tier 3 |

---

### ⚡ 2. Pegunungan Petir Guntur (Thunder Crest Range)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Ular Besi Tembaga** | 🐺 Spirit Beast | Tier 2, Awal (Qi Gathering) | 100 | 30 | Bersisik tembaga keras. Menyengat dengan *Patukan Listrik* (Damage 30 & Paralysis). | Umum: Sisik Besi Tembaga — Jarang: Core Beast Tier 1 |
| **Elang Kilat Ungu** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 380 | 95 | Menukik dari Puncak Petir Surgawi dengan *Sambaran Sayap Kilat* (Damage 95 HP). | Umum: Bulu Kilat Ungu, Paruh Petir — Jarang: Core Beast Tier 2 |
| **Kambing Tebing Petir** | 🐺 Spirit Beast | Tier 2, Mid (Qi Gathering) | 140 | 28 | Memanjat tebing tembaga tegak lurus, menanduk dengan hantaman kejutan listrik. | Umum: Tanduk Tembaga — Jarang: Daging Petir Rank 1 |
| **Serigala Kilat Besi** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 550 | 105 | Berburu dalam kelompok 3–5 ekor di lembah tembaga, pergerakan secepat kilat. | Umum: Kulit Serigala Besi — Jarang: Core Beast Tier 2 |
| **Naga Petir Tebing Purba** | 🗿 Ancient Guardian | Tier 5, Mid (Nascent Soul) | 18.000 | 2.500 | Naga purba penjaga urat tembaga. Menyemburkan badai petir ungu pemusnah benteng. | Legendaris: Sisik Naga Petir Purba, Core Beast Tier 4 |

---

### 🔥 3. Lembah Api Merah (Crimson Blaze Valley)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Salamander Magma** | 🔥 Elemental (Api) | Tier 3, Awal (Foundation) | 400 | 85 | Berenang di danau lahar. Melontarkan *Semburan Lahar Vulkanik* (Damage 85 & Burn). | Umum: Kulit Tahan Api, Darah Magma — Jarang: Core Beast Tier 2 |
| **Kera Api Purba** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.200 | 220 | Menghuni Gua Api Purba. Melancarkan *Hujan Batu Magma Meledak* (Damage 220 HP). | Umum: Tangan Kera Api — Jarang: Core Beast Tier 3 |
| **Kalajengking Lahar** | 🐛 Insect / Gu | Tier 2, Mid (Qi Gathering) | 160 | 35 | Bersembunyi di bawah abu vulkanik panas. Sengatan ekornya memicu luka bakar internal. | Umum: Cangkang Vulkanik — Jarang: Racun Api Lahar (Tier 1) |
| **Burung Merpati Magma** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 480 | 90 | Terbang bergerombol di atas kawah, meneteskan cairan lahar panas dari cakar. | Umum: Bulu Merpati Api — Jarang: Core Beast Tier 2 |

---

### ❄️ 4. Danau Es Bintang (Frost Star Lake)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Hiu Es Kristal** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 420 | 90 | Berenang di bawah permukaan es. Menerjang dengan *Tandukan Sirip Es* (Damage 90 & Freeze). | Umum: Sirip Hiu Es, Mutiara Es — Jarang: Core Beast Tier 2 |
| **Beruang Salju Kristal** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.400 | 230 | Menghuni pulau es abadi. Bulu tebalnya menyerap 30% damage fisik. | Umum: Kulit Beruang Es — Jarang: Core Beast Tier 3 |
| **Serigala Es Bintang** | 🐺 Spirit Beast | Tier 2, Mid (Qi Gathering) | 130 | 28 | Memburu ikan es di tepi danau, memiliki nafas dingin pembeku pergelangan kaki. | Umum: Bulu Serigala Es — Jarang: Daging Es Rank 1 |

---

### 💀 5. Tanah Gersang Tulang (Desolate Bone Wasteland)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Kalajengking Tulang Kelabu** | 🐛 Insect / Gu | Tier 3, Awal (Foundation) | 360 | 75 | Bersembunyi di dalam tanah abu. Melancarkan *Sengatan Racun Jiwa* (Damage 75 & Poison). | Umum: Sengat Kalajengking, Cangkang Tulang — Jarang: Core Beast Tier 2 |
| **Prajurit Tulang Purba** | 👻 Undead | Tier 3, Mid (Foundation) | 500 | 95 | Bangkit dari kuburan tua membawa tombak berkarat. Kebal serangan racun & pendarahan. | Umum: Serpihan Baju Zirah Kuno — Jarang: Inti Jiwa Kelabu (Tier 2) |
| **Gargoyle Tengkorak Hitam** | 🗿 Ancient Guardian | Tier 4, Mid (Golden Core) | 2.500 | 380 | Patung batu penjaga reruntuhan perang. Menerkam dari udara dengan cakar batu. | Umum: Batu Tengkorak Hitam — Jarang: Core Beast Tier 3 |

---

### 🏜️ 6. Gurun Pasir Emas (Golden Sand Desert)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Cacing Pasir Raksasa** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.500 | 250 | Bergerak di bawah bukit pasir. Memicu *Pusaran Telan Pasir* (Damage 250 & Trap 1 Turn). | Umum: Kulit Cacing Gurun, Gigi Pasir — Jarang: Core Beast Tier 3 |
| **Kadal Pasir Emas** | 🐺 Spirit Beast | Tier 2, Mid (Qi Gathering) | 140 | 30 | Berlari secepat angin di atas pasir panas, menyemburkan pasir panas ke mata target. | Umum: Sisik Kadal Gurun — Jarang: Daging Gurun Rank 1 |
| **Kalajengking Emas Purba** | 🐛 Insect / Gu | Tier 3, Mid (Foundation) | 520 | 100 | Menyengat dengan racun dahaga yang menguras Stamina & Satiety target secara cepat. | Umum: Cangkang Emas Gurun — Jarang: Core Beast Tier 2 |

---

### ☣️ 7. Rawa Kabut Racun (Shadow Mist Swamp)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Katak Teratai Hitam** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 390 | 80 | Menyamar sebagai bunga teratai. Menjepit target dengan *Lembatan Lidah Beracun* (Damage 80 & Poison). | Umum: Lendir Katak Racun — Jarang: Core Beast Tier 2 |
| **Ular Rawa Seribu Bisa** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.300 | 210 | Berenang di lumpur hitam. Menyemburkan awan racun yang mengikis HP & Qi. | Umum: Sisik Ular Rawa — Jarang: Core Beast Tier 3 |

---

### 🏔️ 8. Puncak Langit Surgawi (Celestial Sky Peaks)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Burung Rajawali Angin Tajam** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.100 | 210 | Menyambar dari balik awan. Melancarkan *Tebasan Badai Angin* (Damage 210 HP). | Umum: Bulu Angin Tajam — Jarang: Core Beast Tier 3 |
| **Kera Awan Melayang** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 460 | 88 | Bergerak lincah antar puncak tebing dengan bantuan angin Qi. | Umum: Bulu Kera Awan — Jarang: Core Beast Tier 2 |

---

### 🌊 9. Kepulauan Palung Samudra (Oceanic Abyss Islands)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Gurita Palung Samudra** | 🐺 Spirit Beast | Tier 5, Awal (Nascent Soul) | 3.800 | 450 | Menghuni Palung Naga Laut. Menggulung kapal dengan *Cengkeraman Sembilan Tentakel* (Damage 450 HP). | Umum: Tinta Gurita Samudra, Tentakel — Jarang: Core Beast Tier 4 |
| **Hiu Karang Berduri** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 580 | 115 | Berenang di sekitar terumbu karang tajam, menyerang penyelam mutiara Qi. | Umum: Gigi Hiu Karang, Sisik Tajam — Jarang: Core Beast Tier 2 |

---

### 🐉 10. Boss & Monster Langka Lintas Wilayah

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Naga Kabut Purba Huangji** | 🗿 Ancient Guardian | Tier 8, Awal (Tribulation) | 350.000 | 45.000 | Legenda penjaga perbatasan benua. Menyemburkan lahar es & kilat petir purba. | Legendaris (100% First Kill): Sisik Naga Purba (Tier 8), Core Beast Tier 8 |
| **Feniks Api Kegelapan** | 🔥 Elemental (Api/Dark) | Tier 7, Mid (Sacred Spirit) | 120.000 | 18.000 | Bangkit dari kawah tua setiap seratus tahun. Api hitamnya menghanguskan Qi musuh. | Legendaris: Bulu Feniks Hitam (Tier 7), Core Beast Tier 7 |
