# ⚔️ Huangji-World — Sistem Pertempuran & Taktis (Combat & Tactical System)

> **Modul:** 15 — Tactical Turn-Based Combat & Elemental System
> **Prinsip:** Anti-Cheat Enforced — Turn-Based Action Economy — Terintegrasi dengan Sistem HP, QiCap, & Bestiary
> **Rujukan Utama:** [`INDEX.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/INDEX.md?v=1)
> **Rujukan Silang:**
> - [`00_CORE_RULES_AI_GM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/00_CORE_RULES_AI_GM.md?v=1) (Aturan Wajib AI GM)
> - [`12_CULTIVATION_LAW_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/12_CULTIVATION_LAW_SYSTEM.md?v=1) (QiCap & Law Attack Multiplier)
> - [`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1) (Grade Senjata & Durability)
> - [`14_VITALITY_HUNGER_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/14_VITALITY_HUNGER_SYSTEM.md?v=1) (HP & Penalti Kondisi Physical)
> - [`16_BESTIARY.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/16_BESTIARY.md?v=1) (Spesies Monster & Boss Stats)
> - [`18_TAMING_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/18_TAMING_SYSTEM.md?v=1) (Formasi Tempur Companion)
> - [`19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1) (Artefak Tempa & Matrix Array)

---

## 📜 0. Filosofi & Aturan Emas Pertempuran

Pertarungan di Benua Huangji adalah benturan kekuatan raga, teknik pedang, dan dominasi elemen alam semesta. Setiap pertempuran diselesaikan secara **taktis berbasis giliran (*strict turn-based tactical resolution*)** menggunakan perhitungan matematis baku.

**AI GM WAJIB menghitung setiap Inisiatif, Hit Chance, Damage, Perisai Qi, dan Efek Status menggunakan formula resmi di bawah ini.** Kemenangan tidak ditentukan oleh klaim naratif sepihak, melainkan kombinasi strategi, tingkat Ranah, keserasian Elemen, dan efisiensi pengelolaan Qi.

### 🛡️ Aturan Emas Anti-Cheat Pertempuran
1. **Aturan Giliran Bergantian**: Setelah 1 karakter bertindak, giliran otomatis berpindah ke pihak berikutnya sesuai urutan Inisiatif. Tidak ada yang boleh menyerang berturut-turut tanpa giliran mekanis.
2. **Dilarang Klaim Hasil Sepihak**: Pemain hanya menyatakan *aksi yang diambil* dan *jurus/senjata yang digunakan*. AI GM yang menghitung Hit Chance, Defense, dan Final Damage.
3. **Ekonomi Aksi Kaku (Action Economy)**: Setiap giliran (*Turn*), karakter HANYA memiliki **1 Aksi Utama** + **1 Aksi Kecil**. Deskripsi naratif yang panjang tetap dihitung sebagai 1 kali resolusi aksi mekanis.
4. **Resiko Qi Deviation saat Kritis**: Melancarkan Jurus Ultimate saat HP di bawah 25% memicu risiko *Qi Deviation* yang dapat merusak Dantian secara permanen.
5. **Pencatatan Log Bertimestamp**: Setiap pengurangan HP, penggunaan Qi, penurunan Stamina, dan status debuff wajib dicatat secara transparan pada log pertempuran di Profil Karakter.

---

## 🎲 1. Inisiatif & Struktur Ronde Pertempuran (Initiative & Round Structure)

Urutan giliran dalam pertempuran ditentukan di awal setiap Ronde Pertempuran berdasarkan **Inisiatif Score**:

$$\text{InitiativeScore} = (\text{RealmIndex} \times 10) + \text{StageBonus} + \text{SpeedBonus}(\text{Law/Physique}) + \text{Random}(1 - 20)$$

