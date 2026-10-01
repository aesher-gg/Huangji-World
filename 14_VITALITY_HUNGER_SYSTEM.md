# ❤️ Huangji-World — Sistem Vitalitas (HP) & Kelangsungan Hidup (Hunger System)

> **Modul:** 14 — Vitality & Hunger System
> **Prinsip:** Anti-Cheat Enforced — Law-Specific Scaling — Terintegrasi dengan Sistem Hukum Kultivasi & Ekonomi
> **Rujukan Silang:** `12_CULTIVATION_LAW_SYSTEM.md` (QiCap basis HP), `13_ECONOMY_SYSTEM.md` (Harga Obat), `15_COMBAT_SYSTEM.md` (FinalDamage)

---

## 0. Filosofi Sistem

Sama seperti Qi tunduk pada `QiCap` dan harga tunduk pada `FinalPrice`, HP (Vitalitas) dan rasa lapar juga tunduk pada formula tetap. Tiap Hukum kultivasi punya karakter HP berbeda sesuai filosofinya, dan tiap Realm punya ketahanan lapar berbeda.

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

### Law HP Multiplier
| Hukum | LawHPMultiplier | Alasan Filosofis |
|---|---|---|
| Hukum Raga Sejati (Body Tempering) | ×1,5 | Penempaan tubuh — paling tahan banting |
| Hukum Dao Abadi (Standar) | ×1,0 | Baseline — seimbang |
| Hukum Qi Api Vulkanik | ×0,9 | Agresif dan ofensif, sedikit lebih rapuh |
| Hukum Gu Karma | ×0,7 | Trade-off "kekuatan besar, harga mahal" |
| Hukum Bayangan Jiwa Kelabu | ×0,75 | Berbasis jiwa, rapuh secara raga |
| Hukum Pisau Sunyi (Custom) | ×0,8 | Presisi eksekutor — cukup tangguh |

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
| 1 — Pemurnian Fana | ×1,0 | 6 jam |
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
