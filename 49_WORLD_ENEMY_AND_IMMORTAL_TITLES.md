# 👁️‍🗨️ Huangji-World — Sistem Musuh Dunia & Gelar Kehormatan (World Enemy & Immortal Titles System)

> **Modul:** 49 — World Enemy, Imperial Bounty & Reputation Titles System
> **Prinsip:** Anti-Cheat Enforced — Karma-Driven — Bounty-Enforced — Title-Buffed
> **Rujukan Utama:** [`INDEX.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/INDEX.md?v=1)
> **Rujukan Silang:**
> - [`00_CORE_RULES_AI_GM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/00_CORE_RULES_AI_GM.md?v=1) (Aturan Wajib AI GM)
> - [`01`–`10`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/01_WORLD_OVERVIEW_AND_CAPITAL.md?v=1) (Papan Buronan & Markas Faksi)
> - [`11_CROSS_REGION_ORGANIZATIONS.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/11_CROSS_REGION_ORGANIZATIONS.md?v=1) (Organisasi Pemburu Bayaran)
> - [`12_CULTIVATION_LAW_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/12_CULTIVATION_LAW_SYSTEM.md?v=1) (Poin Karma Sin & Merit)
> - [`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1) (Mata Uang Tael & Imbalan Buronan)
> - [`33_PERKUMPULAN_PISAU_SUNYI_HUANGJI.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/33_PERKUMPULAN_PISAU_SUNYI_HUANGJI.md?v=1) (Eksekusi Kontrak Pembunuhan)

---

## 📜 0. Filosofi & Aturan Emas Reputasi & Musuh Dunia

Di Benua Huangji, tatanan moralitas dan keadilan dijaga ketat oleh Kekaisaran Agung Huangji dan Sekte-Sekte Ortodoks Utama. Setiap tindakan karakter meninggalkan jejak **Poin Karma (*Merit Points & Sin Points*)**. Seseorang yang membantai manusia fana secara masif, menyerap Dantian kultivator lain secara haram, atau mengkhianati sekte akan dicap sebagai **Musuh Dunia (*Public Enemy of Huangji-World*)** dan diburu oleh seluruh belahan benua.

Sebaliknya, kultivator yang menegakkan keadilan, membantai iblis purba, atau memenangkan Turnamen Kekaisaran akan dianugerahi **Gelar Kehormatan Abadi (*Immortal Titles*)** yang memberikan aura wibawa dan bonus statistik pasif.

**AI GM WAJIB melacak perubahan Poin Sin/Merit dan memperbarui status Buronan serta Gelar Karakter pada setiap giliran.**

### 🛡️ Aturan Emas Anti-Cheat World Enemy & Titles
1. **Aturan Ambang Sin Mutlak**: Seseorang secara otomatis dicap sebagai **Musuh Dunia (*Red Star Mark*)** apabila Poin Dosa Karma mencapai **$\text{Sin Points} \ge 300$** atau membantai Pejabat Utama Kekaisaran.
2. **Pelacakan Kompas Imperial**: Musuh Dunia dicatat pada Papan Buronan Seluruh 10 Wilayah. Kecepatan kemunculan pemburu bayaran (*Encounter Rate*) meningkat **$\times 5$**.
3. **Embargo Ekonomi Total**: Seluruh Toko, Balai Lelang, Penginapan, dan Rumah Gadai resmi menolak melayani Musuh Dunia.
4. **Batas Maksimal 2 Gelar Aktif**: Setiap karakter hanya dapat mengaktifkan maksimal **2 Gelar Kehormatan sekaligus** untuk memperoleh bonus buff pasifnya.

---

## 🔴 1. Mekanik Penetapan Musuh Dunia (Public Enemy Decree)

Seseorang ditetapkan sebagai **Musuh Dunia (*World Enemy*)** apabila memenuhi salah satu kriteria kejahatan berat berikut:

### ⚠️ Syarat Penetapan Status Red Star
- Accumulasi Poin Dosa Karma ($\text{Sin Points} \ge 300$).
- Menggunakan *Hukum Terlarang Penyerap Dantian / Sacrificial Ritual* pada kota fana.
- Membunuh Pejabat Tinggi Istana Imperial atau Ketua Sekte Utama.

---

### 🚫 Dampak Status Musuh Dunia (*Red Star Penalty*)
1. **Embargo Ekonomi & Kota**: Penjaga pintu gerbang kota melarang masuk. Toko dan Penginapan resmi menolak transaksi.
2. **Pelacakan Kompas Imperial (*Red Star Compass*)**: Posisi geografis Musuh Dunia terdeteksi oleh Kompas Garda Kekaisaran setiap 6 Jam In-Game.
3. **Penyergapan Pemburu Bayaran (*Aggressive Hunting*)**: AI GM melancarkan penyergapan pemburu bayaran dari Perkumpulan Pisau Sunyi ([`33`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/33_PERKUMPULAN_PISAU_SUNYI_HUANGJI.md?v=1)) atau Garda Imperial setiap kali karakter melintasi jalur umum.

---

## 🗡️ 2. Papan Buronan Kekaisaran 5 Tingkat (Imperial Bounty List)