- **Realm Index**: Ranah 0 (Mortal = 0) s/d Ranah 9 (Sovereign = 9).
- **Stage Bonus**: Awal = +0, Menengah = +2, Puncak = +5.
- **Surprise Round (Serangan Mendadak)**: Jika penyerang berhasil melakukan *Stealth Check* (misal dari balik semak atau bayangan), penyerang memperoleh **1 Ronde Kejutan** (1 Aksi Utama gratis) sebelum urutan inisiatif normal dimulai.

---

## ⏳ 2. Ekonomi Aksi (Action Economy) — Anti-Spam System

Setiap karakter (Pemain, NPC, maupun Spirit Beast) dalam gilirannya **HANYA MEMILIKI**:

### 🎯 2.1 Satu Aksi Utama (*Main Action*) — Pilih Salah Satu:
- **Serang (*Attack*)**: Melancarkan Serangan Biasa, Teknik Andalan, atau Jurus Ultimate menggunakan senjata/jurus yang sah.
- **Bertahan (*Defend*)**: Mengaktifkan mode bertahan untuk menambah *Active Defense Bonus* pada turn ini.
- **Gunakan Item (*Use Item*)**: Mengonsumsi pil pemulih, obat luka, atau jimat segel dari Inventory.
- **Melarikan Diri (*Escape*)**: Mencoba kabur dari medan tempur via *Escape Check*.
- **Olah Qi / Meditasi Tempur (*Qi Focus*)**: Memulihkan +15% Qi Cap secara instan.

### 🏃 2.2 Satu Aksi Kecil (*Minor Action*) — Pilih Salah Satu:
- **Pergerakan Taktis (*Reposition/Dash*)**: Berpindah posisi dekat atau menghindari rintangan medan.
- **Komunikasi Singkat (*Brief Speech*)**: Mengucapkan satu kalimat gertakan atau instruksi ke sekutu.
- **Beralih Senjata (*Switch Equipment*)**: Mengganti senjata aktif dengan senjata lain dari Inventory.

---

## ⚔️ 3. Formula Attack Power & Multiplier 11 Hukum Kultivasi

Kekuatan serangan murni (*Attack Power*) seorang kultivator dihitung dari kapasitas Qi Maksimalnya ($QiCap$) dikalikan dengan konstanta serangan dan *LawAttackMultiplier*:

$$\text{AttackPower}(\text{Realm}, \text{Stage}, \text{Law}) = \text{QiCap}(\text{Realm}, \text{Stage}) \times 0,15 \times \text{LawAttackMultiplier}(\text{Law})$$

### 🛡️ Tabel Law Attack Multiplier Resmi 11 Hukum Kultivasi Huangji-World

| Hukum Kultivasi Resmi | LawAttackMultiplier | Karakteristik Gaya Serangan |
|---|:---:|---|
| **Hukum Akar Kayu Suci** (*Immortal Woodroot Law*) | **×0,9** | Serangan berbasis jeratan kayu & penyedotan vitalitas. |
| **Hukum Inti Petir Ungu** (*Purple Lightning Core Law*) | **×1,2** | Serangan kejut kilat dengan penetrasi jaringan saraf tinggi. |
| **Hukum Tungku Api Merah** (*Crimson Furnace Law*) | **×1,3** | Serangan membara ofensif tinggi yang membakar Dantian lawan. |
| **Hukum Istana Es Abadi** (*Eternal Frost Palace Law*) | **×1,1** | Serangan tebasan pembeku berdaya tahan defensif padat. |
| **Hukum Tahta Emas Huangji** (*Huangji Golden Throne Law*)| **×1,2** | Serangan wibawa aura keemasan pemecah pertahanan lawan. |
| **Hukum Benteng Pasir Emas** (*Golden Sand Fortress Law*)| **×0,8** | Serangan pukulan cadas berfokus pada ketahanan raga. |
| **Hukum Bayangan Jiwa Kelabu** (*Desolate Soul Shadow Law*)| **×1,1** | Serangan energi jiwa/Yin yang mengabaikan Physical Armor. |
| **Hukum Racun Teratai Hitam** (*Black Lotus Poison Law*) | **×1,4** | Serangan ber racun Miasma paling mematikan di medan tempur. |
| **Hukum Pedang Awan** (*Cloudblade Law*) | **×1,2** | Tebasan pisau angin berkecepatan tinggi yang sangat lincah. |
| **Hukum Mutiara Samudra** (*Ocean Pearl Law*) | **×1,15** | Hantaman gelombang air bertekanan tinggi yang elastis. |
| **Hukum Pisau Sunyi** (*Silent Blade Law*) | **×1,25** | Tebasan presisi eksekutor (+10% Hit Chance saat Kontrak Aktif). |
| **Fana / Tanpa Hukum** (*Mortal Realm*) | **×1,0** | Pukulan raga biasa tanpa aliran Qi. |

