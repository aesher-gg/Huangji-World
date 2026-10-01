# 18. Taming System — Huangji-World

> **Status File**: Modul Penjinakan & Pemeliharaan Spirit Beast
> **Versi**: 3.0 (Huangji Core Edition)

---

## 🐾 1. Pengenalan Sistem Taming

Sistem Penjinakan memungkinkan kultivator untuk menundukkan, melatih, dan menjadikan Spirit Beast liar sebagai mitra bertarung (*beast companion*) atau hewan tunggangan (*mount*).

---

## 🔗 2. Tahapan Penjinakan (Taming Steps)

1. **Pelemahan Target**: HP Spirit Beast harus dikurangi hingga di bawah **30%** dalam pertarungan.
2. **Penggunaan Jimat Segel / Kontrak Jiwa**: Pemain melancarkan teknik *Soul Binding Contract* atau menggunakan *Jimat Penjinak Beast*.
3. **Pemeriksaan Kekuatan Jiwa (Willpower Check)**:
   - Jika Ranah Pemain $\ge$ Ranah Beast: Peluang berhasil **75%**.
   - Jika Ranah Pemain < Ranah Beast: Peluang berhasil **25%** (Risiko *Soul Backfire*).
4. **Pemberian Nama & Registrasi Companion**: Spirit Beast masuk ke dalam daftar `spirit_beast` pada Profil Karakter.

---

## 🍖 3. Pemeliharaan & Kenaikan Tingkat Companion

* **Tingkat Kesetiaan (Loyalty 0 - 100)**: Dijaga dengan memberi makan daging spiritual secara teratur. Jika Loyalty < 20, Beast dapat kabur atau menyerang pemilik.
* **Evolusi Beast**: Spirit Beast dapat berevolusi menjadi wujud purba jika diberi makan *Pill Mutiara Beast* atau *Buah Spirit Emas*.
