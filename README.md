# SKYPORT — Airport Flight Simulator (Multi Aircraft & Airport)

Project statis HTML + Three.js. Dapat di-host dengan GitHub Pages.

## Model tersedia

Kendaraan:
- Pesawat original (`assets/plane.glb`)
- KF-21A Boramae (`assets/kf-21a_boramae_fighter_jet.glb`)
- AH-1W SuperCobra (`assets/ah-1w_supercobra_attack_helicopter.glb`)

Bandara:
- Airport Pack (`assets/airport_pack_total.glb`)
- Sunshine Airport Sunset (`assets/sunshine_airportsunset.glb`)

## Menjalankan

1. Upload SEMUA isi folder ini ke root repository GitHub.
2. Settings → Pages → Deploy from a branch → main → / (root).
3. Buka alamat GitHub Pages: `https://USERNAME.github.io/NAMA-REPO/`.
4. Pilih kendaraan dan bandara pada menu awal, lalu klik **Mulai Simulator**.
5. Kapan saja klik **Pilih Pesawat / Bandara** untuk mengganti kombinasi.

Bisa juga diuji secara lokal dengan `python -m http.server 8000` lalu membuka `http://localhost:8000/`.

## Kontrol

- Joystick kiri/kanan = belok kiri/kanan.
- Joystick atas/bawah = naik/turun ketika sudah terbang.
- Slider THROTTLE = tenaga / kecepatan.
- TAKE OFF = bantu lepas landas (untuk helikopter: naik vertikal).
- REM, TURUN, Reset, Kamera, Suara ON/OFF.
- PC: W/S = naik/turun, A/D = belok, panah atas/bawah = throttle, spasi = takeoff, C = kamera, R = reset.
- Untuk helikopter, baling-baling utama dan ekor dianimasikan lewat JavaScript. Model tidak memiliki animasi bawaan.

## Mode AR (opsional)

`ar.html` menggunakan MindAR. Supaya mode AR bekerja, kompilasi gambar `markers/airport-marker.png` dengan MindAR Image Target Compiler menjadi `markers/targets.mind`, kemudian upload file tersebut. AR memerlukan kamera, HTTPS dan marker fisik yang terlihat jelas. Tanpa `targets.mind`, mode AR belum siap digunakan.

## Catatan

- Simulasi penerbangan sederhana, bukan simulator fisika penerbangan realistis.
- Penempatan awal di Airport Sunset dan orientasi model pesawat perlu diuji dan mungkin perlu kalibrasi agar persis sejajar landasan.
- Ukuran berkas relatif besar; tunggu proses loading pada HP dan gunakan koneksi stabil.
- Periksa lisensi model 3D asli sebelum mendistribusikan repository publik.
- Aset GLB dimuat saat dipilih, bukan semuanya sekaligus.
