# TPQ Baiturrahman Website

Landing page TPQ Baiturrahman, Masjid Baiturrahman, Setu, Cipayung, Jakarta Timur.

Website: https://www.tpqbaiturrahman.com/

> Menjaga kefitrahan anak dengan pendidikan Qur'an dan Sunnah.

## Isi halaman

- **Beranda**: ilustrasi masjid saat senja dengan animasi (bintang, lampion, santri kecil berjalan ke masjid)
- **Tentang**: visi dan nilai TPQ
- **Layanan**: Pendidikan al-Qur'an, Pembinaan Akhlak, Kegiatan Kreativitas Islam (tiap kartu ada tombol tanya via WhatsApp)
- **Flashcard huruf hijaiyah**: 5 kartu untuk anak, mode pilihan ganda atau tebak sendiri
- **Jadwal sholat** hari ini untuk DKI Jakarta (Cipayung, Jakarta Timur): dihitung otomatis dengan kriteria Kemenag RI, lengkap dengan hitung mundur ke waktu sholat berikutnya
- **Testimoni** orang tua santri
- **Kontak**: langsung ke WhatsApp +62 812-1304-1786 dan alamat

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

## SEO dan performa

- Judul, deskripsi, canonical, Open Graph dan Twitter card ada di `<head>` `index.html`; gambar pratinjau link: `assets/og-image.jpg` (1200x630).
- Data terstruktur (JSON-LD) untuk Google: EducationalOrganization, WebSite, dan tiga Course (gratis).
- `robots.txt`, `sitemap.xml`, dan `site.webmanifest` di root. Perbarui `<lastmod>` di sitemap kalau isi berubah banyak.
- Foto program memakai WebP (480/800 px) dengan cadangan JPG; logo di menu memakai versi 96 px.
- `vercel.json` mengatur cache 7 hari untuk folder `assets/` dan beberapa header keamanan.
- Kalau domain berubah, ganti semua `https://www.tpqbaiturrahman.com/` di `index.html`, `robots.txt`, dan `sitemap.xml`.

## Mengubah konten

Semua teks ada di `index.html`. Logo dan favicon ada di folder `assets/` (plus `favicon.ico` di root); ganti file-file itu untuk memperbarui logo. Nomor WhatsApp ada di tautan `https://wa.me/6281213041786?...` (cari `wa.me`).
