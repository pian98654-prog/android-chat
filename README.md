# Laravel Chat - Proyek APK Android

Aplikasi Android (WebView) yang memuat UI React dan mengambil data dari server Laravel
(paket `laravel-chat.zip`). Alamat server diatur di dalam aplikasi lewat tombol ⚙.

## Cara 1: Tanpa Android Studio (GitHub Actions)
1. Buat repo GitHub, unggah isi folder ini.
2. Tab Actions > "Build APK" > Run workflow.
3. Unduh artefak `LaravelChat-apk` (berisi app-debug.apk), pasang di HP.

## Cara 2: Android Studio
Open folder ini, tunggu Gradle sync, lalu Build > Build APK(s).
Hasil: app/build/outputs/apk/debug/app-debug.apk

## Menjalankan server Laravel
    php artisan serve --host=0.0.0.0
Di aplikasi, tekan ⚙ dan isi alamat, contoh http://192.168.1.5:8000
(HP dan komputer harus satu Wi-Fi; emulator memakai http://10.0.2.2:8000).
