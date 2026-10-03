# 🐉 Huangji-World — Bestiary & Katalog Spesies Spirit (Monster, Spirit Beast, Sprite & Apex Guardians)

> **Modul:** 16 — Bestiary & Monster System
> **Prinsip:** Anti-Cheat Enforced — Habitat-Locked — Terintegrasi dengan Sistem HP, Combat, Taming, & Item Origin Log
> **Rujukan Utama:** [`INDEX.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/INDEX.md?v=1)
> **Rujukan Silang:**
> - [`00_CORE_RULES_AI_GM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/00_CORE_RULES_AI_GM.md?v=1) (Aturan Wajib AI GM)
> - [`12_CULTIVATION_LAW_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/12_CULTIVATION_LAW_SYSTEM.md?v=1) (Tingkat Ranah & Qi Cap)
> - [`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1) (Nilai Loot, Core, & Item Origin Log)
> - [`14_VITALITY_HUNGER_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/14_VITALITY_HUNGER_SYSTEM.md?v=1) (HP, Stamina & Status Effek)
> - [`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1) (Damage Formula & Turn Order)
> - [`18_TAMING_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/18_TAMING_SYSTEM.md?v=1) (Mekanik Penjinakan & Success Rate)
> - [`19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1) (Pengolahan Core & Bahan Crafting)

---

## 📜 0. Filosofi & Aturan Emas Bestiary

Dunia Benua Huangji dihuni oleh jutaan spesies makhluk hidup spiritual dan binatang liar — mulai dari **Binatang Fana / Wild Beast (Tier 0)**, **Spirit Beast (Tier 1–7)**, **Sprite / Roh Elemen**, **Undead / Spirit Rangka**, hingga **Makhluk Purba Apex (*Apex Guardian Beasts*, Tier 8–9)**. Setiap spesies terikat pada hukum alam, kepadatan Qi lingkungan, dan ekosistem wilayah tempat mereka bertumbuh.

### 🛡️ Aturan Emas Anti-Cheat Bestiary
1. **Habitat-Locked**: Monster terikat pada habitat resminya. Pemain dilarang mendatangkan atau menemui monster di luar ekosistem resminya (misalnya menemukan Naga Lahar di Danau Es) tanpa alasan naratif luar biasa yang divalidasi AI GM.
2. **Kalkulasi Terbuka AI GM**: Statistik HP dan Attack Power monster telah ditentukan berdasarkan tingkat Tier dan Ranah Setara. AI GM wajib memakai statistik baku pada katalog ini tanpa mengubah angka secara sepihak.
3. **Validasi Ambush Murni**: Pemain tidak boleh menentukan sendiri kapan monster muncul atau tidak muncul. AI GM melakukan roll *AmbushChance* secara objektif saat perjalanan atau eksplorasi.
4. **Pencatatan Item Origin Log**: Loot hasil buruan tidak sah digunakan atau dijual sebelum dicatat di **Item Origin Log** (`[Nama Loot | Grade/Rarity | Sumber: Nama Monster, Wilayah X | Timestamp]`).

---

## 🎲 1. Formula Ambush & Formasi Encounter

Serangan mendadak (*Ambush*) dan kemunculan monster di medan liar dihitung menggunakan formula:

$$\text{AmbushChance} = \text{BaseChance (5\%)} \times \text{DangerModifier} \times \text{TimeModifier} \times \text{NoiseModifier}$$

### 📊 Tabel Modifier Kemunculan Monster

| Faktor Lingkungan / Kondisi | Kategori Lingkungan | Modifier (`DangerModifier`) | Catatan Operasional AI GM |
|---|---|:---:|---|
| **Area Pemukiman / Kota** | Dalam Ibu Kota Huangji / Benteng Sekte Utama | **×0,1** | Hanya Spirit Beast peliharaan atau penyerangan khusus. |
| **Jalan Utama / Jalur Dagang** | Jalur Kuda & Pos Penjagaan Kekaisaran | **×0,5** | Tingkat patroli tinggi, ancaman monster relatif rendah. |
| **Hutan / Pegunungan Normal** | Pinggiran Hutan Kayu / Perbukitan Hijau | **×1,0** | Ekosistem standar, monster Tier 1–3 sering dijumpai. |
| **Zona Liar / Rawa / Gurun** | Hutan Purba / Rawa Kabut Miasma / Gurun Pasir | **×2,0** | Daerah tidak terjamah, ancaman kelompok & monster aktif. |
| **Zona Terlarang / Kawah Lahar**| Lembah Api Vulkanik / Kawah Lahar / Palung Laut | **×4,0** | Wilayah mematikan, peluang kemunculan Boss & Tier 5+. |

### 🕒 Modifier Waktu (`TimeModifier`) & Kebisingan (`NoiseModifier`)
* **Siang Hari**: `TimeModifier = ×1,0`
* **Malam Hari / Badai**: `TimeModifier = ×2,0` (Monster bertipe Yin/Bayangan/Kegelapan 2x lebih aktif dan agresif).
* **Perjalanan Senyap (Stealth)**: `NoiseModifier = ×0,5`
* **Perjalanan Berisik / Bertarung**: `NoiseModifier = ×2,0` (Mengundang monster terdekat mendekat ke lokasi).

---

## 💎 2. Sistem Drop Loot & Rarity Rate

Setiap kali monster dikalahkan secara sah dalam pertempuran naratif, AI GM melakukan roll keberuntungan (*Loot Drop Roll*) berdasarkan tingkat kelangkaan (*Rarity Rate*):

$$\text{LootDropRate} = \text{BaseDropRate(Rarity)} \times \text{LootModifier}$$

| Rarity Loot | Base Drop Rate | Deskripsi & Contoh Item | Penanganan Log & Transaksi |
|---|:---:|---|---|
| **Umum (Common)** | **70% – 90%** | Bahan dasar tubuh monster: Kulit kasar, taring, daging fana/spirit, bulu, cakar biasa, serpihan batu. | Dicatat di Inventory. Dapat dijual ke pedagang umum atau dimasak. |
| **Jarang (Rare)** | **20% – 40%** | Organ spiritual & esensi: Inti Qi Elemen (*Spirit Core T1–T5*), kelenjar racun murni, sisik keras, empedu bertuah. | Bahan baku utama Alkimia Tier 1–5 & Tempa Senjata Grade 2–3. |
| **Legendaris (Legendary)** | **5% – 15%** *(100% pada Kill Pertama Apex)* | Pusaka purba, Darah Naga, Tanduk Kirin, Inti Jiwa Purba (Tier 6–9), Kristal Hukum Alam. | Membutuhkan *Item Origin Log* khusus. Bahan Alkimia/Tempa Tingkat Atas. |

📌 **Aturan Anti-Cheat Loot**: Tanpa pencatatan di *Item Origin Log* pada Profil Karakter, item loot dianggap **Tidak Sah** dan dilarang digunakan untuk breakthrough kultivasi atau dijual di Paviliun Lelang.

---

## 🌐 3. Spesies Umum Lintas Wilayah (Universal / Cross-Region Beasts)

Spesies umum ini mendiami hampir seluruh belahan Benua Huangji dari pedesaan hingga batas hutan liar (Tier 0 s/d Tier 5):

