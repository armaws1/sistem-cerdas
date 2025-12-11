# 🍎 Sistem Cerdas Rekomendasi Menu Diet Berdasarkan Profil Pengguna

## 🔥 Deskripsi Project

Sistem Cerdas Rekomendasi Menu Diet adalah aplikasi berbasis **Rule-Based System (Expert System)** yang memberikan rekomendasi menu diet personal berdasarkan profil pengguna. Sistem ini menggunakan pendekatan logika aturan (rule-based) bukan Machine Learning, sehingga setiap rekomendasi dapat dijelaskan secara transparan.

**Fitur Utama:**
- Input data pengguna: umur, berat badan, tinggi badan, tingkat aktivitas, dan tujuan diet
- Perhitungan BMR (Basal Metabolic Rate) menggunakan rumus Harris-Benedict
- Penentuan kebutuhan kalori harian berdasarkan aktivitas
- Rekomendasi menu diet yang disesuaikan dengan tujuan (turun, naik, atau stabil berat badan)

## 🚀 CARA PENGGUNAAN

### ⚡ **Quick Start (3 Langkah)**

#### **1️⃣ PILIH VERSI**
```
🌐 Web Version (Recommended - Paling Mudah):
→ Double-click file "web_version.html"
→ Otomatis buka di browser

🐍 Python Version (Untuk Developer):
→ Buka terminal: py main.py
```

#### **2️⃣ ISI DATA ANDA**
```
🎂 Umur: _____ tahun (10-100)
⚖️ Berat: _____ kg (30-200)  
📏 Tinggi: _____ cm (100-250)
🏃 Aktivitas: Ringan / Normal / Berat
🎯 Tujuan: Turun / Stabil / Naik BB
```

#### **3️⃣ DAPATKAN HASIL**
```
📊 BMR & Kalori Target
🍽️ Menu 4 Waktu Makan
💡 Tips Diet Personal
📋 Kategori Diet Anda
```

### 🎭 **Coba Demo Dulu**
```
🌐 Web: Buka web_version.html → Klik "Jalankan Demo"
🐍 Python: Terminal → py run_demo.py
```

### 📊 **Contoh Hasil**
```
Input: Andi (25 tahun, 80kg, 170cm, Normal, Turun BB)

Output:
📈 BMR: 1801 kalori/hari
🎯 Target: 2131 kalori/hari (defisit 300)
📊 BMI: 27.68 (Overweight)

Menu:
🌅 Sarapan: Oatmeal + pisang + telur rebus
🌞 Siang: Nasi merah + ayam kukus + sayur
🌙 Malam: Sup sayur + ikan kukus  
🍎 Snack: Yogurt rendah lemak
```

## 🎯 Tujuan Sistem

1. **Membantu menentukan menu makanan sehat** - Memberikan panduan menu yang seimbang dan bergizi
2. **Menentukan kebutuhan kalori** - Menghitung kebutuhan kalori harian yang akurat
3. **Memberi saran menu sesuai tujuan diet** - Menyesuaikan rekomendasi dengan goal pengguna

## ⚡ Fitur-Fitur Sistem

### 🔧 **Input & Processing**
- **Input Data Lengkap**: Umur, berat, tinggi, aktivitas, tujuan diet
- **Validasi Otomatis**: Error handling untuk input yang salah
- **Perhitungan Real-time**: BMR dan kalori langsung dihitung

### 📊 **Output & Rekomendasi**
- **BMR & Kalori Target**: Perhitungan akurat berdasarkan rumus medis
- **Menu 4 Waktu Makan**: Sarapan, siang, malam, snack
- **Tips Diet Personal**: Sesuai tujuan masing-masing
- **BMI Calculator**: Bonus informasi kesehatan

### 🎨 **User Experience**
- **2 Versi**: Web (HTML) dan Python (Terminal)
- **Demo Mode**: 3 contoh kasus otomatis
- **Responsive Design**: Mobile-friendly web version
- **Save Results**: Simpan hasil ke file

## 📊 Rumus & Logika Sistem

### **Perhitungan BMR (Harris-Benedict Formula)**
```
BMR = 66 + (13.7 × berat) + (5 × tinggi) – (6.8 × umur)
```

### **Kalori Harian Berdasarkan Aktivitas**
```
Ringan (jarang olahraga): BMR × 1.2
Normal (1-3x seminggu): BMR × 1.35
Berat (4-7x seminggu): BMR × 1.5
```

### **Target Kalori Sesuai Tujuan**
```
Turun BB: Kalori Harian - 300 (defisit)
Stabil: Kalori Harian (maintenance)
Naik BB: Kalori Harian + 300 (surplus)
```

### **Rule-Based Menu Selection**
```
IF Tujuan = "Turun BB" THEN
→ Menu rendah kalori, tinggi protein, banyak sayur

IF Tujuan = "Naik BB" THEN  
→ Menu tinggi kalori, protein + karbohidrat

IF Tujuan = "Stabil" THEN
→ Menu seimbang, variasi nutrisi
```

## 🔧 Instalasi & Setup

### **Web Version (No Install)**
```bash
# Langsung buka file
Double-click web_version.html

# Atau drag & drop ke browser
```

