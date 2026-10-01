# 📜 Huangji-World — Sistem Hukum Kultivasi (Cultivation Laws System)

> **Modul:** 12 — Cultivation Law System
> **Prinsip:** Anti-Cheat Enforced — Stable Tier Scaling — Karma-Linked Tribulation
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md` (aturan wajib), `13_ECONOMY_SYSTEM.md` (harga bahan), `14_VITALITY_HUNGER_SYSTEM.md` (HP), `15_COMBAT_SYSTEM.md` (Combat), modul wilayah `01`–`10`

---

## 🧭 1. Filosofi Sistem

Setiap "Hukum" (Law) adalah jalur kultivasi berbeda dengan sumber daya berbeda (Qi Murni, Qi Petir Ungu, Qi Api Vulkanik, Qi Akar Kayu, dll.), tetapi **semua Hukum tunduk pada satu Formula Batas Qi (Qi Cap Formula)** yang sama, supaya tidak ada jalur yang overpowered dibanding yang lain.

**AI GM WAJIB menolak** klaim kekuatan/qi/item yang melampaui batas formula di bawah ini — tanpa pengecualian, tanpa "power creep" naratif.

### Aturan Emas Anti-Cheat
- Qi/energi karakter tidak boleh melebihi `QiCap(realm, stage)` — dihitung ulang tiap turn oleh AI.
- Breakthrough (terobosan) HARUS memenuhi 3 syarat sekaligus: bahan minimum, insight/comprehension tervalidasi GM, dan (untuk realm 7+) selamat dari Tribulasi.
- Tidak ada retroactive edit stat oleh player — semua log qi/item bertimestamp dan tidak bisa diubah mundur.
- Item/pil hanya boleh menaikkan qi sebatas ±1 tier dari tier user saat ini (material tier matching).
- Law custom TETAP tunduk pada formula qi cap yang sama — hanya reskin mekanik, bukan reskin batas.
- **Player TIDAK BOLEH mendeklarasikan sendiri "aku terobosan pakai Hukum X" di saat momen terobosan.** AI GM yang menentukan Hukum/teknik apa yang berlaku, berdasarkan teknik yang benar-benar dilatih/dipraktikkan player sepanjang cerita — dan itu hanya sah jika sudah punya **Asal-Usul Hukum** yang tervalidasi (§3.0). Deklarasi sepihak tanpa asal-usul = otomatis DITOLAK.

---

## 🌀 2. Struktur Realm Universal (9 Major Realm × 3 Stage = 27 Sub-Tier)

| # | Major Realm (Universal) | Realm Base (RB) | Qi Cap Awal (×1,0) | Qi Cap Menengah (×1,5) | Qi Cap Puncak (×2,0) |
|---|---|---|---|---|---|
| 1 | **Pemurnian Fana (Mortal Refining)** | 0 | 0 | 0 | 0 |
| 2 | **Pengumpulan Qi (Qi Gathering)** | 100 | 100 | 150 | 200 |
| 3 | **Pembentukan Fondasi (Foundation Establishment)** | 500 | 500 | 750 | 1.000 |
| 4 | **Pembentukan Inti Emas (Golden Core)** | 2.500 | 2.500 | 3.750 | 5.000 |
| 5 | **Melahirkan Jiwa Nascent (Nascent Soul)** | 12.500 | 12.500 | 18.750 | 25.000 |
| 6 | **Transformasi Kehampaan (Void Transformation)** | 62.500 | 62.500 | 93.750 | 125.000 |
| 7 | **Penyatuan Roh Suci (Sacred Spirit)** | 312.500 | 312.500 | 468.750 | 625.000 |
| 8 | **Penerobosan Tribulasi (Tribulation Crossing) ⚡** | 1.562.500 | 1.562.500 | 2.343.750 | 3.125.000 |
| 9 | **Kaisar Agung Abadi (Huangji Sovereign)** | 7.812.500 | 7.812.500 | 11.718.750 | 15.625.000 |

### 🔒 Formula Qi Cap (WAJIB DIPAKAI AI GM)
```
QiCap(realm, stage) = RealmBase(realm) × StageMultiplier(stage)
```

Contoh: Golden Core Puncak = 2.500 × 2,0 = **5.000 poin Qi maksimum**.

---

## 🔐 3. Daftar Hukum Kultivasi Resmi Huangji-World

### A. 🌿 Hukum Akar Kayu Suci (*Immortal Woodroot Law*)
* **Sumber Daya**: **Qi Kayu Vitalitas**, diserap dari pepohonan purba dan herba spiritual.
* **Mekanik Unik**: Efisiensi berkebun (*Gardening*) +50%, kecepatan pemulihan luka +20%.
* **Sekte Utama**: Sekte Akar Kayu Abadi (`20_SEKTE_AKAR_KAYU_ABADI.md`).

### B. ⚡ Hukum Inti Petir Ungu (*Purple Lightning Core Law*)
* **Sumber Daya**: **Qi Petir Ungu**, dialirkan melalui pembuluh darah dan tulang.
* **Mekanik Unik**: Kecepatan gerak +30%, damage serangan Petir +25%. Imun efek Paralysis ringan.
* **Sekte Utama**: Sekte Petir Ungu (`22_SEKTE_PETIR_UNGU.md`).

### C. 🔥 Hukum Tungku Api Merah (*Crimson Furnace Law*)
* **Sumber Daya**: **Qi Api Vulkanik**, dibakar di Dantian sebagai energi penyulingan.
* **Mekanik Unik**: Efisiensi meracik Alkimia +40%, serangan fisik memicu efek Burn.
* **Sekte Utama**: Sekte Tungku Api Merah (`25_SEKTE_TUNGKU_API_MERAH.md`).

### D. ❄️ Hukum Istana Es Abadi (*Eternal Frost Palace Law*)
* **Sumber Daya**: **Qi Es Kristal**, memadatkan energi pembeku di meridian.
* **Mekanik Unik**: Perisai Qi Es +30% lebih tebal, serangan memicu efek Freeze.
* **Sekte Utama**: Sekte Istana Es Abadi (`27_SEKTE_ISTANA_ES_ABADI.md`).

### E. 👑 Hukum Tahta Emas Huangji (*Huangji Golden Throne Law*)
* **Sumber Daya**: **Qi Kekaisaran Emas**, dipancarkan melalui wibawa kepemimpinan.
* **Mekanik Unik**: Aura Auric Pressure (menekan Damage musuh di bawah ranah sebesar -20%).
* **Akademi / Faksi**: Akademi Kekaisaran Huangji (`24_AKADEMI_KEKAISARAN_HUANGJI.md`).

### F. 🏜️ Hukum Benteng Pasir Emas (*Golden Sand Fortress Law*)
* **Sumber Daya**: **Qi Pasir & Tanah**, memadatkan pertahanan dinding cadas.
* **Mekanik Unik**: HP Max +40%, Perisai Pasir menyerap 30% damage serangan.
* **Sekte Utama**: Sekte Benteng Pasir (`31_SEKTE_BENTENG_PASIR.md`).

### G. 💀 Hukum Bayangan Jiwa Kelabu (*Desolate Soul Shadow Law*)
* **Sumber Daya**: **Qi Jiwa & Kegelapan**, mengendalikan rangka tulang dan energi roh.
* **Mekanik Unik**: Memanggil boneka tulang (*bone puppetry*), Damage serangan Jiwa +35%.
* **Sekte Utama**: Sekte Bayangan Jiwa (`29_SEKTE_BAYANGAN_JIWA.md`).

### H. ☣️ Hukum Racun Teratai Hitam (*Black Lotus Poison Law*)
* **Sumber Daya**: **Qi Racun & Kabut**, menyebarkan miasma beracun.
* **Mekanik Unik**: Imun racun biasa & sedang, serangan memicu Poison Damage bertahap.
* **Sekte Utama**: Sekte Racun Bayangan (`33_SEKTE_RACUN_BAYANGAN.md`).

### I. 🏔️ Hukum Pedang Awan (*Cloudblade Law*)
* **Sumber Daya**: **Qi Angin Tajam**, memfokuskan kecepatan tebasan pedang.
* **Mekanik Unik**: Kecepatan tebasan pedang +35%, peluang melarikan diri (Escape) +20%.
* **Sekte Utama**: Sekte Pedang Awan (`35_SEKTE_PEDANG_AWAN.md`).

### J. 🌊 Hukum Mutiara Samudra (*Ocean Pearl Law*)
* **Sumber Daya**: **Qi Samudra & Air**, mengendalikan pusaran air dan mutiara qi.
* **Mekanik Unik**: Pertarungan di atas/dalam air +35% damage, imun tekanan kedalaman laut.
* **Sekte Utama**: Sekte Mutiara Samudra (`37_SEKTE_MUTIARA_SAMUDRA.md`).

### K. 🗡️ Hukum Custom Resmi: Hukum Pisau Sunyi (*Silent Blade Law*)
* **Sumber Daya**: **Qi Pembunuh Senyap**, menyerap fokus eksekusi kontrak.
* **Mekanik Unik**: +10% HitChance selama kontrak resmi masih aktif.
* **Organisasi**: Perkumpulan Pisau Sunyi (`33_PERKUMPULAN_PISAU_SUNYI_HUANGJI.md`).

---

## 🧪 4. Bahan Minimum Terobosan (Breakthrough Material Floor)

```
Bahan Utama Minimum = n × 10 unit material Tier-n
Inti/Core Minimum   = n unit Core Tier-n
Insight Point       = WAJIB, didapat dari event naratif
```

| Realm (n) | Bahan Utama Min. | Core Min. | Insight Wajib? |
|---|---|---|---|
| 1→2 | 10 unit Tier-1 | 1 Core Tier-1 | Tidak |
| 2→3 | 20 unit Tier-2 | 2 Core Tier-2 | Ya |
| 3→4 | 30 unit Tier-3 | 3 Core Tier-3 | Ya |
| 4→5 | 40 unit Tier-4 | 4 Core Tier-4 | Ya |
| 5→6 | 50 unit Tier-5 | 5 Core Tier-5 | Ya + Restu Sekte/Guru |
| 6→7 | 60 unit Tier-6 | 6 Core Tier-6 | Ya + Trial Kehampaan |
| 7→8 | 70 unit Tier-7 | 7 Core Tier-7 | Ya + **Tribulasi Petir wajib** |
| 8→9 | 80 unit Tier-8 | 8 Core Tier-8 | Ya + Tribulasi Petir Agung |

---

## 🧬 5. Sistem Tubuh Khusus (10 Special Physiques)

1. **Tubuh Pohon Suci Abadi**: HP Max +50%, Regenerasi Qi +100% di wilayah Kayu.
2. **Tubuh Inti Petir Guntur**: Imun Paralysis, Damage Petir +40%.
3. **Tubuh Teratai Api Vulkanik**: Efisiensi Alkimia +50%, Imun Burn Damage.
4. **Tubuh Es Kristal Bintang**: Defense +30%, Efek Freeze Damage +25%.
5. **Tubuh Tulang Kelabu Jiwa**: Damage Serangan Jiwa +35%, Sin Points tidak menambah Karma Modifier.
6. **Tubuh Benteng Pasir Emas**: HP Max +40%, Perisai Qi +50%.
7. **Tubuh Kabut Racun Bayangan**: Imun Racun Biasa & Sedang, Stealth Success +30%.
8. **Tubuh Kepak Angin Langit**: Kecepatan Gerak +40%, Peluang Escape +25%.
9. **Tubuh Naga Samudra Abadi**: Imun Tekanan Laut, Damage Air/Gelombang +35%.
10. **Tubuh Tahta Emas Huangji**: Aura Kepemimpinan (-20% Damage musuh di bawah ranah).

---

## ⚡ 6. Tribulasi Petir & Formula Karma Score

```
Tribulation_Damage = BasePunishment(realm) × KarmaModifier × BoltFactor × Random(0,8–1,2)
Karma_Score        = Merit_Points − Sin_Points
KarmaModifier      = clamp(1 + (Sin_Points − Merit_Points) / 1000, 0,5, 3,0)
```

---

## 🛡️ 7. Checklist Validasi AI GM

- [ ] Hukum/teknik yang dipakai sudah tercatat di **Law Origin Log** karakter?
- [ ] Qi reported ≤ `QiCap(realm, stage)` saat ini?
- [ ] Bahan & Core memenuhi tabel minimum §4?
- [ ] Material tier dalam rentang ±1 dari realm player?
- [ ] Insight/comprehension sudah divalidasi lewat event naratif?
- [ ] Untuk realm 7+: Tribulasi sudah dijalankan dengan formula §6?