| Nama Spesies | Kategori Jenis | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Deskripsi Naratif | Drop Loot Utama (Umum / Jarang / Legendaris) |
|---|:---:|:---:|:---:|:---:|:---:|---|---|
| **Ayam Hutan Fana** | 🐓 Avian | Tier 0 (Fana) | 25 | 4 | LV 1 | Pemakan serangga tanah. Berisik saat terkejut, memicu perhatian predator. | **U:** Daging Ayam (+10% Satiety) <br>**J:** Bulu Unggul <br>**L:** - |
| **Kelinci Padang Rumput** | 🐇 Beast | Tier 0 (Fana) | 30 | 5 | LV 1 | Sangat lincah, bersembunyi di lubang tanah saat mendengar langkah kaki. | **U:** Daging Kelinci (+10% Satiety) <br>**J:** Kulit Kelinci Lembut <br>**L:** - |
| **Katak Air Fana** | 🐸 Amphibian | Tier 0 (Fana) | 20 | 3 | LV 1 | Menghuni tepian sungai fana. Suaranya menjadi petunjuk keberadaan air. | **U:** Daging Katak (+10% Satiety) <br>**J:** Lendir Bening <br>**L:** - |
| **Babi Hutan Taring Besi** | 🐗 Beast | Tier 1 (Body Ref) | 90 | 18 | LV 1 | *Serudukan Lurus*: Menyeruduk target dengan taring ganda keras sekeras besi. | **U:** Daging Babi (+25% Satiety) <br>**J:** Taring Besi T1 <br>**L:** Core Spirit T1 |
| **Serigala Kelabu Liar** | 🐺 Spirit Beast | Tier 1 (Body Ref) | 85 | 20 | LV 1 | Berburu dalam kelompok (3–5 ekor). Menggunakan taktik *Mencakar & Menggigit*. | **U:** Kulit Serigala Kasar <br>**J:** Taring Serigala Tajam <br>**L:** Core Spirit T1 |
| **Ular Sawah Hijau** | 🐍 Serpent | Tier 1 (Body Ref) | 60 | 15 | LV 1 | Bersembunyi di semak-semak. *Patukan Beracun Ringan* (Debuff Poison 1 Turn). | **U:** Kulit Ular Hijau <br>**J:** Kantong Empedu Ular <br>**L:** Core Spirit T1 |
| **Elang Pengembara** | 🦅 Avian | Tier 1 (Body Ref) | 75 | 16 | LV 1 | Menukik tajam dari udara. *Sabetan Cakar Udara* (Mengabaikan 10% Armor). | **U:** Bulu Elang <br>**J:** Paruh Keras <br>**L:** Core Spirit T1 |
| **Kera Hutan Cokelat** | 🐒 Beast | Tier 1 (Body Ref) | 80 | 14 | LV 1 | Lemparan buah keras & batu dari dahan pohon. Cerdik dan suka mencuri pakan. | **U:** Kulit Kera Cokelat <br>**J:** Buah Hutan Bertuah <br>**L:** Core Spirit T1 |
| **Gagak Malam Berbintang**| 🦅 Avian | Tier 1 (Body Ref) | 50 | 12 | LV 1 | Aktif malam hari. *Kekek Gelisah* (Gagal Stealth bagi karakter yang lewat). | **U:** Bulu Gagak Hitam <br>**J:** Mata Gagak Malam <br>**L:** Core Spirit T1 |
| **Bunglon Bayang Lintas** | 🦎 Reptile | Tier 2 (Qi Gath) | 130 | 32 | LV 2 | *Kamuflase Sempurna*: Menjadi tidak terlihat selama 2 Turn (Dodge +40%). | **U:** Kulit Bunglon <br>**J:** Esens Kamuflase <br>**L:** Core Spirit T2 |
| **Kelelawar Darah Malam** | 🦇 Avian/Beast | Tier 2 (Qi Gath) | 110 | 28 | LV 2 | *Penghisapan Darah*: Menyerap 20% Damage yang dihasilkan sebagai HP. | **U:** Sayap Kelelawar <br>**J:** Taring Penghisap Darah <br>**L:** Core Spirit T2 |
| **Kelabang Kerangka Hitam**| 🐛 Insect/Gu | Tier 2 (Qi Gath) | 125 | 35 | LV 2 | *Racun Kelumpuhan*: Menginfeksi racun yang memberi debuff Slow -20% (2 Turn). | **U:** Cangkang Kelabang <br>**J:** Kelenjar Racun Paralis <br>**L:** Core Spirit T2 |
| **Laba-Laba Sutra Jingga** | 🕷️ Insect | Tier 3 (Found) | 380 | 85 | LV 3 | *Jaring Penjerat Qi*: Mengunci pergerakan target (Stun 1 Turn). | **U:** Benang Sutra Spirit <br>**J:** Kelenjar Penjerat <br>**L:** Core Spirit T3 |
| **Serigala Bayangan Tanduk**| 🐺 Spirit Beast| Tier 3 (Found) | 420 | 95 | LV 3 | *Tandukan Qi Bayangan*: Penetrasi Defense Murni sebesar 25%. | **U:** Kulit Serigala Tanduk <br>**J:** Tanduk Bayangan <br>**L:** Core Spirit T3 |
| **Piton Batu Raksasa** | 🐍 Serpent | Tier 3 (Found) | 450 | 90 | LV 3 | *Lilitan Pemutus Tulang*: Memberikan Bleeding Damage 15 HP/Turn. | **U:** Sisik Piton Batu <br>**J:** Empedu Piton Raksasa <br>**L:** Core Spirit T3 |
| **Macan Tutul Angin Malam**| 🐆 Spirit Beast| Tier 4 (Golden C)| 1.300 | 240 | LV 4 | *Kecepatan Angin*: Move Speed +40%, Critical Hit Chance +25%. | **U:** Kulit Macan Angin <br>**J:** Cakar Badai Angin <br>**L:** Core Spirit T4 |
| **Kadal Lahar Karat** | 🦎 Elemental | Tier 4 (Golden C)| 1.450 | 230 | LV 4 | *Aura Api Kerak*: Membakar lawan yang menyerang jarak dekat (+20 Burn Damage). | **U:** Sisik Lahar Karat <br>**J:** Inti Api Karat <br>**L:** Core Spirit T4 |
| **Elang Badai Petir Purba**| 🦅 Avian | Tier 5 (Nascent S)| 4.600 | 680 | LV 5 | *Sabetan Badai Petir*: Attack AoE Elemen Petir dengan efek Stun 1 Turn. | **U:** Bulu Elang Badai <br>**J:** Paruh Petir Purba <br>**L:** Core Spirit T5 |
| **Banteng Batu Dinding** | 🐂 Spirit Beast| Tier 5 (Nascent S)| 5.200 | 620 | LV 5 | *Tembok Batu Abadi*: Defense Murni +150 saat mengaktifkan mode bertahan. | **U:** Tanduk Banteng Batu <br>**J:** Kulit Batu Abadi <br>**L:** Core Spirit T5 |

---

## 📖 4. Katalog Lengkap Monster & Spirit Beast per 10 Wilayah (Tier 0 s/d 9)

---

### 🌿 4.1 Dataran Hijau Abadi (Verdant Qi Plains) — Elemen Kayu & Vitalitas
*(Rujukan Peta Wilayah: [`02_VERDANT_QI_PLAINS.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/02_VERDANT_QI_PLAINS.md?v=1))*

Dataran kaya Qi Kayu yang dipenuhi hutan purba, padang rumput hijau, dan perbukitan tenang. Monster di sini didominasi spesies flora, herbivora spiritual, dan penjaga akar purba.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Rusa Kayu Duri** | Wild Beast | Tier 0 (Fana) | 35 | 6 | LV 1 | Berlari kencang saat terancam. *Tandukan Duri Ringan*. | **U:** Daging Rusa Fana <br>**J:** Tanduk Kayu Duri <br>**L:** - |
| 2 | **Peri Bunga Embun (*Dew Sprite*)** | Sprite / Roh | Tier 1 (Body Ref) | 80 | 12 | LV 2 | **Imun fisik murni**. *Sentuhan Penyembuh*: Memulihkan +15 HP ke sekutu. | **U:** Esensi Bunga Embun <br>**J:** Serbuk Embun Murni <br>**L:** Core Spirit T1 |
| 3 | **Serigala Akar Hijau** | Spirit Beast | Tier 2 (Qi Gath) | 120 | 25 | LV 2 | *Gigitan Duri Kayu*: Menyergap dari semak-semak, memicu efek Slow 10%. | **U:** Kulit Serigala Hijau <br>**J:** Taring Akar Kayu <br>**L:** Core Spirit T2 |
| 4 | **Beruang Kayu Kuno** | Spirit Beast | Tier 3 (Found) | 450 | 80 | LV 3 | *Hantaman Batang Jati*: Tamparan keras memicu efek Stun 1 Turn. | **U:** Empedu Beruang Jati <br>**J:** Cakar Kayu Kuno <br>**L:** Core Spirit T3 |
| 5 | **Ular Sanca Daun Hijau** | Spirit Beast | Tier 4 (Golden C) | 1.200 | 220 | LV 4 | *Melilit Vitalitas*: Menguras 30 Stamina & HP target per Turn. | **U:** Kulit Sanca Hijau <br>**J:** Empedu Sanca Purba <br>**L:** Core Spirit T4 |
| 6 | **Sprite Pohon Purba (*Treant*)** | Sprite / Roh | Tier 5 (Nascent S) | 4.500 | 650 | LV 5 | *Akar Penjerat Alam*: Mengunci 3 target sekaligus selama 2 Turn. | **U:** Kayu Purba Vitalitas <br>**J:** Teras Pohon Spirit <br>**L:** Core Spirit T5 |
| 7 | **Rusa Bambu Pelangi** | Spirit Beast | Tier 6 (Spirit Form) | 18.000 | 2.200 | LV 6 | *Langkah Embun Suci*: Agility +50%, menciptakan ilusi bayangan rusa. | **U:** Tanduk Bambu Pelangi <br>**J:** Darah Rusa Pelangi <br>**L:** Core Spirit T6 |
| 8 | **Kera Raksasa Hutan Purba** | Spirit Beast | Tier 7 (Void Trans) | 90.000 | 12.000 | LV 7 | *Pukulan Badai Kayu*: Serangan AoE meremukkan tanah & pertahanan. | **U:** Tangan Kera Purba <br>**J:** Jantung Kera Raksasa <br>**L:** Core Spirit T7 |
| 9 | **Naga Kayu Suci Abadi** | Apex Guardian | Tier 8 (Tribulation) | 400.000 | 50.000 | LV 9 | *Restorasi Alam Abadi*: Mengubah Qi Kayu menjadi regenerasi HP 5%/Turn. | **U:** Sisik Naga Kayu <br>**J:** Darah Naga Vitalitas <br>**L:** Core Naga Kayu T8 |
| 10 | **Dewa Pohon Suci Huangji** | Sovereign Guardian| Tier 9 (Sovereign) | 2.000.000 | 250.000 | Mustahil | *Hukuman Akar Alam Semesta*: Menghancurkan Dantian & raga penyusup. | **U:** Kayu Dewa Suci <br>**J:** Teras Pohon Huangji <br>**L:** Esensi Pohon Suci Huangji |

---

### ⚡ 4.2 Pegunungan Petir Guntur (Thunder Crest Range) — Elemen Petir & Logam
*(Rujukan Peta Wilayah: [`03_THUNDER_CREST_RANGE.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/03_THUNDER_CREST_RANGE.md?v=1))*