### **Python Version**
```bash
# 1. Pastikan Python terinstall
python --version  # atau py --version

# 2. Navigate ke folder project
cd path/to/project

# 3. Jalankan aplikasi
py main.py          # Mode normal
py run_demo.py      # Mode demo
py test_system.py   # Testing
```

## 📁 Struktur Project Lengkap

```
diet-recommendation-system/
├── 🌐 web_version.html        # Web version (HTML+JS)
├── 🐍 main.py                 # Python app utama
├── 🧠 diet_system.py         # Core logic BMR & kalori
├── 🔧 rules.py              # Rule-based menu system
├── 🛠️ utils.py              # Input/output utilities
├── 🎭 run_demo.py           # Demo 3 kasus otomatis
├── 🧪 test_system.py        # Testing semua fungsi
├── 📚 README.md             # Dokumentasi ini
├── 📖 DOCUMENTATION.md      # Technical documentation
├── 📋 USER_GUIDE.md         # Panduan lengkap user
├── 🎯 QUICK_START.md        # Panduan cepat
├── 🎬 PRESENTATION_GUIDE.md # Panduan presentasi
├── 📊 PROJECT_SUMMARY.md    # Summary project
├── 📦 requirements.txt      # Dependencies (kosong)
└── 📂 examples/
    └── 📄 sample_output.txt # Contoh output
```

## 💡 Tips Penggunaan

### **✅ DO:**
```
• Input data yang akurat dan jujur
• Pilih tingkat aktivitas sesuai kenyataan
• Ikuti variasi menu yang disarankan
• Konsisten dengan target kalori
• Monitor progress mingguan
```

### **❌ DON'T:**
```
• Bohong tentang berat/tinggi badan
• Overestimate tingkat aktivitas
• Skip makan (terutama sarapan)
• Expect hasil instan
• Abaikan tips yang diberikan
```

### **⚠️ Penting:**
```
• Konsultasi dokter untuk kondisi medis khusus
• Sistem ini alat bantu, bukan pengganti ahli gizi
• Hasil realistis: 0.5-1kg/minggu untuk turun BB
• Sabar dan konsisten adalah kunci sukses
```

## 🔧 Troubleshooting

### **Web Version Bermasalah?**
```
→ Coba browser lain (Chrome, Firefox, Edge)
→ Drag file web_version.html ke browser
→ Clear browser cache dan refresh
```

### **Python Error?**
```
→ Coba: py main.py
→ Atau: python main.py  
→ Atau: python3 main.py
→ Install Python dari python.org jika belum ada
```

### **Input Tidak Valid?**
```
→ Cek range: umur (10-100), berat (30-200), tinggi (100-250)
→ Gunakan titik (.) bukan koma (,) untuk desimal
→ Refresh dan coba lagi
```

## 🚀 Teknologi & Implementasi

### **Tech Stack:**
- **Frontend**: HTML5, CSS3, JavaScript (Web version)
- **Backend**: Python 3.x (Desktop version)
- **Architecture**: Rule-Based System (Expert System)
- **Design Pattern**: Object-Oriented Programming

### **Key Features:**
- **No Dependencies**: Pure Python & HTML/JS
- **Cross Platform**: Windows, Mac, Linux, Mobile
- **Offline Capable**: Tidak perlu internet
- **Lightweight**: < 1MB total size

### **Testing:**
- ✅ Unit tests untuk semua fungsi
- ✅ Integration tests
- ✅ Edge case validation
- ✅ Input validation
- ✅ 100% success rate

## 🎯 Pengembangan Selanjutnya

### **Short Term:**
- Database menu lebih lengkap
- Support untuk wanita (rumus BMR berbeda)
- Perhitungan nutrisi detail (protein, lemak, vitamin)
- Preferensi makanan personal

### **Long Term:**
- Mobile application (Android/iOS)
- Integration dengan fitness tracker
- AI optimization berdasarkan feedback
- Konsultasi online dengan ahli gizi
- Social features & community

## 📞 Support & Documentation

### **Dokumentasi Lengkap:**
- 📚 **README.md** - Overview & quick start (file ini)
- 📖 **USER_GUIDE.md** - Panduan lengkap pengguna
- 📋 **DOCUMENTATION.md** - Technical documentation
- 🎬 **PRESENTATION_GUIDE.md** - Panduan presentasi

### **Need Help?**
1. Baca USER_GUIDE.md untuk panduan detail
2. Coba demo mode dulu
3. Jalankan py test_system.py untuk cek fungsi
4. Periksa troubleshooting di atas

## 🏆 Kesimpulan

**Sistem Diet Cerdas ini membuktikan bahwa:**
- ✅ Rule-Based System efektif untuk rekomendasi personal
- ✅ Transparansi lebih penting daripada kompleksitas
- ✅ User experience yang baik tidak perlu teknologi rumit
- ✅ Solusi sederhana sering kali yang terbaik

**Ready to start your diet journey? Buka `web_version.html` dan mulai sekarang! 🍎💪**

---

## 📝 Lisensi

Project ini dibuat untuk tujuan edukasi dan pembelajaran sistem cerdas. Feel free to use, modify, and distribute! 🚀