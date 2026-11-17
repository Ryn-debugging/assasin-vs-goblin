# 🗡️ Shadow Assassin vs Goblins

**Shadow Assassin vs Goblins** adalah game 2D Action Platformer seru berbasis HTML5 Canvas yang telah dibungkus menjadi aplikasi **Android APK** native (Signed Release APK) dengan dukungan offline penuh, kontrol layar sentuh (touchscreen), dan efek audio sintetis tanpa ketergantungan internet.

---

## 📱 Download APK Android

Kamu bisa langsung mengunduh file APK versi terbaru (**v1.1.0 - Release APK**) melalui tautan berikut:

👉 **[Download ShadowAssassin.apk (v1.1.0)](https://github.com/Ryn-debugging/assasin-vs-goblin/releases/latest/download/ShadowAssassin.apk)**

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
| **Gerak Kiri / Kanan** | `A` / `D` atau `Panah Kiri` / `Kanan` | D-Pad `◀` / `▶` (Kiri Bawah, dukung geser jari) |
| **Lompat / Double Jump** | `W` / `Panah Atas` | Tombol `LOMPAT` (Kanan Bawah) |
| **Serang / Combo Pedang** | `J` / `Z` / `Spasi` | Tombol `SERANG` (Kanan Bawah) |
| **Lempar Kunai Bayangan** | `L` / `C` | Tombol `KUNAI` (Kanan Bawah) |
| **Dash (Menghindar Cepat)** | `K` / `X` / `Shift` | Tombol `DASH` (Kanan Bawah) |
| **Buka Toko / Upgrade** | `B` atau klik tombol Toko | Sentuh tombol Toko (Kiri Atas) |
| **Pause / Restart / Mute** | `P` / `Esc` atau HUD Atas | Tombol di HUD Atas |

---

## ✨ Fitur Utama

- **6 Stage Campaign (2 Babak Lengkap):**
  - **Babak I (Benteng Grommash):** Stage 1 Hutan Gelap, Stage 2 Gua Goblin, Stage 3 Benteng Goblin (Boss: *Raja Goblin Grommash* — Phase 2).
  - **Babak II (Menuju Matahari):** Stage 4 Jurang Kabut (*platform* bergerak & jurang), Stage 5 Kuil Obsidian, Stage 6 Puncak Fajar (Final Boss: *Kaisar Goblin Kraven* + *Summon Guards*).
  - **Alur Cerita Antar-Stage** di Toko Bayangan & fitur **Pilih Stage Terbuka** di menu awal.
- **Combat & Eksplorasi Mendalam:**
  - **Serangan Belakang (`1.5x` Crit!)** & penghitung **Combo Streak**.
  - **Kunai Bayangan (`L`/`C` & `KUNAI`):** proyektil jarak jauh yang juga dapat menangkis panah musuh!
  - **Variasi Musuh Baru:** *Goblin Brute* (perisai depan, rentan diserang dari belakang), *Goblin Ninja* (sergap cepat), dan *Goblin Shaman* (bola sihir & penyembuh kawan).
  - **Checkpoint Lentera Bayangan & Nyawa Bayangan** (1× bangkit otomatis di stage lanjut) serta **12 Peti Harta Tersembunyi** (2 per stage).
  - **Peringkat Kemenangan (`Rank S / A / B / C`)**, pencatat waktu tempuh, dan rekor tersimpan di `localStorage`.
- **CG Ending Fajar Kedamaian:**
  - Adegan epilog animasi sang Shadow Assassin menyaksikan matahari terbit setelah menumbangkan Kaisar Kraven, lengkap dengan fitur *Putar Ulang CG*.
- **Sistem Toko & Upgrade Karakter:**
  - Upgrade *Belati Bayangan* (Damage), *Jubah Pelindung* (Max HP), *Langkah Angin* (Kecepatan & Cooldown Dash), dan *Eliksir Darah*.
- **Audio Sintetis (Web Audio API):**
  - 6 pola BGM unik per stage serta efek suara tebasan, crit, kunai, parry, checkpoint, peti harta, bangkit bayangan, dan akord fajar tanpa file audio eksternal.
- **100% Offline & Ringan (~3.2 MB):**
  - Kompatibel dengan **Android 5.0 (Lollipop) hingga Android 15** (`minSdk 21`, signed v1+v2+v3).
  - Menggunakan `WebViewAssetLoader` dan tampilan Fullscreen Immersive Mode (Landscape).

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
