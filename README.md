# TPQ Baiturrahman — Website

Landing page TPQ Baiturrahman, Masjid Baiturrahman, Setu, Cipayung, Jakarta Timur.

> Menjaga kefitrahan anak dengan pendidikan Qur'an dan Sunnah.

## Isi halaman

- **Beranda**: ilustrasi santri kecil membaca Qur'an di depan lengkung mihrab, dikelilingi objek tanah liat yang melayang; panel program dan info singkat
- **Tentang**: visi dan nilai TPQ
- **Layanan**: Pendidikan al-Qur'an, Pembinaan Akhlak, Kegiatan Kreativitas Islam (tiap kartu ada tombol tanya via WhatsApp)
- **Pojok anak**: flashcard huruf hijaiyah 5 kartu, mode pilihan ganda atau tebak sendiri
- **Testimoni** orang tua santri (carousel)
- **Kolase** ilustrasi bersama slogan TPQ
- **Kontak**: langsung ke WhatsApp +62 812-1304-1786, alamat, dan jam belajar

## Versi

- **Versi 2** (branch `main`): gaya hangat/cozy — krem pasir, cokelat kopi, terakota; logo masjid di atas Al-Qur'an.
- **Versi 1** (branch `v1`): tema masjid saat senja dengan nuansa merah.

## Tech stack

- HTML + CSS modern (satu file, tanpa proses build)
- [GSAP](https://gsap.com/) + ScrollTrigger (dari CDN) untuk animasi
- Font: Plus Jakarta Sans, Amiri (Google Fonts)

Halaman tetap tampil normal walaupun GSAP gagal dimuat, dan animasi otomatis dimatikan untuk pengunjung yang memilih *reduce motion*.

## Menjalankan / deploy

Cukup buka `index.html` di browser.

Untuk online gratis:

- **GitHub Pages**: Settings → Pages → Source: *Deploy from a branch* → branch `main`, folder `/ (root)` → Save.
- **Netlify / Vercel**: import repo ini, tanpa build command, publish directory `/`.

## Mengubah konten

Semua teks ada di `index.html`. Nomor WhatsApp ada di tautan `https://wa.me/6281213041786?...` (cari `wa.me`).