Wilayah tebing terjal bertanduk tembaga dan perak tempat kilat menyambar sepanjang tahun. Monster di sini memiliki ketahanan fisik tinggi dan serangan kejut saraf (*Paralysis*).

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Tikus Kilat Tembaga** | Wild Beast | Tier 0 (Fana) | 25 | 5 | LV 1 | Menghasilkan percikan kejut kecil saat disentuh. | **U:** Daging Tikus Tembaga <br>**J:** Bulu Tembaga <br>**L:** - |
| 2 | **Ular Besi Tembaga** | Spirit Beast | Tier 2 (Qi Gath) | 100 | 30 | LV 2 | *Patukan Listrik*: Sisik tembaga keras memantulkan 10% Physical Damage. | **U:** Sisik Tembaga Keras <br>**J:** Taring Besi Kilat <br>**L:** Core Spirit T2 |
| 3 | **Roh Kilat Ungu (*Volt Sprite*)**| Sprite / Roh | Tier 2 (Qi Gath) | 90 | 35 | LV 3 | *Paralysis Shock*: Memicu efek kelumpuhan saraf target (Stun 1 Turn). | **U:** Percikan Esensi Petir <br>**J:** Kristal Kilat Ungu <br>**L:** Core Spirit T2 |
| 4 | **Elang Kilat Ungu** | Spirit Beast | Tier 3 (Found) | 380 | 95 | LV 3 | Menukik cepat dari puncak gunung. *Sabetan Paruh Listrik*. | **U:** Bulu Kilat Ungu <br>**J:** Cakar Tembaga Spirit <br>**L:** Core Spirit T3 |
| 5 | **Macan Tutul Logam Guntur** | Spirit Beast | Tier 4 (Golden C) | 1.300 | 230 | LV 4 | *Cakar Logam Guntur*: Menembus 30% Armor Zirah target. | **U:** Kulit Macan Logam <br>**J:** Taring Guntur Perak <br>**L:** Core Spirit T4 |
| 6 | **Banteng Besi Badai Petir** | Spirit Beast | Tier 5 (Nascent S) | 4.800 | 700 | LV 5 | *Tandukan Guntur*: Memicu efek Daze/Pusing (-30% Accuracy musuh). | **U:** Tanduk Besi Badai <br>**J:** Kulit Besi Petir <br>**L:** Core Spirit T5 |
| 7 | **Rajawali Petir Emas** | Spirit Beast | Tier 6 (Spirit Form) | 20.000 | 2.500 | LV 6 | *Sabetan Kilat Emas*: Damage Petir AoE yang membakar meridian Qi. | **U:** Bulu Petir Emas <br>**J:** Paruh Emas Guntur <br>**L:** Core Spirit T6 |
| 8 | **Kirin Logam Guntur Purba** | Apex Guardian | Tier 7 (Void Trans) | 95.000 | 13.000 | LV 8 | *Hujan Sambaran Petir Ungu*: Menjadikan medan pertempuran zona petir. | **U:** Tanduk Kirin Logam <br>**J:** Sisik Kirin Guntur <br>**L:** Core Spirit T7 |
| 9 | **Naga Petir Ungu Surgawi** | Apex Guardian | Tier 8 (Tribulation) | 420.000 | 55.000 | LV 9 | *Palu Petir Tribulasi Surgawi*: Menyambar dengan kekuatan petir langit. | **U:** Sisik Naga Petir <br>**J:** Darah Naga Guntur <br>**L:** Core Naga Petir T8 |
| 10 | **Penguasa Kilat Alam Semesta** | Sovereign Guardian| Tier 9 (Sovereign) | 2.100.000 | 260.000 | Mustahil | *Hukuman Petir Keabadian*: Ledakan petir pemusnah jiwa dan fisik. | **U:** Logam Dewa Petir <br>**J:** Inti Kilat Surgawi <br>**L:** Esensi Petir Agung Huangji |

---

### 🔥 4.3 Lembah Api Merah (Crimson Blaze Valley) — Elemen Api & Vulkanik
*(Rujukan Peta Wilayah: [`04_CRIMSON_BLAZE_VALLEY.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/04_CRIMSON_BLAZE_VALLEY.md?v=1))*

Lembah jurang lahar mendidih tempat api spiritual dan abu vulkanik membakar udara. Monster di sini kebal api dan memberikan efek status *Burn* beruntun.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Kadal Abu Vulkanik** | Wild Beast | Tier 0 (Fana) | 30 | 6 | LV 1 | Berenang di atas batuan hangat kawah lahar. Tahan panas sedang. | **U:** Kulit Kadal Abu <br>**J:** Daging Kadal Hangat <br>**L:** - |
| 2 | **Kalajengking Api Merah** | Spirit Beast | Tier 2 (Qi Gath) | 110 | 28 | LV 2 | *Sengatan Bara Api*: Memicu status Burn (10 Damage/Turn selama 2 Turn). | **U:** Sengat Api Merah <br>**J:** Cangkang Vulkanik <br>**L:** Core Spirit T2 |
| 3 | **Salamander Magma** | Spirit Beast | Tier 3 (Found) | 400 | 85 | LV 3 | *Semburan Lahar*: Memicu Burn & melelehkan durability senjata fisik. | **U:** Kulit Tahan Api <br>**J:** Darah Magma Murni <br>**L:** Core Spirit T3 |
| 4 | **Sprite Api Vulkanik (*Lava Flame*)**| Sprite / Roh | Tier 3 (Found) | 250 | 110 | LV 3 | **Meledak saat mati**: Memberikan Fire Damage AoE 100 HP ke sekeliling. | **U:** Esensi Api Merah <br>**J:** Bunga Api Vulkanik <br>**L:** Core Spirit T3 |
| 5 | **Kera Api Purba** | Spirit Beast | Tier 4 (Golden C) | 1.200 | 220 | LV 4 | *Hujan Batu Lahar*: Melempar pecahan batu membara dari jarak jauh. | **U:** Tangan Kera Api <br>**J:** Taring Api Purba <br>**L:** Core Spirit T4 |
| 6 | **Serigala Lahar Vulkanik** | Spirit Beast | Tier 5 (Nascent S) | 4.200 | 680 | LV 5 | *Aura Pembakar Dantian*: Mengurangi 20 Qi musuh per Turn yang mendekat. | **U:** Kulit Serigala Lahar <br>**J:** Taring Lahar Murni <br>**L:** Core Spirit T5 |
| 7 | **Ular Piton Kawah Merah** | Spirit Beast | Tier 6 (Spirit Form) | 17.500 | 2.300 | LV 6 | *Semburan Api Vulkanik Pekat*: Menyemburkan lidah api sejauh 20 meter. | **U:** Sisik Piton Api <br>**J:** Kantong Api Piton <br>**L:** Core Spirit T6 |
| 8 | **Burung Feniks Api Lahar** | Apex Guardian | Tier 7 (Void Trans) | 110.000 | 19.500 | LV 8 | **Reborn 1x saat HP 0%**: Pulih kembali dengan 50% HP Max. | **U:** Bulu Feniks Api <br>**J:** Darah Feniks Murni <br>**L:** Core Spirit T7 |
| 9 | **Naga Lahar Purba Vulkanik** | Apex Guardian | Tier 8 (Tribulation) | 410.000 | 52.000 | LV 9 | *Gelombang Tsunami Magma*: Melalap seluruh area pertarungan dengan lahar. | **U:** Sisik Naga Lahar <br>**J:** Jantung Naga Lahar <br>**L:** Core Naga Lahar T8 |
| 10 | **Dewa Api Tungku Huangji** | Sovereign Guardian| Tier 9 (Sovereign) | 2.050.000 | 255.000 | Mustahil | *Pembakaran Esensi Alam Semesta*: Mereduksi Defense & Qi target jadi 0. | **U:** Batu Inti Api Dewa <br>**J:** Serbuk Tungku Suci <br>**L:** Esensi Api Tungku Huangji |

---

### ❄️ 4.4 Danau Es Bintang (Frost Star Lake) — Elemen Es & Air Pembeku
*(Rujukan Peta Wilayah: [`05_FROST_STAR_LAKE.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/05_FROST_STAR_LAKE.md?v=1))*

