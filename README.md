# 🗡️ Shadow Assassin vs Goblins

**Shadow Assassin vs Goblins** adalah game 2D Action Platformer seru berbasis HTML5 Canvas yang telah dibungkus menjadi aplikasi **Android APK** native (Signed Release APK) dengan dukungan offline penuh, kontrol layar sentuh (touchscreen), dan efek audio sintetis tanpa ketergantungan internet.

---

## 📱 Download APK Android

Kamu bisa langsung mengunduh file APK versi terbaru (**v2.0.0 - Release APK**) melalui tautan berikut:

👉 **[Download ShadowAssassin.apk (v2.0.0)](https://github.com/Ryn-debugging/assasin-vs-goblin/releases/latest/download/ShadowAssassin.apk)**

atau lihat semua rilis di halaman **[GitHub Releases](https://github.com/Ryn-debugging/assasin-vs-goblin/releases/latest)**.

### 📲 Cara Install di HP Android (Penting!)
1. Unduh file **`ShadowAssassin.apk`** menggunakan browser (Chrome/Safari/dll).
2. Jika muncul *"Tidak dapat membuka file"* saat diketuk langsung dari notifikasi/browser dalam aplikasi (WhatsApp/Telegram/dll), buka aplikasi **Pengelola File / File Manager / Files** bawaan HP kamu, lalu masuk ke folder **Download** dan ketuk file **`ShadowAssassin.apk`**.
3. Jika diminta izin keamanan, pilih **Setelan** dan aktifkan **"Izinkan dari sumber ini"** (*Install from Unknown Sources*).
4. Jika muncul peringatan **Google Play Protect** karena aplikasi berasal dari luar Play Store, ketuk **"Detail selengkapnya"** (*More details*) → **"Tetap instal"** (*Install anyway*).
5. Buka aplikasi **Shadow Assassin** dan mainkan secara **100% offline**!

---

## 🎮 Kontrol Permainan

Game ini dirancang untuk dapat dimainkan di **Smartphone (Touchscreen)** maupun di **PC/Laptop (Keyboard)**:

| Aksi | Keyboard (PC) | Layar Sentuh (Android) |
|---|---|---|
| **Gerak Kiri / Kanan** | `A` / `D` atau `Panah Kiri` / `Kanan` | D-Pad `◀` / `▶` (Kiri Bawah, bebas geser jari) |
| **Lompat / Double Jump** | `W` / `Panah Atas` | Tombol `LOMPAT` + indikator *pip* (Kanan Bawah) |
| **Serang / Combo Pedang** | `J` / `Z` / `Spasi` | Tombol `SERANG` (Kanan Bawah) |
| **Lempar Kunai Bayangan** | `L` / `C` | Tombol `KUNAI` (Kanan Bawah) |
| **Dash (Menghindar Cepat)** | `K` / `X` / `Shift` | Tombol `DASH` (Kanan Bawah) |
| **Badai Bayangan (ULTI)** | `Q` / `E` / `F` | Tombol `ULTI` saat Fury 100% (Kanan Bawah) |
| **Buka Toko / Upgrade** | `B` atau klik tombol Toko | Sentuh tombol Toko (Kiri Atas) |
| **Pause / Restart / Mute** | `P` / `Esc` atau HUD Atas | Tombol di HUD Atas |

---

## ✨ Fitur Utama (v2.0.0)

- **8 Stage Campaign (3 Babak Penuh + Final Boss Baru):**
  - **Babak I (Benteng Grommash):** Stage 1 Hutan Gelap, Stage 2 Gua Goblin, Stage 3 Benteng Goblin (Boss: *Raja Goblin Grommash*).
  - **Babak II (Menuju Matahari):** Stage 4 Jurang Kabut (*platform* bergerak & jurang), Stage 5 Kuil Obsidian, Stage 6 Puncak Fajar (Boss: *Kaisar Goblin Kraven* + *Summon Guards*).
  - **Babak III (Gerhana Abadi — Baru di v2.0.0!):** Stage 7 Jembatan Magma (jembatan gantung magma, **Batu Pegas Bayangan**, & *Goblin Pengebom*), Stage 8 Tahta Gerhana (Final Boss 3 Fase: *Overlord Goblin Malakor* + *Garda Gerhana*).
  - **Alur Cerita Antar-Stage** di Toko Bayangan & fitur **Pilih Stage Terbuka (Stage 1–8)** di menu awal.
- **Mekanik Combat & Arena Baru:**
  - **Badai Bayangan (`Q`/`E`/`F` & `ULTI`):** Kumpulkan *Shadow Fury* (`0–100%`) dari serangan, backstab, parry, & kill untuk melepaskan badai AoE masif yang menembus tameng dan menyapu proyektil!
  - **Belati Bayangan Lv.3+ (*Sabit Bayangan*):** Combo ke-3 meluncurkan gelombang sabit energi menembus banyak musuh + **Air Slash** jangkauan ekstra di udara.
  - **Batu Pegas Bayangan:** Landasan pegas bercahaya untuk melontarkan Assassin ke platform tinggi sekaligus mereset kuota *Double Jump*.
  - **Variasi Musuh Lengkap:** *Goblin Brute* (tameng depan vs *Backstab 1.5x Crit!*), *Goblin Ninja*, *Goblin Shaman* (bola sihir & penyembuh kawan), plus **Goblin Pengebom** (*bom parabola* yang bisa ditangkis belati/kunai!).
  - **Checkpoint Lentera Bayangan & Nyawa Bayangan** (1× bangkit otomatis) serta **16 Peti Harta Tersembunyi** (2 per stage).
  - **Peringkat Kemenangan (`Rank S / A / B / C`)**, pencatat waktu tempuh, dan rekor tersimpan di `localStorage`.
- **Perbaikan Bug Tombol Lompat & Optimasi Zero-Lag:**
  - Menghapus `setPointerCapture` contention & mutasi kelas DOM per-frame (diganti `data-active` / `data-jumps` cache) agar tombol `LOMPAT` dan D-Pad tidak pernah nyangkut, double-consume jump, atau memicu stutter WebView.
  - Sinkronisasi *frame pacing* 60Hz, pembersihan node Web Audio API, dan indikator *2 Pip Double Jump* langsung pada tombol `LOMPAT`.
- **CG Ending Fajar Kedamaian & Audio Sintetis:**
  - Epilog animasi sang Shadow Assassin menyaksikan matahari terbit setelah menumbangkan Overlord Malakor, dengan fitur *Putar Ulang CG*.
  - 8 pola BGM sintetis unik per stage + efek suara tebasan, crit, kunai, pegas, bom, badai bayangan, dan akord fajar 100% offline (~3.3 MB).
  - Kompatibel dengan **Android 5.0 (Lollipop) hingga Android 15** (`minSdk 21`, signed v1+v2+v3) dalam WebView Fullscreen Immersive Mode (Landscape).

---

## 🚀 Build APK Sendiri (Lokal)

1. Pastikan telah terinstall **JDK 17** dan **Android SDK (Platform 34, Build-Tools 34.0.0)**.
2. Clone repository:
   ```bash
   git clone https://github.com/Ryn-debugging/assasin-vs-goblin.git
   cd assasin-vs-goblin
   ```
3. Jalankan Gradle wrapper untuk membangun Release APK:
   ```bash
   ./gradlew assembleRelease
   ```
4. File APK akan berada di:
   ```
   app/build/outputs/apk/release/app-release.apk
   ```
