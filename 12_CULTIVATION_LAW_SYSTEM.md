# 📜 Huangji-World — Sistem Hukum Kultivasi (Cultivation Laws System)

> **Modul:** 12 — Cultivation Law System
> **Prinsip:** Anti-Cheat Enforced — Stable Tier Scaling — Karma-Linked Tribulation
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md` (aturan wajib), `13_ECONOMY_SYSTEM.md` (harga bahan), `14_VITALITY_HUNGER_SYSTEM.md` (HP), `15_COMBAT_SYSTEM.md` (Combat), modul wilayah `01`–`10`

---

## 🧭 1. Filosofi Sistem

Setiap "Hukum" (Law) adalah jalur kultivasi berbeda dengan sumber daya berbeda (Qi Murni, Qi Petir, Qi Api Vulkanik, dll.), tetapi **semua Hukum tunduk pada satu Formula Batas Qi (Qi Cap Formula)** yang sama, supaya tidak ada jalur yang overpowered dibanding yang lain.

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

## 🔐 3. Asal-Usul Hukum (Law Origin) — WAJIB SEBELUM APAPUN

| Jalur Asal-Usul | Syarat Sah | Contoh Tidak Sah (Ditolak) |
|---|---|---|
| **1. Guru (Master/Mentor)** | Harus ada NPC guru yang sudah diperkenalkan & berinteraksi lewat adegan pengajaran nyata. | Tiba-tiba mengaku punya guru Hukum Petir tanpa pernah ada di narasi. |
| **2. Manual/Kitab Pusaka** | Kitab/manual harus sudah ada di inventory karakter lewat cara yang sah dan tercatat. | Mengaku punya kitab rahasia tepat sebelum terobosan. |
| **3. Pencerahan (Genuine Enlightenment)** | Hanya bisa dipicu **oleh AI GM** setelah Insight Point terkumpul cukup. | Mengaku tiba-tiba tercerahkan di tengah pertarungan tanpa proses insight. |

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
