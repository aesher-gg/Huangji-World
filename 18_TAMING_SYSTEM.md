# 🐾 Huangji-World — Sistem Penjinakan Spirit Beast (Taming System)

> **Modul:** 18 — Spirit Beast Taming & Companion System
> **Prinsip:** Anti-Cheat Enforced — Willpower & Loyalty Dependent — Terintegrasi dengan Bestiary & Pertempuran
> **Rujukan Utama:** [`INDEX.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/INDEX.md?v=1)
> **Rujukan Silang:**
> - [`00_CORE_RULES_AI_GM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/00_CORE_RULES_AI_GM.md?v=1) (Aturan Wajib AI GM)
> - [`12_CULTIVATION_LAW_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/12_CULTIVATION_LAW_SYSTEM.md?v=1) (Ranah Kultivasi & Qi Cap)
> - [`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1) (Mata Uang Tael & Harga Segel)
> - [`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1) (Formasi Tempur Companion)
> - [`16_BESTIARY.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/16_BESTIARY.md?v=1) (Spesies Beast & Taming LV)

---

## 📜 0. Filosofi & Aturan Emas Penjinakan

Di Benua Huangji, menjinakkan Spirit Beast (Monster Roh) adalah seni mengikat Jiwa dan Kesadaran antara Kultivator dan Makhluk Gaib. Penjinakan bukan sekadar menaklukkan binatang dengan kekerasan, melainkan memerlukan pelemahan fisik target, penggunaan jimat/kontrak segel jiwa, serta uji benturan kekuatan kehendak (*Willpower Check / Soul Affinity*).

**AI GM WAJIB menghitung kalkulasi Success Rate dan Soul Backfire secara transparan sebelum menetapkan status penjinakan.**

### 🛡️ Aturan Emas Anti-Cheat Taming
1. **Syarat Pelemahan HP**: Spirit Beast **TIDAK BISA** dijinakkan saat HP-nya berada di atas **30% dari HP Maksimal**, kecuali menggunakan *Jimat Kontrak Master Grade (Tier 6+)* atau pakan pelet aroma khusus (*Sedative Potion*).
2. **Kalkulasi Terbuka AI GM**: AI GM wajib mencantumkan perhitungan peluang sukses penjinakan secara terbuka sebelum memunculkan hasil giliran (*Turn*).
3. **Resiko Soul Backfire (Bait Jiwa)**: Kegagalan penjinakan pada beast yang peringkatnya lebih tinggi dari ranah kultivasi pemain memicu **Soul Backfire** — memberikan Damage Jiwa sebesar 30% HP Max pemain dan efek *Stun* selama 1 Turn.
4. **Pencatatan Companion Sheet**: Setiap beast yang berhasil dijinakkan wajib memiliki slot khusus di profil karakter (`Spirit Beast Companion`) yang mencatat HP, Qi, Tier, Kesetiaan (*Loyalty*), dan Kemampuan Aktif.

---

## 📜 1. Media Segel & Jimat Penjinak (Taming Seals Tiers 1–9)

