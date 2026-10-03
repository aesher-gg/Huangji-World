# 🐉 Huangji-World — Bestiary & Katalog Spesies Spirit (Monster, Spirit Beast, Sprite & Apex Guardians)

> **Modul:** 16 — Bestiary & Monster System
> **Prinsip:** Anti-Cheat Enforced — Habitat-Locked — Terintegrasi dengan Sistem HP, Combat, Taming, & Item Origin Log
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md` (aturan wajib), `12_CULTIVATION_LAW_SYSTEM.md` (Tingkat Ranah), `13_ECONOMY_SYSTEM.md` (Nilai Loot/Core), `15_COMBAT_SYSTEM.md` (Damage Formula), `18_TAMING_SYSTEM.md` (Penjinakan)

---

## 0. Filosofi Sistem

Dunia Huangji dihuni oleh berbagai spesies makhluk hidup spiritual dan binatang liar — mulai dari **Binatang Fana / Wild Beast**, **Spirit Beast (Tier 1–9)**, **Sprite / Roh Elemen**, hingga **Makhluk Purba Apex (*Apex Guardian Beasts*)**.

Setiap makhluk memiliki habitat resmi, batas stat fisik, peluang kemunculan (*Ambush Rate*), dan formula drop loot yang wajib divalidasi oleh AI GM. **Pemain dilarang mendatangkan monster di luar habitat resminya atau mengklaim loot tanpa mengalahkan monster tersebut dalam pertarungan naratif.**

---

## 🎲 1. Formula Ambush & Formasi Encounter

```
AmbushChance = BaseChance (5%) × DangerModifier × TimeModifier × NoiseModifier
```

### 📊 Tabel Modifier Kemunculan Monster

| Faktor Lingkungan | Kategori Lingkungan / Kondisi | Modifier (`DangerModifier`) |
|---|---|:---:|
| **Area Pemukiman / Kota** | Dalam Ibu Kota Huangji / Desa Sekte Utama | **×0,1** (Hanya Beast Peliharaan) |
| **Jalan Utama / Jalur Dagang** | Jalur Kuda & Pos Penjagaan Kekaisaran | **×0,5** |
| **Hutan / Pegunungan Normal** | Pinggiran Hutan Kayu / Bukit Rendah | **×1,0** |
| **Zona Liar / Rawa / Gurun** | Hutan Purba / Rawa Kabut Miasma / Gurun Pasir | **×2,0** |
| **Zona Terlarang / Kawah Lahar**| Lembah Api Vulkanik / Kawah Lahar / Palung Laut | **×4,0** |

---

## 🌐 2. Spesies Umum Lintas Wilayah (Universal / Cross-Region Beasts)

Spesies ini dapat ditemukan di **hampir seluruh wilayah Benua Huangji** (hutan, jalan desa, gurun, rawa, pegunungan, dan pantai umum) dari Tier 0 (Fana) hingga Tier 5 (Setara Ranah Jiwa Nascent):

| Nama Spesies | Kategori Jenis | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Deskripsi | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Ayam Hutan Fana** | 🐓 Avian | Tier 0 (Fana) | 25 | 4 | LV 1 | Ayam liar pemakan serangga. Berisik saat terkejut. | Daging Ayam Fana (+10% Satiety), Bulu |
| **Kelinci Padang Rumput** | 🐇 Beast | Tier 0 (Fana) | 30 | 5 | LV 1 | Lincah dan cepat masuk ke lubang tanah. | Daging Kelinci Fana (+10% Satiety) |
| **Katak Air Fana** | 🐸 Amphibian | Tier 0 (Fana) | 20 | 3 | LV 1 | Berada di pinggiran sungai/danau fana. | Daging Katak Fana (+10% Satiety) |
| **Babi Hutan Taring Besi** | 🐗 Beast | Tier 1 (Body Ref) | 90 | 18 | LV 1 | *Serudukan Lurus*: Menyeruduk target dengan taring ganda. | Daging Babi Hutan (+25% Satiety), Taring Besi |
| **Serigala Kelabu Liar** | 🐺 Beast | Tier 1 (Body Ref) | 85 | 20 | LV 1 | Berburu dalam kelompok (3–5 ekor). *Mencakar & Menggigit*. | Kulit Serigala Kasar, Daging Serigala |
| **Ular Sawah Hijau** | 🐍 Serpent | Tier 1 (Body Ref) | 60 | 15 | LV 1 | Bersembunyi di semak-semak. *Patukan Beracun Ringan*. | Kantong Empedu Ular, Kulit Ular |
| **Elang Pengembara** | 🦅 Avian | Tier 1 (Body Ref) | 75 | 16 | LV 1 | Mengincar mangsa dari udara. *Sabetan Cakar Udara*. | Bulu Elang, Paruh Keras |
| **Kera Hutan Cokelat** | 🐒 Beast | Tier 1 (Body Ref) | 80 | 14 | LV 1 | Melempar buah keras dan batu ke arah penyusup. | Kulit Kera, Buah Hutan |
| **Gagak Malam Berbintang**| 🦅 Avian | Tier 1 (Body Ref) | 50 | 12 | LV 1 | Terbang saat malam hari. *Kekek Gelisah* (Gagal Stealth).| Bulu Gagak Hitam |
| **Bunglon Bayang Lintas** | 🦎 Reptile | Tier 2 (Qi Gath) | 130 | 32 | LV 2 | *Kamuflase Sempurna*: Menjadi tidak terlihat selama 2 Turn. | Kulit Bunglon Bayang, Core T1 |
| **Kelelawar Darah Malam** | 🦇 Avian/Beast | Tier 2 (Qi Gath) | 110 | 28 | LV 2 | *Penghisapan Darah*: Menyerap 20% Damage sebagai HP. | Sayap Kelelawar, Core T1 |
| **Kelabang Kerangka Hitam**| 🐛 Insect/Gu | Tier 2 (Qi Gath) | 125 | 35 | LV 2 | *Racun Kelumpuhan*: Debuff Slow -20% selama 2 Turn. | Racun Kelabang, Core T1 |
| **Laba-Lava Sutra Jingga** | 🕷️ Insect | Tier 3 (Found) | 380 | 85 | LV 3 | *Jaring Penjerat Qi*: Mengunci gerakan target (Stun 1 Turn).| Benang Sutra Spirit, Core T2 |
| **Serigala Bayangan Tanduk**| 🐺 Spirit Beast| Tier 3 (Found) | 420 | 95 | LV 3 | *Tandukan Qi Bayangan*: Membusuk Pertahanan target. | Taring Serigala Tanduk, Core T2 |
| **Piton Batu Raksasa** | 🐍 Serpent | Tier 3 (Found) | 450 | 90 | LV 3 | *Lilitan Pemutus Tulang*: Damage beruntun per Turn. | Sisik Piton Batu, Core T2 |
| **Macan Tutul Angin Malam**| 🐆 Spirit Beast| Tier 4 (Golden C)| 1.300 | 240 | LV 4 | *Kecepatan Angin*: Move Speed +40%, Critical Chance +25%.| Kulit Macan Angin, Core T3 |
| **Kadal Lahar Karat** | 🦎 Elemental | Tier 4 (Golden C)| 1.450 | 230 | LV 4 | *Aura Api Kerak*: Membakar lawan saat diserang jarak dekat. | Sisik Lahar Karat, Core T3 |
| **Elang Badai Petir Purba**| 🦅 Avian | Tier 5 (Nascent S)| 4.600 | 680 | LV 5 | *Sabetan Badai Petir*: Damage Elemen Petir AoE. | Bulu Elang Badai, Core T4 |
| **Banteng Batu Dinding** | 🐂 Spirit Beast| Tier 5 (Nascent S)| 5.200 | 620 | LV 5 | *Tembok Batu Abadi*: Defense Murni +150. | Tanduk Banteng Batu, Core T4 |
Spesies ini dapat ditemukan di **hampir seluruh wilayah Benua Huangji** (hutan, jalan desa, dan pegunungan umum):

| Nama Spesies | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming Difficulty | Kemampuan Utama & Deskripsi | Drop Loot Utama |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Ayam Hutan Fana** | 🐺 Wild Beast | Tier 0 (Fana) | 25 | 4 | Sangat Mudah (LV 1) | Ayam liar pemakan serangga. Berisik saat terkejut. | Daging Ayam Fana (+10% Satiety), Bulu |
| **Kelinci Padang Rumput** | 🐺 Wild Beast | Tier 0 (Fana) | 30 | 5 | Sangat Mudah (LV 1) | Lincah dan cepat masuk ke lubang tanah. | Daging Kelinci Fana (+10% Satiety) |
| **Babi Hutan Taring Besi** | 🐺 Wild Beast | Tier 1 (Body Refining) | 90 | 18 | Mudah (LV 1) | *Serudukan Lurus*: Menyeruduk target dengan taring ganda. | Daging Babi Hutan (+25% Satiety), Taring Besi |
| **Serigala Kelabu Liar** | 🐺 Wild Beast | Tier 1 (Body Refining) | 85 | 20 | Mudah (LV 1) | Berburu dalam kelompok (3–5 ekor). *Mencakar & Menggigit*. | Kulit Serigala Kasar, Daging Serigala |
| **Ular Sawah Hijau** | 🐺 Wild Beast | Tier 1 (Body Refining) | 60 | 15 | Mudah (LV 1) | Bersembunyi di semak-semak. *Patukan Beracun Ringan*. | Kantong Empedu Ular, Kulit Ular |
| **Elang Pengembara** | 🐺 Wild Beast | Tier 1 (Body Refining) | 75 | 16 | Mudah (LV 1) | Mengincar mangsa dari udara. *Sabetan Cakar Udara*. | Bulu Elang, Paruh Keras |
| **Kera Hutan Cokelat** | 🐺 Wild Beast | Tier 1 (Body Refining) | 80 | 14 | Mudah (LV 1) | Melempar buah keras dan batu ke arah penyusup. | Kulit Kera, Buah Hutan |
| **Gagak Malam Berbintang**| 🐺 Wild Beast | Tier 1 (Body Refining) | 50 | 12 | Mudah (LV 1) | Terbang saat malam hari. *Kekek Gelisah* (Gagal Stealth).| Bulu Gagak Hitam |

---

## 📖 3. Katalog Lengkap Monster & Spirit Beast per 10 Wilayah (Tier 0 s/d 9)

---

### 🌿 3.1 Dataran Hijau Abadi (Verdant Qi Plains) — Elemen Kayu & Vitalitas

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Rusa Kayu Duri** | Wild Beast | Tier 0 (Fana) | 35 | 6 | LV 1 | Berlari kencang saat terancam. | Daging Rusa Fana, Tanduk Kayu |
| 2 | **Peri Bunga Embun (*Dew Sprite*)** | Sprite / Roh | Tier 1 (Body Ref) | 80 | 12 | LV 2 | **Imun fisik**. Menyembuhkan luka +15 HP. | Esensi Bunga Embun (Pil T1) |
| 3 | **Serigala Akar Hijau** | Spirit Beast | Tier 2 (Qi Gath) | 120 | 25 | LV 2 | *Gigitan Duri*: Menyergap dari semak. | Kulit Serigala, Core T1 |
| 4 | **Beruang Kayu Kuno** | Spirit Beast | Tier 3 (Found) | 450 | 80 | LV 3 | *Hantaman Jati*: Stun 1 turn. | Empedu Beruang, Core T2 |
| 5 | **Ular Sanca Daun Hijau** | Spirit Beast | Tier 4 (Golden C) | 1.200 | 220 | LV 4 | *Melilit Vitalitas*: Menguras Stamina target. | Kulit Sanca Hijau, Core T3 |
| 6 | **Sprite Pohon Purba (*Treant*)** | Sprite / Roh | Tier 5 (Nascent S) | 4.500 | 650 | LV 5 | *Akar Penjerat*: Mengunci pergerakan musuh.| Kayu Purba Vitalitas, Core T4 |
| 7 | **Rusa Bambu Pelangi** | Spirit Beast | Tier 6 (Spirit Form) | 18.000 | 2.200 | LV 6 | *Langkah Embun*: Kecepatan gerak +50%. | Tanduk Bambu Pelangi, Core T5 |
| 8 | **Kera Raksasa Hutan Purba** | Spirit Beast | Tier 7 (Void Trans) | 90.000 | 12.000 | LV 7 | *Pukulan Badai Kayu*: Kerusakan AoE. | Tangan Kera Purba, Core T6 |
| 9 | **Naga Kayu Suci Abadi** | Apex Guardian | Tier 8 (Tribulation) | 400.000 | 50.000 | LV 9 | *Restorasi Alam*: Regenerasi HP 5%/turn. | Sisik Naga Kayu Purba, Core T7 |
| 10 | **Dewa Pohon Suci Huangji** | Sovereign Guardian| Tier 9 (Sovereign) | 2.000.000 | 250.000 | Mustahil | *Hukuman Akar Alam Semesta*. | Esensi Pohon Suci Huangji |

---

### ⚡ 3.2 Pegunungan Petir Guntur (Thunder Crest Range) — Elemen Petir & Logam

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Tikus Kilat Tembaga** | Wild Beast | Tier 0 (Fana) | 25 | 5 | LV 1 | Menghasilkan percikan listrik kecil. | Daging Tikus Tembaga |
| 2 | **Ular Besi Tembaga** | Spirit Beast | Tier 2 (Qi Gath) | 100 | 30 | LV 2 | *Patukan Listrik*: Kulit tembaga keras. | Sisik Tembaga, Core T1 |
| 3 | **Roh Kilat Ungu (*Volt Sprite*)**| Sprite / Roh | Tier 2 (Qi Gath) | 90 | 35 | LV 3 | *Paralysis*: Efek kejut ke saraf musuh. | Percikan Esensi Petir |
| 4 | **Elang Kilat Ungu** | Spirit Beast | Tier 3 (Found) | 380 | 95 | LV 3 | Menukik cepat dari puncak pegunungan. | Bulu Kilat Ungu, Core T2 |
| 5 | **Macan Tutul Logam Guntur** | Spirit Beast | Tier 4 (Golden C) | 1.300 | 230 | LV 4 | Cakar logam tajam menembus zirah. | Kulit Macan Logam, Core T3 |
| 6 | **Banteng Besi Badai Petir** | Spirit Beast | Tier 5 (Nascent S) | 4.800 | 700 | LV 5 | *Tandukan Guntur*: Memicu Daze/Pusing. | Tanduk Besi Badai, Core T4 |
| 7 | **Rajawali Petir Emas** | Spirit Beast | Tier 6 (Spirit Form) | 20.000 | 2.500 | LV 6 | *Sabetan Kilat Emas*: Damage Petir AoE. | Bulu Petir Emas, Core T5 |
| 8 | **Kirin Logam Guntur Purba** | Apex Guardian | Tier 7 (Void Trans) | 95.000 | 13.000 | LV 8 | *Hujan Sambaran Petir Ungu*. | Tanduk Kirin Logam, Core T6 |
| 9 | **Naga Petir Ungu Surgawi** | Apex Guardian | Tier 8 (Tribulation) | 420.000 | 55.000 | LV 9 | *Palu Petir Tribulasi Surgawi*. | Sisik Naga Petir Ungu, Core T7 |
| 10 | **Penguasa Kilat Alam Semesta** | Sovereign Guardian| Tier 9 (Sovereign) | 2.100.000 | 260.000 | Mustahil | *Hukuman Petir Keabadian*. | Esensi Petir Agung Huangji |

---

### 🔥 3.3 Lembah Api Merah (Crimson Blaze Valley) — Elemen Api & Vulkanik

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Kadal Abu Vulkanik** | Wild Beast | Tier 0 (Fana) | 30 | 6 | LV 1 | Tahan panas kawah lahar. | Kulit Kadal Abu |
| 2 | **Kalajengking Api Merah** | Spirit Beast | Tier 2 (Qi Gath) | 110 | 28 | LV 2 | *Sengatan Bara Api*: Memicu Burn. | Sengat Api, Core T1 |
| 3 | **Salamander Magma** | Spirit Beast | Tier 3 (Found) | 400 | 85 | LV 3 | *Semburan Lahar*: Memicu Burn 2 turn. | Kulit Tahan Api, Core T2 |
| 4 | **Sprite Api Vulkanik (*Lava Flame*)**| Sprite / Roh | Tier 3 (Found) | 250 | 110 | LV 3 | **Meledak saat mati** (AoE Fire Damage). | Esensi Api Merah |
| 5 | **Kera Api Purba** | Spirit Beast | Tier 4 (Golden C) | 1.200 | 220 | LV 4 | *Hujan Batu Lahar*: Lemparan batu membara.| Tangan Kera Api, Core T3 |
| 6 | **Serigala Lahar Vulkanik** | Spirit Beast | Tier 5 (Nascent S) | 4.200 | 680 | LV 5 | *Aura Pembakar Dantian*. | Kulit Serigala Lahar, Core T4 |
| 7 | **Ular Piton Kawah Merah** | Spirit Beast | Tier 6 (Spirit Form) | 17.500 | 2.300 | LV 6 | *Semburan Api Vulkanik Pekat*. | Sisik Piton Api, Core T5 |
| 8 | **Burung Feniks Api Lahar** | Apex Guardian | Tier 7 (Void Trans) | 110.000 | 19.500 | LV 8 | **Reborn 1x saat HP 0%** (HP pulih 50%). | Bulu Feniks Api, Core T6 |
| 9 | **Naga Lahar Purba Vulkanik** | Apex Guardian | Tier 8 (Tribulation) | 410.000 | 52.000 | LV 9 | *Gelombang Tsunami Magma*. | Sisik Naga Lahar, Core T7 |
| 10 | **Dewa Api Tungku Huangji** | Sovereign Guardian| Tier 9 (Sovereign) | 2.050.000 | 255.000 | Mustahil | *Pembakaran Esensi Alam Semesta*. | Esensi Api Tungku Huangji |

---

### ❄️ 3.4 Danau Es Bintang (Frost Star Lake) — Elemen Es & Air Pembeku

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Ikan Perak Es** | Wild Beast | Tier 0 (Fana) | 25 | 3 | LV 1 | Sisik kaca bening. Lezat dimasak. | Daging Ikan Es (+15% Satiety) |
| 2 | **Rubah Es Bintang** | Spirit Beast | Tier 2 (Qi Gath) | 105 | 24 | LV 2 | *Hembusan Salju Pembeku*. | Bulu Rubah Es, Core T1 |
| 3 | **Hiu Es Kristal** | Spirit Beast | Tier 3 (Found) | 420 | 90 | LV 3 | *Tandukan Sirip Es*: Freeze 1 turn. | Sirip Hiu Es, Core T2 |
| 4 | **Sprite Kristal Bintang (*Frost*)**| Sprite / Roh | Tier 3 (Found) | 280 | 85 | LV 3 | *Dinding Es Pembeku*: Perisai Es. | Esensi Es Kristal |
| 5 | **Beruang Kutub Es Bintang** | Spirit Beast | Tier 4 (Golden C) | 1.400 | 215 | LV 4 | *Tamparan Es Kristal*: Memicu Slow. | Kulit Beruang Es, Core T3 |
| 6 | **Serigala Kristal Salju Purba**| Spirit Beast | Tier 5 (Nascent S) | 4.600 | 660 | LV 5 | *Aura Pembeku Miasma Es*. | Taring Serigala Es, Core T4 |
| 7 | **Ular Laut Bintang Pembeku** | Spirit Beast | Tier 6 (Spirit Form) | 19.000 | 2.400 | LV 6 | *Semburan Napas Pembeku Abadi*. | Sisik Ular Es, Core T5 |
| 8 | **Burung Rajawali Es Bintang** | Spirit Beast | Tier 7 (Void Trans) | 88.000 | 11.500 | LV 7 | *Badai Salju Bintang Pembeku*. | Bulu Rajawali Es, Core T6 |
| 9 | **Naga Es Kristal Purba** | Apex Guardian | Tier 8 (Tribulation) | 390.000 | 48.000 | LV 9 | *Pembekuan Lautan Abadi*. | Sisik Naga Es Purba, Core T7 |
| 10 | **Penguasa Es Bintang Abadi** | Sovereign Guardian| Tier 9 (Sovereign) | 1.950.000 | 245.000 | Mustahil | *Pembekuan Waktu & Alam Semesta*. | Esensi Es Bintang Huangji |

---

### 💀 3.5 Tanah Gersang Tulang (Desolate Bone Wasteland) — Elemen Jiwa & Kegelapan

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Gagak Jiwa Kelabu** | Wild Beast | Tier 0 (Fana) | 20 | 4 | LV 1 | Menghisap aura kematian dari bangkai. | Bulu Gagak Kelabu |
| 2 | **Tikus Rangka Tulang** | Undead Beast | Tier 1 (Body Ref) | 65 | 14 | LV 1 | Berburu dalam koloni besar (10+ ekor).| Tulang Tikus Kuno |
| 3 | **Kalajengking Tulang Kelabu** | Insect / Gu | Tier 3 (Found) | 360 | 75 | LV 3 | *Sengatan Racun Jiwa*: Abaikan Zirah. | Sengat Kalajengking, Core T2 |
| 4 | **Sprite Jiwa Kelabu (*Soul Wisp*)**| Sprite / Roh | Tier 3 (Found) | 200 | 95 | Tidak Bisa | *Jeritan Jiwa*: Serang Dantian langsung.| Esensi Jiwa Kelabu |
| 5 | **Serigala Tulang Rangka** | Undead Beast | Tier 4 (Golden C) | 1.400 | 210 | LV 4 | **Imun racun dan pendarahan**. | Tulang Serigala Kuno, Core T3 |
| 6 | **Naga Rangka Tulang Kelabu** | Undead Beast | Tier 5 (Nascent S) | 5.000 | 720 | LV 5 | *Semburan Kabut Kematian*. | Tulang Naga Kuno, Core T4 |
| 7 | **Prajurit Rangka Purba** | Undead / Skeleton| Tier 6 (Spirit Form) | 21.000 | 2.600 | Tidak Bisa | Menggunakan pedang bertuah kuno. | Pedang Rangka Kuno, Core T5 |
| 8 | **Raja Tulang Jiwa Kelabu** | Undead Boss | Tier 7 (Void Trans) | 92.000 | 12.500 | LV 8 | *Panggilan Seribu Rangka*. | Mahta Tulang Kuno, Core T6 |
| 9 | **Iblis Jiwa Kelabu Purba** | Apex Guardian | Tier 8 (Tribulation) | 430.000 | 58.000 | LV 9 | *Penyedotan Jiwa Abadi*. | Kristal Jiwa Purba, Core T7 |
| 10 | **Penguasa Kehampaan Kematian** | Sovereign Guardian| Tier 9 (Sovereign) | 2.150.000 | 270.000 | Mustahil | *Hukuman Musnah Jiwa Huangji*. | Esensi Jiwa Kematian Huangji |

---

### 🏜️ 3.6 Gurun Pasir Emas (Golden Sand Desert) — Elemen Pasir & Tanah

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Kadal Pasir Gurun** | Wild Beast | Tier 1 (Body Ref) | 70 | 15 | LV 1 | Bersembunyi di dalam pasir panas. | Daging Kadal, Kulit Pasir |
| 2 | **Kalajengking Gurun Emas** | Spirit Beast | Tier 2 (Qi Gath) | 115 | 26 | LV 2 | *Sengatan Kelumpuhan Pasir*. | Sengat Pasir, Core T1 |
| 3 | **Kobra Pasir Emas** | Spirit Beast | Tier 3 (Found) | 390 | 82 | LV 3 | *Patukan Racun Pasir Panas*. | Kulit Kobra Pasir, Core T2 |
| 4 | **Cacing Pasir Raksasa** | Spirit Beast | Tier 4 (Golden C) | 1.500 | 250 | LV 4 | *Pusaran Telan Pasir*: Memendam mangsa.| Kulit Cacing Gurun, Core T3 |
| 5 | **Sprite Pasir Emas (*Dust*)** | Sprite / Roh | Tier 4 (Golden C) | 750 | 210 | LV 4 | *Badai Pasir Buta*: Reduce Hit Chance.| Esensi Pasir Emas |
| 6 | **Srigala Pasir Emas Purba** | Spirit Beast | Tier 5 (Nascent S) | 4.400 | 670 | LV 5 | Pergerakan cepat di atas bukit pasir. | Kulit Serigala Pasir, Core T4 |
| 7 | **Banteng Batu Pasir Emas** | Spirit Beast | Tier 6 (Spirit Form) | 22.000 | 2.700 | LV 6 | *Benteng Dinding Batu Pasir*. | Tanduk Batu Pasir, Core T5 |
| 8 | **Raksasa Pasir Gurun Purba** | Elemental Boss | Tier 7 (Void Trans) | 96.000 | 13.500 | LV 8 | *Badai Pasir Raksasa AoE*. | Hati Batu Gurun, Core T6 |
| 9 | **Naga Pasir Emas Purba** | Apex Guardian | Tier 8 (Tribulation) | 405.000 | 51.000 | LV 9 | *Gempa Gurun Pasir Abadi*. | Sisik Naga Pasir, Core T7 |
| 10 | **Penguasa Gurun Pasir Huangji** | Sovereign Guardian| Tier 9 (Sovereign) | 2.020.000 | 250.000 | Mustahil | *Penguburan Pasir Abadi Alam Semesta*.| Esensi Pasir Emas Huangji |

---

### ☣️ 3.7 Rawa Kabut Racun (Shadow Mist Swamp) — Elemen Racun & Kabut

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Katak Lendir Rawa** | Wild Beast | Tier 0 (Fana) | 30 | 5 | LV 1 | Menembakkan asam ringan. | Daging Katak Rawa |
| 2 | **Nyamuk Kabut Beracun** | Insect / Gu | Tier 1 (Body Ref) | 50 | 12 | LV 1 | Menyerang dalam kawanan pekat. | Kelenjar Nyamuk Racun |
| 3 | **Katak Teratai Hitam** | Spirit Beast | Tier 3 (Found) | 390 | 80 | LV 3 | *Semburan Lendir Asam Pekat*. | Lendir Katak, Core T2 |
| 4 | **Sprite Kabut Miasma (*Poison*)**| Sprite / Roh | Tier 3 (Found) | 220 | 85 | LV 3 | Menghirup kabut memicu Poison. | Kelenjar Miasma Murni |
| 5 | **Ular Piton Kabut Racun** | Spirit Beast | Tier 4 (Golden C) | 1.350 | 225 | LV 4 | *Lilitan Beracun Miasma*. | Kulit Piton Racun, Core T3 |
| 6 | **Lintah Rawa Raksasa** | Spirit Beast | Tier 5 (Nascent S) | 4.700 | 690 | LV 5 | *Penghisapan Darah & HP*. | Lendir Lintah Purba, Core T4 |
| 7 | **Buaya Rawa Teratai Hitam** | Spirit Beast | Tier 6 (Spirit Form) | 20.500 | 2.550 | LV 6 | *Gigitan Putaran Kematian*. | Kulit Buaya Racun, Core T5 |
| 8 | **Hydra Rawa Sembilan Kepala** | Spirit Boss | Tier 7 (Void Trans) | 98.000 | 14.000 | LV 8 | **Memiliki 9 Kepala (Menyerang 9x)**.| Darah Hydra Purba, Core T6 |
| 9 | **Naga Racun Miasma Purba** | Apex Guardian | Tier 8 (Tribulation) | 425.000 | 56.000 | LV 9 | *Hujan Miasma Racun Mematikan*. | Sisik Naga Racun, Core T7 |
| 10 | **Penguasa Miasma Teratai Hitam**| Sovereign Guardian| Tier 9 (Sovereign) | 2.120.000 | 268.000 | Mustahil | *Penyebaran Racun Kematian Semesta*. | Esensi Racun Teratai Huangji |

---

### 🏔️ 3.8 Puncak Langit Surgawi (Celestial Sky Peaks) — Elemen Angin Langit

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Burung Merpati Awan** | Wild Beast | Tier 0 (Fana) | 20 | 4 | LV 1 | Terbang sangat tinggi di celah tebing. | Bulu Merpati Awan |
| 2 | **Musang Angin Puncak** | Spirit Beast | Tier 2 (Qi Gath) | 95 | 22 | LV 2 | *Gerakan Angin Cepat*. | Bulu Musang Angin, Core T1 |
| 3 | **Burung Rajawali Angin Tajam**| Spirit Beast | Tier 4 (Golden C) | 1.100 | 210 | LV 4 | *Tebasan Badai Angin*. | Bulu Angin Tajam, Core T3 |
| 4 | **Sprite Angin Awan (*Sylph*)** | Sprite / Roh | Tier 4 (Golden C) | 800 | 240 | LV 5 | Move speed +50% (Sangat lincah). | Esensi Angin Langit |
| 5 | **Monyet Badai Puncak Awan** | Spirit Beast | Tier 5 (Nascent S) | 4.300 | 660 | LV 5 | *Lemparan Pusaran Angin Tajam*. | Kulit Monyet Angin, Core T4 |
| 6 | **Gryphon Angin Langit Purba** | Spirit Beast | Tier 6 (Spirit Form) | 18.500 | 2.350 | LV 6 | *Sabetan Sayap Badai Angin*. | Paruh Gryphon Kuno, Core T5 |
| 7 | **Elang Raksasa Puncak Surgawi**| Spirit Beast | Tier 7 (Void Trans) | 87.000 | 11.200 | LV 7 | *Pusaran Badai Angin AoE*. | Bulu Elang Purba, Core T6 |
| 8 | **Kirin Angin Langit Purba** | Apex Guardian | Tier 8 (Tribulation) | 395.000 | 49.000 | LV 9 | *Tornando Angin Tajam Abadi*. | Tanduk Kirin Angin, Core T7 |
| 9 | **Naga Angin Langit Surgawi** | Apex Guardian | Tier 8 (Tribulation) | 415.000 | 53.000 | LV 9 | *Penebasan Badai Langit Purba*. | Sisik Naga Angin, Core T7 |
| 10 | **Penguasa Angin Langit Huangji**| Sovereign Guardian| Tier 9 (Sovereign) | 1.980.000 | 248.000 | Mustahil | *Badai Pemotong Keabadian Semesta*.| Esensi Angin Langit Huangji |

---

### 🌊 3.9 Kepulauan Palung Samudra (Oceanic Abyss Islands) — Elemen Samudra

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Ikan Terbang Pantai** | Wild Beast | Tier 0 (Fana) | 20 | 3 | LV 1 | Melompat di atas permukaan air laut. | Daging Ikan Terbang |
| 2 | **Mutiara Kerang Air** | Wild Beast | Tier 1 (Body Ref) | 90 | 10 | LV 1 | Cangkang keras menutup rapat. | Mutiara Air, Daging Kerang |
| 3 | **Kepiting Batu Karang Laut** | Spirit Beast | Tier 2 (Qi Gath) | 130 | 27 | LV 2 | *Cengkeraman Supit Besi Laut*. | Supit Kepiting, Core T1 |
| 4 | **Ular Laut Pusaran Mutiara** | Spirit Beast | Tier 3 (Found) | 410 | 88 | LV 3 | *Semburan Pusaran Air Pekat*. | Kulit Ular Laut, Core T2 |
| 5 | **Sprite Air Samudra (*Naiad*)** | Sprite / Roh | Tier 4 (Golden C) | 820 | 230 | LV 4 | Mengendalikan arus dan gelombang laut.| Esensi Air Murni |
| 6 | **Hiu Palung Laut Purba** | Spirit Beast | Tier 5 (Nascent S) | 4.900 | 710 | LV 5 | *Tandukan Sirip Pembunuh Laut*. | Sirip Hiu Purba, Core T4 |
| 7 | **Gurita Palung Samudra** | Spirit Beast | Tier 5 (Nascent S) | 3.800 | 450 | LV 5 | *Cengkeraman Sembilan Tentakel*. | Tinta Gurita Murni, Core T4 |
| 8 | **Cumi-Cumi Raksasa Palung** | Spirit Boss | Tier 7 (Void Trans) | 94.000 | 12.800 | LV 8 | *Gelombang Tsunami Palung Laut*. | Mata Cumi Purba, Core T6 |
| 9 | **Naga Samudra Purba Huangji** | Apex Guardian | Tier 8 (Tribulation) | 435.000 | 57.000 | LV 9 | *Ledakan Pasang Lautan Abadi*. | Sisik Naga Samudra, Core T7 |
| 10 | **Penguasa Palung Samudra Abadi**| Sovereign Guardian| Tier 9 (Sovereign) | 2.180.000 | 275.000 | Mustahil | *Penenggelaman Alam Semesta*. | Esensi Samudra Agung Huangji |

---

### 🏛️ 3.10 Ibu Kota Agung Huangji (Capital & Royal Hunting Grounds)

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama | Drop Loot |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Kuda Perang Kerajaan** | Mount / Beast | Tier 1 (Body Ref) | 100 | 15 | LV 1 | Daya tahan lari jarak jauh tinggi. | Zirah Kuda Kerajaan |
| 2 | **Burung Merpati Surat Istana** | Wild Beast | Tier 0 (Fana) | 20 | 2 | LV 1 | Terbang cepat membawa berita istana. | Bulu Merpati Istana |
| 3 | **Anjing Pemburu Kekaisaran** | Spirit Beast | Tier 2 (Qi Gath) | 110 | 25 | LV 2 | *Pelacakan Jejak Qi Murni*. | Kulit Anjing Pemburu, Core T1 |
| 4 | **Rusa Emas Istana Huangji** | Spirit Beast | Tier 3 (Found) | 370 | 75 | LV 3 | Berlari kencang di taman kekaisaran.| Tanduk Emas Istana, Core T2 |
| 5 | **Sprite Emas Istana (*Auric*)** | Sprite / Roh | Tier 4 (Golden C) | 850 | 250 | LV 4 | Pancaran Aura Kepemimpinan Emas. | Esensi Emas Istana |
| 6 | **Harimau Emas Kekaisaran** | Spirit Beast | Tier 5 (Nascent S) | 4.500 | 670 | LV 5 | *Aura Auric Pressure Istana*. | Kulit Harimau Emas, Core T4 |
| 7 | **Gajah Perang Zirah Besi** | Spirit Beast | Tier 6 (Spirit Form) | 23.000 | 2.800 | LV 6 | *Tandukan Zirah Gajah Perang*. | Tading Gajah Besi, Core T5 |
| 8 | **Burung Garuda Emas Istana** | Spirit Beast | Tier 7 (Void Trans) | 91.000 | 12.200 | LV 8 | *Kepakan Sayap Emas Kekaisaran*. | Bulu Garuda Emas, Core T6 |
| 9 | **Kirin Emas Kekaisaran** | Apex Guardian | Tier 8 (Tribulation) | 380.000 | 47.000 | LV 9 | Pembawa berkah Tahta Emas Huangji. | Tanduk Kirin Emas, Core T7 |
| 10 | **Pengawal Naga Tahta Emas** | Sovereign Guardian| Tier 9 (Sovereign) | 2.000.000 | 250.000 | Mustahil | *Perlindungan Abadi Tahta Huangji*.| Esensi Tahta Emas Huangji |

---

## 🛡️ 4. Checklist Validasi AI GM (Wajib Diperiksa Tiap Turn)

- [ ] Apakah statistik HP dan Attack Power monster sesuai dengan tabel katalog Tier 0–9 di atas?
- [ ] Apakah habitat dan lokasi kemunculan monster tervalidasi dengan peta wilayah pemain?
- [ ] Apakah Sprite/Roh diberi properti imun serangan fisik murni jika belum diserang dengan senjata Qi/Elemen?
- [ ] Apakah drop loot hasil pertarungan telah dicatat di *Item Origin Log* pada Profil Karakter pemain?
