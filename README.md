# HOKTIVA POS

Aplikasi kasir dan manajemen usaha UMKM berbasis web/PWA.

Source POS diperbarui dari file tahap 6 PDF/WhatsApp yang diunggah pengguna; identitas toko tetap dikelola melalui Profil Toko.

## Deploy ke GitHub Pages
1. Unggah seluruh isi folder ini ke branch `main` pada repository.
2. Aktifkan GitHub Pages dari Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
3. Buka URL GitHub Pages melalui HTTPS.
4. Setelah deployment, periksa manifest dan service worker melalui Chrome DevTools → Application.
5. Gunakan https://www.pwabuilder.com/ untuk pemeriksaan PWA dan pembuatan paket Android.

## Catatan
- Data usaha disimpan menggunakan `localStorage` pada origin/domain browser yang sama.
- Jangan mengganti domain atau menghapus data browser sebelum melakukan backup.
- Service worker menyimpan app shell dan aset lokal untuk membantu membuka aplikasi saat offline.
- Beberapa library eksternal pada aplikasi masih memerlukan internet; mode offline penuh belum dijamin.
- Logika transaksi dan nama key `localStorage` pada aplikasi tidak diubah dalam pembaruan identitas/PWA ini.
