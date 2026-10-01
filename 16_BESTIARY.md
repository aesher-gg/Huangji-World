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
| **Kelinci Qi Rumput Hijau** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 30 | 5 | Kelinci pemakan herba liar. Cepat melarikan diri jika dikagetkan. | Umum: Daging Kelinci Fana (+10% Satiety), Bulu Halus |
| **Ayam Hutan Spirit Kayu** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 40 | 8 | Ayam liar bertanduk kayu kecil. Mematuk tanah mencari benih herba. | Umum: Daging Ayam Spirit, Bulu Warna-Warni |
| **Tikus Tanah Qi Kayu** | 🐛 Insect / Small Beast | Tier 1 (Qi Gathering Awal) | 60 | 12 | Menggerogoti akar tanaman herbal kebun. Menyebabkan status Hama Kebun. | Umum: Daging Tikus Spirit — Jarang: Benih Herba Liar |
| **Serigala Akar Hijau** | 🐺 Spirit Beast | Tier 2, Awal (Qi Gathering) | 120 | 25 | Bergerak lincah di semak-semak. Menyergap dengan *Gigitan Akar Duri* (Damage 25 & Root 1 Turn). | Umum: Kulit Serigala, Taring Duri — Jarang: Core Beast Tier 1 |
| **Beruang Kayu Kuno** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 450 | 80 | Tubuh keras bagaikan kayu jati purba. Menyapu lawan dengan *Hantaman Batang Jati* (Damage 80 & Stun 1 Turn). | Umum: Empedu Beruang Kayu, Daging Spirit Rank 2 — Jarang: Core Beast Tier 2 |
| **Kera Duri Belukar** | 🐺 Spirit Beast | Tier 2, Mid (Qi Gathering) | 150 | 32 | Bersarang di pohon tua, melontarkan buah duri beracun dari jarak jauh. | Umum: Bulu Duri Hijau — Jarang: Buah Duri Spirit (Tier 1) |
| **Piton Bambu Hijau** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 600 | 110 | Menyamar di antara dahan bambu, melilit target dan meremukkan perisai Qi. | Umum: Sisik Bambu Hijau — Jarang: Kelenjar Bisa Bambu (Tier 2) |
| **Rusa Embun Suci** | 🐺 Spirit Beast (Langka) | Tier 4, Awal (Golden Core) | 1.800 | 220 | Makhluk anggun pemancar aura vitalitas. Menyembuhkan luka sekitar saat terancam. | Umum: Tanduk Embun Suci — Legendaris: Core Beast Tier 3 |

---

### ⚡ 2. Pegunungan Petir Guntur (Thunder Crest Range)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Kambing Liar Batu Besi** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 50 | 10 | Kambing tebing pemakan bijih tembaga halus. Tanduknya keras seperti besi. | Umum: Daging Kambing Fana, Tanduk Besi Kecil |
| **Kadal Tembaga Kecil** | 🐺 Spirit Beast Liar | Tier 1 (Qi Gathering Awal) | 70 | 15 | Merayap di tebing batu tembaga, menyengat dengan kejutan aliran listrik kecil. | Umum: Sisik Tembaga Kecil — Jarang: Serpihan Tembaga Suci |
| **Ular Besi Tembaga** | 🐺 Spirit Beast | Tier 2, Awal (Qi Gathering) | 100 | 30 | Bersisik tembaga keras. Menyengat dengan *Patukan Listrik* (Damage 30 & Paralysis). | Umum: Sisik Besi Tembaga — Jarang: Core Beast Tier 1 |
| **Elang Kilat Ungu** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 380 | 95 | Menukik dari Puncak Petir Surgawi dengan *Sambaran Sayap Kilat* (Damage 95 HP). | Umum: Bulu Kilat Ungu, Paruh Petir — Jarang: Core Beast Tier 2 |
| **Kambing Tebing Petir** | 🐺 Spirit Beast | Tier 2, Mid (Qi Gathering) | 140 | 28 | Memanjat tebing tembaga tegak lurus, menanduk dengan hantaman kejutan listrik. | Umum: Tanduk Tembaga — Jarang: Daging Petir Rank 1 |
| **Serigala Kilat Besi** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 550 | 105 | Berburu dalam kelompok 3–5 ekor di lembah tembaga, pergerakan secepat kilat. | Umum: Kulit Serigala Besi — Jarang: Core Beast Tier 2 |
| **Naga Petir Tebing Purba** | 🗿 Ancient Guardian | Tier 5, Mid (Nascent Soul) | 18.000 | 2.500 | Naga purba penjaga urat tembaga. Menyemburkan badai petir ungu pemusnah benteng. | Legendaris: Sisik Naga Petir Purba, Core Beast Tier 4 |