Pemerintah Kekaisaran Agung Huangji memajang nama-nama buronan di Papan Buronan (*Imperial Bounty Boards*) di seluruh 10 wilayah dengan imbalan mata uang Tael dan Batu Spiritual ([`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1)):

| Tingkat Buronan | Syarat Akumulasi Sin Points | Imbalan Buronan (*Bounty Reward*) | Eksekutor Pemburu yang Dikirim |
|:---:|---|---|---|
| **Bounty Bintang 1** | Sin 50 – 149 Points | 100 Tael Giok Putih Kekaisaran | Penjaga Benteng Lokal & Pemburu Fana |
| **Bounty Bintang 2** | Sin 150 – 299 Points | 10 Batu Spiritual Rendah | Pemburu Bayaran *Pisau Sunyi* T3 ([`33`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/33_PERKUMPULAN_PISAU_SUNYI_HUANGJI.md?v=1)) |
| **Bounty Bintang 3 (Musuh Dunia)** | Sin 300 – 499 Points | 50 Batu Spiritual Rendah + Senjata T4 | *Garda Bayangan Imperial T4* & Aliansi Sekte |
| **Bounty Bintang 4 (Ancaman Benua)**| Sin 500 – 999 Points | 20 Batu Spiritual Menengah + Material T6 | Tetua Sekte Utama T5 & Pemburu Tingkat Atas |
| **Bounty Bintang 5 (Pemusnah Alam)**| Sin 1.000+ Points | 100 Batu Spiritual Menengah + Artefak T8 | *Sovereign Guardians T8/T9* & Tentara Gabungan |

---

## 📜 3. Katalog Gelar Kehormatan Abadi (Immortal Titles)

Kultivator jalur kebaikan (*Righteous Path*), netral, maupun iblis (*Demonic Path*) dapat memperoleh **Gelar Kehormatan** setelah menyelesaikan pencapaian besar:

### 🌟 3.1 Gelar Jalur Kebajikan & Pahlawan (*Righteous Titles*)

| Nama Gelar Kehormatan | Syarat Pencapaian Sah | Bonus Buff Pasif Karakter |
|---|---|---|
| **Pahlawan Lembah** | Merit Points $\ge 100$ di 1 Wilayah | Diskon **10%** Belanja & Penginapan di Wilayah tersebut. |
| **Pembersih Miasma** | Membasmi 50+ Beast Rawa / Iblis | Imunitas terhadap Debuff *Poison Miasma* Tier 1–2. |
| **Pedang Suci Huangji** | Memenangkan Turnamen Akademi Imperial | **Aura Pressure**: Mereduksi Attack Power musuh di bawah Inti Emas sebesar **-10%**. |
| **Tabib Dermawan** | Menyembuhkan 100+ Warga Fana | Kecepatan pemulihan HP alami karakter **+25%**. |
| **Penguasa Benua** | Mencapai Ranah Sovereign (Realm 9) | Imun Hukuman Buronan & Disembah oleh seluruh NPC Fana. |

---

### 💀 3.2 Gelar Jalur Iblis & Outlaw (*Demonic & Outlaw Titles*)

| Nama Gelar Kejahatan | Syarat Pencapaian Sah | Bonus Buff Pasif Karakter |
|---|---|---|
| **Tangan Blood-Shed** | Membunuh 30+ Kultivator Ortodoks | Physical Attack Damage **+15%**, namun Sin Points bertambah +10. |
| **Raja Bayangan Kelam** | Sin Points $\ge 200$ + Anggota Pisau Sunyi | Keberhasilan Aksi *Stealth & Ambush* **+25%**. |
| **Penyerap Dantian** | Menyerap 10 Dantian Kultivator | Output Damage Jurus Yin **+20%**, namun *HeartDevilChance* **+15%**. |

---

## 📄 4. Format Title & Reputation Sheet pada Profil Karakter

Seluruh reputasi, poin Karma, dan Gelar yang dimiliki dicatat dalam format resmi berikut pada Profil Karakter:

```text
[Title & Reputation Sheet — Status Reputasi]
- Poin Karma: Merit: 150 Points | Sin: 12 Points (Status: Terpuji / Righteous)
- Gelar Aktif 1: Pedang Suci Huangji (Buff: Aura Pressure -10% Atk Power Musuh)
- Gelar Aktif 2: Pembersih Miasma (Buff: Imun Poison Miasma T1–2)
- Status Buronan: Bebas / Tidak Ada Bounty
- Tanggal Gelar Dianugerahkan: Tahun 1, Bulan 9, Hari 15
```

---

## 🛡️ 5. Checklist Validasi & Anti-Cheat AI GM

Sebelum menetapkan status Musuh Dunia atau memberikan bonus Gelar Kehormatan, AI GM **wajib** memeriksa checklist berikut:

- [ ] Apakah akumulasi Sin Points dan Merit Points dicatat secara tepat pada Profil Karakter?
- [ ] Jika Sin Points $\ge 300$, apakah status Musuh Dunia (*Red Star Mark*) dan embargo ekonomi kota diterapkan?
- [ ] Apakah multiplier kemunculan pemburu bayaran ($\times 5$) dijalankan saat Musuh Dunia melintasi jalur umum?
- [ ] Apakah pemain hanya mengaktifkan maksimal **2 Gelar Kehormatan sekaligus**?
- [ ] Apakah imbalan pencabutan buronan dicatat memakai mata uang Tael / Batu Spiritual yang sah?
