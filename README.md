# 🔒 Mining Rate Calculator (Encrypted)

Dashboard kalkulator rate & TCO penambangan — **terenkripsi (AES-256)**.

## Cara membuka
1. Buka link GitHub Pages repo ini.
2. Masukkan **password** (diberikan oleh pemilik).
3. Konten ter-dekripsi di browser Anda. Tidak ada data yang dikirim ke server.

## Keamanan
- Isi file `index.html` dienkripsi **AES-256-GCM** dengan key turunan **PBKDF2-SHA256 (250.000 iterasi)**.
- Tanpa password yang benar, konten tidak dapat dibaca.
- Gunakan password yang kuat & jangan bagikan ke pihak yang tidak berhak.

## Catatan
- Aplikasi berjalan sepenuhnya di browser (client-side). Perubahan data tersimpan di `localStorage` perangkat masing-masing.
- Untuk update konten: pemilik meng-enkripsi ulang `index.html` lalu push kembali.
