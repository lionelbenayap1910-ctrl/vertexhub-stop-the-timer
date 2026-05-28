# ⚡ VertexHub - Auto Click

**Auto clicker presisi untuk game Stop Timer di Roblox.**  
Dilengkapi UI premium, kontrol offset manual (input teks), dan tombol toggle untuk menyembunyikan/menampilkan jendela.

![Version](https://img.shields.io/badge/version-2.2-brightgreen)
![Roblox](https://img.shields.io/badge/Roblox-Script-red)
![Language](https://img.shields.io/badge/Lua-5.1-blue)

---

## 🎯 Fitur Utama

- ✅ **Klik otomatis** pada tombol stop dengan timing akurat (menggunakan `RunService.PreRender`)
- 🎚️ **Offset manual** (input teks + tombol +/-) → nilai dari -100 ms hingga +100 ms, step 5 ms
- 🎨 **UI premium** – gelap, sudut membulat, efek glow, animasi halus
- 🔘 **Tombol toggle** di kanan atas untuk menyembunyikan/menampilkan UI (ikon ◀/▶)
- 🖱️ **Draggable window** – geser jendela utama dengan menahan title bar
- 📊 **Status real-time** – mendeteksi apakah game sedang berjalan
- 🧹 **Cleanup otomatis** – semua koneksi dihapus saat GUI ditutup

---

## 📦 Cara Instalasi

1. **Salin seluruh kode script** dari file `VertexHub-AutoClick.lua` (atau dari source di atas).
2. **Jalankan di executor Roblox** (Synapse X, Krnl, ScriptWare, Hydrogen, dll) saat berada di dalam game **Stop Timer**.
3. **Tunggu UI muncul** – sebuah jendela kecil dengan judul "VertexHub AutoClick" akan tampil.

> ⚠️ **Catatan**: Pastikan executor Anda mendukung fungsi berikut:  
> `cloneref`, `getconnections`, `gethui`, `getrenv`, `newcclosure`, dll. (kebanyakan executor modern sudah mendukung).

---

## 🕹️ Cara Penggunaan

| Kontrol | Fungsi |
|--------|--------|
| **Toggle "Auto Clicker"** | Aktif/nonaktifkan auto click |
| **Input Offset (ms)** | Ketik angka lalu tekan Enter, atau gunakan tombol +/-. Nilai negatif = lebih cepat, positif = lebih lambat. |
| **Tombol ◀ / ▶** (kanan atas layar) | Sembunyikan / tampilkan jendela utama |
| **Tombol ✕** (di title bar) | Tutup script sepenuhnya |
| **Drag title bar** | Pindahkan jendela |

### Contoh pengaturan offset:
- **-20 ms** → klik terjadi 0.02 detik *sebelum* waktu ideal
- **+30 ms** → klik terjadi 0.03 detik *setelah* waktu ideal

> 🧠 Gunakan offset untuk menyesuaikan dengan latency executor atau koneksi internet.

---

## 🖼️ Tampilan UI

┌─────────────────────────────────┐
│ ⚡ VertexHub AutoClick        ✕ │
├─────────────────────────────────┤
│ ⚙️ Kontrol                       │
│   Auto Clicker        [ ●──── ]  │
│   Offset Timing (ms)   [  0  ]  │
│                         [ - ] [+ ]│
│ 📊 Status                        │
│   ✅ Game terdeteksi | Siap       │
│ ℹ️ Info                          │
│   VertexHub - Auto Click         │
│   Khusus game Stop Timer         │
│   Versi 2.2 | Input manual       │
└─────────────────────────────────┘


---

## 🛠️ Teknis & Kompatibilitas

- **Bahasa**: Lua 5.1 (Luau)
- **Fungsi yang digunakan**:  
  `RunService.PreRender`, `TweenService`, `UserInputService`, `getconnections`, `gethui`
- **Game target**: Stop Timer (mode stopwatch)
- **Executor yang terbukti bekerja**:  
  - Synapse X  
  - Krnl  
  - ScriptWare  
  - Hydrogen  
  - Fluxus (dengan dukungan `getconnections`)

> Jika auto click tidak berfungsi, pastikan game *Stop Timer* sudah dimulai (bukan di lobby). Status di UI akan berubah menjadi hijau saat game terdeteksi.

---

## 📄 Lisensi

**MIT License** – bebas digunakan, dimodifikasi, dan didistribusikan.  
Hanya untuk keperluan edukasi. Gunakan dengan bijak dan patuhi aturan Roblox.

---

## 👥 Kontribusi

Pull request atau issue dipersilakan jika Anda menemukan bug atau ingin menambahkan fitur (misalnya dukungan multi-game, preset offset, dll).

---

## 🙏 Kredit

- **VertexHub Team** – desain UI dan logika auto clicker
- Library UI murni buatan sendiri (tanpa dependensi eksternal)

---

**Selamat mencoba dan raih high score!** 🚀
