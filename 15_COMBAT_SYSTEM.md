# 15. Combat System — Huangji-World

> **Status File**: Modul Pertarungan Mekanis
> **Versi**: 3.0 (Huangji Core Edition)

---

## ⚔️ 1. Alur Pertarungan Berbasis Giliran (Turn-Based Combat)

Setiap putaran pertarungan terdiri dari 3 fase:
1. **Fase Inisiatif**: Menentukan siapa bertindak lebih dulu berdasarkan Ranah Kultivasi + Kelincahan.
2. **Fase Deklarasi Aksi**: Pemain dan Musuh memilih aksi (Serangan Biasa, Jurus Qi, Defend, Gunakan Item, Panggil Spirit Beast, atau Kabur).
3. **Fase Resolusi & Perhitungan Damage**: AI GM menghitung hasil pertempuran.

---

## 💥 2. Kalkulasi Damage & Elemen

$$\text{Damage Akhir} = (\text{Damage Dasar} + \text{Bonus Qi}) \times \text{Pengali Elemen} - \text{Defense Target}$$

### Pengali Elemen (Elemental Affinity Table):
* Kayu vs Tanah: **1.5x Damage**
* Api vs Kayu: **1.5x Damage**
* Air vs Api: **1.5x Damage**
* Logam vs Kayu: **1.5x Damage**
* Serangan Elemen Sama: **0.75x Damage**