---

### 🔥 3. Lembah Api Merah (Crimson Blaze Valley)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Babi Abu Vulkanik** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 45 | 8 | Babi hutan berkulit tebal pemakan abu gunung berapi. | Umum: Daging Babi Panas, Kulit Abu Vulkanik |
| **Kadal Api Abu** | 🐺 Spirit Beast Liar | Tier 1 (Qi Gathering Awal) | 65 | 14 | Merayap di sekitar kawah lahar dingin, menyemburkan cipratan abu panas. | Umum: Kulit Tahan Panas — Jarang: Batu Api Kecil |
| **Salamander Magma** | 🔥 Elemental (Api) | Tier 3, Awal (Foundation) | 400 | 85 | Berenang di danau lahar. Melontarkan *Semburan Lahar Vulkanik* (Damage 85 & Burn). | Umum: Kulit Tahan Api, Darah Magma — Jarang: Core Beast Tier 2 |
| **Kera Api Purba** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.200 | 220 | Menghuni Gua Api Purba. Melancarkan *Hujan Batu Magma Meledak* (Damage 220 HP). | Umum: Tangan Kera Api — Jarang: Core Beast Tier 3 |
| **Kalajengking Lahar** | 🐛 Insect / Gu | Tier 2, Mid (Qi Gathering) | 160 | 35 | Bersembunyi di bawah abu vulkanik panas. Sengatan ekornya memicu luka bakar internal. | Umum: Cangkang Vulkanik — Jarang: Racun Api Lahar (Tier 1) |
| **Burung Merpati Magma** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 480 | 90 | Terbang bergerombol di atas kawah, meneteskan cairan lahar panas dari cakar. | Umum: Bulu Merpati Api — Jarang: Core Beast Tier 2 |

---

### ❄️ 4. Danau Es Bintang (Frost Star Lake)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Ikan Es Perak** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 25 | 4 | Ikan bening transparan berenang di air danau membeku. Sangat lezat dipanggang. | Umum: Daging Ikan Es (+15% Satiety) |
| **Anjing Laut Salju** | 🐺 Spirit Beast Liar | Tier 1 (Qi Gathering Awal) | 75 | 12 | Berjemur di atas bongkahan es, menyemburkan embun dingin jika terganggu. | Umum: Kulit Lemak Es — Jarang: Lemak Pemulih Luka |
| **Hiu Es Kristal** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 420 | 90 | Berenang di bawah permukaan es. Menerjang dengan *Tandukan Sirip Es* (Damage 90 & Freeze). | Umum: Sirip Hiu Es, Mutiara Es — Jarang: Core Beast Tier 2 |
| **Beruang Salju Kristal** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.400 | 230 | Menghuni pulau es abadi. Bulu tebalnya menyerap 30% damage fisik. | Umum: Kulit Beruang Es — Jarang: Core Beast Tier 3 |
| **Serigala Es Bintang** | 🐺 Spirit Beast | Tier 2, Mid (Qi Gathering) | 130 | 28 | Memburu ikan es di tepi danau, memiliki nafas dingin pembeku pergelangan kaki. | Umum: Bulu Serigala Es — Jarang: Daging Es Rank 1 |