Danau luas yang tertutup lapisan es abadi bercahaya bintang. Monster di sini menguasai pembekuan air (*Freeze*) dan pengurangan Agility/Speed musuh.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Ikan Perak Es** | Wild Beast | Tier 0 (Fana) | 25 | 3 | LV 1 | Sisik transparan bening. Sangat lezat dimasak (+15% Satiety). | **U:** Daging Ikan Es <br>**J:** Sisik Perak Bening <br>**L:** - |
| 2 | **Rubah Es Bintang** | Spirit Beast | Tier 2 (Qi Gath) | 105 | 24 | LV 2 | *Hembusan Salju Pembeku*: Memicu efek Slow -15% pada pergerakan musuh. | **U:** Bulu Rubah Es <br>**J:** Taring Es Bintang <br>**L:** Core Spirit T2 |
| 3 | **Hiu Es Kristal** | Spirit Beast | Tier 3 (Found) | 420 | 90 | LV 3 | *Tandukan Sirip Es*: Menyeruduk dari dalam air dan memicu Freeze 1 Turn. | **U:** Sirip Hiu Es <br>**J:** Gigi Hiu Kristal <br>**L:** Core Spirit T3 |
| 4 | **Sprite Kristal Bintang (*Frost*)**| Sprite / Roh | Tier 3 (Found) | 280 | 85 | LV 3 | *Dinding Es Pembeku*: Menciptakan perisai es yang menyerap 150 Damage. | **U:** Esensi Es Kristal <br>**J:** Pelet Bintang Es <br>**L:** Core Spirit T3 |
| 5 | **Beruang Kutub Es Bintang** | Spirit Beast | Tier 4 (Golden C) | 1.400 | 215 | LV 4 | *Tamparan Es Kristal*: Tamparan keras dengan probabilitas Slow 30%. | **U:** Kulit Beruang Es <br>**J:** Cakar Es Bintang <br>**L:** Core Spirit T4 |
| 6 | **Serigala Kristal Salju Purba**| Spirit Beast | Tier 5 (Nascent S) | 4.600 | 660 | LV 5 | *Aura Pembeku Miasma Es*: Mengurangi Health Regeneration musuh 50%. | **U:** Taring Serigala Es <br>**J:** Kulit Kristal Salju <br>**L:** Core Spirit T5 |
| 7 | **Ular Laut Bintang Pembeku** | Spirit Beast | Tier 6 (Spirit Form) | 19.000 | 2.400 | LV 6 | *Semburan Napas Pembeku Abadi*: Membekukan musuh dalam balok es (Stun 2 Turn). | **U:** Sisik Ular Es <br>**J:** Empedu Ular Bintang <br>**L:** Core Spirit T6 |
| 8 | **Burung Rajawali Es Bintang** | Spirit Beast | Tier 7 (Void Trans) | 88.000 | 11.500 | LV 7 | *Badai Salju Bintang Pembeku*: Serangan badai es AoE ber radius luas. | **U:** Bulu Rajawali Es <br>**J:** Paruh Es Bintang <br>**L:** Core Spirit T7 |
| 9 | **Naga Es Kristal Purba** | Apex Guardian | Tier 8 (Tribulation) | 390.000 | 48.000 | LV 9 | *Pembekuan Lautan Abadi*: Menghentikan aliran Qi & pergerakan seluruh lawan. | **U:** Sisik Naga Es <br>**J:** Darah Naga Kristal <br>**L:** Core Naga Es T8 |
| 10 | **Penguasa Es Bintang Abadi** | Sovereign Guardian| Tier 9 (Sovereign) | 1.950.000 | 245.000 | Mustahil | *Pembekuan Waktu & Alam Semesta*: Membekukan waktu dan raga musuh. | **U:** Kristal Es Abadi <br>**J:** Inti Salju Huangji <br>**L:** Esensi Es Bintang Huangji |

---

### 💀 4.5 Tanah Gersang Tulang (Desolate Bone Wasteland) — Elemen Jiwa & Kegelapan
*(Rujukan Peta Wilayah: [`06_DESOLATE_BONE_WASTELAND.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/06_DESOLATE_BONE_WASTELAND.md?v=1))*

Padang gersang berisi reruntuhan perang purba dan kuburan massa. Monster di sini berupa mahluk Undead, spirit rangka, dan pemangsa jiwa ber racun *Yin*.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Gagak Jiwa Kelabu** | Wild Beast | Tier 0 (Fana) | 20 | 4 | LV 1 | Hinggap di atas tulang bangkai. Menghisap sisa aura kematian. | **U:** Bulu Gagak Kelabu <br>**J:** Paruh Gagak Kuno <br>**L:** - |
| 2 | **Tikus Rangka Tulang** | Undead Beast | Tier 1 (Body Ref) | 65 | 14 | LV 1 | Berburu dalam koloni besar (10+ ekor). Menggerogoti kaki target. | **U:** Tulang Tikus Kuno <br>**J:** Tengkorak Tikus Spirit <br>**L:** Core Spirit T1 |
| 3 | **Kalajengking Tulang Kelabu** | Insect / Gu | Tier 3 (Found) | 360 | 75 | LV 3 | *Sengatan Racun Jiwa*: Mengabaikan Physical Armor (True Damage Jiwa). | **U:** Sengat Kalajengking <br>**J:** Cangkang Tulang Kelabu <br>**L:** Core Spirit T3 |
| 4 | **Sprite Jiwa Kelabu (*Soul Wisp*)**| Sprite / Roh | Tier 3 (Found) | 200 | 95 | Tidak Bisa | *Jeritan Jiwa*: Menyerang Dantian secara langsung (Mereduksi 40 Qi). | **U:** Esensi Jiwa Kelabu <br>**J:** Api Spirit Kematian <br>**L:** Core Spirit T3 |
| 5 | **Serigala Tulang Rangka** | Undead Beast | Tier 4 (Golden C) | 1.400 | 210 | LV 4 | **Imun racun & pendarahan**. Struktur tulang keras memantulkan serangan. | **U:** Tulang Serigala Kuno <br>**J:** Taring Rangka Kelabu <br>**L:** Core Spirit T4 |
| 6 | **Naga Rangka Tulang Kelabu** | Undead Beast | Tier 5 (Nascent S) | 5.000 | 720 | LV 5 | *Semburan Kabut Kematian*: Menyemburkan racun busuk penguras Vitalitas. | **U:** Tulang Naga Kuno <br>**J:** Tengkorak Naga Spirit <br>**L:** Core Spirit T5 |
| 7 | **Prajurit Rangka Purba** | Undead / Skeleton| Tier 6 (Spirit Form) | 21.000 | 2.600 | Tidak Bisa | Menggunakan pedang bertuah kuno dengan teknik bertarung masa lalu. | **U:** Pedang Rangka Kuno <br>**J:** Zirah Rangka Purba <br>**L:** Core Spirit T6 |
| 8 | **Raja Tulang Jiwa Kelabu** | Undead Boss | Tier 7 (Void Trans) | 92.000 | 12.500 | LV 8 | *Panggilan Seribu Rangka*: Membangkitkan 5 prajurit rangka tiap 3 Turn. | **U:** Mahkota Tulang Kuno <br>**J:** Tongkat Jiwa Kelabu <br>**L:** Core Spirit T7 |
| 9 | **Iblis Jiwa Kelabu Purba** | Apex Guardian | Tier 8 (Tribulation) | 430.000 | 58.000 | LV 9 | *Penyedotan Jiwa Abadi*: Menyerap 10% HP & Qi musuh di medan tempur. | **U:** Kristal Jiwa Purba <br>**J:** Tangan Iblis Kematian <br>**L:** Core Jiwa Purba T8 |
| 10 | **Penguasa Kehampaan Kematian** | Sovereign Guardian| Tier 9 (Sovereign) | 2.150.000 | 270.000 | Mustahil | *Hukuman Musnah Jiwa Huangji*: Menghapus kesadaran & raga musuh. | **U:** Tulang Dewa Kematian <br>**J:** Permata Jiwa Hampa <br>**L:** Esensi Jiwa Kematian Huangji |

---

### 🏜️ 4.6 Gurun Pasir Emas (Golden Sand Desert) — Elemen Pasir & Tanah
*(Rujukan Peta Wilayah: [`07_GOLDEN_SAND_DESERT.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/07_GOLDEN_SAND_DESERT.md?v=1))*

