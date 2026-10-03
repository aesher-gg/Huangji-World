# 🛸 Huangji-World — Sistem Kapal Terbang Spirit & Pertempuran Udara (Spirit Vessels & Airships System)

> **Modul:** 48 — Spirit Vessels, Airships & Aerial Combat System
> **Prinsip:** Anti-Cheat Enforced — Fuel-Consumption Bound — Durability-Tracked — Fall-Damage Enforced
> **Rujukan Utama:** [`INDEX.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/INDEX.md?v=1)
> **Rujukan Silang:**
> - [`00_CORE_RULES_AI_GM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/00_CORE_RULES_AI_GM.md?v=1) (Aturan Wajib AI GM)
> - [`01`–`10`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/01_WORLD_OVERVIEW_AND_CAPITAL.md?v=1) (Jarak Antar-Wilayah Li & Pos Jalur Udara)
> - [`13_ECONOMY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/13_ECONOMY_SYSTEM.md?v=1) (Mata Uang Tael & Harga Sewa Tiket)
> - [`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1) (Damage Meriam Qi & Defense Kapal)
> - [`16_BESTIARY.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/16_BESTIARY.md?v=1) (Ancaman Beast Terbang Udara T4+)
> - [`18_TAMING_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/18_TAMING_SYSTEM.md?v=1) (Companion Terbang & Mount)
> - [`19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1) (Formasi Segel Angin & Perbaikan)

---

## 📜 0. Filosofi & Aturan Emas Transportasi Udara

Di Benua Huangji yang membentang seluas puluhan ribu Li, perjalanan antar-wilayah menembus pegunungan terjal dan rawa beracun mengandalkan armada **Kapal Terbang Spirit (*Spirit Vessels / Airships / Floating Ark*)**. Kapal-kapal ini merupakan mahakarya gabungan ilmu tempa logam dan formasi susunan *Array Matrix Segel Angin* yang ditopang oleh bahan bakar Batu Spiritual.

**AI GM WAJIB mencatat konsumsi bahan bakar Batu Spiritual per Li perjalanan dan mengawasi Durability Kapal saat pertempuran udara.**

### 🛡️ Aturan Emas Anti-Cheat Spirit Vessels
1. **Aturan Konsumsi Bahan Bakar Vokal**: Setiap perjalanan udara mengonsumsi Batu Spiritual sesuai jarak Li. Tanpa bahan bakar yang cukup di penyimpanan kapal, kapal terhenti di udara dan perlahan jatuh bebas (*Freefall Descent*).
2. **Kapasitas Penumpang & Muatan Kaku**: Kapal terbang memiliki batas tonase muatan kaku. Kelebihan muatan (*Overload*) mereduksi kecepatan kapal sebesar **-50%** dan menggandakan konsumsi bahan bakar.
3. **Pencatatan Durability & Perbaikan**: Kerusakan kapal akibat serangan meriam Qi atau penyergapan beast terbang tercatat permanen sampai diperbaiki dengan mineral tempa M-3/M-4 oleh ahli penempa ([`19_ALCHEMY_FORGING_ARRAY_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1)).
4. **Hukuman Karam di Udara (*Shipwreck Fall Damage*)**: Jika Durability Kapal mencapai **0 HP**, kapal pecah di udara. Penumpang tanpa *Flying Mount* (`18`) atau *Jurus Terbang (Realm 4+)* menderita Fall Damage mematikan.

---

## 🛸 1. Matriks 5 Kelas Kapal Terbang Spirit (Spirit Vessel Tiers)

Kapal Terbang Spirit di Benua Huangji dikategorikan ke dalam 5 kelas berdasarkan ukuran raga, kecepatan jelajah, dan kapasitas tempur:

| Kode Kelas | Jenis Kapal Terbang | Kapasitas Penumpang & Muatan | Kecepatan Jelajah (Li / Jam) | Durability Kapal (HP) | Konsumsi Bahan Bakar per 500 Li | Biaya Sewa Tiket / Beli |
|:---:|---|---|:---:|:---:|---|---|
| **SV-1** | **Perahu Jelajah Angin (*Gale Skiff*)** | 5 Orang / 500 Kg Cargo | 100 Li / Jam | 800 HP | 2 Batu Spiritual Rendah | Sewa: 2 Tael Giok Putih / 100 Li <br>Beli: 20 Batu Spiritual Rendah |
| **SV-2** | **Kapal Dagang Awan Emas (*Cloud Merchant*)**| 30 Orang / 10 Ton Cargo | 80 Li / Jam | 3.500 HP | 10 Batu Spiritual Rendah | Sewa: 5 Tael Giok Putih / 100 Li <br>Beli: 80 Batu Spiritual Rendah |
| **SV-3** | **Kapal Perang Badai (*Gale Warship*)** | 100 Prajurit / 4 Meriam Qi | 120 Li / Jam | 12.000 HP | 2 Batu Spiritual Menengah | Khusus Militer / Faksi Sekte <br>Beli: 15 Batu Spiritual Menengah |
| **SV-4** | **Benteng Melayang Sekte (*Floating Fortress*)**| 300 Murid / 8 Meriam Qi | 60 Li / Jam | 35.000 HP | 5 Batu Spiritual Menengah | Armada Resmi Sekte Elite <br>Beli: 50 Batu Spiritual Menengah |
| **SV-5** | **Bahtera Perang Kekaisaran (*Imperial Ark*)**| 1.000 Prajurit / 16 Meriam Qi | 150 Li / Jam | 100.000 HP | 20 Batu Spiritual Menengah | Armada Utama Tahta Agung Huangji <br>Tak Terhitung (Kekaisaran) |

---

## ⛽ 2. Formula Konsumsi Bahan Bakar & Perhitungan Jarak

Waktu jelajah dan biaya operasional penerbangan dihitung menggunakan formula:

$$\text{KonsumsiBatuSpirit} = \left(\frac{\text{TotalJarakLi}}{500 \text{ Li}}\right) \times \text{BaseFuelRate}(\text{VesselClass}) \times \text{PayloadModifier}$$

- **Payload Modifier**:
  - *Muatan Normal ($\le 100\%$)*: $\times 1,0$
  - *Overload ($101\% - 150\%$)*: $\times 2,0$ (Kecepatan Jelajah terpotong **-50%**)

---

## ⚔️ 3. Mekanik Pertempuran Udara (Aerial Combat Rules)