---

### 💀 5. Tanah Gersang Tulang (Desolate Bone Wasteland)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Gagak Mata Merah** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 20 | 5 | Burung pemakan bangkai di padang tengkorak. Bersuara nyaring pertanda sial. | Umum: Bulu Gagak Hitam, Paruh Kecil |
| **Kelelawar Jiwa Kelabu** | 🐺 Spirit Beast Liar | Tier 1 (Qi Gathering Awal) | 55 | 11 | Bersarang di dalam goa kuburan, menggigit dan menyedot sedikit Qi stamina. | Umum: Sayap Kelelawar — Jarang: Gigi Vampir Kecil |
| **Kalajengking Tulang Kelabu** | 🐛 Insect / Gu | Tier 3, Awal (Foundation) | 360 | 75 | Bersembunyi di dalam tanah abu. Melancarkan *Sengatan Racun Jiwa* (Damage 75 & Poison). | Umum: Sengat Kalajengking, Cangkang Tulang — Jarang: Core Beast Tier 2 |
| **Prajurit Tulang Purba** | 👻 Undead | Tier 3, Mid (Foundation) | 500 | 95 | Bangkit dari kuburan tua membawa tombak berkarat. Kebal serangan racun & pendarahan. | Umum: Serpihan Baju Zirah Kuno — Jarang: Inti Jiwa Kelabu (Tier 2) |
| **Gargoyle Tengkorak Hitam** | 🗿 Ancient Guardian | Tier 4, Mid (Golden Core) | 2.500 | 380 | Patung batu penjaga reruntuhan perang. Menerkam dari udara dengan cakar batu. | Umum: Batu Tengkorak Hitam — Jarang: Core Beast Tier 3 |

---

### 🏜️ 6. Gurun Pasir Emas (Golden Sand Desert)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Kancil Pasir Emas** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 35 | 6 | Hewan lincah gurun pemakan akar kaktus suci. | Umum: Daging Kancil Gurun (+15% Satiety) |
| **Kadal Gurun Kecil** | 🐺 Spirit Beast Liar | Tier 1 (Qi Gathering Awal) | 60 | 12 | Menyelam di bawah bukit pasir halus, menggigit pergelangan kaki. | Umum: Kulit Kadal Pasir — Jarang: Daging Gurun Tier 1 |
| **Cacing Pasir Raksasa** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.500 | 250 | Bergerak di bawah bukit pasir. Memicu *Pusaran Telan Pasir* (Damage 250 & Trap 1 Turn). | Umum: Kulit Cacing Gurun, Gigi Pasir — Jarang: Core Beast Tier 3 |
| **Kadal Pasir Emas** | 🐺 Spirit Beast | Tier 2, Mid (Qi Gathering) | 140 | 30 | Berlari secepat angin di atas pasir panas, menyemburkan pasir panas ke mata target. | Umum: Sisik Kadal Gurun — Jarang: Daging Gurun Rank 1 |
| **Kalajengking Emas Purba** | 🐛 Insect / Gu | Tier 3, Mid (Foundation) | 520 | 100 | Menyengat dengan racun dahaga yang menguras Stamina & Satiety target secara cepat. | Umum: Cangkang Emas Gurun — Jarang: Core Beast Tier 2 |

---

