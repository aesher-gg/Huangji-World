# ⚔️ Huangji-World — Sistem Pertempuran & Elemen (Combat & Elemental System)

> **Modul:** 15 — Tactical Turn-Based Combat & Elemental Mechanics
> **Prinsip:** Anti-Cheat Enforced — Turn-Based Resolution — Terintegrasi dengan Sistem HP, QiCap, & Equipment
> **Rujukan Silang:** `00_CORE_RULES_AI_GM.md` (aturan wajib), `12_CULTIVATION_LAW_SYSTEM.md` (QiCap & Law), `13_ECONOMY_SYSTEM.md` (Grade Senjata), `14_VITALITY_HUNGER_SYSTEM.md` (HP & Penalti Luka)

---

## 0. Filosofi Sistem

Pertarungan di Benua Huangji adalah benturan kekuatan raga, teknik pedang, dan dominasi elemen alam. Setiap pertempuran diselesaikan secara **berbasis giliran (*turn-based tactical resolution*)** menggunakan perhitungan matematis yang pasti.

**AI GM WAJIB menghitung setiap Hit Chance, Damage, Perisai Qi, dan Efek Status menggunakan formula resmi di bawah ini.** Kemenangan tidak ditentukan oleh narasi pahlawan semata, melainkan kombinasi strategi, tingkat Ranah, keserasian Elemen, dan efisiensi pengelolaan Qi.

### Aturan Emas Anti-Cheat Pertempuran
1. **Dilarang Klaim Hit/Damage Sepihak**: Semua hit chance dan besaran damage dihitung mutlak oleh AI GM. Player hanya menyatakan *jenis aksi* dan *teknik/senjata yang dipakai*.
2. **Struktur Turn yang Kaku**: Setiap giliran (*turn*) terdiri dari: **1 Aksi Utama** (Serangan / Jurus Qi / Meditasi) + **1 Aksi Pergerakan/Kecil** (Dodge, Dash, Pakai Pil, Ganti Senjata).
3. **Pencatatan Log Bertimestamp**: Setiap pengurangan HP, konsumsi Qi, penurunan Stamina, dan status debuff wajib dicatat secara transparan pada log pertempuran di Profil Karakter.
4. **Resiko Qi Deviation saat Kritis**: Melancarkan jurus Qi berdaya besar saat HP di bawah 25% memicu risiko *Qi Deviation* yang dapat merusak Dantian secara permanen.
5. **Aturan Kabur (*Escape*)**: Pelarian diri dari pertempuran hanya sah jika memenuhi *Escape Check* berbasis Kecepatan Gerak dan Kecepatan Reaksi.

---

## 🎲 1. Struktur Giliran & Urutan Inisiatif (Turn Order & Initiative)

Urutan giliran dalam pertempuran ditentukan di awal giliran pertama berdasarkan **Inisiatif Speed**:

```
Initiative_Score = BaseSpeed(realm, law) + SpeedBonus(equipment/physique) + Random(1–20)
```

- Karakter/NPC dengan `Initiative_Score` tertinggi melancarkan aksinya terlebih dahulu.
- **Surprise Round (Serangan Mendadak)**: Jika lawan berhasil melakukan *Stealth Check* (misal dari balik semak/bayangan), penyerang mendapatkan **Surprise Round** (1 turn gratis tanpa balasan) sebelum giliran inisiatif normal dimulai.

---

## 🎯 2. Formula Hit Chance & Lokasi Serangan (Hit Chance & Location)

Peluang keberhasilan serangan mendarat pada target dihitung menggunakan formula perbedaan ranah dan modifier lingkungan:

```
HitChance = clamp(BaseHit (70%) + (RealmIndex_Penyerang − RealmIndex_Bertahan) × 5% + Modifier, 10%, 95%)
```

### 🎯 2.1 Tabel Target Lokasi Serangan (Hit Location Modifier)

Pemain dapat memilih bagian tubuh spesifik yang diserang dengan konsekuensi marjin kesalahan (*Hit Penalty*) dan efek kritikal berbeda:

| Bagian Tubuh Target | Penalti Hit Chance | Efek Kritikal / Luka Tambahan Saat Hit |
|---|:---:|---|
| **Dada / Tubuh Utama (Torso)** | **0%** (Standar) | Hit standar, damage sesuai kalkulasi normal. |
| **Tangan / Senjata (Limb - Arm)** | **−15%** | Memicu efek *Disarm* (Senjata musuh terlepas) / Hit Chance musuh −20%. |
| **Kaki / Paha (Limb - Leg)** | **−15%** | Memicu efek *Crippled* (Move Speed musuh −50% selama 2 turn). |
| **Kepala / Leher (Head - Vital)** | **−30%** | **Damage x1,8** + Memicu efek *Stun/Daze* (Gagal Aksi 1 Turn). |
| **Dantian / Titik Pusar Qi** | **−35%** | **Damage x2,0** + Membocorkan Qi musuh sebesar 20% QiCap. |

---

## ⚔️ 3. Formula Attack Power, Defense, & Final Damage

```
AttackPower = (QiCap × 0,15 × LawAttackMultiplier) + BaseDamageSenjata + QiBonus
PassiveDefense = (QiCap × 0,05) + BaseDefenseZirah + PhysiqueDefBonus
```

### 💥 Formula Final Damage (Damage Akhir)

