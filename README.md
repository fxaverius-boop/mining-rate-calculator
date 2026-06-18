# ⛏️ Mining Rate Calculator (Team Cloud)

Dashboard kalkulator rate & TCO penambangan — data **tim bersama** tersinkron via Supabase.

## Cara membuka
1. Buka link GitHub Pages repo ini.
2. **Login** dengan akun tim Anda (email + password). Belum punya akun? Klik **Daftar akun baru**, konfirmasi email, lalu login.
3. Hanya email yang ada di **allowlist** (diatur admin) yang dapat melihat & mengedit data tim.

## Cara kerja
- Aplikasi statis (GitHub Pages) + **Supabase** (Auth + Postgres).
- Data (project, katalog, history) tersimpan di cloud dan dibagikan ke seluruh anggota tim.
- Perubahan tersimpan otomatis. Tombol **🔄** (badge kanan-bawah) menarik perubahan terbaru rekan tim.
- Akses dijaga login + allowlist email + Row Level Security. anon key bersifat publik (aman by design).

## Untuk admin
- Tambah anggota: masukkan email mereka ke tabel `allowed_members` (Supabase Dashboard).
- Build & deploy ulang: `node build_cloud.js` lalu commit `index.html` (hanya file ini + README yang masuk repo publik).
