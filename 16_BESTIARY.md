# 🐉 Huangji-World — Bestiary & Katalog Monster (Monster & Spirit Beast System)

> **Modul:** 16 — Bestiary System
> **Prinsip:** Anti-Cheat Enforced — Habitat-Locked — Terintegrasi dengan System HP, Combat, & Item Origin Log
> **Rujukan Silang:** `12_CULTIVATION_LAW_SYSTEM.md`, `13_ECONOMY_SYSTEM.md`, `15_COMBAT_SYSTEM.md`, modul wilayah `01`–`10`

---

## 0. Filosofi Sistem

Setiap Spirit Beast dan Monster di dunia ini tunduk pada batas kekuatan, habitat resmi, dan formula drop loot. Monster tidak muncul sekehendak hati pemain, dan loot tidak pernah jatuh tanpa validasi AI GM.

### Aturan Emas Anti-Cheat Bestiary
- HP & Attack Power monster dihitung dari formula berbasis QiCap, bukan klaim sepihak player.
- Kemunculan monster (ambush) dilempar via `AmbushChance` oleh AI GM, bukan diatur sepihak oleh player.
- Monster Tier tinggi hanya muncul di habitat resminya, tidak di zona pemukiman biasa.
- Loot hanya didapat setelah monster dikalahkan di roleplay dan dicatat di Item Origin Log.

---

## 🎲 1. Mekanisme Ambush & Formasi Encounter

$$\text{AmbushChance} = 5\% \times \text{DangerModifier} \times \text{TimeModifier}$$

| Modifier | Nilai |
|---|---|
| **DangerModifier — Area Pemukiman / Jalan Utama** | ×0,5 |
| **DangerModifier — Wilayah Hutan / Pegunungan Normal** | ×1,0 |
| **DangerModifier — Zona Liar / Rawa / Gurun Liar** | ×2,0 |
| **DangerModifier — Zona Terlarang / Kawah / Palung Dalam** | ×4,0 |
| **TimeModifier — Siang Hari** | ×1,0 |
| **TimeModifier — Malam Hari** | ×2,0 |

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

### 🌿 1. Dataran Hijau Abadi (Verdant Qi Plains)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Kelinci Qi Rumput Hijau** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 30 | 5 | Kelinci pemakan herba. Cepat lari. | Umum: Daging Kelinci Fana (+10% Satiety) |
| **Ayam Hutan Spirit Kayu** | 🐺 Spirit Beast Liar | Tier 0 (Mortal Refining) | 40 | 8 | Ayam liar bertanduk kayu kecil. | Umum: Daging Ayam Spirit, Bulu Warna-Warni |
| **Serigala Akar Hijau** | 🐺 Spirit Beast | Tier 2, Awal (Qi Gathering) | 120 | 25 | Menyergap dengan *Gigitan Akar Duri*. | Umum: Kulit Serigala — Jarang: Core Beast Tier 1 |
| **Beruang Kayu Kuno** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 450 | 80 | *Hantaman Batang Jati* (Damage 80 & Stun). | Umum: Empedu Beruang — Jarang: Core Beast Tier 2 |

### ⚡ 2. Pegunungan Petir Guntur (Thunder Crest Range)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Ular Besi Tembaga** | 🐺 Spirit Beast | Tier 2, Awal (Qi Gathering) | 100 | 30 | Bersisik tembaga. *Patukan Listrik*. | Umum: Sisik Besi — Jarang: Core Beast Tier 1 |
| **Elang Kilat Ungu** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 380 | 95 | Menukik dari Puncak Petir. | Umum: Bulu Kilat — Jarang: Core Beast Tier 2 |

### 🔥 3. Lembah Api Merah (Crimson Blaze Valley)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Salamander Magma** | 🔥 Elemental (Api) | Tier 3, Awal (Foundation) | 400 | 85 | Melontarkan *Semburan Lahar*. | Umum: Kulit Tahan Api — Jarang: Core Beast Tier 2 |
| **Kera Api Purba** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.200 | 220 | *Hujan Batu Magma Meledak*. | Umum: Tangan Kera Api — Jarang: Core Beast Tier 3 |

### ❄️ 4. Danau Es Bintang (Frost Star Lake)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Hiu Es Kristal** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 420 | 90 | *Tandukan Sirip Es* (Freeze). | Umum: Sirip Hiu Es — Jarang: Core Beast Tier 2 |

### 💀 5. Tanah Gersang Tulang (Desolate Bone Wasteland)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Kalajengking Tulang Kelabu** | 🐛 Insect / Gu | Tier 3, Awal (Foundation) | 360 | 75 | *Sengatan Racun Jiwa*. | Umum: Sengat Kalajengking — Jarang: Core Beast Tier 2 |

### 🏜️ 6. Gurun Pasir Emas (Golden Sand Desert)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Cacing Pasir Raksasa** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.500 | 250 | *Pusaran Telan Pasir*. | Umum: Kulit Cacing Gurun — Jarang: Core Beast Tier 3 |

### ☣️ 7. Rawa Kabut Racun (Shadow Mist Swamp)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Katak Teratai Hitam** | 🐺 Spirit Beast | Tier 3, Awal (Foundation) | 390 | 80 | *Lembatan Lidah Beracun*. | Umum: Lendir Katak — Jarang: Core Beast Tier 2 |

### 🏔️ 8. Puncak Langit Surgawi (Celestial Sky Peaks)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Burung Rajawali Angin Tajam** | 🐺 Spirit Beast | Tier 4, Awal (Golden Core) | 1.100 | 210 | *Tebasan Badai Angin*. | Umum: Bulu Angin — Jarang: Core Beast Tier 3 |

### 🌊 9. Kepulauan Palung Samudra (Oceanic Abyss Islands)
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Gurita Palung Samudra** | 🐺 Spirit Beast | Tier 5, Awal (Nascent Soul) | 3.800 | 450 | *Cengkeraman Sembilan Tentakel*. | Umum: Tinta Gurita — Jarang: Core Beast Tier 4 |

### 🐉 10. Boss & Monster Langka Lintas Wilayah
| Nama Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| **Naga Kabut Purba Huangji** | 🗿 Ancient Guardian | Tier 8, Awal (Tribulation) | 350.000 | 45.000 | Penjaga perbatasan benua. | Legendaris (100% First Kill): Sisik Naga Purba |

---

## 4. Checklist Validasi AI GM

- [ ] HP & Attack Power monster dihitung dari formula resmi?
- [ ] AmbushChance dilempar oleh AI GM?
- [ ] Monster terkunci pada habitat resminya?
- [ ] Loot tercatat di Item Origin Log setelah pertarungan selesai?
