# 🐾 Huangji-World — Sistem Penjinakan Spirit Beast (Taming System)

> **Modul:** 18 — Taming System
> **Prinsip:** Anti-Cheat Enforced — Willpower & Loyalty Dependent — Terintegrasi dengan Bestiary & Combat
> **Rujukan Silang:** `16_BESTIARY.md`, `15_COMBAT_SYSTEM.md`, `12_CULTIVATION_LAW_SYSTEM.md`

---

## 0. Filosofi Sistem

Menjinakkan Spirit Beast membutuhkan pelemahan fisik target, media jimat segel, dan uji kekuatan kehendak (Willpower Check). Beast tidak bisa dijinakkan secara instan tanpa proses yang sah.

### Aturan Emas Anti-Cheat Taming
- HP Beast harus dikurangi hingga di bawah **30% dari HP Max** sebelum proses penjinakan dilakukan.
- Formula Willpower Check dihitung secara terbuka oleh AI GM.
- Kegagalan penjinakan pada beast yang ranahnya lebih tinggi memicu *Soul Backfire* (HP Pemain -30 Poin & Stun 1 Turn).

---

## 🔗 1. Tahapan Penjinakan & Formula Success Rate

$$\text{Peluang Berhasil} = \text{BaseSuccess} + \left[(\text{Ranah Pemain} - \text{Rank Beast}) \times 20\%\right] - \left(\frac{\text{HP Beast Sisa}}{\text{HP Max Beast}} \times 50\%\right)$$

* **Jika Ranah Pemain $\ge$ Rank Beast**: BaseSuccess = **60%**.
* **Jika Ranah Pemain < Rank Beast**: BaseSuccess = **20%** (Risiko *Soul Backfire* jika gagal).

---

## 🍖 2. Indikator Kesetiaan (Loyalty 0 - 100)

* **Loyalty 100 - 80 (Sangat Setia)**: Damage Companion +15%, siap mengorbankan HP untuk menahan serangan pemain.
* **Loyalty 79 - 50 (Patuh)**: Performa standar.
* **Loyalty 49 - 20 (Ragu-ragu)**: Peluang 20% menolak perintah aksi pertarungan.
* **Loyalty 19 - 0 (Memberontak)**: Companion kabur dari pertempuran atau menyerang pemain.

---

## 3. Checklist Validasi AI GM

- [ ] Pelemahan HP target ( <30%) terverifikasi sebelum penjinakan?
- [ ] Willpower Check dihitung dari formula resmi?
- [ ] Status Loyalty dicatat dan diperbarui pada profil karakter?
