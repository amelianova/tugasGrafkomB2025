# Tugas Grafika Komputer B 2025

## Identitas
|    NRP     |      Nama      |
| :--------: | :------------: |
| 5025231041 | Amelia Nova Safitri |

Proyek ini adalah implementasi rendering 3D menggunakan WebGL yang menampilkan objek teks "NO1" dengan pencahayaan dinamis dan kontrol interaktif.
NO: "Nova"
1: Digit terakhir NRP

## Deskripsi

Aplikasi ini mendemonstrasikan berbagai konsep grafika komputer 3D, termasuk:
- **Rendering 3D** dengan WebGL
- **Pencahayaan Phong** (Ambient, Diffuse, Specular)
- **Transformasi 3D** (Rotasi dan Translasi)
- **Normal Mapping** untuk pencahayaan yang realistis
- **Animasi real-time** dengan kontrol interaktif

Objek yang dirender adalah teks "NO1" dalam bentuk 3D dengan tiga warna berbeda:
- **N** - Biru terang
- **O** - Pink
- **1** - Hijau terang

## Cara Menjalankan

1. **Clone atau download** repository ini
2. **Buka file `index.html`** di browser modern yang mendukung WebGL (Chrome, Firefox, Edge, Safari)
3. Objek 3D akan langsung muncul dan berputar secara otomatis

## Kontrol

### Keyboard Controls

| Tombol | Fungsi |
|--------|--------|
| **X** | Rotasi pada sumbu X |
| **Y** | Rotasi pada sumbu Y (default) |
| **Z** | Rotasi pada sumbu Z |
| **Space** | Pause/Resume rotasi (tekan dan tahan untuk pause) |
| **Arrow Up (↑)** | Gerakkan objek ke atas |
| **Arrow Down (↓)** | Gerakkan objek ke bawah |
| **Arrow Left (←)** | Gerakkan objek ke kiri |
| **Arrow Right (→)** | Gerakkan objek ke kanan |

### Mouse Controls

| Aksi | Fungsi |
|------|--------|
| **Click** | Toggle pause/resume rotasi |

## Penjelasan tambahan tentang pencayahaan, transformasi, dan geometri

### Pencahayaan
- **Ambient Light**: Memberikan pencahayaan dasar pada semua objek (30% intensity)
- **Diffuse Light**: Pencahayaan berdasarkan sudut permukaan terhadap sumber cahaya
- **Specular Light**: Highlight mengkilap pada permukaan objek (shininess: 32)

### Transformasi
- **Model Matrix**: Untuk rotasi dan translasi objek
- **View Matrix**: Posisi kamera di (0, 0, 2) menghadap origin
- **Projection Matrix**: Perspektif dengan FOV 60°

### Geometri
- **Huruf N**: Terdiri dari 3 bagian (bar kiri, bar kanan, diagonal)
- **Huruf O**: Ring berbentuk octagon dengan lubang di tengah
- **Angka 1**: Terdiri dari bar utama, serif atas, dan base bawah