Kultivator memerlukan media spiritual berupa Jimat Kontrak (*Contract Scroll*) atau Segel Darah (*Blood Seal*) untuk mengikat jiwa Spirit Beast. Harga media disesuaikan dengan hirarki mata uang Tael resmi ([`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1)):

| Tier Jimat / Segel | Nama Item Media | Bahan Baku Utama | Maks. Tier Beast | Bonus Peluang Sukses | Harga Pasar Standar |
|---|---|---|---|:---:|---|
| **Tier 1** | **Jimat Ikatan Kulit Lembu** | Kulit Beast T1 + Tinta Spirit Rendah | Tier 1 (Awal) | **+0%** | 50 Tael Perak |
| **Tier 2** | **Jimat Kontrak Darah Giok** | Kertas Xuan Spirit + Darah Beast T2 | Tier 2 | **+10%** | 3 Tael Giok Putih |
| **Tier 3** | **Segel Kontrak Jiwa Perak** | Serbuk Esens Perak + Tinta Jiwa T3 | Tier 3 | **+15%** | 15 Tael Giok Putih |
| **Tier 4** | **Jimat Rantai Jiwa Emas** | Benang Sutra Emas + Darah Inti Emas | Tier 4 | **+20%** | 1 Batu Spiritual Rendah |
| **Tier 5** | **Scroll Segel Jiwa Nascent** | Kulit Beast T5 + Tinta Kristal Jiwa | Tier 5 | **+25%** | 5 Batu Spiritual Rendah |
| **Tier 6 – 9** | **Segel Suci Abadi Huangji** | Sutra Urat Naga + Tinta Darah Sovereign | Tier 6 – Tier 9 | **+35% (Imun Backfire)** | 50 Batu Spiritual Rendah / Lelang |

---

## 🎲 2. Formula Success Rate & Soul Backfire

Saat pemain mengaktifkan jimat penjinak pada Spirit Beast di medan tempur, AI GM melakukan roll **1d100** berdasarkan formula berikut:

$$\text{PeluangBerhasil}(\%) = \text{BaseRate} + \text{BonusJimat} + \left[(\text{RanahPemain} - \text{TierBeast}) \times 15\%\right] + \text{BonusPakan} - \left(\frac{\text{SisaHPBeast}}{\text{HPMaxBeast}} \times 40\%\right)$$

### 📊 Batasan BaseRate
* **Ranah Pemain $\ge$ Tier Beast**: $\text{BaseRate} = \mathbf{50\%}$.
* **Ranah Pemain < Tier Beast**: $\text{BaseRate} = \mathbf{15\%}$.

---

### ⚡ Resiko Soul Backfire (Gagal Penjinakan)
Jika hasil roll **1d100** gagal dan **Ranah Pemain < Tier Beast**:
- Pemain menderita **Soul Backfire**: Pengurangan **30% HP Max** (True Damage / Mengabaikan Armor).
- Debuff **Stun** selama 1 Turn.
- Spirit Beast menjadi **Enraged** (Damage Spirit Beast +50% selama 2 Turn berikutnya).

---

## 🍖 3. Makanan, Pelet, & Suplemen Spirit Beast

Merawat Spirit Beast membutuhkan pakan khusus untuk meningkatkan poin Kesetiaan (*Loyalty*) dan mempercepat pertumbuhan/evolusi:

| Nama Pakan / Suplemen | Komposisi & Bahan Baku Utama | Efek Poin Loyalty | Efek Khusus & Buff Companion | Harga Pasar Standar |
|---|---|:---:|---|---|
| **Daging Beast Fana** | Daging Hewan Liar Biasa | **+2 Loyalty** | Mencegah Kelaparan (+30% Satiety Beast) | 20 Tael Tembaga / Kg |
| **Daging Inti Spirit (Fresh Meat)**| Daging Beast Tier 1–2 | **+5 Loyalty** | Pemulihan HP Beast +20% per Hari | 50 Tael Perak / Kg |
| **Pelet Nutrisi Qi Kayu** | Herba Tier 1 + Serbuk Batu Spirit | **+10 Loyalty** | Pemulihan Qi Beast +50% | 2 Tael Giok Putih |
| **Buah Spirit Emas Matang** | Buah Spirit Emas Kebun Tier 2 | **+15 Loyalty** | EXP Evolusi +50 Poin | 5 Tael Giok Putih |
| **Pil Purifikasi Darah Beast** | Darah Beast Unggul + Herba Tier 3 | **+25 Loyalty** | Memicu Roll Evolusi Fisik Spirit Beast | 20 Tael Giok Putih |
| **Nektar Teratai Abadi** | Esens Teratai Sembilan Warna Tier 6 | **Loyalty MAX (100)**| Membuka Bentuk Wujud Manusia (*Humanoid Form*)| 10 Batu Spiritual Rendah |

---

## ❤️ 4. Tingkatan Kesetiaan (Loyalty Meter 0 – 100)

Status Kesetiaan Spirit Beast memengaruhi perilaku dan efektivitasnya dalam pertarungan maupun eksplorasi:

| Rentang Loyalty | Status Hubungan | Efek Perilaku dalam Pertarungan | Dampak Eksplorasi & Perintah |
|:---:|---|---|---|
| **90 – 100** | **Jiwa Menyatu (*Very Loyal*)** | Damage Companion **+20%**, Kecepatan **+20%**. Menyerap serangan mematikan ke pemain. | Mematuhi semua perintah tanpa ragu. Bisa dikirim berburu mandiri. |
| **70 – 89** | **Patuh & Percaya (*Lobedient*)** | Performa Standar (100% Stat). | Mematuhi semua perintah standar. |
| **40 – 69** | **Ragu-Ragu (*Hesitant*)** | Peluang **25%** menolak perintah pertempuran dan diam di tempat. | Hanya mau bertarung jika diberi pakan pemicu (*Treat*). |
| **20 – 39** | **Benci & Liar (*Hostile*)** | Peluang **50%** menolak perintah dan kabur dari pertempuran. | Tidak bisa diajak eksplorasi. Satiety berkurang 2x lebih cepat. |
| **0 – 19** | **Pemberontakan (*Rebellion*)** | **Menyerang Pemain!** Kontrak segel terancam putus permanen. | Memerlukan Re-Seal Check (Injeksi Qi Paksa). |

---

## 🛡️ 5. Peran & Formasi Pertempuran Spirit Beast

Pemain dapat memerintahkan Spirit Beast yang aktif ke dalam salah satu dari 3 Formasi Tempur ([`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1)):