Lautan pasir panas yang bergulung dengan ancaman badai pasir buta dan monster penggali tanah.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Kadal Pasir Gurun** | Wild Beast | Tier 1 (Body Ref) | 70 | 15 | LV 1 | Bersembunyi di dalam pasir panas untuk melancarkan penyergapan mendadak. | **U:** Daging Kadal Pasir <br>**J:** Kulit Pasir Keras <br>**L:** - |
| 2 | **Kalajengking Gurun Emas** | Spirit Beast | Tier 2 (Qi Gath) | 115 | 26 | LV 2 | *Sengatan Kelumpuhan Pasir*: Menyuntikkan racun lumpuh (Slow -25%). | **U:** Sengat Pasir Emas <br>**J:** Cangkang Gurun T2 <br>**L:** Core Spirit T2 |
| 3 | **Kobra Pasir Emas** | Spirit Beast | Tier 3 (Found) | 390 | 82 | LV 3 | *Patukan Racun Pasir Panas*: Menyebabkan racun pendarahan & dehidrasi. | **U:** Kulit Kobra Pasir <br>**J:** Empedu Kobra Emas <br>**L:** Core Spirit T3 |
| 4 | **Cacing Pasir Raksasa** | Spirit Beast | Tier 4 (Golden C) | 1.500 | 250 | LV 4 | *Pusaran Telan Pasir*: Memendam mangsa ke dalam pasir (Stun 1 Turn). | **U:** Kulit Cacing Gurun <br>**J:** Gigi Cacing Pasir <br>**L:** Core Spirit T4 |
| 5 | **Sprite Pasir Emas (*Dust*)** | Sprite / Roh | Tier 4 (Golden C) | 750 | 210 | LV 4 | *Badai Pasir Buta*: Mereduksi Hit Chance musuh sebesar 40% (2 Turn). | **U:** Esensi Pasir Emas <br>**J:** Permata Pasir Murni <br>**L:** Core Spirit T4 |
| 6 | **Serigala Pasir Emas Purba** | Spirit Beast | Tier 5 (Nascent S) | 4.400 | 670 | LV 5 | Pergerakan sangat cepat di atas bukit pasir. *Cakaran Badai Pasir*. | **U:** Kulit Serigala Pasir <br>**J:** Taring Pasir Emas <br>**L:** Core Spirit T5 |
| 7 | **Banteng Batu Pasir Emas** | Spirit Beast | Tier 6 (Spirit Form) | 22.000 | 2.700 | LV 6 | *Benteng Dinding Batu Pasir*: Meningkatkan Defense fisik sebesar +200. | **U:** Tanduk Batu Pasir <br>**J:** Kulit Benteng Gurun <br>**L:** Core Spirit T6 |
| 8 | **Raksasa Pasir Gurun Purba** | Elemental Boss | Tier 7 (Void Trans) | 96.000 | 13.500 | LV 8 | *Badai Pasir Raksasa AoE*: Menciptakan pusaran pasir pemusnah area. | **U:** Hati Batu Gurun <br>**J:** Inti Pasir Purba <br>**L:** Core Spirit T7 |
| 9 | **Naga Pasir Emas Purba** | Apex Guardian | Tier 8 (Tribulation) | 405.000 | 51.000 | LV 9 | *Gempa Gurun Pasir Abadi*: Mengguncang tanah & mengubur musuh hidup-hidup. | **U:** Sisik Naga Pasir <br>**J:** Darah Naga Gurun <br>**L:** Core Naga Pasir T8 |
| 10 | **Penguasa Gurun Pasir Huangji** | Sovereign Guardian| Tier 9 (Sovereign) | 2.020.000 | 250.000 | Mustahil | *Penguburan Pasir Abadi Alam Semesta*: Mengubah area pertarungan jadi gurun hampa. | **U:** Batu Inti Gurun <br>**J:** Debu Pasir Suci <br>**L:** Esensi Pasir Emas Huangji |

---

### ☣️ 4.7 Rawa Kabut Racun (Shadow Mist Swamp) — Elemen Racun & Kabut
*(Rujukan Peta Wilayah: [`08_SHADOW_MIST_SWAMP.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/08_SHADOW_MIST_SWAMP.md?v=1))*

Rawa berlumpur hitam yang diselimuti gas Miasma beracun dan tumbuhan parasit.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Katak Lendir Rawa** | Wild Beast | Tier 0 (Fana) | 30 | 5 | LV 1 | Menembakkan lendir asam ringan dari jarak 3 meter. | **U:** Daging Katak Rawa <br>**J:** Lendir Asam Ringan <br>**L:** - |
| 2 | **Nyamuk Kabut Beracun** | Insect / Gu | Tier 1 (Body Ref) | 50 | 12 | LV 1 | Menyerang dalam kawanan pekat. Mengakibatkan gatal & luka kecil. | **U:** Kelenjar Nyamuk Racun <br>**J:** Sayap Nyamuk Spirit <br>**L:** Core Spirit T1 |
| 3 | **Katak Teratai Hitam** | Spirit Beast | Tier 3 (Found) | 390 | 80 | LV 3 | *Semburan Lendir Asam Pekat*: Memicu status Poison (15 HP Damage/Turn). | **U:** Lendir Katak Hitam <br>**J:** Empedu Teratai Rawa <br>**L:** Core Spirit T3 |
| 4 | **Sprite Kabut Miasma (*Poison*)**| Sprite / Roh | Tier 3 (Found) | 220 | 85 | LV 3 | Miasma beracun sekitar memicu Poison otomatis saat didekati. | **U:** Kelenjar Miasma Murni <br>**J:** Esensi Kabut Racun <br>**L:** Core Spirit T3 |
| 5 | **Ular Piton Kabut Racun** | Spirit Beast | Tier 4 (Golden C) | 1.350 | 225 | LV 4 | *Lilitan Beracun Miasma*: Mengombinasikan efek fisik & debuff Poison. | **U:** Kulit Piton Racun <br>**J:** Kelenjar Piton Rawa <br>**L:** Core Spirit T4 |
| 6 | **Lintah Rawa Raksasa** | Spirit Beast | Tier 5 (Nascent S) | 4.700 | 690 | LV 5 | *Penghisapan Darah & HP*: Menyerap 25% Damage sebagai pemulihan HP. | **U:** Lendir Lintah Purba <br>**J:** Mulut Penghisap Lintah <br>**L:** Core Spirit T5 |
| 7 | **Buaya Rawa Teratai Hitam** | Spirit Beast | Tier 6 (Spirit Form) | 20.500 | 2.550 | LV 6 | *Gigitan Putaran Kematian*: Damage Murni + efek Bleeding parah. | **U:** Kulit Buaya Racun <br>**J:** Gigi Buaya Teratai <br>**L:** Core Spirit T6 |
| 8 | **Hydra Rawa Sembilan Kepala** | Spirit Boss | Tier 7 (Void Trans) | 98.000 | 14.000 | LV 8 | **Memiliki 9 Kepala**: Menyerang 9x per Turn dengan elemen racun/asam berbeda. | **U:** Darah Hydra Purba <br>**J:** Kulit Hydra Sembilan <br>**L:** Core Spirit T7 |
| 9 | **Naga Racun Miasma Purba** | Apex Guardian | Tier 8 (Tribulation) | 425.000 | 56.000 | LV 9 | *Hujan Miasma Racun Mematikan*: Menyiramkan hujan racun ke seluruh area. | **U:** Sisik Naga Racun <br>**J:** Kantong Racun Purba <br>**L:** Core Naga Racun T8 |
| 10 | **Penguasa Miasma Teratai Hitam**| Sovereign Guardian| Tier 9 (Sovereign) | 2.120.000 | 268.000 | Mustahil | *Penyebaran Racun Kematian Semesta*: Mereduksi HP Max lawan secara permanen. | **U:** Teratai Hitam Suci <br>**J:** Esensi Miasma Agung <br>**L:** Esensi Racun Teratai Huangji |

---

### 🏔️ 4.8 Puncak Langit Surgawi (Celestial Sky Peaks) — Elemen Angin Langit
*(Rujukan Peta Wilayah: [`09_CELESTIAL_SKY_PEAKS.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/09_CELESTIAL_SKY_PEAKS.md?v=1))*

