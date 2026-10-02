# ❤️ Huangji-World — Sistem Vitalitas (HP), Kelaparan (Satiety), & Kelangsungan Hidup

> **Modul:** 14 — Vitality, Hunger, Stamina & Trauma System
> **Prinsip:** Anti-Cheat Enforced — Law-Specific Scaling — Terintegrasi dengan Sistem Hukum Kultivasi, Pertarungan, & Ekonomi
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md` (aturan wajib), `12_CULTIVATION_LAW_SYSTEM.md` (QiCap basis HP), `13_ECONOMY_SYSTEM.md` (Harga Obat & Tabib), `15_COMBAT_SYSTEM.md` (Final Damage), `19_ALCHEMY_FORGING_ARRAY_SYSTEM.md` (Pil Pemulihan)

---

## 0. Filosofi Sistem

Di Benua Huangji, tubuh raga kultivator adalah wadah penyimpan Qi. Ketahanan raga (HP), daya tahan fisik (Stamina), dan keterikatan pada kebutuhan fana (Satiety/Makan) semuanya saling berkaitan. Tiap Hukum Kultivasi resmi memiliki karakteristik fisik berbeda, dan setiap tingkatan Ranah (*Realm*) secara bertahap membebaskan kultivator dari belenggu kelaparan.

**AI GM WAJIB memvalidasi dan memperbarui statistik HP, Stamina, dan Kelaparan karakter pada setiap giliran narasi.**

### Aturan Emas Anti-Cheat Vitalitas & Kelaparan
1. **Dilarang Klaim HP Sepihak**: Maksimal HP karakter dihitung mutlak oleh AI GM berdasarkan formula `HP(realm, stage, law, physique)`.
2. **Log Luka & Damage Bertimestamp**: Semua kerusakan fisik (damage) dan status luka akibat pertempuran atau lingkungan dicatat secara permanen di log status. Tidak bisa "dilupakan" atau diedit mundur oleh player.
3. **Regenerasi Alami vs Item**: Pemulihan HP alami berjalan lambat. Pemulihan instan HANYA sah melalui konsumsi pil alkimia, obat herba, atau jasa tabib resmi yang tercatat di log inventory dan tunduk pada Sistem Ekonomi (`13_ECONOMY_SYSTEM.md`).
4. **Penurunan Satiety Otomatis**: Setiap giliran yang melibatkan perjalanan atau aktivitas fisik, Satiety berkurang secara otomatis berdasarkan Fasting Multiplier ranah pemain.
5. **Trauma Fisik & Qi Deviation**: Cedera berat di organ vital atau dantian memicu status trauma khusus yang tidak bisa disembuhkan dengan istirahat biasa.

---

## 1. Formula HP Universal & Law Multiplier

```
HPBase(realm, stage) = QiCap(realm, stage) × K_HP
K_HP = 0,4 (Konstanta Vitalitas Universal)

