# ❤️ Huangji-World — Sistem Vitalitas (HP) & Kelangsungan Hidup (Hunger System)

> **Modul:** 14 — Vitality & Hunger System
> **Prinsip:** Anti-Cheat Enforced — Law-Specific Scaling — Terintegrasi dengan Sistem Hukum Kultivasi & Ekonomi
> **Rujukan Silang:** `12_CULTIVATION_LAW_SYSTEM.md` (QiCap basis HP), `13_ECONOMY_SYSTEM.md` (Harga Obat), `15_COMBAT_SYSTEM.md` (FinalDamage)

---

## 0. Filosofi Sistem

Sama seperti Qi tunduk pada `QiCap` dan harga tunduk pada `FinalPrice`, HP (Vitalitas) dan rasa lapar juga tunduk pada formula tetap. Tiap Hukum kultivasi resmi Huangji-World memiliki karakter HP berbeda sesuai filosofinya, dan tiap Realm punya ketahanan lapar berbeda.

### Aturan Emas Anti-Cheat Vitalitas & Kelaparan
- HP TIDAK BOLEH dideklarasikan sepihak oleh player — dihitung AI GM lewat formula `HP(realm, stage, law)`.
- Kerusakan HP (damage) dicatat di log bertimestamp, tidak bisa diedit mundur atau "dilupakan" player.
- Regenerasi HP di luar batas alami hanya lewat pil/jasa tabib yang tunduk Sistem Ekonomi (`13_ECONOMY_SYSTEM.md`).
- Status kelaparan dihitung otomatis per jam in-game oleh AI GM, bukan klaim sepihak player.
- Breakthrough Realm langsung memperbarui HP Cap dan Fasting Multiplier karakter secara otomatis.

---

## 1. Formula HP Universal

```
HPBase(realm, stage) = QiCap(realm, stage) × K_HP
K_HP = 0,4 (Konstanta Vitalitas Universal)

HP(realm, stage, law) = HPBase(realm, stage) × LawHPMultiplier(law)
```

### Law HP Multiplier Resmi Huangji-World

| Hukum Kultivasi Resmi | LawHPMultiplier | Alasan Filosofis & Karakteristik |
|---|---|---|
| **Hukum Akar Kayu Suci** | ×1,4 | Energi vitalitas kayu melimpah — sangat tahan banting & cepat pulih |
| **Hukum Benteng Pasir Emas** | ×1,5 | Penempaan dinding cadas — pertahanan fisik terkuat |
| **Hukum Inti Petir Ungu** | ×1,0 | Baseline serangan kilat — seimbang |
| **Hukum Tungku Api Merah** | ×0,9 | Agresif ofensif, sedikit lebih rapuh |
| **Hukum Istana Es Abadi** | ×1,1 | Perisai kristal es — padat defensif |
| **Hukum Tahta Emas Huangji** | ×1,2 | Kepemimpinan elit istana — fisik tangguh berwibawa |
| **Hukum Bayangan Jiwa Kelabu** | ×0,75 | Berbasis jiwa/tulang — rapuh secara raga |
| **Hukum Racun Teratai Hitam** | ×0,7 | Racun miasma — trade-off pertahanan demi racun mematikan |
| **Hukum Pedang Awan** | ×0,85 | Kecepatan angin — fleksibel & lincah |
| **Hukum Mutiara Samudra** | ×1,15 | Energi cairan samudra — regeneratif |
| **Hukum Pisau Sunyi** | ×0,8 | Presisi eksekutor — tangguh namun bukan tanky |

---

## 2. Status Kondisi HP & Ambang Bahaya

| % HP Tersisa | Status | Efek |
|---|---|---|
| 100%–50% | Sehat (Healthy) | Tidak ada penalti |
| 49%–20% | Terluka (Wounded) | −10% output Qi, −5% efektivitas serangan |
| 19%–1% | Kritis (Critical) | −30% output Qi, −20% efektivitas serangan, risiko Qi Deviation |
| 0% | Pingsan / Qi Deviation | Tak sadarkan diri, WAJIB pertolongan tabib |
| Di bawah −50% | Kematian | Overkill ekstrem tervalidasi GM |

---

## 3. Sistem Kelaparan (Hunger System)

```
SatietyMax = 100 poin (universal)
JamSampaiKosong(realm) = 6 jam × FastingMultiplier(realm)
```

### Fasting Multiplier per Realm
| Realm | FastingMultiplier | Waktu Sampai Sangat Lapar |
|---|---|---|
| 0 — Fana | ×1,0 | 6 jam |
| 1 — Pembersihan Tubuh | ×1,0 | 6 jam |
| 2 — Pengumpulan Qi | ×2,0 | 12 jam |
| 3 — Pembentukan Fondasi | ×5,0 | 30 jam (~1,25 hari) |
| 4 — Pembentukan Inti Emas | ×15,0 | 90 jam (~3,75 hari) |
| 5 — Melahirkan Jiwa Nascent | ×50,0 | 300 jam (~12,5 hari) |
| 6 — Transformasi Kehampaan | ×150,0 | 900 jam (~37,5 hari) |
| 7 — Penyatuan Roh Suci | ×500,0 | 3.000 jam (~4 bulan) |
| 8 — Penerobosan Tribulasi | ×2.000,0 | 12.000 jam (~1,4 tahun) |
| 9 — Kaisar Agung Abadi | Tak terbatas | Bi Gu Sempurna (Tidak butuh makan) |

---

## 4. Checklist Anti-Cheat

- [ ] HP dihitung dari formula `HP(realm, stage, law)`, bukan klaim sepihak player?
- [ ] Damage yang diterima tercatat di log bertimestamp, tidak diedit mundur?
- [ ] Status kondisi diperbarui otomatis tiap kali HP berubah?
- [ ] FastingMultiplier sesuai realm karakter saat ini?