Puncak-puncak gunung pencakar langit bertutup awan tempat badai angin tajam bertiup tanpa henti.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Burung Merpati Awan** | Wild Beast | Tier 0 (Fana) | 20 | 4 | LV 1 | Terbang sangat tinggi di celah tebing. Sulit ditangkap tanpa busur. | **U:** Bulu Merpati Awan <br>**J:** Daging Merpati Segar <br>**L:** - |
| 2 | **Musang Angin Puncak** | Spirit Beast | Tier 2 (Qi Gath) | 95 | 22 | LV 2 | *Gerakan Angin Cepat*: Agility tinggi, memicu efek Evasion +20%. | **U:** Bulu Musang Angin <br>**J:** Taring Musang Puncak <br>**L:** Core Spirit T2 |
| 3 | **Burung Rajawali Angin Tajam**| Spirit Beast | Tier 4 (Golden C) | 1.100 | 210 | LV 4 | *Tebasan Badai Angin*: Melepaskan tebasan pisau angin dari sayap. | **U:** Bulu Angin Tajam <br>**J:** Cakar Rajawali Puncak <br>**L:** Core Spirit T4 |
| 4 | **Sprite Angin Awan (*Sylph*)** | Sprite / Roh | Tier 4 (Golden C) | 800 | 240 | LV 5 | Move speed +50%. Sering meluncur dengan hembusan angin puncak. | **U:** Esensi Angin Langit <br>**J:** Kristal Awan Murni <br>**L:** Core Spirit T4 |
| 5 | **Monyet Badai Puncak Awan** | Spirit Beast | Tier 5 (Nascent S) | 4.300 | 660 | LV 5 | *Lemparan Pusaran Angin Tajam*: Melempar pusaran angin bertekanan tinggi. | **U:** Kulit Monyet Angin <br>**J:** Taring Monyet Badai <br>**L:** Core Spirit T5 |
| 6 | **Gryphon Angin Langit Purba** | Spirit Beast | Tier 6 (Spirit Form) | 18.500 | 2.350 | LV 6 | *Sabetan Sayap Badai Angin*: Menghasilkan angin topan ber radius sedang. | **U:** Paruh Gryphon Kuno <br>**J:** Sayap Gryphon Spirit <br>**L:** Core Spirit T6 |
| 7 | **Elang Raksasa Puncak Surgawi**| Spirit Beast | Tier 7 (Void Trans) | 87.000 | 11.200 | LV 7 | *Pusaran Badai Angin AoE*: Menjatuhkan musuh dari ketinggian tebing. | **U:** Bulu Elang Purba <br>**J:** Cakar Elang Surgawi <br>**L:** Core Spirit T7 |
| 8 | **Kirin Angin Langit Purba** | Apex Guardian | Tier 8 (Tribulation) | 395.000 | 49.000 | LV 9 | *Tornado Angin Tajam Abadi*: Menciptakan badai topan permanen di area. | **U:** Tanduk Kirin Angin <br>**J:** Sisik Kirin Surgawi <br>**L:** Core Spirit T8 |
| 9 | **Naga Angin Langit Surgawi** | Apex Guardian | Tier 8 (Tribulation) | 415.000 | 53.000 | LV 9 | *Penebasan Badai Langit Purba*: Memotong pertahanan raga dengan bilah angin. | **U:** Sisik Naga Angin <br>**J:** Darah Naga Langit <br>**L:** Core Naga Angin T8 |
| 10 | **Penguasa Angin Langit Huangji**| Sovereign Guardian| Tier 9 (Sovereign) | 1.980.000 | 248.000 | Mustahil | *Badai Pemotong Keabadian Semesta*: Penebasan angin yang merobek dimensi. | **U:** Kristal Angin Dewa <br>**J:** Permata Awan Suci <br>**L:** Esensi Angin Langit Huangji |

---

### 🌊 4.9 Kepulauan Palung Samudra (Oceanic Abyss Islands) — Elemen Samudra
*(Rujukan Peta Wilayah: [`10_OCEANIC_ABYSS_ISLANDS.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/10_OCEANIC_ABYSS_ISLANDS.md?v=1))*

Gugusan pulau karang dan palung laut dalam yang dipenuhi gelombang raksasa dan monster perairan.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Ikan Terbang Pantai** | Wild Beast | Tier 0 (Fana) | 20 | 3 | LV 1 | Melompat melintasi permukaan air laut. Mangsa populer nelayan. | **U:** Daging Ikan Terbang <br>**J:** Sisik Ikan Laut <br>**L:** - |
| 2 | **Mutiara Kerang Air** | Wild Beast | Tier 1 (Body Ref) | 90 | 10 | LV 1 | Cangkang sangat keras. Menutup rapat saat tersentuh bahaya. | **U:** Daging Kerang Laut <br>**J:** Mutiara Air Fana <br>**L:** Core Spirit T1 |
| 3 | **Kepiting Batu Karang Laut** | Spirit Beast | Tier 2 (Qi Gath) | 130 | 27 | LV 2 | *Cengkeraman Supit Besi Laut*: Menjepit target dengan supit keras. | **U:** Supit Kepiting Karang <br>**J:** Cangkang Batu Laut <br>**L:** Core Spirit T2 |
| 4 | **Ular Laut Pusaran Mutiara** | Spirit Beast | Tier 3 (Found) | 410 | 88 | LV 3 | *Semburan Pusaran Air Pekat*: Menyemburkan pusaran air bertekanan tinggi. | **U:** Kulit Ular Laut <br>**J:** Mutiara Pusaran Air <br>**L:** Core Spirit T3 |
| 5 | **Sprite Air Samudra (*Naiad*)** | Sprite / Roh | Tier 4 (Golden C) | 820 | 230 | LV 4 | Mengendalikan arus air dan menciptakan pusaran perlindungan. | **U:** Esensi Air Murni <br>**J:** Permata Air Samudra <br>**L:** Core Spirit T4 |
| 6 | **Hiu Palung Laut Purba** | Spirit Beast | Tier 5 (Nascent S) | 4.900 | 710 | LV 5 | *Tandukan Sirip Pembunuh Laut*: Memicu efek Bleeding parah pada target. | **U:** Sirip Hiu Purba <br>**J:** Gigi Hiu Palung <br>**L:** Core Spirit T5 |
| 7 | **Gurita Palung Samudra** | Spirit Beast | Tier 5 (Nascent S) | 3.800 | 450 | LV 5 | *Cengkeraman Sembilan Tentakel*: Membelit target dan menyemprotkan tinta membutakan. | **U:** Tentakel Gurita Laut <br>**J:** Tinta Gurita Murni <br>**L:** Core Spirit T5 |
| 8 | **Cumi-Cumi Raksasa Palung** | Spirit Boss | Tier 7 (Void Trans) | 94.000 | 12.800 | LV 8 | *Gelombang Tsunami Palung Laut*: Menghancurkan kapal & zona daratan pantai. | **U:** Mata Cumi Purba <br>**J:** Paruh Cumi Raksasa <br>**L:** Core Spirit T7 |
| 9 | **Naga Samudra Purba Huangji** | Apex Guardian | Tier 8 (Tribulation) | 435.000 | 57.000 | LV 9 | *Ledakan Pasang Lautan Abadi*: Menciptakan gelombang pasang raksasa. | **U:** Sisik Naga Samudra <br>**J:** Darah Naga Samudra <br>**L:** Core Naga Samudra T8 |
| 10 | **Penguasa Palung Samudra Abadi**| Sovereign Guardian| Tier 9 (Sovereign) | 2.180.000 | 275.000 | Mustahil | *Penenggelaman Alam Semesta*: Menenggelamkan seluruh daratan ke dasar laut. | **U:** Batu Inti Samudra <br>**J:** Permata Palung Suci <br>**L:** Esensi Samudra Agung Huangji |

---

### 🏛️ 4.10 Ibu Kota Agung Huangji (Capital & Royal Hunting Grounds)
*(Rujukan Peta Wilayah: [`01_WORLD_OVERVIEW_AND_CAPITAL.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/01_WORLD_OVERVIEW_AND_CAPITAL.md?v=1))*

Wilayah pusat kekaisaran, taman perburuan kerajaan, dan benteng pertahanan istana agung.