HP_Max = HPBase(realm, stage) × LawHPMultiplier(law) × PhysiqueHPMultiplier
```

*Contoh Calculation:*
Karakter Ranah Fondasi Jiwa Awal (Realm 3 Early) dengan Hukum Akar Kayu Suci (`LawHPMultiplier = 1,4`) dan Tubuh Tanpa Physique Khusus (`1,0`):
- `QiCap` = 2.500
- `HPBase` = 2.500 × 0,4 = 1.000
- `HP_Max` = 1.000 × 1,4 × 1,0 = **1.400 HP Maksimal**.

---

### 🛡️ Tabel Law HP Multiplier Resmi Huangji-World

| Hukum Kultivasi Resmi | LawHPMultiplier | Filosofi & Karakteristik Fisik |
|---|:---:|---|
| **Hukum Akar Kayu Suci** (`20`) | **×1,4** | Energi vitalitas kayu melimpah — sangat tahan banting & cepat pulih. |
| **Hukum Benteng Pasir Emas** (`31`) | **×1,5** | Penempaan dinding cadas — pertahanan fisik & volume darah tertinggi. |
| **Hukum Inti Petir Ungu** (`22`) | **×1,0** | Baseline serangan kilat — seimbang antara kecepatan dan daya tahan. |
| **Hukum Tungku Api Merah** (`25`) | **×0,9** | Agresif ofensif — energi dibakar di dantian, fisik sedikit lebih rapuh. |
| **Hukum Istana Es Abadi** (`27`) | **×1,1** | Perisai kristal es — padat defensif, pembuluh darah beku tahan trauma. |
| **Hukum Tahta Emas Huangji** (`24`) | **×1,2** | Kepemimpinan elit istana — fisik tangguh berwibawa. |
| **Hukum Bayangan Jiwa Kelabu** (`29`) | **×0,75** | Berbasis jiwa/tulang — rapuh secara raga, fokus kekuatan roh. |
| **Hukum Racun Teratai Hitam** (`33`) | **×0,7** | Racun miasma — trade-off pertahanan demi racun mematikan. |
| **Hukum Pedang Awan** (`35`) | **×0,85** | Kecepatan angin — fleksibel & lincah, mengorbankan ketebalan kulit. |
| **Hukum Mutiara Samudra** (`37`) | **×1,15** | Energi cairan samudra — elastis & cepat menutup luka terbuka. |
| **Hukum Pisau Sunyi** (`33`) | **×0,8** | Presisi eksekutor — tangguh namun ramping, bukan perthanan tank. |
| **Fana / Tanpa Hukum (Realm 0)** | **×1,0** | Manusia biasa (Base HP = 100). |

---

## 2. Tingkat Kerusakan & Ambang Bahaya HP

Setiap kali HP karakter tergerus serangan, kondisi fisik karakter secara otomatis berpindah ke tingkatan berikut:

| % HP Tersisa | Status Kondisi | Efek Penalti Mekanik | Deskripsi Naratif AI GM |
|:---:|:---:|---|---|
| **100% – 75%** | **Prima (Prima)** | Tidak ada penalti. | Tubuh dalam kondisi puncak, napas teratur, gerakan lincah. |
| **74% – 50%** | **Luka Ringan (Lightly Wounded)** | Stamina Cost +10% untuk semua aksi. | Memar di kulit, goresan pedang ringan, pendarahan tipis. |
| **49% – 25%** | **Terluka Berat (Severely Wounded)** | Output Qi −20%, Hit Chance −15%, Move Speed −25%. | Tulang retak, pendarahan aktif, napas terengah-engah. |
| **24% – 1%** | **Kritis (Critical Condition)** | Output Qi −50%, Risiko *Qi Deviation* 30% per turn, Hit Chance −35%. | Pendarahan organ dalam, Dantian terguncang, penglihatan kabur. |
| **0%** | **Lumpuh / Koma (Incapacitated)** | Tak sadarkan diri. Wajib pertolongan darurat medis dalam `(Realm + 3)` turn. | Tubuh ambruk, nadi melemah, tidak sanggup bergerak atau mengeluarkan Qi. |
| **< −50% HP Max** | **Kematian Permanen (Permadeath)** | Jiwa melayang, raga hancur. Game Over. | Jantung hancur / Dantian meledak / Tubuh terbelah dua. |

---

## 3. Sistem Stamina (Daya Tahan Fisik)

Stamina adalah indikator daya tahan otot dan fokus karakter saat melakukan aksi fisik, pertarungan, atau perjalanan.

```
Stamina_Max = 100 poin (universal untuk semua realm)
```

### ⚡ Penggunaan Stamina (Stamina Cost Table)

| Aktivitas | Biaya Stamina | Pemulihan Alami |
|---|:---:|---|
| **Serangan Biasa (Fisik)** | −5 Poin / Turn | +10 Poin / Turn saat bertahan / tidak beraksi |
| **Penggunaan Jurus/Teknik Qi** | −10 Poin / Turn | +20 Poin / Jam saat berjalan santai |
| **Berlari Cepat / Dash / Dodging** | −15 Poin / Turn | +50 Poin / Jam saat duduk beristirahat |
| **Perjalanan Jalan Kaki (Area Liar)** | −10 Poin / Jam | **Pemulihan Penuh**: Istirahat tidur 8 jam + Satiety > 50% |
| **Bekerja Kasar / Menambang / Tempa** | −20 Poin / Jam | — |

*Penalti Stamina Kosong (0 Poin):* Karakter terkena efek **Kelelahan Ekstrem (Exhaustion)** — Hit Chance −30%, tidak bisa berlari/dodge, dan pemulihan Qi alami terhenti.

---

## 4. Sistem Kelaparan (Satiety & Bi Gu System)

Kebutuhan makanan diukur lewat poin **Satiety (Lapar)**. Karakter baru memulai petualangan dengan Satiety `100%`.

```
Satiety_Max = 100% (universal)
Waktu_Lapar_Total = 6 jam × FastingMultiplier(realm)
```

### 🍙 Fasting Multiplier & Ketahanan Lapar per Ranah (*Realm*)

| Ranah (Realm) | FastingMultiplier | Waktu dari 100% → 0% Satiety | Status *Bi Gu* (Puasa Spiritual) |
|:---:|:---:|:---:|---|
| **0 — Fana (Mortal)** | **×1,0** | **6 Jam** | Butuh makan 3 kali sehari. Tanpa makan → Tubuh melemah cepat. |
| **1 — Pembersihan Tubuh** | **×1,0** | **6 Jam** | Metabolisme cepat karena tempaan otot. |
| **2 — Pengumpulan Qi** | **×2,0** | **12 Jam** | Qi alam mulai menggantikan separuh energi makanan biasa. |
| **3 — Pembentukan Fondasi** | **×5,0** | **30 Jam (~1,25 Hari)** | Mampu menahan lapar seharian penuh tanpa penalti fisik. |
| **4 — Pembentukan Inti Emas** | **×15,0** | **90 Jam (~3,75 Hari)** | Inti Emas menyuplai energi kehidupan. Makanan biasa terasa hambar. |
| **5 — Jiwa Nascent** | **×50,0** | **300 Jam (~12,5 Hari)** | *Bi Gu Tingkat Awal* — Hanya butuh pil nutrisi / herba sesekali. |
| **6 — Formasi Roh** | **×150,0** | **900 Jam (~37,5 Hari)** | *Bi Gu Tingkat Menengah* — Tubuh menyerap esensi alam liar. |
| **7 — Transformasi Kehampaan**| **×500,0** | **3.000 Jam (~4 Bulan)** | *Bi Gu Tingkat Lanjut* — Tidak membutuhkan makanan fana. |
| **8 — Tribulasi Surgawi** | **×2.000,0** | **12.000 Jam (~1,4 Tahun)**| *Bi Gu Sempurna* — Energi alam semesta memenuhi raga. |
| **9 — Kaisar Agung Abadi** | **Tak Terbatas** | **Abadi (Puasa Mutlak)** | Menyatu dengan hukum alam semesta — bebas dari rasa lapar. |

---

### ⚠️ Tingkatan Penalti Kelaparan (Satiety Debuff)

1. **Satiety 50% – 21% (Lapar)**: Stamina Regen −25%.
2. **Satiety 20% – 1% (Sangat Lapar)**: Max HP −20%, Output Qi −30%, Stamina Max terpotong menjadi 50 poin.
3. **Satiety 0% (Kelaparan Ekstrem / Starvation)**: Karakter kehilangan 5% HP Max setiap jam in-game. Pemulihan Qi alami **terhenti sepenuhnya**.

---

## 5. Trauma Fisik & Qi Deviation (Penyakit Khusus Kultivator)

Luka berat dari pertarungan atau kegagalan breakthrough memicu efek status khusus yang memerlukan penanganan khusus dari Tabib atau Pil Kelas Tinggi:

| Jenis Trauma | Penyebab Utama | Efek Mekanik | Cara Penyembuhan |
|---|---|---|---|
| **Pendarahan Organ Dalam** | Serangan mematikan / blunt damage besar | Kerusakan HP permanen 2% HP Max / Turn saat bertarung. | *Pil Pemulihan Darah Tier-2* / Jasa Tabib Balai Tabib Pengembara (`37`). |
| **Retak Dantian** | Kegagalan Breakthrough / Serangan Jiwa | Qi Cap terpotong 50%. Penggunaan Qi memicu damage ke HP sendiri. | *Pil Penambal Dantian Tier-3* / Meditasi di Sumber Qi Abadi selama 1 bulan. |
| **Meridian Terbakar** | Konsumsi pil berlebih / Serangan Api/Petir | Regen Qi terhenti, teknik elemen memicu efek Burn pada diri sendiri. | *Salep Es Bintang Tier-2* / Pengobatan Es dari Sekte Istana Es (`27`). |
| **Keracunan Miasma** | Gigitan Beast Racun / Senjata Beracun | Kerusakan HP bertahap per turn + penalti Hit Chance −20%. | *Pil Penawar Seribu Racun Tier-1/2* / Bantuan Kelompok Racun Bayangan (`34`). |

---

## 🧪 6. Item & Jasa Pemulihan Resmi Huangji-World

Semua transaksi dan pembuatan item pemulihan wajib merujuk pada `13_ECONOMY_SYSTEM.md` dan `19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`.

| Nama Item / Jasa | Fungsi Pemulihan | Harga Pasar Standar |
|---|---|---|
| **Roti Kering / Daging Asap** | Memulihkan +30% Satiety (Hanya untuk Realm 0–2) | 5 Koin Perak |
| **Daging Spirit Beast Tier-1** | Memulihkan +60% Satiety + 20 Poin Qi | 1 Batu Spiritual Rendah |
| **Pil Pemulihan Darah (Tier 1)** | Memulihkan +150 HP secara instan | 5 Batu Spiritual Rendah |
| **Pil Pemulihan Darah (Tier 2)** | Memulihkan +800 HP + menyembuhkan Luka Dalam | 25 Batu Spiritual Rendah |
| **Salep Herba Vitalitas (Tier 1)**| Menghilangkan efek Luka Ringan / Memar dalam 1 jam | 2 Batu Spiritual Rendah |
| **Jasa Pengobatan Tabib Senior**| Menyembuhkan Trauma Organ / Dantian sampai pulih penuh | 50–200 Batu Spiritual Rendah |

---

## 🛡️ 7. Checklist Validasi AI GM (Wajib Diperiksa Tiap Turn)

- [ ] Apakah `HP_Max` sudah dihitung memakai formula `HPBase × LawHPMultiplier × Physique`?
- [ ] Apakah penurunan HP akibat damage telah dicatat di log status karakter?
- [ ] Apakah penalti akibat kondisi HP (Prima / Terluka / Kritis) telah diterapkan pada kalkulasi Hit Chance dan Output Qi turn ini?
- [ ] Apakah Satiety telah dipotong sesuai waktu perjalanan dan `FastingMultiplier` realm karakter?
- [ ] Apakah item pemulihan yang dikonsumsi pemain benar-benar ada di *Inventory* dan telah dihapus setelah dipakai?
