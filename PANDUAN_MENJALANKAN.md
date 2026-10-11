# 🚀 Panduan Menjalankan Website (JAWAA)

Panduan langkah demi langkah untuk menjalankan project React + Vite ini di komputer lokal Anda.

> 🌐 **Demo Online (Vercel):**  
> Website ini sudah aktif dan dapat diakses langsung di: **[https://kage-kyoto-nightwalk-web-iota.vercel.app/](https://kage-kyoto-nightwalk-web-iota.vercel.app/)**

---

## 📌 1. Prasyarat Sistem

Pastikan Anda sudah menginstal **Node.js** dan **npm**.

Cek melalui terminal:
```bash
node -v
npm -v
```
*(Direkomendasikan Node.js versi 18 atau lebih baru).*

---

## 🛠️ 2. Langkah-Langkah Menjalankan

### Langkah 1: Buka Terminal dan Masuk ke Direktori Project
```bash
cd /home/ifhalfaizi/Downloads/JAWAA
```

### Langkah 2: Install Dependensi
Jalankan perintah ini jika baru pertama kali atau jika belum ada folder `node_modules`:
```bash
npm install
```

### Langkah 3: Jalankan Server Pengembangan (Dev Server)
```bash
npm run dev
```

Jika berhasil, terminal akan menampilkan output seperti ini:
```text
  VITE v8.2.2  ready in ... ms

  ➜  Local:   http://localhost:5175/
  ➜  Network: use --host to expose
```

### Langkah 4: Buka Website di Browser
Buka browser favorit Anda (Chrome, Firefox, Edge, dll) dan akses:
👉 **[http://localhost:5175/](http://localhost:5175/)**

---

## ⏹️ 3. Cara Menghentikan Server

Untuk mematikan website yang sedang berjalan di terminal, tekan:
```text
Ctrl + C
```

---

## ⚠️ 4. Solusi Error Umum

### Kasus: `Error: Port 5175 is already in use`

**Penyebab:**
Port `5175` sedang dipakai oleh proses lain (misalnya server Vite sebelumnya masih berjalan di background). Konfigurasi `strictPort: true` di `vite.config.ts` mewajibkan penggunaan port tersebut dan tidak otomatis pindah ke port lain.

**Solusi 1 — Matikan proses yang memakai port 5175:**
```bash
# Cari dan hentikan proses di port 5175
npx kill-port 5175

# Atau menggunakan perintah Linux:
lsof -ti:5175 | xargs kill -9
```
Setelah itu jalankan kembali:
```bash
npm run dev
```

**Solusi 2 — Jalankan di Port Lain:**
Anda dapat menentukan port lain melalui variabel environment tanpa mengubah konfigurasi:
```bash
PORT=3000 npm run dev
# Website akan berjalan di http://localhost:3000/
```

---

## 📦 5. Perintah Tambahan

| Perintah | Fungsi |
| :--- | :--- |
| `npm run dev` | Menjalankan server lokal untuk pengembangan (dengan Hot Module Replacement) |
| `npm run build` | Melakukan build file produksi ke folder `dist/` |
| `npm run preview` | Menjalankan preview dari hasil build produksi |
| `npm run lint` | Menjalankan linter oxlint untuk mengecek kualitas kode |