| # | Nama Makhluk | Kategori | Tier (Ranah Setara) | HP | Atk Power | Taming LV | Kemampuan Utama & Pola Bertarung | Drop Loot Utama (Umum / Jarang / Legendaris) |
|:---:|---|:---:|:---:|:---:|:---:|:---:|---|---|
| 1 | **Kuda Perang Kerajaan** | Mount / Beast | Tier 1 (Body Ref) | 100 | 15 | LV 1 | Daya tahan lari jarak jauh sangat tinggi. Terlatih dalam kavaleri. | **U:** Kulit Kuda Perang <br>**J:** Zirah Kuda Kerajaan <br>**L:** - |
| 2 | **Burung Merpati Surat Istana** | Wild Beast | Tier 0 (Fana) | 20 | 2 | LV 1 | Terbang cepat membawa pesan rahasia istana. | **U:** Bulu Merpati Istana <br>**J:** Tabung Surat Perak <br>**L:** - |
| 3 | **Anjing Pemburu Kekaisaran** | Spirit Beast | Tier 2 (Qi Gath) | 110 | 25 | LV 2 | *Pelacakan Jejak Qi Murni*: Mampu melacak jejak kultivator yang bersembunyi. | **U:** Kulit Anjing Pemburu <br>**J:** Taring Anjing Istana <br>**L:** Core Spirit T2 |
| 4 | **Rusa Emas Istana Huangji** | Spirit Beast | Tier 3 (Found) | 370 | 75 | LV 3 | Berlari kencang di taman kekaisaran. Memiliki aura aura keemasan. | **U:** Tanduk Emas Istana <br>**J:** Kulit Rusa Emas <br>**L:** Core Spirit T3 |
| 5 | **Sprite Emas Istana (*Auric*)** | Sprite / Roh | Tier 4 (Golden C) | 850 | 250 | LV 4 | Pancaran Aura Kepemimpinan Emas (Buff Defense +20% untuk penguasa). | **U:** Esensi Emas Istana <br>**J:** Permata Auric Murni <br>**L:** Core Spirit T4 |
| 6 | **Harimau Emas Kekaisaran** | Spirit Beast | Tier 5 (Nascent S) | 4.500 | 670 | LV 5 | *Auric Pressure Istana*: Memicu intimidasi aura kekaisaran (Fear 1 Turn). | **U:** Kulit Harimau Emas <br>**J:** Taring Emas Kekaisaran <br>**L:** Core Spirit T5 |
| 7 | **Gajah Perang Zirah Besi** | Spirit Beast | Tier 6 (Spirit Form) | 23.000 | 2.800 | LV 6 | *Tandukan Zirah Gajah Perang*: Menghancurkan barisan pertahanan musuh. | **U:** Gading Gajah Besi <br>**J:** Zirah Gajah Perang <br>**L:** Core Spirit T6 |
| 8 | **Burung Garuda Emas Istana** | Spirit Beast | Tier 7 (Void Trans) | 91.000 | 12.200 | LV 8 | *Kepakan Sayap Emas Kekaisaran*: Menghasilkan angin kencang ber aura emas. | **U:** Bulu Garuda Emas <br>**J:** Paruh Garuda Kekaisaran <br>**L:** Core Spirit T7 |
| 9 | **Kirin Emas Kekaisaran** | Apex Guardian | Tier 8 (Tribulation) | 380.000 | 47.000 | LV 9 | Pembawa berkah Tahta Emas Huangji. *Aura Kebijaksanaan Emas*. | **U:** Tanduk Kirin Emas <br>**J:** Sisik Kirin Kekaisaran <br>**L:** Core Spirit T8 |
| 10 | **Pengawal Naga Tahta Emas** | Sovereign Guardian| Tier 9 (Sovereign) | 2.000.000 | 250.000 | Mustahil | *Perlindungan Abadi Tahta Huangji*: Membentengi Istana Agung dari serangan. | **U:** Sisik Naga Emas <br>**J:** Inti Tahta Huangji <br>**L:** Esensi Tahta Emas Huangji |

---

## 🏞️ 5. Sub-Zona Risiko Tinggi & Ekosistem Khusus

Di setiap wilayah Benua Huangji, terdapat sub-zona bahaya tinggi (*High-Danger Sub-Zones*) tempat kepadatan Qi liar berlipat ganda, memicu tingkat kemunculan monster yang sangat agresif:

### 🌿 5.1 Sub-Zona Dataran Hijau Abadi — *Hutan Kayu Purba Abadi*
- **Karakteristik**: Pohon-pohon raksasa berumur ribuan tahun dengan akar yang saling melilit.
- **Daftar Penghuni Utama**: *Sprite Pohon Purba (T5)*, *Kera Raksasa Hutan Purba (T7)*, *Naga Kayu Suci Abadi (T8)*.
- **Efek Lingkungan**: Regenerasi HP monster bertipe Kayu meningkat +10% per Turn.

### ⚡ 5.2 Sub-Zona Pegunungan Petir Guntur — *Puncak Sambaran Guntur*
- **Karakteristik**: Puncak batu tembaga yang disambar kilat ungu secara terus-menerus.
- **Daftar Penghuni Utama**: *Roh Kilat Ungu (T2)*, *Rajawali Petir Emas (T6)*, *Naga Petir Ungu Surgawi (T8)*.
- **Efek Lingkungan**: Setiap 2 Turn, terjadi sambaran petir acak yang memberikan 50 Lightning Damage ke pemain tanpa perlindungan logam/jimat.

### 🔥 5.3 Sub-Zona Lembah Api Merah — *Kawah Lahar Mendidih*
- **Karakteristik**: Danau lahar cair berdinding batu obsidian panas.
- **Daftar Penghuni Utama**: *Salamander Magma (T3)*, *Serigala Lahar Vulkanik (T5)*, *Naga Lahar Purba Vulkanik (T8)*.
- **Efek Lingkungan**: Karakter tanpa obat penghangat/perlindungan es menderita -10 Stamina & status *Burn* per Turn.

---

## 👑 6. Monster Apex Guardian & Boss Langka Lintas Wilayah (Rare / Boss Tier 7–9)

Monster tipe ini berstatus **Apex Guardians** atau **World-Level Bosses**. Mereka menjaga rahasia kuno, gua rahasia (*Secret Realms*), atau urat naga spiritual utama Benua Huangji.

| Nama Apex Boss | Tier (Ranah Setara) | HP | Atk Power | Habitat & Ekosistem Utama | Kemampuan Utama & Mekanik Unik | Drop Loot Legendaris (100% Unique Kill) |
|---|:---:|:---:|:---:|---|---|---|
| **Bayangan Tanpa Wujud** | Tier 5 (Menengah) | 5.625 | 4.218 | Berkelana acak di zona-zona gelap seluruh dunia (hutan malam, reruntuhan, rawa kabut). | **Teleportasi Bayangan**: Menghilang saat HP di bawah 50% jika tidak diisolasi oleh Array Segel. | *Esens Bayangan Murni (T4)* + *Kristal Melintas Dimensi*. |
| **Naga Kabut Purba** | Tier 8 (Tribulation) | 1.562.500 | 421.875 | Bersemayam di ruang hampa udara antara *Puncak Langit Surgawi* & *Secret Realms*. | **Domain Kabut Hampa**: Membutakan seluruh indra musuh & menetralisir 50% Damage Jurus Elemen. | *Sisik Naga Kabut Purba (T8)* + *Insight Point +2* untuk seluruh peserta fight. |
| **Feniks Kegelapan** | Tier 8 (Tribulation) | 1.562.500 | 421.875 | Kawah Gunung Api Terlarang di *Lembah Api Merah*. | **Api Hitam Pemusnah Dantian**: Menghancurkan 200 Qi Max target secara permanen jika tidak diobati. | *Bulu Feniks Kegelapan (T8)* + *Inti Api Hitam Keabadian*. |
| **Naga Samudra Purba** | Tier 8 (Tribulation) | 1.562.500 | 421.875 | Palung Terdalam *Kepulauan Palung Samudra*. | **Tsunami Pemusnah Alam**: Menyapu seluruh medan tempur dengan damage air bertekanan maha dahsyat. | *Sisik Naga Samudra Purba (T8)* + *Mutiara Samudra Agung (T9)*. |
| **Kura-Kura Giok Purba** | Tier 7 (Void Trans) | 390.625 | 56.250 | Dasar Danau *Frost Star Lake*. | **Tempurung Giok Tak Tertembus**: Kebal terhadap Physical Damage di bawah 1.000 Attack Power. | *Cangkang Kura-Kura Giok (T7)* + *Batu Inti Pertahanan Abadi*. |

---

## 🔄 7. Integrasi Sistem dengan Modul Lain

Dokumen Bestiary ini terhubung langsung secara teknis dan naratif dengan modul-modul utama Huangji-World:

1. **Sistem Hukum Kultivasi & Qi Cap** ([`12_CULTIVATION_LAW_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/12_CULTIVATION_LAW_SYSTEM.md?v=1)):
   - Statistik HP & Attack Power monster dipetakan langsung dari batas Qi Cap dan formula multiplier per Ranah.
   - Core dan organ Spirit Beast Tier 3+ menjadi syarat bahan breakthrough kultivasi untuk teknik elemen spesifik.
2. **Sistem Ekonomi & Loot** ([`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1)):
   - Nilai perunggu, perak, dan Batu Spiritual dari penjualan organ monster wajib mengikuti tabel harga pasar.
   - Semua item hasil buruan wajib dicatat di **Item Origin Log** sebelum dapat ditransaksikan.
3. **Sistem HP, Stamina & Status Effect** ([`14_VITALITY_HUNGER_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/14_VITALITY_HUNGER_SYSTEM.md?v=1)):
   - Daging hasil buruan memberikan efek pemulihan *Satiety* (Kelaparan) dan pemulihan HP berlanjut.
   - Serangan debuff monster (*Burn, Freeze, Poison, Paralysis*) diproses dengan formula status effect yang baku.
4. **Sistem Pertarungan Turn-Based** ([`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1)):
   - Attack Power dan HP monster pada katalog ini langsung dimasukkan ke dalam perhitungan Turn Order dan Damage Resolution.
5. **Sistem Penjinakan Beast** ([`18_TAMING_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/18_TAMING_SYSTEM.md?v=1)):
   - Kolom *Taming LV* pada tabel menunjukkan syarat tingkat keahlian taming dan jenis jimat segel yang dibutuhkan.
6. **Alkimia, Tempa & Formasi** ([`19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1)):
   - Core Spirit Beast (Tier 1–9) berfungsi sebagai katalis pembentukan pil alkimia dan penguat struktur tempa senjata.

