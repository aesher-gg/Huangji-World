# 🩸 14. Vitality & Hunger System — Huangji-World

> **Status File**: Modul Utama Vitalitas, Luka & Kelaparan
> **Versi**: 3.0 (Huangji Core Edition)
> **Rujukan Silang**: `00_CORE_RULES_AI_GM.md`, `12_CULTIVATION_LAW_SYSTEM.md`, `15_COMBAT_SYSTEM.md`

---

## 🩸 1. Formula HP & Stamina Maksimum

Kapasitas Kesehatan (HP) dan Daya Tahan (Stamina) pemain dihitung secara otomatis berdasarkan Ranah Kultivasi dan pengali Physique:

$$\text{HP Maksimum} = \left(100 + (\text{Tingkat Ranah} \times 50) + \frac{\text{QiCap}}{10}\right) \times \text{PhysiqueMultiplier}$$
$$\text{Stamina Maksimum} = 100 + (\text{Tingkat Ranah} \times 25) + \frac{\text{QiCap}}{20}$$

---

## 🩺 2. 5 Tingkat Status Kesehatan & Luka (Injury Status)

Kondisi fisik karakter dikategorikan ke dalam 5 status luka berdasarkan persentase sisa HP:

| Persentase Sisa HP | Status Luka | Efek & Penalti Mekanis |
|---|---|---|
| **100% - 90%** | **Sempurna (Prima)** | Tidak ada penalti. Regenerasi Stamina normal. |
| **89% - 70%** | **Luka Ringan** | Damage Fisik & Jurus berkurang **5%**. |
| **69% - 40%** | **Luka Sedang** | Kecepatan Gerak berkurang **20%**, Konsumsi Qi membengkak **+25%**. |
| **39% - 15%** | **Luka Parah** | Kecepatan Gerak berkurang **50%**, Damage Fisik & Jurus berkurang **40%**, tidak bisa menggunakan jurus berat. |
| **14% - 1%** | **Kritis (Pingsan / Sekarat)** | Karakter pingsan atau tidak bisa bertindak. Butuh pertolongan darurat dalam 3 turn atau mengalami kematian fisik. |

---

## 🍚 3. Sistem Kelaparan & Satiety (0% - 100%)

Indikator Satiety menggambarkan kecukupan nutrisi dan energi tubuh:

* **Satiety 100% - 80% (Kenyang & Prima)**: Regenerasi HP +2% per jam meditasi, Regenerasi Qi normal.
* **Satiety 79% - 40% (Cukup)**: Kondisi standar tanpa penalti.
* **Satiety 39% - 15% (Lapar)**: Regenerasi HP & Qi terhenti. Kecepatan gerak -10%.
* **Satiety 14% - 1% (Kelaparan Parah)**: Malnutrisi Spirit. Stamina Max berkurang 50%.
* **Satiety 0% (Kelaparan Ekstrem)**: Organ dalam menyusut. HP berkurang **5% per turn** sampai karakter makan atau mati.

### 🥩 Tabel Pemulihan Satiety Makanan Spiritual
| Makanan / Minuman Spiritual | Pemulihan Satiety | Bonus Tambahan Qi |
|---|---|---|
| **Roti Daging Fana** | +20% Satiety | 0 Qi |
| **Daging Spirit Beast Rank 1** | +40% Satiety | +15 Qi |
| **Daging Spirit Beast Rank 2** | +60% Satiety | +50 Qi |
| **Buah Spirit Emas Matang** | +100% Satiety | +150 Qi & Pemulihan 30 HP |
