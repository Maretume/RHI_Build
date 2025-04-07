---

# 🏗️ Sistem Manajemen Konstruksi Terintegrasi - RHI Build (Kemungkinan di buat)

Sistem ini dikembangkan menggunakan **Laravel 12** dengan pendekatan modular dan memanfaatkan **Filament Admin Panel**. Dirancang khusus untuk digitalisasi proses di perusahaan **RHI Build**, mulai dari HRM, CRM, Manajemen Proyek, Logistik, Keuangan, hingga Keamanan Data.

---

## 📦 Modul Utama

### 1. Human Resource Management (HRM)
- Tracking absensi digital berbasis waktu  
- Penilaian kinerja menggunakan KPI  
- Manajemen data karyawan  
- Kontrol akses berjenjang berbasis role  

### 2. Customer Relationship Management (CRM)
- Tracking leads otomatis  
- Manajemen komunikasi klien  
- Dokumentasi proyek per klien  
- Sistem penawaran & kontrak digital  
- Integrasi AI sorting leads *(roadmap)*  

### 3. Project Management
- Workflow digital: dari desain ke konstruksi  
- Manajemen revisi desain  
- Tracking progress proyek real-time  
- Komunikasi tim lapangan ↔ kantor pusat  
- Penjadwalan otomatis  

### 4. Inventory & Logistik
- Pencatatan stok material & logistik proyek  
- Pemantauan pemakaian material harian  
- Prediksi kebutuhan material  
- Integrasi pembelian & distribusi  

### 5. Keuangan & Akuntansi
- Pencatatan biaya proyek  
- Laporan pengeluaran & pemasukan real-time  
- Estimasi biaya otomatis  
- Integrasi metode pembayaran digital  

### 6. Keamanan & Infrastruktur
- Enkripsi data enterprise-grade  
- Backup otomatis ke cloud  
- Kontrol akses bertingkat  
- Sistem recovery data bencana  
- Monitoring keamanan 24/7  

---

## 🚀 Fitur Tambahan (Jika Diaktifkan)
- UI responsif (desktop & mobile)  
- Mode offline + sinkronisasi saat online  
- Multi-bahasa (internasionalisasi)  
- Dukungan PWA *(jika diaktifkan)*  
- Skalabilitas cloud-ready (Laravel Vapor kompatibel)  

---

## ⚙️ Instalasi (Local Development)

### 1. Clone Repository
```bash
git clone https://github.com/Samsulmaarif01/RHI_Build.git
cd rhi-build
```

### 2. Install Dependensi Laravel
```bash
composer install
npm install && npm run build
```

### 3. Konfigurasi Environment
```bash
cp .env.example .env
php artisan key:generate
```

Edit file `.env` seperti berikut:
```
APP_NAME="RHI Build"
APP_URL=http://localhost:8000

DB_DATABASE=rhi_build
DB_USERNAME=root
DB_PASSWORD=
```

### 4. Jalankan Migrasi & Seeder
```bash
php artisan migrate --seed
```

### 5. Jalankan Server
```bash
php artisan serve
```

---

## 🔐 Login Admin (Filament)
- **URL:** `/admin`  
- **Email:** `admin@rhibuild.test`  
- **Password:** `password`  

> 💡 *Data admin bisa diubah lewat seed atau perintah artisan.*

---
