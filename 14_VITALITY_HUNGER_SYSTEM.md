# ❤️ Huangji-World — Sistem Vitalitas (HP), Kelaparan (Satiety), & Kelangsungan Hidup

> **Modul:** 14 — Vitality, Hunger, Stamina & Trauma System
> **Prinsip:** Anti-Cheat Enforced — Law-Specific Scaling — Terintegrasi dengan Sistem Hukum Kultivasi, Pertarungan, & Ekonomi
> **Rujukan Utama:** [`INDEX.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/INDEX.md?v=1)
> **Rujukan Silang:**
> - [`00_CORE_RULES_AI_GM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/00_CORE_RULES_AI_GM.md?v=1) (Aturan Wajib AI GM)
> - [`12_CULTIVATION_LAW_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/12_CULTIVATION_LAW_SYSTEM.md?v=1) (QiCap Basis HP)
> - [`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1) (Harga Obat & Tabib)
> - [`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1) (Final Damage)
> - [`16_BESTIARY.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/16_BESTIARY.md?v=1) (Spesies & Daging Spirit)
> - [`18_TAMING_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/18_TAMING_SYSTEM.md?v=1) (Satiety Companion)
> - [`19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1) (Pil Pemulihan Alkimia)

---

## 📜 0. Filosofi & Aturan Emas Vitalitas

Di Benua Huangji, tubuh raga seorang kultivator adalah bejana tempat menyimpan Qi. Ketahanan raga (**Hit Points / HP**), daya tahan fisik (**Stamina**), dan keterikatan pada kebutuhan fana (**Satiety / Kelaparan**) semuanya saling terkait secara biologis dan spiritual. Setiap Hukum Kultivasi resmi memiliki karakteristik fisik berbeda, dan setiap kenaikan Ranah (*Realm*) secara bertahap membebaskan kultivator dari ketergantungan makanan fana (*Bi Gu / Puasa Spiritual*).

**AI GM WAJIB memvalidasi dan memperbarui statistik HP, Stamina, dan Kelaparan karakter pada setiap giliran narasi secara objektif.**