---

## 🎯 4. Peluang Kena (Hit Chance) & Target Lokasi Serangan

Peluang keberhasilan serangan mendarat pada target dihitung berdasarkan selisih Ranah:

$$\text{HitChance} = \text{Clamp}\left(70\% + (\text{RealmIndex}_{\text{Penyerang}} - \text{RealmIndex}_{\text{Bertahan}}) \times 5\% + \text{TargetModifier}, 10\%, 95\%\right)$$

### 🎯 4.1 Tabel Target Lokasi Serangan (Hit Location Modifiers)

Pemain dapat menargetkan anggota tubuh spesifik dengan konsekuensi penalti akurasi dan efek tambahan saat Hit:

| Bagian Tubuh Target | Target Modifier | Efek Kritis / Status Tambahan Saat Hit |
|---|:---:|---|
| **Dada / Tubuh Utama (*Torso*)** | **0%** (Standar) | Hit standar, damage sesuai kalkulasi normal. |
| **Tangan / Senjata (*Arm/Weapon*)** | **-15%** | Memicu efek *Disarm* (Senjata musuh terlepas / Hit Chance musuh -20%). |
| **Kaki / Paha (*Legs/Thigh*)** | **-15%** | Memicu efek *Crippled* (Kecepatan Gerak musuh -50% selama 2 Turn). |
| **Kepala / Leher (*Head/Neck*)** | **-30%** | **Damage $\times 1,8$** + Memicu efek *Stun/Daze* (Gagal Aksi 1 Turn). |
| **Dantian / Titik Pusar Qi** | **-35%** | **Damage $\times 2,0$** + Bocor Qi (Musuh kehilangan 20% QiCap). |

---

## 💥 5. Formula Damage Akhir & Cooldown Jurus

$$\text{RawDamage} = \text{AttackPower} \times \text{TechniqueMultiplier} \times \text{WeaponGradeBonus}$$
$$\text{TotalDefense} = \text{PassiveDefense} + \text{ActiveDefenseBonus} + \text{ArmorDefense}$$
$$\text{FinalDamage} = \max\left(1, \left[(\text{RawDamage} - \text{TotalDefense}) \times \text{ElementalMultiplier}\right] - \text{PerisaiQi}\right)$$

### 📊 Multiplier Jurus & Cooldown Rules
- **Serangan Biasa (*Basic Attack*)**: $\text{TechniqueMultiplier} = \times 1,0$ (Tanpa Cooldown, Konsumsi $5\% \text{ QiCap}$).
- **Teknik Andalan (*Signature Technique*)**: $\text{TechniqueMultiplier} = \times 1,5$ (Cooldown 1 Turn, Konsumsi $12\% \text{ QiCap}$).
- **Jurus Ultimate (*Ultimate Art*)**: $\text{TechniqueMultiplier} = \times 3,0$ (**Cooldown Wajib 3 Ronde**, Konsumsi $25\% \text{ QiCap}$).

---

## 🔮 6. Siklus 5 Elemen & Efek Status Terikat

Setiap serangan berunsur elemen tunduk pada Siklus Saling Menaklukkan 5 Elemen Huangji-World:

```text
              ┌─────────── Kayu ───────────┐
              │                            │
              ▼                            ▼
           Tanah ◄───────── Air / Es ◄─── Api
              │                            ▲
              └──────── Logam / Petir ─────┘
```

