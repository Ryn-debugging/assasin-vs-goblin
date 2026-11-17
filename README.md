# 🗡️ Shadow Assassin vs Goblins

**Shadow Assassin vs Goblins** adalah game 2D Action Platformer seru berbasis HTML5 Canvas yang telah dibungkus menjadi aplikasi **Android APK** native dengan dukungan offline penuh, kontrol layar sentuh (touchscreen), dan efek audio sintetis tanpa ketergantungan internet.

---

## 📱 Download APK Android

Kamu bisa langsung mengunduh file APK game ini melalui tautan rilis GitHub:

👉 **[Download ShadowAssassin-v1.0.0.apk](https://github.com/Ryn-debugging/assasin-vs-goblin/releases/latest)**

> **Catatan Instalasi:**
> 1. Unduh file `.apk` ke smartphone Android kamu.
> 2. Buka file APK dan izinkan *"Install from Unknown Sources"* jika diminta.
> 3. Mainkan langsung tanpa perlu koneksi internet (100% offline)!

---

## 🎮 Kontrol Permainan

Game ini dirancang untuk dapat dimainkan di **Smartphone (Touchscreen)** maupun di **PC/Laptop (Keyboard)**:

| Aksi | Keyboard (PC) | Layar Sentuh (Android) |
|---|---|---|
| **Gerak Kiri / Kanan** | `A` / `D` atau `Panah Kiri` / `Kanan` | Tombol `◀` / `▶` (Kiri Bawah) |
| **Lompat / Double Jump** | `W` / `Space` / `Panah Atas` | Tombol `JUMP` (Kanan Bawah) |
| **Dash (Menghindar Cepat)** | `Shift` / `L` | Tombol `DASH` (Kanan Bawah) |
| **Serang / Combo Pedang** | `J` / `K` / `Enter` | Tombol `ATK` (Kanan Bawah) |
| **Buka Toko / Upgrade** | Klik tombol Toko | Sentuh tombol Toko (Kiri Atas) |
| **Restart / Mute Audio** | Tombol di HUD Atas | Tombol di HUD Atas |

---

## ✨ Fitur Utama

- **3 Stage Menantang:**
  - Stage 1: Hutan Goblin Liar (Forest of Shadows)
  - Stage 2: Reruntuhan Kuno (Ancient Ruins)
  - Stage 3: Benteng Raja Goblin (Goblin Warlord Stronghold)
- **Combat Mechanics:**
  - Kombo tebasan pedang bayangan (3-hit slash combo).
  - Dash tembus musuh dengan masa kebal (invulnerability frames).
  - Double jump untuk manuver vertikal.
- **Sistem Toko & Upgrade Karakter:**
  - Upgrade Attack Power, Max HP, Movement Speed, dan Heal Potion menggunakan koin yang didapat dari goblin.
- **Audio Sintetis (Web Audio API):**
  - Efek suara tebasan, lompatan, dash, kena pukul, goblin mati, koin, dan latar belakang tanpa file audio eksternal.
- **100% Offline & Ringan:**
  - Semua font (Cinzel, Plus Jakarta Sans), ikon (FontAwesome), dan styling telah dibundel secara lokal.
  - Ukuran file APK hanya ~6 MB.
- **Layar Penuh (Immersive Mode):**
  - Mengisi penuh layar ponsel lanskap tanpa gangguan bilah status / navigasi.

---

## 🛠️ Struktur Proyek

```
assasin-vs-goblin/
├── app/                               # Modul Aplikasi Android
│   ├── src/main/
│   │   ├── AndroidManifest.xml        # Konfigurasi aplikasi Android (landscape, fullscreen)
│   │   ├── java/com/ryn/shadowassassin/
│   │   │   └── MainActivity.java      # Android WebView Immersive Runner
│   │   ├── assets/www/                # Web bundle lokal offline
│   │   └── res/                       # Icon (mipmap) & resources
│   └── build.gradle                   # Gradle config modul app
├── .github/workflows/
│   └── build-apk.yml                  # GitHub Actions CI/CD otomatis untuk build APK
├── index.html                         # Game web (dapat dimainkan langsung via browser/GitHub Pages)
├── css/                               # Styling lokal (FontAwesome & Fonts)
├── js/                                # Tailwind JS runtime
├── fonts/                             # Font Cinzel & Plus Jakarta Sans offline
├── webfonts/                          # FontAwesome webfonts
├── build.gradle                       # Root gradle build file
├── settings.gradle                    # Project settings
├── gradlew & gradlew.bat              # Gradle wrapper
└── README.md
```

---

## 🚀 Cara Build APK Sendiri (Lokal)

Jika kamu ingin melakukan modifikasi dan melakukan build APK sendiri di komputer kamu:

1. Pastikan telah terinstall **JDK 17** dan **Android SDK (Platform 34, Build-Tools 34.0.0)**.
2. Clone repository:
   ```bash
   git clone https://github.com/Ryn-debugging/assasin-vs-goblin.git
   cd assasin-vs-goblin
   ```
3. Jalankan Gradle wrapper:
   ```bash
   ./gradlew assembleDebug
   ```
4. File APK yang sudah jadi akan berada di:
   ```
   app/build/outputs/apk/debug/app-debug.apk
   ```

---

## 🤖 Build Otomatis via GitHub Actions

Setiap kali kamu melakukan `git push` ke branch `main`, GitHub Actions akan otomatis:
1. Menyiapkan environment Java 17 dan Android SDK.
2. Melakukan build file `app-debug.apk`.
3. Mengunggah file APK ke tab **Actions** sebagai artifact yang bisa langsung diunduh.
4. Jika kamu membuat git tag versi (misalnya `v1.0.1`), GitHub Actions akan otomatis membuat **GitHub Release** baru beserta file APK-nya.
