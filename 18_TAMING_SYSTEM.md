# 🐾 18. Taming System — Huangji-World

> **Status File**: Modul Utama Penjinakan & Companion Spirit Beast
> **Versi**: 3.0 (Huangji Core Edition)
> **Rujukan Silang**: `16_BESTIARY.md`, `15_COMBAT_SYSTEM.md`, `12_CULTIVATION_LAW_SYSTEM.md`

---

## 🔗 1. Tahapan Penjinakan Spirit Beast (4 Steps)

Sistem Penjinakan memungkinkan kultivator untuk menundukkan, mengikat jiwa, dan melatih Spirit Beast liar dari *Bestiary* sebagai mitra pertempuran (*companion*) atau hewan tunggangan (*mount*).

### Step 1: Pelemahan Fisik Target
HP Spirit Beast liar harus dikurangi hingga di bawah **30% dari HP Maksimumnya** dalam pertempuran.

### Step 2: Penggunaan Media Penjinak
Pemain menggunakan salah satu dari media penjinak:
* **Jimat Segel Beast Rendah (Tier 1 - 2)**: Untuk Beast Rank 1 & 2.
* **Jimat Segel Beast Agung (Tier 3 - 4)**: Untuk Beast Rank 3 & 4.
* **Teknik Segel Kontrak Jiwa Direct (Soul Binding Technique)**: Mengonsumsi 50 Poin Qi.

### Step 3: Formula Pemeriksaan Kehendak (Willpower Check)
$$\text{Peluang Berhasil} = \text{BaseSuccess} + \left[(\text{Ranah Pemain} - \text{Rank Beast}) \times 20\%\right] - \left(\frac{\text{HP Beast Sisa}}{\text{HP Max Beast}} \times 50\%\right)$$

* **Jika Ranah Pemain $\ge$ Rank Beast**: BaseSuccess = **60%**.
* **Jika Ranah Pemain < Rank Beast**: BaseSuccess = **20%** (Risiko *Soul Backfire*: HP Pemain berkurang 30 Poin & Stun 1 Turn jika gagal).

### Step 4: Registrasi Companion
Jika penjinakan berhasil, Spirit Beast dicatat di dalam Profil Karakter pada kolom `spirit_beast`:
```json
{
  "nama_beast": "Serigala Akar Hijau",
  "rank": 1,
  "loyalty": 80,
  "hp_current": 120,
  "hp_max": 120,
  "status": "Aktif / Mount"
}
```

---

## 🍖 2. Indikator Kesetiaan (Loyalty 0 - 100)

* **Loyalty 100 - 80 (Sangat Setia)**: Damage Companion +15%, siap mengorbankan HP untuk menahan serangan pemain.
* **Loyalty 79 - 50 (Patuh)**: Performa standar.
* **Loyalty 49 - 20 (Ragu-ragu)**: Peluang 20% menolak perintah aksi pertarungan.
* **Loyalty 19 - 0 (Memberontak)**: Companion kabur dari pertempuran atau menyerang pemain.

### Pemeliharaan Loyalty
Berikan makanan *Daging Spirit Beast* atau *Buah Spirit Emas* secara rutin (+10 Loyalty per porsi).

---

## 🧬 3. Sistem Evolusi Spirit Beast

Companion dapat berevolusi menjadi wujud purba dengan memberi makan **Pill Mutiara Beast** + **Material Core**:
* *Serigala Akar Hijau* $\rightarrow$ **Serigala Raja Akar Purba (Rank 2)** (+100% HP & Damage).
* *Elang Kilat Ungu* $\rightarrow$ **Rajawali Badai Guntur Suci (Rank 3)**.
