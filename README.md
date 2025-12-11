# Sistem Cerdas Rekomendasi Menu Diet Berdasarkan Profil Pengguna

## 🔥 Deskripsi Project

Sistem Cerdas Rekomendasi Menu Diet adalah aplikasi berbasis Rule-Based System (Expert System) yang memberikan rekomendasi menu diet personal berdasarkan profil pengguna. Sistem ini menggunakan pendekatan logika aturan (rule-based) bukan Machine Learning, sehingga setiap rekomendasi dapat dijelaskan secara transparan.

**Fitur Utama:**
- Input data pengguna: umur, berat badan, tinggi badan, tingkat aktivitas, dan tujuan diet
- Perhitungan BMR (Basal Metabolic Rate) menggunakan rumus Harris-Benedict
- Penentuan kebutuhan kalori harian berdasarkan aktivitas
- Rekomendasi menu diet yang disesuaikan dengan tujuan (turun, naik, atau stabil berat badan)

## 🎯 Tujuan Sistem

1. **Membantu menentukan menu makanan sehat** - Memberikan panduan menu yang seimbang dan bergizi
2. **Menentukan kebutuhan kalori** - Menghitung kebutuhan kalori harian yang akurat
3. **Memberi saran menu sesuai tujuan diet** - Menyesuaikan rekomendasi dengan goal pengguna

## ⚡ Fitur-Fitur Sistem

### 1. Input Data Pengguna
- **Umur**: Untuk perhitungan BMR
- **Berat Badan**: Dalam kilogram
- **Tinggi Badan**: Dalam sentimeter
- **Tingkat Aktivitas**: Ringan, Normal, atau Berat
- **Tujuan Diet**: Turun BB, Stabil, atau Naik BB

### 2. Perhitungan BMR Sederhana
Menggunakan rumus Harris-Benedict untuk menghitung metabolisme basal

### 3. Penentuan Kategori Diet
- **Defisit Kalori**: Untuk turun berat badan (-300 kalori)
- **Maintenance**: Untuk menjaga berat badan (sesuai kebutuhan)
- **Surplus Kalori**: Untuk naik berat badan (+300 kalori)

### 4. Rekomendasi Menu Diet
Memberikan saran menu lengkap untuk:
- Sarapan
- Makan Siang
- Makan Malam
- Snack

### 5. Output Ringkas dan Jelas
Menampilkan hasil dalam format yang mudah dipahami

## 📊 Rumus & Logika Sistem

### Perhitungan BMR (Basal Metabolic Rate)
```
BMR = 66 + (13.7 × berat_badan) + (5 × tinggi_badan) - (6.8 × umur)
```

### Perhitungan Kalori Harian Berdasarkan Aktivitas
- **Aktivitas Ringan**: BMR × 1.2
- **Aktivitas Normal**: BMR × 1.35
- **Aktivitas Berat**: BMR × 1.5

### Aturan Tujuan Diet
- **Turun Berat Badan**: Total Kalori - 300
- **Stabil Berat Badan**: Total Kalori (maintenance)
- **Naik Berat Badan**: Total Kalori + 300

## 🔧 Instalasi dan Penggunaan

1. Clone atau download project ini
2. Pastikan Python 3.x terinstall
3. Jalankan file `main.py`:
   ```bash
   python main.py
   ```
4. Ikuti instruksi input yang muncul
5. Lihat hasil rekomendasi diet Anda

## 📁 Struktur Project

```
diet-recommendation-system/
├── main.py                 # File utama aplikasi
├── diet_system.py         # Core logic sistem diet
├── rules.py              # Rule-based system
├── utils.py              # Utility functions
├── README.md             # Dokumentasi
├── DOCUMENTATION.md      # Dokumentasi detail
└── examples/
    └── sample_output.txt # Contoh output
```

## 🚀 Teknologi yang Digunakan

- **Python 3.x**: Bahasa pemrograman utama
- **Rule-Based System**: Metode expert system
- **Object-Oriented Programming**: Struktur code yang rapi

## 📝 Lisensi

Project ini dibuat untuk tujuan edukasi dan pembelajaran sistem cerdas.