---

## 📊 8. Ringkasan Statistik Monster per Wilayah

| Wilayah Geografis | Total Spesies Katalog | Monster Tier Tertinggi | Karakteristik Utama Ekosistem |
|:---|:---:|:---:|:---|
| **Spesies Umum Lintas Wilayah** | 19 Spesies | Tier 5 (Nascent Soul) | Tersebar di pedesaan, jalur umum, dan hutan sekunder. |
| **01. Dataran Hijau Abadi** | 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Kayu, regenerasi vitalitas, dan flora purba. |
| **02. Pegunungan Petir Guntur** | 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Petir & Logam, efek kelumpuhan kejut (*Paralysis*). |
| **03. Lembah Api Merah** | 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Api & Vulkanik, serangan debuff pembakar (*Burn*). |
| **04. Danau Es Bintang** | 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Es & Air Pembeku, pembekuan raga (*Freeze* & Slow). |
| **05. Tanah Gersang Tulang** | 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Jiwa & Kegelapan, mahluk Undead & True Damage Jiwa. |
| **06. Gurun Pasir Emas** | 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Pasir & Tanah, jebakan pasir isap & dehidrasi. |
| **07. Rawa Kabut Racun** | 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Racun & Miasma, debuff racun bertumpuk (*Poison*). |
| **08. Puncak Langit Surgawi** | 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Angin Langit, serangan topan & tebasan angin. |
| **09. Kepulauan Palung Samudra**| 10 Spesies | Tier 9 (Sovereign Guardian) | Elemen Samudra & Air Dalam, gulungan ombak & tsunami. |
| **10. Ibu Kota Agung Huangji** | 10 Spesies | Tier 9 (Sovereign Guardian) | Hewan kavaleri, aura kepemimpinan keemasan, & Kirin. |
| **Apex Boss Lintas Wilayah** | 5 Spesies | Tier 8–9 (Tribulation/Sovereign) | Penjaga rahasia dunia, habitat khusus & dimensi hampa. |

---

## 🛠️ 9. Panduan Operasional AI GM & Contoh Skenario Pertarungan (Step-by-Step)

### 9.1 Langkah-Langkah Eksekusi AI GM Saat Menangani Encounter Monster

1. **Penetapan Lokasi & Habitat**: AI GM memeriksa posisi pemain pada peta wilayah. Pilih monster dari katalog yang ber habitat di lokasi tersebut.
2. **Kalkulasi Roll Ambush**:
   - Hitung `AmbushChance = 5% × DangerModifier × TimeModifier × NoiseModifier`.
   - Lakukan roll `1d100`. Jika angka roll $\le \text{AmbushChance}$, pertarungan dimulai secara mendadak (*Surprise Attack*).
3. **Pengambilan Data Stat Baku**:
   - Ambil nilai HP, Attack Power, dan Kemampuan Utama monster secara persis dari tabel Katalog §4.
4. **Eksekusi Pertarungan Turn-Based**:
   - Jalankan alur pertarungan sesuai aturan [`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1).
   - Terapkan efek status effect (Burn, Freeze, Poison, Paralysis) secara terbuka pada log giliran.
5. **Kalkulasi Drop Loot & Item Origin Log**:
   - Setelah monster kalah (HP 0), AI GM melakukan roll Rarity Drop (§2).
   - Cetak entri **Item Origin Log** ke dalam profil inventory pemain secara otomatis.

---

### 📝 9.2 Contoh Skenario Pertarungan Lengkap (Naratif & Mekanis)

**Konteks Skenario**:
Pemain bernama **Li Wei** (Ranah Pengumpulan Qi / Tier 2, HP Max: 350, Qi: 120) sedang melintasi *Hutan Purba Dataran Hijau Abadi* di malam hari (`DangerModifier = ×2,0`, `TimeModifier = ×2,0`).

---

#### 🎲 Step 1: Roll Ambush & Inisiasi Encounter
* **Kalkulasi AI GM**:
  $$\text{AmbushChance} = 5\% \times 2,0 (\text{Zona Liar}) \times 2,0 (\text{Malam Hari}) \times 1,0 (\text{Jalan Biasa}) = 20\%$$
* **Roll 1d100**: Hasil = **14** (Sukses Ambush!).
* **Naratif AI GM**:
  > *"Malam semakin pekat di Hutan Purba Dataran Hijau Abadi. Dedaunan bergoyang hebat saat bayangan hijau melompat dari semak-semak Duri! Seekor **Serigala Akar Hijau (Tier 2 Spirit Beast)** muncul dengan taring berlapis duri tajam melompat menyergapmu!"*
* **Statistik Monster**:
  - **Nama**: Serigala Akar Hijau (Tier 2)
  - **HP**: 120 / 120
  - **Attack Power**: 25
  - **Kemampuan**: *Gigitan Duri Kayu* (Debuff Slow -10%)

---

#### ⚔️ Step 2: Turn 1 — Serangan Mendadak Monster
* **Aksi Monster**: Serigala Akar Hijau melancarkan *Gigitan Duri Kayu*.
* **Hit & Damage Calculation**:
  - Attack Power = 25. Li Wei menggunakan Zirah Kain (Defense = 5).
  - Net Damage = $25 - 5 = 20 \text{ HP}$.
  - HP Li Wei berkurang menjadi **330 / 350**. Li Wei terkena debuff *Slow -10%*.
* **Aksi Pemain**: Li Wei membalas dengan *Tebasan Pedang Angin* (Damage Base 60, Konsumsi 15 Qi).
  - Damage ke Monster = $60 - 0 \text{ (Defense Spirit)} = 60 \text{ Damage}$.
  - HP Serigala Akar Hijau berkurang menjadi **60 / 120**.

---

#### ⚔️ Step 3: Turn 2 — Penuntasan Pertarungan
* **Aksi Monster**: Serigala Akar Hijau mencakar dengan panik (Attack Power = 25).
  - Net Damage = $25 - 5 = 20 \text{ HP}$.
  - HP Li Wei berkurang menjadi **310 / 350**.
* **Aksi Pemain**: Li Wei mengeksekusi *Jurus Penebas Akar* (Damage Base 80, Konsumsi 20 Qi).
  - Damage ke Monster = 80 Damage.
  - HP Serigala Akar Hijau berkurang menjadi **0 / 120** (**Kalah!**).

---

#### 🎁 Step 4: Resolution & Roll Loot Drop
* **Kalkulasi Drop Loot AI GM**:
  - Roll Base Drop Rate Umum (80%): **Berhasil** → mendapatkan *Kulit Serigala Hijau*.
  - Roll Base Drop Rate Jarang (30%): **Berhasil** → mendapatkan *Taring Akar Kayu*.
  - Roll Base Drop Rate Legendaris (10%): **Gagal** (Core T2 didapat secara standar).
* **Pencatatan Item Origin Log AI GM**:
  ```text
  [Item Origin Log — Pembunuhan Monster]
  - Kulit Serigala Hijau (Grade: Common) ×1 | Sumber: Serigala Akar Hijau T2 (Dataran Hijau Abadi)
  - Taring Akar Kayu (Grade: Rare) ×1 | Sumber: Serigala Akar Hijau T2 (Dataran Hijau Abadi)
  - Spirit Core T2 (Elemen Kayu) ×1 | Sumber: Serigala Akar Hijau T2 (Dataran Hijau Abadi)
  Timestamp: Tahun 1, Bulan 3, Hari 12 (Sesi Malam)
  ```

---

## 🛡️ 10. Checklist Validasi & Anti-Cheat AI GM

Sebelum merilis hasil pertarungan atau menyerahkan loot buruan kepada pemain, AI GM **wajib** melakukan verifikasi atas checklist berikut:

- [ ] Apakah statistik HP dan Attack Power monster yang dimunculkan sudah tepat sesuai dengan tabel katalog Tier 0–9 di modul ini?
- [ ] Apakah habitat dan lokasi munculnya monster telah tervalidasi cocok dengan posisi pemain pada Peta Wilayah (`01`–`10`)?
- [ ] Apakah formula `AmbushChance` dihitung secara terbuka beserta modifier lingkungan, waktu, dan kebisingan?
- [ ] Apakah efek status khusus (*Burn, Freeze, Poison, Paralysis, Slow*) dicatat durasi dan dampaknya pada log turn secara disiplin?
- [ ] Apakah monster tipe Sprite/Roh telah diberi properti imun terhadap serangan fisik murni jika pemain belum melapisi senjatanya dengan Qi/Elemen?
- [ ] Apakah seluruh loot hasil kemenangan telah dicatat secara rinci ke dalam **Item Origin Log** pada Profil Karakter pemain?
- [ ] Apakah monster kelas *Apex Guardian* (Tier 8–9) hanya dimunculkan pada momen krisis naratif/Secret Realms dan bukan sebagai encounter harian biasa?
