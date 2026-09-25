# ReadME — Website Landing Page "Lestari"

> Landing page **satu halaman (single page)** bertema **konservasi lingkungan** untuk audiens umum.
> Dibuat sebagai pemenuhan **Penugasan Week-1 Project-Dev**.

---

## Ringkasan Website

**Lestari** adalah gerakan konservasi lingkungan yang mengajak masyarakat bertindak lewat aksi nyata: menanam pohon, membersihkan pantai & sungai, serta edukasi lingkungan ke sekolah. Halaman ini dibuat dengan navigasi _scroll_ ke tiap section dalam satu halaman.

### Penjelasan dari Header sampai Footer

#### 1. Navbar
- **Kiri:** judul website **"Lestari"** beserta ikon daun sebagai logo.
- **Tengah/Kanan:** tepat **2 link navigasi** — *Mengapa Ini Penting* (`#mengapa`) dan *Program* (`#program`).
- **Tombol CTA menonjol:** *"Dukung Sekarang"* (warna emerald, rounded penuh).
- Navbar bersifat `fixed` + `backdrop-blur` sehingga tetap terlihat saat di-scroll. Di layar kecil muncul tombol hamburger untuk membuka menu (dikontrol JavaScript).

#### 2. Halaman Utama (Hero)
- **Headline:** *"Selamatkan Alam, Mulai dari Langkah Kecil"*, diikuti sub-judul singkat (2 kalimat) yang mengajak peduli lingkungan.
- **Gambar pendukung wajib:** foto hutan dari Unsplash (bebas royalti), lengkap dengan atribut `alt` dan keterangan sumber pada komentar.
- **Tombol aksi:** *"Lihat Program Kami"* menuju section `#program`.
- Bonus: badge, tiga angka statistik singkat, dan kartu kecil penegas pesan.

#### 3. Section 1 — Mengapa Ini Penting (`#mengapa`)
- Berisi judul + paragraf deskripsi penjelas tentang urgensinya (sampah plastik, deforestasi, perubahan iklim).
- Tiga kartu masalah dalam grid, masing-masing dengan teks penjelas (bukan hanya ikon).
- Blok tambahan **tidak simetris**: gambar di kiri, poin-poin manfaat konservasi di kanan.

#### 4. Section 2 — Program & Kegiatan (`#program`)
- Berisi judul + paragraf deskripsi penjelas.
- Grid **3 program** (card): *Tanam 1.000 Pohon*, *Bersih-Bersih Pantai & Sungai*, *Edukasi Lingkungan Sekolah*.
- Latar hijau tua (`emerald-950`) sebagai kontras dari section sebelumnya.
- Kotak ajakan **CTA** menuju `#kontak` (footer).

#### 5. Footer
- **Nama judul website:** Lestari.
- **Visi & Misi** singkat (opsional, diisi sesuai ketentuan).
- **3 media sosial** dari pilihan 4: Instagram, YouTube, dan TikTok.
- Baris hak cipta.

---

## Teknologi yang Digunakan

| Teknologi | Peran |
|---|---|
| **HTML5** | Struktur halaman (`index.html`) |
| **CSS3** | Styling tambahan (`style.css`) |
| **Tailwind CSS (CDN)** | Utility class untuk spacing, warna, & tipografi |

- `style.css` dihubungkan lewat `<link rel="stylesheet" href="style.css">` pada `<head>` `index.html`.
- Konfigurasi Tailwind (font custom) dilakukan lewat blok `tailwind.config` di `<head>`.
- Font: **Plus Jakarta Sans** (Google Fonts) — dipasang via link.
- Sedikit JavaScript (vanilla) untuk menu mobile dan animasi muncul saat scroll.

## Palet Warna (5 warna konsisten)

| Warna | Tailwind | Fungsi |
|---|---|---|
| Hijau emerald tua | `emerald-950/700/600` | Latar section program, CTA, aksen utama |
| Hijau lime | `lime-300/400` | Aksen, badge, tombol kontras |
| Krem netral | `stone-50` | Latar halaman |
| Abu netral | `stone-200/500/700/900` | Border, teks sekunder, footer |

## Hierarki Tipografi

| Elemen | Ukuran |
|---|---|
| Judul utama hero (`h1`) | `text-4xl` → `sm:text-5xl` |
| Judul section (`h2`) | `text-3xl` → `sm:text-4xl` |
| Sub-judul kartu (`h3`) | `text-xl` / `text-2xl` |
| Paragraf | `text-base` / `text-sm` |

## Sumber Gambar (Bebas Royalti)

| Gambar | Sumber | Komentar |
|---|---|---|
| Hero (hutan) | Unsplash — `https://unsplash.com/photos/1441974231531-c6227db76b6e` | ✓ |
| Section Mengapa (pegunungan) | Unsplash — `https://unsplash.com/photos/1470071459604-3b5ec3a7fe05` | ✓ |

Kredit sumber dicantumkan juga pada komentar pada file `index.html`.

## Struktur File Project

```
web/
├── index.html          # Struktur + konten halaman (Tailwind CDN)
├── style.css           # Styling tambahan (animasi, scrollbar, font)
├── ReadME.md           # Penjelasan website ini
└── PengerjaanKelompok.md  # Laporan & pembagian kerja kelompok
```

## AI yang Digunakan

Tugas ini dibantu oleh **opencode** (model `big-pickle`) sebagai asisten pemrograman selama proses pembuatan struktur, konten, dan gaya halaman. Seluruh teks ditulis sendiri dan tidak menyalin dari website lain.