### 💥 Matriks Pengali Elemen & Efek Status

| Elemen Penyerang | Elemen Bertahan | Multiplier | Efek Status Khusus yang Dipicu |
|:---:|:---:|:---:|---|
| **Kayu** (`20`, `21`) | Tanah (`31`, `32`) | **×1,5 (Unggul)** | **Entangle**: Mengikat target di tanah (Gagal Move 1 Turn). |
| **Api** (`25`, `26`) | Kayu (`20`, `21`) | **×1,5 (Unggul)** | **Burn**: Kerusakan HP 5% HP Max per Turn selama 3 Turn. |
| **Air / Es** (`27`, `28`, `37`)| Api (`25`, `26`) | **×1,5 (Unggul)** | **Freeze**: Kecepatan gerak -50% + Output Qi -20%. |
| **Logam / Petir** (`22`, `23`)| Kayu (`20`, `21`) | **×1,5 (Unggul)** | **Paralysis**: Peluang 30% gagal melancarkan aksi tiap Turn. |
| **Tanah / Pasir** (`31`, `32`)| Air (`37`) | **×1,5 (Unggul)** | **Stun**: Pusing hebat, kehilangan 1 Turn penuh. |
| **Elemen Sama** | Elemen Sama | **×0,75 (Resisted)**| Tidak memicu status efek tambahan. |
| **Elemen Lemah** | Elemen Unggul | **×0,5 (Weak)** | Damage terpotong setengah, tidak ada status efek. |

---

## 🛡️ 7. Perisai Qi & Aturan Pelarian Diri (Escape System)

### 🛡️ 7.1 Perisai Qi (*Qi Barrier*)
Pemain dapat menginvestasikan sejumlah Qi untuk membentuk Perisai Pertahanan sebelum menerima serangan:

$$\text{PerisaiQi} = \text{QiInvested} \times 2,0$$
- Perisai Qi menyerap damage terlebih dahulu sebelum mengikis HP raga.
- Perisai Qi bertahan selama 1 Turn atau hingga hancur tergerus damage musuh.

---

### 🏃 7.2 Aturan Pelarian Diri (*Escape Rules*)
Untuk melarikan diri dari pertarungan di area liar:

$$\text{EscapeScore} = \text{PlayerSpeed} + \text{D20Check}$$
$$\text{DifficultyScore} = \text{EnemySpeed} + \text{D20Check}$$
- **Jika $\text{EscapeScore} > \text{DifficultyScore}$**: Pemain berhasil melarikan diri ke area aman terdekat.
- **Jika $\text{EscapeScore} \le \text{DifficultyScore}$**: Pelarian **GAGAL**. Musuh memperoleh 1 kali serangan bebas (*Opportunity Attack*) ke punggung pemain.

---

## 🛡️ 8. Checklist Validasi & Anti-Cheat AI GM

Sebelum merilis hasil pertempuran pada setiap Turn, AI GM **wajib** memeriksa checklist berikut:

- [ ] Apakah urutan inisiatif telah dihitung di awal ronde dan dipatuhi tanpa ada pihak yang melompati giliran?
- [ ] Apakah pemain hanya menggunakan **1 Aksi Utama + 1 Aksi Kecil** dalam gilirannya?
- [ ] Apakah `AttackPower` dihitung menggunakan `LawAttackMultiplier` yang tepat dari 11 Hukum Kultivasi?
- [ ] Apakah `HitChance` dihitung dengan memperhitungkan selisih Ranah dan penalti lokasi target serangan?
- [ ] Apakah Jurus Ultimate ditegakkan aturan **Cooldown Wajib 3 Ronde**?
- [ ] Apakah konsumsi Qi per aksi dipotong secara tepat dari ketersediaan Qi karakter?
- [ ] Apakah pengali Elemen ($\times 1,5 / \times 0,75 / \times 0,5$) applied sesuai matriks 5 Elemen Huangji-World?
