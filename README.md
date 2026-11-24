# TPQ Baiturrahman — Website

Landing page TPQ Baiturrahman, Masjid Baiturrahman, Setu, Cipayung, Jakarta Timur.

> Menjaga kefitrahan anak dengan pendidikan Qur'an dan Sunnah.

## Isi halaman

- **Beranda**: ilustrasi masjid saat senja dengan animasi (bintang, lampion, santri kecil berjalan ke masjid)
- **Tentang**: visi dan nilai TPQ
- **Layanan**: Pendidikan al-Qur'an, Pembinaan Akhlak, Kegiatan Kreativitas Islam (tiap kartu ada tombol tanya via WhatsApp)
- **Flashcard huruf hijaiyah**: kuis singkat 5 kartu untuk anak
- **Testimoni** orang tua santri
- **Kontak**: langsung ke WhatsApp +62 812-1304-1786, alamat, dan jam belajar

## Tech stack

- HTML + CSS modern (satu file, tanpa proses build)
- [GSAP](https://gsap.com/) + ScrollTrigger (dari CDN) untuk animasi
- Font: Fredoka, Nunito, Amiri (Google Fonts)

Halaman tetap tampil normal walaupun GSAP gagal dimuat, dan animasi otomatis dimatikan untuk pengunjung yang memilih *reduce motion*.

## Menjalankan / deploy

Cukup buka `index.html` di browser.

Untuk online gratis:

- **GitHub Pages**: Settings → Pages → Source: *Deploy from a branch* → branch `main`, folder `/ (root)` → Save.
- **Netlify / Vercel**: import repo ini, tanpa build command, publish directory `/`.

## Mengubah konten

Semua teks ada di `index.html`. Nomor WhatsApp ada di tautan `https://wa.me/6281213041786?...` (cari `wa.me`).
