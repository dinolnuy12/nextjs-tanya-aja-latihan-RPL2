# TanyaAja! — proyek latihan

Proyek ini dibangun bertahap mengikuti Handbook Hari 03 dan Hari 04. Setiap siswa bekerja di **fork** miliknya sendiri.

## Mulai (siswa baru)
1. Buka `https://github.com/AdlinMH/nextjs-tanya-aja-latihan`, klik **Fork**, pilih akunmu sebagai **Owner**, lalu **Create fork**.
2. Clone fork milikmu (ganti `NAMA-AKUN` dengan nama akun GitHub-mu), lalu pasang dependensi dan jalankan:

```bash
git clone https://github.com/NAMA-AKUN/nextjs-tanya-aja-latihan.git tanyaaja
```

```bash
npm install
```

```bash
npm run dev
```

Buka http://localhost:3000. Starter berjalan tanpa `.env.local`.

## Isi proyek

| Bagian | Keterangan |
|---|---|
| `app/page.js` dan komponen buatanmu | Dikerjakan siswa: Hari 03 (tampilan) dan Hari 04 (menghubungkan fungsi). |
| `components/ui/` | Komponen shadcn/ui. |
| `app/actions.js`, `lib/` | **Kode pendukung yang sudah disediakan**: Server Actions, validasi, konfigurasi, koneksi Supabase, sesi login, batas percobaan. Baru dipakai di Hari 04. |
| `components/tombol-login.jsx`, `mode-pemilik.jsx`, `panel-pemilik.jsx`, `kartu-pemilik.jsx`, `status-halaman.jsx` | Komponen login dan pemilik yang sudah disediakan untuk Hari 04. |
| `supabase/setup.sql` | Pembuat tabel. Sudah dijalankan pemateri di database latihan; dipakai hanya untuk bonus Supabase pribadi. |
| `tests/` | `npm test` menguji aturan validasi tanpa database. |
| `.env.example` | Contoh konfigurasi Hari 04 tanpa rahasia. Salin menjadi `.env.local`. |

`.env.local` berisi rahasia dan tidak ikut ke GitHub (lihat `.gitignore`).

## Memperbarui fork yang sudah ada

Fork tidak otomatis mendapat perubahan dari repo induk.

1. Commit progresmu dulu. Jangan memasukkan `.env.local`.
2. Di GitHub, buka fork milikmu, pilih branch `main`, klik **Sync fork** → **Update branch**.
3. Di terminal proyek, pastikan `git remote -v` menunjuk fork milikmu, lalu jalankan:

```bash
git checkout main
```

```bash
git pull --no-rebase --no-edit origin main
```

Jika muncul konflik, atau GitHub meminta pull request, berhenti dan minta bantuan pemateri. Jangan memakai opsi yang membuang commit.
