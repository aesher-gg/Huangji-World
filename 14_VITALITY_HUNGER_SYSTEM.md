# 14. Vitality & Hunger System — Huangji-World

> **Status File**: Modul Vitalitas, Luka & Kelaparan
> **Versi**: 3.0 (Huangji Core Edition)

---

## 🩸 1. Status Kesehatan & Luka (Injury Conditions)

* **Luka Ringan (HP 75%-99%)**: Tidak ada penalti aksi.
* **Luka Sedang (HP 50%-74%)**: Damage fisik & Qi berkurang 15%.
* **Luka Parah (HP 25%-49%)**: Kecepatan gerak berkurang 50%, pemakaian Qi membengkak 2x lipat.
* **Kritis (HP 1%-24%)**: Karakter pingsan atau tidak bisa melancarkan jurus berat.

---

## 🍚 2. Kelaparan & Nutrisi Spiritual

Kultivator di ranah rendah (Body Refining - Qi Gathering) masih membutuhkan makanan.
* **Persentase Kelaparan (0% - 100%)**:
  - `0% - 30%`: Kondisi Prima.
  - `31% - 70%`: Stamina berkurang 20%.
  - `71% - 99%`: Regenerasi HP & Qi mati.
  - `100%`: Kelaparan parah, HP berkurang 5% setiap turn.
* **Buah / Daging Spirit Beast**: Memakan daging monster Spirit Beast memberikan pemulihan Kelaparan sekaligus bonus tambahan Qi sementara.
