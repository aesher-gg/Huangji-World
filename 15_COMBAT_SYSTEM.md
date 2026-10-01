# ⚔️ Huangji-World — Sistem Pertempuran (Combat System)

> **Modul:** 15 — Combat System
> **Prinsip:** Anti-Cheat Enforced — Turn-Based Resolution — Terintegrasi dengan System HP & QiCap
> **Rujukan Silang:** `12_CULTIVATION_LAW_SYSTEM.md` (QiCap & Law), `14_VITALITY_HUNGER_SYSTEM.md` (HP & Damage)

---

## 0. Filosofi Sistem

Pertarungan di dunia ini diselesaikan secara turn-based dengan formula matematis pasti. Tidak ada kemenangan "ajaib" tanpa perhitungan rasional atas Realm, Qi, Senjata, dan Pengali Elemen.

### Aturan Emas Anti-Cheat Pertempuran
- Damage dan Hit Chance dihitung AI GM lewat formula — bukan klaim sepihak player.
- Setiap serangan dan aksi pertarungan bertimestamp dan dicatat di log pertempuran.
- Mengganti/memasang Equipment saat bertarung membutuhkan 1 Aksi Kecil.
- Pelarian diri (Escape) tunduk pada pengecekan inisiatif & kecepatan gerak.

---

## 1. Formula Pertempuran Dasar

### 1.1 Hit Chance (Peluang Kena)
```
HitChance = clamp(70% + (RealmIndex_penyerang − RealmIndex_bertahan) × 5%, 10%, 95%)
```

### 1.2 Formula Attack Power & Defense
```
AttackPower    = QiCap × 0,15 × LawAttackMultiplier(law) + BaseDamageSenjata
PassiveDefense = QiCap × 0,05 + BaseDefenseZirah
```

### 1.3 Formula Damage Akhir (Final Damage)
$$\text{FinalDamage} = \left[(\text{AttackPower} - \text{PassiveDefense}) \times \text{ElementalMultiplier}\right] - \text{Perisai Qi}$$

---

## 2. Tabel Pengali Elemen (Elemental Affinity Chart)

| Elemen Penyerang | Elemen Bertahan | Pengali Damage | Status Efek Dipicu |
|---|---|---|---|
| **Kayu** | Tanah | **1.5x (Super Effective)** | Entangle (Root 1 Turn) |
| **Api** | Kayu | **1.5x (Super Effective)** | Burn Damage (10 HP / Turn) |
| **Air / Es** | Api | **1.5x (Super Effective)** | Freeze (-20% Movement Speed) |
| **Logam / Petir** | Kayu | **1.5x (Super Effective)** | Paralysis (Peluang Skip Turn 25%) |
| **Tanah** | Air | **1.5x (Super Effective)** | Stun (Gagal Aksi Pergerakan) |
| **Elemen Sama** | Elemen Sama | **0.75x (Resisted)** | No Status Effect |

---

## 3. Perisai Qi (Qi Barrier) & Escape Rules

* **Perisai Qi**: 1 Poin Qi diinvestasikan menjadi **2 Poin Perisai Qi**.
* **Formula Escape Check**: `Kecepatan Gerak Pemain + D20` vs `Kecepatan Gerak Musuh + D20`.

---

## 4. Checklist Validasi AI GM

- [ ] Hit Chance dan Final Damage dihitung dari formula resmi?
- [ ] Pengali elemen diterapkan dengan benar?
- [ ] Perisai Qi mengurangi damage sebelum memotong HP?
- [ ] Log pertarungan bertimestamp dan tidak diedit mundur?
