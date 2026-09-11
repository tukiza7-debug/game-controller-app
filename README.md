# 🎮 Game Controller App

> Aplikasi pengawal permainan untuk peranti Android yang anda pegang. Memaparkan skrin peranti Host dan menukar skrin sentuh menjadi gamepad maya.

## 📋 Penerangan
Aplikasi ini adalah bahagian **Controller** dalam sistem Scrcpy Game Controller. Ia dipasang pada telefon/tablet fizikal anda dan bertindak sebagai pengawal jauh untuk peranti Host (sama ada peranti fizikal lain atau Cloud Phone).

## ✨ Ciri-ciri
- 📺 Paparan skrin peranti Host secara langsung (video + audio)
- 🎯 Kawalan sentuh penuh — skrin anda menjadi gamepad maya
- ⚙️ Tetapan resolusi dan bitrate boleh laras
- 📶 Menyokong sambungan WiFi dan USB OTG
- 🌐 Boleh mengawal Cloud Phone dari mana-mana sahaja
- 🔒 Sambungan selamat melalui ADB

## 🚀 Cara Deploy di GitHub

### 1. Muat Naik Kod ke GitHub
```bash
git init
git add .
git commit -m "Initial commit: Game Controller App"
git branch -M main
git remote add origin https://github.com/USERNAME/game-controller-app.git
git push -u origin main
```

### 2. GitHub Actions Auto-Build
Fail `.github/workflows/build.yml` sudah sedia dikonfigurasi. Ia akan:
- ✅ Build APK secara automatik pada setiap `push` ke branch `main`
- ✅ Muat naik APK sebagai **Artifact** (boleh dimuat turun dari halaman Actions)
- ✅ Auto-cipta **GitHub Release** apabila anda buat tag `v*` (contoh: `v1.0.0`)

### 3. Cara Dapatkan APK
#### Daripada Artifact (setiap push):
1. Pergi ke tab **Actions** di repo GitHub anda
2. Klik pada workflow run yang terkini
3. Scroll ke bahagian **Artifacts**
4. Muat turun `game-controller-apk`

#### Daripada Release (versi stabil):
1. Buat tag versi: `git tag v1.0.0 && git push origin v1.0.0`
2. Pergi ke tab **Releases**
3. Muat turun APK dari bahagian Assets

## 📱 Cara Guna
1. Pasang APK pada telefon/tablet anda
2. Pastikan peranti Host sudah disediakan (ADB diaktifkan)
3. Buka aplikasi, masukkan alamat IP peranti Host
4. Pilih tetapan paparan yang sesuai
5. Tekan **Start** dan mula mengawal!

## 🔗 Berkaitan
- [Host/Game Device App](../host-game-device-app/) — Aplikasi untuk peranti sasaran
- [Dokumentasi Sistem](../docs/) — Panduan lengkap penggunaan
