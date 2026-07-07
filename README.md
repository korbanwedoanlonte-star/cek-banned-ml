# 🎮 Cek Banned Mobile Legends

Website untuk cek status ban akun Mobile Legends dengan akurasi 80-90%.

## 🚀 Quick Start

### 1. Buka Website
Akses di: https://korbanwedoanlonte-star.github.io/cek-banned-ml/

### 2. Setup API Key (PENTING!)
Website ini membutuhkan RapidAPI Key untuk berfungsi.

**Langkah-langkah:**

1. Buka https://rapidapi.com
2. Sign up (pakai Google/GitHub)
3. Cari API: **"Mobile Legends User Info Lookup"**
4. Klik **"Subscribe to Test"** (free tier)
5. Pergi ke **Dashboard** → Copy **X-RapidAPI-Key**
6. Edit `index.html` (baris ~280):
   ```javascript
   const RAPIDAPI_KEY = 'PASTE_YOUR_KEY_HERE';
   ```
7. Save dan refresh browser

### 3. Cara Menggunakan

1. Masukkan **Player ID** (cari di profile MLBB)
2. Pilih **Server/Zone** lo
3. Klik **"CEK SEKARANG"**
4. Tunggu hasil ✅ atau 🚫

## 📊 Format Respons

**Jika AMAN (Status = 0):**
```
✅ AMAN
Nickname: YourNick
Rank: Legend V
Hero Owned: 45
Win Rate: 52%
```

**Jika BANNED (Status = 1):**
```
🚫 BANNED 30 HARI
Alasan Ban: Toxic Behavior
Durasi: 30 hari
```

## 🌍 Server/Zone List

- 10001 - Indonesia
- 10002 - Philippines
- 10003 - Thailand
- 10004 - Malaysia
- 10005 - Vietnam
- 10012 - Global
- 10006 - Singapore
- 10007 - Myanmar
- 10008 - Brunei

## ⚠️ Disclaimer

- **Akurasi tergantung API** (80-90%)
- Ban chat 1-3 hari mungkin **tidak terdeteksi**
- Hasil hanya untuk **referensi**, bukan sumber resmi
- Gunakan dengan **tanggung jawab sendiri**

## 🛠️ Tech Stack

- HTML5
- CSS3 (Dark Theme MLBB)
- JavaScript (Vanilla)
- RapidAPI (Mobile Legends API)
- CORS Proxy (cors.sh)

## 📱 Responsive Design

✅ Mobile-friendly  
✅ Desktop-friendly  
✅ Tablet-friendly  

## 🔐 Privacy

- Tidak ada data yang disimpan
- Semua request langsung ke RapidAPI
- CORS Proxy hanya sebagai bridge

## 🐛 Troubleshooting

**Q: "API Key tidak valid"**  
A: Pastikan API Key sudah di-copy dengan benar dan belum expired.

**Q: "Rate limit tercapai"**  
A: Tunggu beberapa menit, API memiliki batas request.

**Q: "Player ID tidak ditemukan"**  
A: Cek ulang Player ID dan zone/server-nya.

**Q: "Response dari API tidak valid"**  
A: CORS Proxy atau API server sedang error. Coba lagi.

## 📞 Support

Untuk pertanyaan atau laporan bug, silakan buat issue di GitHub.

---

**Made with ❤️ for MLBB Community**