Saat melintasi zona udara liar (seperti Puncak Langit Surgawi atau Gurun Pasir), pertempuran udara dapat terpicu oleh *Perompak Udara* atau *Kawanan Beast Terbang Tier 4+* ([`16_BESTIARY.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/16_BESTIARY.md?v=1)):

### 💣 3.1 Penembakan Meriam Qi (*Qi Cannon Fire*)
- **Konsumsi Amunisi**: 1 Batu Spiritual Rendah per Tembakan.
- **Hit Chance Meriam**: $75\%$ (Bisa ditargetkan ke Hull Kapal Musuh atau Meriam Musuh).
- **Damage Meriam Qi**:
  - *Meriam Qi Ringan (SV-3)*: **500 Elemental Damage / Tembakan**.
  - *Meriam Qi Berat (SV-4 & SV-5)*: **1.500 Elemental Damage / Tembakan** (Efek AoE Radius 10 Meter).

---

### 🗡️ 3.2 Serbuan Invasi Geladak (*Boarding Action*)
- Pemain atau perompak dapat melompati jarak antar-kapal menggunakan *Flying Mount* (`18`) atau *Jurus Angin* untuk memulai **Pertarungan Geladak (*Deck Combat*)**.
- Pertarungan di geladak menggunakan aturan pertempuran taktis biasa ([`15_COMBAT_SYSTEM.md`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/15_COMBAT_SYSTEM.md?v=1)).

---

### 🔧 3.3 Perbaikan Darurat Udara (*In-Flight Repair*)
- Anggota kelompok dengan keahlian Penempaan (*Forging*) atau Formasi (*Array*) dapat memperbaiki Durability Kapal di tengah pertempuran:
  - **Aksi Turn**: Memerlukan 1 Aksi Utama + 2 Unit Mineral M-3/M-4 ([`19`](https://raw.githubusercontent.com/aesher-gg/Huangji-World/main/19_ALCHEMY_FORGING_ARRAY_SYSTEM.md?v=1)).
  - **Pemulihan Durability**: Memulihkan **+10% Durability Max Kapal**.

---

## 🪂 4. Tabel Dampak Hancurnya Kapal & Fall Damage

Jika Durability Kapal mencapai **0 HP**, kapal hancur dan runtuh di udara. Seluruh penumpang wajib melakukan **Fall Damage Check**:

| Ranah Pemain (Indonesian / English) | Fasilitas Keselamatan Udara | Dampak Fisik Jatuh Bebas (*Fall Damage Penalty*) |
|:---:|---|---|
| **Ranah 0–3 (Mortal s/d Found Est)** | Tanpa Flying Mount / Parasut Qi | **Jatuh Bebas Mematikan (500 True Damage)** $\rightarrow$ **Kematian Instan**. |
| **Ranah 0–3 (Mortal s/d Found Est)** | Memiliki Flying Mount / Parasut Spirit | Menderita **100 Physical Damage** + Luka Memar Ringan. |
| **Ranah 4+ (Golden Core s/d Sovereign)**| Mampu Terbang Mandiri (*Void Flight*) | Mereduksi $100\%$ Fall Damage (Terbang melayang ke tanah dengan aman). |

---

## 🗺️ 5. Rute Pelayaran Udara & Pos Dermaga Langit 10 Wilayah

Setiap wilayah utama Benua Huangji memiliki Dermaga Langit (*Sky Port*) tempat bertambatnya armada kapal terbang:

| Wilayah Geografis | Nama Dermaga Langit Utama | Rute Udara Utama & Tujuan Populer |
|:---|---|---|
| **01. Ibu Kota Huangji** | **Dermaga Langit Tahta Emas** | Rute Utama ke seluruh 9 Wilayah Benua. |
| **02. Dataran Hijau Abadi** | **Pos Udara Kayu Vitalitas** | Rute Ekspor Herba ke Ibu Kota & Lembah Api. |
| **03. Pegunungan Petir Guntur**| **Pelabuhan Udara Puncak Guntur**| Rute Tambang Bijih Logam ke Sekte Tempa. |
| **04. Lembah Api Merah** | **Dermaga Kawah Vulkanik** | Rute Ekspor Alkimia ke Danau Es & Gurun. |
| **05. Danau Es Bintang** | **Pos Udara Bintang Pembeku** | Rute Khusus Kapal Berlapis Zirah Tahan Dingin. |
| **06. Tanah Gersang Tulang** | **Dermaga Gelap Rangka Purba** | Rute Pasar Gelap ke Rawa Racun. |
| **07. Gurun Pasir Emas** | **Dermaga Oase Angin Emas** | Rute Kapal Dagang Jalur Pasir ke Ibu Kota. |
| **08. Rawa Kabut Racun** | **Pos Udara Teratai Miasma** | Rute Khusus Kapal Ber-Array Penawar Miasma. |
| **09. Puncak Langit Surgawi** | **Pelabuhan Udara Puncak Awan** | Pusat Perbaikan & Perakitan Kapal Terbang. |
| **10. Kepulauan Palung Samudra**| **Dermaga Armada Garda Laut** | Rute Gabungan Kapal Laut & Kapal Terbang. |

---

## 📄 6. Format Spirit Vessel Sheet pada Profil Karakter

Setiap Kepemilikan atau Penyewaan Kapal Terbang dicatat dalam format resmi berikut pada Profil Karakter:

```text
[Spirit Vessel Sheet — Active Ship]
- Nama Kapal: Kapal Perang Badai "Gelombang Awan"
- Kelas Kapal: SV-3 (Kapal Perang Badai — Tier 3)
- Durability Kapal: 12.000 / 12.000 HP
- Persediaan Bahan Bakar: 15 Batu Spiritual Rendah (Jangkauan: 3.750 Li)
- Persenjataan: 4 Meriam Qi Ringan (Amunisi: 20 Batu Spirit Rendah)
- Status Penerbangan: Mengudara (Rute: Ibu Kota -> Puncak Langit Surgawi)
- Timestamp Keberangkatan: Tahun 2, Bulan 2, Hari 1
```

---

## 🛡️ 7. Checklist Validasi & Anti-Cheat AI GM

Sebelum mengesahkan perjalanan udara atau pertempuran kapal terbang, AI GM **wajib** memeriksa checklist berikut:

- [ ] Apakah konsumsi bahan bakar Batu Spiritual dipotong secara sah sesuai jarak Li perjalanan?
- [ ] Jika muatan melebihi kapasitas (*Overload*), apakah penalti kecepatan (-50%) dan boros bahan bakar (2x) diterapkan?
- [ ] Apakah Durability Kapal dan amunisi Meriam Qi dicatat transparan pada setiap Turn pertempuran udara?
- [ ] Jika kapal hancur di udara (Durability 0), apakah *Fall Damage Check* dieksekusi secara tepat sesuai Ranah penumpang?
- [ ] Apakah seluruh biaya tiket sewa atau pembelian kapal dicatat di sheet keuangan pemain dengan mata uang Tael / Batu Spiritual yang sah?
