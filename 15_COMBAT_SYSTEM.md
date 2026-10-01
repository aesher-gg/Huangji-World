# ⚔️ 15. Combat System — Huangji-World

> **Status File**: Modul Utama Pertarungan Mekanis
> **Versi**: 3.0 (Huangji Core Edition)
> **Rujukan Silang**: `00_CORE_RULES_AI_GM.md`, `12_CULTIVATION_LAW_SYSTEM.md`, `14_VITALITY_HUNGER_SYSTEM.md`

---

## ⚔️ 1. Fase Pertarungan Turn-Based (3 Turn Phases)

Setiap putaran pertarungan dihitung secara teliti dalam 3 fase:

1. **Fase Inisiatif (Initiative Check)**: Menentukan giliran bertindak berdasarkan `Kecepatan Gerak + Bonus Ranah + Dadu D10`.
2. **Fase Aksi (Action Phase)**: Karakter dapat memilih 1 Aksi Utama (Serangan Senjata, Jurus Qi, Gunakan Item, Panggil Companion Beast, atau Kabur) + 1 Aksi Pergerakan.
3. **Fase Resolusi & Damage Check**: AI GM menghitung hasil kerusakan, perisai Qi, dan status efek yang dipicu.

---

## 💥 2. Formula Damage & Pengali Elemen

$$\text{Damage Akhir} = \left[(\text{Base Damage Senjata} + \text{Bonus Qi Diinvestasikan}) \times \text{ElementalMultiplier}\right] - \text{Defense Target}$$

### Tabel Pengali Elemen (Elemental Affinity Chart)
| Elemen Penyerang | Elemen Bertahan | Pengali Damage | Status Efek Dipicu |
|---|---|---|---|
| **Kayu** | Tanah | **1.5x (Super Effective)** | Entangle (Root 1 Turn) |
| **Api** | Kayu | **1.5x (Super Effective)** | Burn Damage (10 HP / Turn) |
| **Air / Es** | Api | **1.5x (Super Effective)** | Freeze (-20% Movement Speed) |
| **Logam / Petir** | Kayu | **1.5x (Super Effective)** | Paralysis (Peluang Skip Turn 25%) |
| **Tanah** | Air | **1.5x (Super Effective)** | Stun (Gagal Aksi Pergerakan) |
| **Elemen Sama** | Elemen Sama | **0.75x (Resisted)** | No Status Effect |

---

## 🛡️ 3. Perisai Qi (Qi Barrier) & Mitigasi Damage

Kultivator dapat mengaktifkan **Perisai Qi** untuk menyerap damage sebelum mengurangi HP:
* **Konsumsi Qi**: 1 Poin Qi disalurkan menjadi **2 Poin Perisai Qi**.
* **Ketahanan Perisai**: Perisai Qi bertahan selama 2 turn atau sampai poin perisai habis diserang.

---

## ☣️ 4. Status Efek Pertarungan (Status Effects)

* **Burn (Luka Bakar)**: HP berkurang 10 poin per turn selama 3 turn.
* **Frozen (Membeku)**: Kecepatan gerak berkurang 50% & Defense berkurang 20%.
* **Paralysis (Lumpuh Kilat)**: Peluang gagal melakukan aksi sebesar 30% per turn.
* **Bleeding (Pendarahan)**: HP berkurang 15 poin setiap kali karakter melakukan serangan fisik.
* **Poison (Keracunan)**: HP & Stamina berkurang 8 poin per turn, regenerasi mati.

---

## 🏃‍♂️ 5. Aturan Melarikan Diri (Escape Rules)

Pemain dapat mencoba melarikan diri dari pertarungan:
* **Formula Escape Check**: `Kecepatan Gerak Pemain + D20` vs `Kecepatan Gerak Musuh + D20`.
* **Jika Berhasil**: Pertarungan berakhir, pemain berpindah ke lokasi terdekat dengan konsumsi Stamina 20 poin.
* **Jika Gagal**: Pemain kehilangan giliran aksi & menerima serangan bebas (Opportunity Attack) dari musuh.