1. **Formasi Vanguard (Garis Depan)**:
   - Spirit Beast berdiri di depan pemain.
   - **Efek**: Menyerap 60% serangan fisik musuh. Threat/Aggro musuh tertuju pada Companion.
2. **Formasi Support (Garis Belakang)**:
   - Spirit Beast berdiri di samping/belakang pemain.
   - **Efek**: Menggunakan skill elemental/buff/debuff untuk membantu pemain dari jarak jauh.
3. **Formasi Fusion (Penyatuan Qi / Khusus Kultivator Tinggi)**:
   - Menyatu sementara dengan tubuh pemain (Memerlukan Loyalty $\ge 90$ dan Ranah Fondasi Jiwa).
   - **Efek**: Pemain mendapatkan +30% Stat Fisik Spirit Beast dan wujud visual aura elemen beast.

---

## 🦅 6. Mekanik Evolusi Spirit Beast

Spirit Beast dapat berevolusi menjadi wujud yang lebih kuat setelah memenuhi syarat berikut:
1. **Level / EXP Maksimal**: Berhasil memenangkan 20 pertempuran bersama pemain.
2. **Pakan Purifikasi**: Mengonsumsi *Pil Purifikasi Darah Beast* atau *Batu Inti Elemen* yang sesuai.
3. **Ritual Evolusi**: Bermeditasi di lokasi dengan ketebalan Qi Elemen yang cocok (misal: Es Bintang untuk Beast Elemen Es).

---

## 📄 7. Format Companion Sheet pada Profil Karakter

Setiap Spirit Beast yang berhasil dijinakkan dicatat dalam format resmi berikut:

```text
[Spirit Beast Companion Sheet]
- Nama Companion: Serigala Akar Hijau
- Spesies Origin: Spirit Beast Tier 2 (Dataran Hijau Abadi)
- HP Companion: 120 / 120 | Qi Companion: 60 / 60
- Loyalty Level: 85 / 100 (Status: Patuh & Percaya)
- Formasi Tempur Aktif: Vanguard (Garis Depan)
- Kemampuan Aktif: Gigitan Duri Kayu (Slow -10%)
```

---

## 🛡️ 8. Checklist Validasi AI GM untuk Penjinakan

- [ ] Apakah HP target Spirit Beast sudah di bawah 30% dari HP Max sebelum penjinakan dilakukan?
- [ ] Apakah pemain memiliki Jimat/Segel Penjinak di inventory-nya?
- [ ] Apakah formula kalkulasi *Success Rate* dihitung dengan rinci beserta roll 1d100?
- [ ] Apakah resiko *Soul Backfire* diterapkan jika penjinakan gagal pada target bertier lebih tinggi?
- [ ] Apakah data companion yang baru dijinakkan telah dimasukkan ke dalam sheet karakter pemain?