### 🛡️ Aturan Emas Anti-Cheat Vitalitas & Kelaparan
1. **Dilarang Klaim HP Sepihak**: Maksimal HP karakter dihitung mutlak oleh AI GM berdasarkan formula `HP(realm, stage, law, physique)`.
2. **Log Luka & Damage Bertimestamp**: Semua kerusakan fisik (*damage*) dan status luka akibat pertempuran atau lingkungan dicatat secara permanen di log status. Tidak bisa "dilupakan" atau diedit mundur oleh player.
3. **Regenerasi Alami vs Item**: Pemulihan HP alami berjalan lambat. Pemulihan instan HANYA SAH melalui konsumsi pil alkimia, obat herba, atau jasa tabib resmi yang tercatat di log inventory dan tunduk pada Sistem Ekonomi ([`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1)).
4. **Penurunan Satiety Otomatis**: Setiap giliran yang melibatkan perjalanan atau aktivitas fisik, Satiety berkurang secara otomatis berdasarkan Fasting Multiplier ranah pemain.
5. **Trauma Fisik & Qi Deviation**: Cedera berat di organ vital atau Dantian memicu status trauma khusus yang tidak bisa disembuhkan dengan istirahat biasa.

---

## 🩸 1. Formula HP Universal & Law Multiplier

Maksimal HP (*HP Max*) seorang karakter dihitung berdasarkan kapasitas Qi maksimal (*Qi Cap*) pada ranahnya dikalikan dengan Konstanta Vitalitas Universal ($K_{HP} = 0,4$) dan Multiplier Hukum Kultivasi (*LawHPMultiplier*):

$$\text{HPBase}(\text{Realm}, \text{Stage}) = \text{QiCap}(\text{Realm}, \text{Stage}) \times 0,4$$
$$\text{HPMax} = \text{HPBase}(\text{Realm}, \text{Stage}) \times \text{LawHPMultiplier}(\text{Law}) \times \text{PhysiqueHPMultiplier}$$

### 📊 Contoh Perhitungan HP
Karakter di **Ranah Fondasi Jiwa Awal (Foundation Establishment Realm - Early Stage)** dengan **Hukum Akar Kayu Suci** (`LawHPMultiplier = ×1,4`) dan tanpa Tubuh Khusus (`PhysiqueHPMultiplier = ×1,0`):
- $\text{QiCap} = 2.500 \text{ Poin Qi}$
- $\text{HPBase} = 2.500 \times 0,4 = 1.000 \text{ HP}$
- $\text{HPMax} = 1.000 \times 1,4 \times 1,0 = \mathbf{1.400 \text{ HP Max}}$

---

### 🛡️ Tabel Law HP Multiplier Resmi 11 Hukum Kultivasi Huangji-World

| Hukum Kultivasi Resmi | LawHPMultiplier | Modul Sekte & Karakteristik Fisik Raga |
|---|:---:|---|
| **Hukum Akar Kayu Suci** (*Immortal Woodroot Law*) | **×1,4** | Sekte Akar Kayu Abadi ([`20`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/20_SEKTE_AKAR_KAYU_ABADI.md?v=1)) — Energi vitalitas kayu melimpah; sangat tahan banting. |
| **Hukum Benteng Pasir Emas** (*Golden Sand Fortress Law*) | **×1,5** | Sekte Benteng Pasir ([`31`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/31_SEKTE_BENTENG_PASIR.md?v=1)) — Penempaan dinding cadas; pertahanan fisik & volume darah tertinggi. |
| **Hukum Inti Petir Ungu** (*Purple Lightning Core Law*) | **×1,0** | Sekte Petir Ungu ([`22`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/22_SEKTE_PETIR_UNGU.md?v=1)) — Baseline serangan kilat; seimbang antara kecepatan dan daya tahan. |
| **Hukum Tungku Api Merah** (*Crimson Furnace Law*) | **×0,9** | Sekte Tungku Api Merah ([`25`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/25_SEKTE_TUNGKU_API_MERAH.md?v=1)) — Agresif ofensif; energi dibakar di Dantian, fisik sedikit lebih rapuh. |
| **Hukum Istana Es Abadi** (*Eternal Frost Palace Law*) | **×1,1** | Sekte Istana Es Abadi ([`27`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/27_SEKTE_ISTANA_ES_ABADI.md?v=1)) — Perisai kristal es; padat defensif, pembuluh darah beku tahan trauma. |
| **Hukum Tahta Emas Huangji** (*Huangji Golden Throne Law*)| **×1,2** | Akademi Kekaisaran Huangji ([`24`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/24_AKADEMI_KEKAISARAN_HUANGJI.md?v=1)) — Kepemimpinan elit istana; fisik tangguh berwibawa. |
| **Hukum Bayangan Jiwa Kelabu** (*Desolate Soul Shadow Law*)| **×0,75** | Sekte Bayangan Jiwa ([`29`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/29_SEKTE_BAYANGAN_JIWA.md?v=1)) — Berbasis jiwa/tulang; rapuh secara raga, fokus kekuatan roh. |
| **Hukum Racun Teratai Hitam** (*Black Lotus Poison Law*) | **×0,7** | Kelompok Racun Bayangan ([`34`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/34_KELOMPOK_RACUN_BAYANGAN.md?v=1)) — Miasma beracun; trade-off pertahanan demi racun mematikan. |
| **Hukum Pedang Awan** (*Cloudblade Law*) | **×0,85** | Perguruan Panah Oase ([`32`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/32_PERGURUAN_PANAH_OASE.md?v=1)) — Kecepatan angin; lincah & fleksibel, mengorbankan ketebalan kulit. |
| **Hukum Mutiara Samudra** (*Ocean Pearl Law*) | **×1,15** | Kepulauan Palung Samudra ([`10`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/10_OCEANIC_ABYSS_ISLANDS.md?v=1)) — Energi perairan samudra; elastis & cepat menutup luka terbuka. |
| **Hukum Pisau Sunyi** (*Silent Blade Law*) | **×0,8** | Perkumpulan Pisau Sunyi ([`33`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/33_PERKUMPULAN_PISAU_SUNYI_HUANGJI.md?v=1)) — Presisi eksekutor; tangguh namun ramping. |
| **Fana / Tanpa Hukum** (*Mortal Realm*) | **×1,0** | Manusia biasa tanpa kultivasi (Base HP = 100). |

---

## 💔 2. Tingkat Kerusakan & Ambang Bahaya HP

Setiap kali HP karakter berkurang akibat serangan atau kondisi lingkungan, status fisik karakter secara otomatis berpindah ke tingkatan berikut:

| % HP Tersisa | Status Kondisi Physical Condition | Efek Penalti Mekanik | Deskripsi Naratif AI GM |
|:---:|:---:|---|---|
| **100% – 75%** | **Prima (*Healthy / Prime*)** | Tidak ada penalti. | Tubuh dalam kondisi puncak, napas teratur, gerakan lincah. |
| **74% – 50%** | **Luka Ringan (*Lightly Wounded*)** | Stamina Cost **+10%** untuk semua aksi. | Memar di kulit, goresan pedang ringan, pendarahan tipis. |
| **49% – 25%** | **Terluka Berat (*Severely Wounded*)**| Output Qi **-20%**, Hit Chance **-15%**, Speed **-25%**. | Tulang retak, pendarahan aktif, napas terengah-engah. |
| **24% – 1%** | **Kritis (*Critical Condition*)** | Output Qi **-50%**, Risiko *Qi Deviation* 30%/Turn. | Pendarahan organ dalam, Dantian terguncang, penglihatan kabur. |
| **0%** | **Lumpuh / Koma (*Incapacitated*)** | Tak sadarkan diri. Wajib diobati dalam `(Realm + 3)` Turn. | Tubuh ambruk, nadi melemah, tidak sanggup mengeluarkan Qi. |
| **< -50% HP Max**| **Kematian Permanen (*Permadeath*)** | Jiwa melayang, raga hancur. **Game Over**. | Jantung hancur / Dantian meledak / Tubuh terbelah dua. |

---

## ⚡ 3. Sistem Stamina (Daya Tahan Otot & Fisik)

Stamina adalah indikator daya tahan otot dan fokus karakter saat melakukan aksi fisik, pertarungan, atau eksplorasi:

$$\text{StaminaMax} = 100 \text{ Poin (Universal untuk semua Ranah)}$$

### 🏃 Penggunaan & Pemulihan Stamina

| Aktivitas Karakter | Biaya Stamina (*Cost*) | Pemulihan Alami (*Recovery Rate*) |
|---|:---:|---|
| **Serangan Biasa (Fisik)** | -5 Poin / Turn | +10 Poin / Turn saat bertahan / tidak beraksi |
| **Penggunaan Jurus / Teknik Qi** | -10 Poin / Turn | +20 Poin / Jam saat berjalan santai |
| **Berlari Cepat / Dash / Dodging** | -15 Poin / Turn | +50 Poin / Jam saat duduk bermeditasi |
| **Perjalanan Jalan Kaki (Area Liar)** | -10 Poin / Jam | **Pemulihan Penuh**: Istirahat tidur 8 jam + Satiety > 50% |
| **Bekerja Kasar / Menambang / Tempa** | -20 Poin / Jam | — |

📌 *Penalti Stamina Kosong (0 Poin)*: Karakter menderita efek **Kelelahan Ekstrem (*Exhaustion*)** — Hit Chance **-30%**, tidak bisa berlari/dodge, dan pemulihan Qi alami terhenti.

---

## 🍙 4. Sistem Kelaparan (Satiety & Bi Gu System per Ranah)

Kebutuhan makanan diukur lewat poin **Satiety (Kekenyangan)**. Karakter memulai petualangan dengan Satiety `100%`.

$$\text{SatietyMax} = 100\% \text{ (Universal)}$$
$$\text{WaktuLaparTotal} = 10 \text{ Jam} \times \text{FastingMultiplier}(\text{Realm})$$

### 🍚 Fasting Multiplier & Bi Gu System Dwibahasa (Indonesian / English)

Untuk ranah awal (0 s/d 2), laju pengurangan kelaparan diperlambat agar kultivator pemula dan warga fana tidak perlu mencari makanan terlalu sering:

| Ranah (Indonesian / English Realm) | Fasting Multiplier | Durasi dari 100% → 0% Satiety | Status *Bi Gu* (*Spiritual Fasting*) |
|:---:|:---:|:---:|---|
| **0 — Ranah Fana (*Mortal Realm*)** | **×1,0** | **10 Jam** | Membutuhkan makanan fana 2 kali sehari. |
| **1 — Pembersihan Tubuh (*Body Refining*)** | **×1,5** | **15 Jam** | Tempaan fisik menahan lapar lebih lama dari manusia fana. |
| **2 — Pengumpulan Qi (*Qi Gathering*)** | **×3,0** | **30 Jam (~1,25 Hari)** | Qi alam mulai menggantikan separuh kebutuhan nutrisi. |
| **3 — Fondasi Jiwa (*Foundation Establishment*)**| **×8,0** | **80 Jam (~3,3 Hari)** | Mampu menahan lapar beberapa hari tanpa penalti fisik. |
| **4 — Inti Emas (*Golden Core Realm*)** | **×20,0** | **200 Jam (~8,3 Hari)** | Inti Emas menyuplai energi kehidupan. Makanan biasa terasa hambar. |
| **5 — Jiwa Nascent (*Nascent Soul Realm*)** | **×60,0** | **600 Jam (~25 Hari)** | *Bi Gu Awal* — Hanya butuh pil nutrisi / herba sesekali. |
| **6 — Formasi Roh (*Spirit Formation*)** | **×200,0** | **2.000 Jam (~2,7 Bulan)** | *Bi Gu Menengah* — Tubuh menyerap esensi alam liar. |
| **7 — Transformasi Kehampaan (*Void Trans*)**| **×600,0** | **6.000 Jam (~8,3 Bulan)** | *Bi Gu Lanjut* — Bebas dari makanan fana. |
| **8 — Tribulasi Surgawi (*Tribulation Realm*)** | **×2.500,0** | **25.000 Jam (~3,4 Tahun)**| *Bi Gu Sempurna* — Energi alam semesta memenuhi raga. |
| **9 — Kaisar Agung Abadi (*Huangji Sovereign*)**| **Tak Terbatas** | **Abadi (*Absolute Fasting*)** | Menyatu dengan hukum alam semesta — bebas dari rasa lapar. |

---

### ⚠️ Tingkatan Penalti Kelaparan (Satiety Debuffs)

1. **Satiety 30% – 21% (*Lapar*)**: Stamina Regen **-25%**.
2. **Satiety 20% – 1% (*Sangat Lapar*)**: Max HP **-20%**, Output Qi **-30%**, Stamina Max terpotong menjadi 50 poin.
3. **Satiety 0% (*Kelaparan Ekstrem / Starvation*)**: Karakter kehilangan **5% HP Max per jam in-game**. Pemulihan Qi alami **terhenti sepenuhnya**.

---

## 🩺 5. Trauma Fisik & Qi Deviation (Penyakit Khusus Kultivator)

Luka berat dari pertempuran atau kegagalan breakthrough memicu status trauma khusus yang membutuhkan penanganan dari Tabib atau Pil Kelas Tinggi:

| Jenis Trauma | Penyebab Utama | Efek Mekanik Penalti | Cara Penyembuhan / Solusi |
|---|---|---|---|
| **Pendarahan Organ Dalam** | Serangan mematikan / blunt damage besar | Kerusakan HP 2% HP Max / Turn saat bertarung. | *Pil Pemulihan Darah Tier-2* / Jasa Tabib Balai Tabib Pengembara ([`37`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/37_BALAI_TABIB_PENGEMBARA_HUANGJI.md?v=1)). |
| **Retak Dantian** | Kegagalan Breakthrough / Serangan Jiwa | Qi Cap terpotong 50%. Penggunaan Qi melukai HP sendiri. | *Pil Penambal Dantian Tier-3* / Meditasi di Urat Naga selama 1 bulan. |
| **Meridian Terbakar** | Overuse Pil / Serangan Api/Petir | Regen Qi terhenti, teknik elemen memicu Burn pada raga. | *Salep Es Bintang Tier-2* / Pengobatan Sekte Istana Es ([`27`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/27_SEKTE_ISTANA_ES_ABADI.md?v=1)). |
| **Keracunan Miasma** | Gigitan Beast Racun / Senjata Beracun | Kerusakan HP bertahap per turn + Hit Chance **-20%**. | *Pil Penawar Seribu Racun Tier-1/2* / Bantuan Kelompok Racun Bayangan ([`34`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/34_KELOMPOK_RACUN_BAYANGAN.md?v=1)). |

---

## 💊 6. Item & Jasa Pemulihan Resmi Huangji-World

Seluruh item pemulihan wajib merujuk pada Sistem Ekonomi ([`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1)) dan Sistem Alkimia ([`19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1)):

| Nama Item / Jasa Pemulihan | Efek Pemulihan Fisik & Qi | Harga Pasar Resmi |
|---|---|---|
| **Roti Kering / Daging Asap / Bubur** | Memulihkan **+30% Satiety** (Hanya untuk Realm 0–2) | 5 Koin Perak |
| **Daging Spirit Beast Tier-1** | Memulihkan **+60% Satiety** + 20 Poin Qi | 1 Batu Spiritual Rendah |
| **Pil Pemulihan Darah (Tier 1)** | Memulihkan **+150 HP** secara instan | 5 Batu Spiritual Rendah |
| **Pil Pemulihan Darah (Tier 2)** | Memulihkan **+800 HP** + menyembuhkan Luka Dalam | 25 Batu Spiritual Rendah |
| **Salep Herba Vitalitas (Tier 1)**| Menghilangkan efek Luka Ringan / Memar dalam 1 jam | 2 Batu Spiritual Rendah |
| **Jasa Pengobatan Tabib Senior**| Menyembuhkan Trauma Organ / Dantian sampai pulih penuh | 50–200 Batu Spiritual Rendah |

---

## 🛡️ 7. Checklist Validasi & Anti-Cheat AI GM

Sebelum merilis update status HP atau kelaparan pemain, AI GM **wajib** memeriksa checklist berikut:

- [ ] Apakah `HPMax` dihitung dengan presisi memakai formula `HPBase × LawHPMultiplier × Physique`?
- [ ] Apakah pengurangan HP akibat damage tercatat pada log status bertimestamp?
- [ ] Apakah penalti kondisi HP (*Healthy / Lightly Wounded / Severely Wounded / Critical*) diterapkan pada Hit Chance & Output Qi?
- [ ] Apakah penurunan poin Satiety telah dihitung berdasarkan durasi perjalanan dan `FastingMultiplier` ranah karakter?
- [ ] Apakah item atau pil pemulihan yang dikonsumsi pemain telah dihapus dari sheet *Inventory*?
- [ ] Apakah pemulihan trauma berat organ/Dantian melibatkan jasa tabib atau pil yang valid sesuai ketersediaan di pasar?