$$\text{FinalDamage} = \max\left(1, \left[(\text{AttackPower} - \text{PassiveDefense}) \times \text{ElementalMultiplier}\right] - \text{Perisai Qi}\right)$$

---

## 🔮 4. Matriks Elemen & Status Effect (Elemental Affinity Matrix)

Setiap Hukum Kultivasi resmi terikat pada salah satu Elemen Alam semesta. Efektivitas serangan ditentukan oleh siklus saling menaklukkan antar elemen:

```
              ┌─────────── Kayu ───────────┐
              │                            │
              ▼                            ▼
           Tanah ◄───────── Air / Es ◄─── Api
              │                            ▲
              └──────── Logam / Petir ─────┘
```

---

### 💥 Matriks Pengali Elemen & Efek Status Dipicu

| Elemen Penyerang | Elemen Bertahan | Multiplier | Efek Status Khusus yang Dipicu |
|:---:|:---:|:---:|---|
| **Kayu** (`20`, `21`) | Tanah (`31`, `32`) | **×1,5 (Unggul)** | **Entangle**: Mengikat target di tanah (Gagal Move 1 turn). |
| **Api** (`25`, `26`) | Kayu (`20`, `21`) | **×1,5 (Unggul)** | **Burn**: Kerusakan HP 5% HP_Max per turn selama 3 turn. |
| **Air / Es** (`27`, `28`, `37`) | Api (`25`, `26`) | **×1,5 (Unggul)** | **Freeze**: Kecepatan gerak −50% + Output Qi −20%. |
| **Logam / Petir** (`22`, `23`) | Kayu (`20`, `21`) | **×1,5 (Unggul)** | **Paralysis**: Peluang 30% gagal melancarkan aksi tiap turn. |
| **Tanah / Pasir** (`31`, `32`) | Air (`37`) | **×1,5 (Unggul)** | **Stun**: Pusing hebat, kehilangan 1 turn penuh. |
| **Elemen Sama** | Elemen Sama | **×0,75 (Resisted)**| Tidak memicu status efek tambahan. |
| **Elemen Lemah** | Elemen Unggul | **×0,5 (Weak)** | Damage terpotong setengah, tidak ada status efek. |

---

## 🧬 5. Mekanik Status Effect & Debuff Khusus

| Nama Status Effect | Cara Menghilangkan / Menyembuhkan | Efek Mekanik pada Karakter / NPC |
|---|---|---|
| **Burn (Terkikis Api)** | *Salep Es Bintang* / Meditasi Es 1 turn. | Kehilangan 5% HP_Max di awal setiap turn. |
| **Freeze (Pembekuan Es)**| *Pil Pembakar Api* / Serangan Api sekutu. | Hit Chance −20%, Move Speed −50%. |
| **Paralysis (Lumpuh Kilat)**| *Pil Netralisir Petir* / Istirahat 2 turn. | Peluang 30% aksi membalas/menyerang gagal total. |
| **Poison (Keracunan Miasma)**| *Pil Penawar Seribu Racun* (`19`). | Kehilangan 3% HP_Max + Stamina Regen −50% per turn. |
| **Bleeding (Pendarahan)**| *Salep Herba Vitalitas* / Tabib (`37`). | Kehilangan 4% HP_Max setiap kali bergerak/menyerang. |
| **Qi Deviation (Guncangan)**| *Pil Penambal Dantian* / Meditasi 1 bulan.| Penggunaan Qi memicu damage ke HP sendiri sebesar QiCost. |

---

## 🛡️ 6. Sistem Perisai Qi & Pelarian Diri (Qi Barrier & Escape System)

### 🛡️ 6.1 Perisai Qi (Qi Barrier)
Pemain dapat menginvestasikan sejumlah Qi untuk membentuk Perisai Pertahanan sebelum menerima serangan:

```
PerisaiQi = Qi_Invested × 2,0
```
- Perisai Qi menyerap damage terlebih dahulu sebelum mengikis HP raga.
- Perisai Qi bertahan selama 1 turn atau hingga hancur tergerus damage musuh.

---

### 🏃 6.2 Aturan Pelarian Diri (Escape Rules)
Untuk melarikan diri dari pertarungan di area liar:

```
Escape_Score = PlayerSpeed + D20_Check
Difficulty_Score = EnemySpeed + D20_Check
```
- Jika `Escape_Score > Difficulty_Score`: Pemain berhasil melarikan diri ke area aman terdekat.
- Jika `Escape_Score ≤ Difficulty_Score`: Pelarian **GAGAL**. Musuh mendapatkan 1 kali serangan bebas (*Free Attack*) ke punggung pemain.

---

## 🛡️ 7. Checklist Validasi AI GM (Wajib Diperiksa Tiap Combat Turn)

- [ ] Apakah `HitChance` dihitung memakai perbedaan ranah dan penalti lokasi target serangan?
- [ ] Apakah `FinalDamage` telah mengkalkulasikan `AttackPower`, `PassiveDefense`, `ElementalMultiplier`, dan `Perisai Qi`?
- [ ] Apakah penggunaan Qi untuk teknik berada dalam batas `QiCap` karakter saat ini?
- [ ] Apakah status efek dipicu dan dicatat durasinya di log status pertempuran?
- [ ] Apakah pengurangan HP/Qi/Stamina setelah giliran selesai telah diperbarui di *Profil Karakter*?