### ☣️ 7. Rawa Kabut Racun (Shadow Mist Swamp)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Lintah Rawa Kecil** | 🐛 Insect / Small Beast | Tier 0 (Mortal Refining) | 20 | 4 | Menempel di kaki penjelajah rawa, menyedot darah dan memicu pendarahan ringan. | Umum: Lendir Lintah Rawa |
| **Nyamuk Kabut Beracun** | 🐛 Insect / Gu | Tier 1 (Qi Gathering Awal) | 50 | 10 | Terbang bergerombol di kabut tebal, menyuntikkan gatal racun. | Umum: Sayap Nyamuk Rawa — Jarang: Jarum Nyamuk Racun |
| **Katak Teratai Hitam** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 390 | 80 | Menyamar sebagai bunga teratai. Menjepit target dengan *Lembatan Lidah Beracun* (Damage 80 & Poison). | Umum: Lendir Katak Racun — Jarang: Core Beast Tier 2 |
| **Ular Rawa Seribu Bisa** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.300 | 210 | Berenang di lumpur hitam. Menyemburkan awan racun yang mengikis HP & Qi. | Umum: Sisik Ular Rawa — Jarang: Core Beast Tier 3 |

---

### 🏔️ 8. Puncak Langit Surgawi (Celestial Sky Peaks)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Burung Pipit Angin** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 25 | 5 | Terbang melayang mengikuti hembusan angin tebing. | Umum: Bulu Pipit Angin |
| **Tupai Terbang Awan** | 🐺 Spirit Beast Liar | Tier 1 (Qi Gathering Awal) | 60 | 11 | Meluncur dari pohon pinus tebing ke tebing lain, suka mencuri buah spirit. | Umum: Bulu Tupai Awan — Jarang: Buah Pinus Spirit |
| **Burung Rajawali Angin Tajam** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.100 | 210 | Menyambar dari balik awan. Melancarkan *Tebasan Badai Angin* (Damage 210 HP). | Umum: Bulu Angin Tajam — Jarang: Core Beast Tier 3 |
| **Kera Awan Melayang** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 460 | 88 | Bergerak lincah antar puncak tebing dengan bantuan angin Qi. | Umum: Bulu Kera Awan — Jarang: Core Beast Tier 2 |

---

### 🌊 9. Kepulauan Palung Samudra (Oceanic Abyss Islands)

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Kepiting Karang Kecil** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 35 | 6 | Merayap di pantai pasir putih, menjepit jari kaki penjelajah. | Umum: Daging Kepiting Pantai (+10% Satiety) |
| **Ikan Buntal Racun Laut** | 🐺 Spirit Beast Liar | Tier 1 (Qi Gathering Awal) | 65 | 13 | Menggelembung berduri saat terancam, menyuntikkan racun gatal laut. | Umum: Duri Ikan Buntal — Jarang: Kelenjar Racun Laut |
| **Gurita Palung Samudra** | 🐺 Spirit Beast | Tier 5, Awal (Nascent Soul) | 3.800 | 450 | Menghuni Palung Naga Laut. Menggulung kapal dengan *Cengkeraman Sembilan Tentakel* (Damage 450 HP). | Umum: Tinta Gurita Samudra, Tentakel — Jarang: Core Beast Tier 4 |
| **Hiu Karang Berduri** | 🐺 Spirit Beast | Tier 3, Mid (Foundation) | 580 | 115 | Berenang di sekitar terumbu karang tajam, menyerang penyelam mutiara Qi. | Umum: Gigi Hiu Karang, Sisik Tajam — Jarang: Core Beast Tier 2 |

---

### 🐉 10. Boss & Monster Langka Lintas Wilayah

| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Naga Kabut Purba Huangji** | 🗿 Ancient Guardian | Tier 8, Awal (Tribulation) | 350.000 | 45.000 | Legenda penjaga perbatasan benua. Menyemburkan lahar es & kilat petir purba. | Legendaris (100% First Kill): Sisik Naga Purba (Tier 8), Core Beast Tier 8 |
| **Feniks Api Kegelapan** | 🔥 Elemental (Api/Dark) | Tier 7, Mid (Sacred Spirit) | 120.000 | 18.000 | Bangkit dari kawah tua setiap seratus tahun. Api hitamnya menghanguskan Qi musuh. | Legendaris: Bulu Feniks Hitam (Tier 7), Core Beast Tier 7 |
