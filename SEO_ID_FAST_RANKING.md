# Template SEO Google Indonesia (Fokus Kecepatan + Ranking Cepat)

> Tujuan: meningkatkan peluang ranking cepat di Google Search Indonesia dengan halaman yang **cepat dibuka**, relevan lokal Indonesia, dan mudah dipahami crawler.

## 1) Prinsip utama untuk "cepat naik"

1. **Intent-first**: satu halaman target satu intent (contoh: `jadwal bola hari ini`, `live score liga inggris`, `prediksi skor malam ini`).
2. **Freshness harian**: update konten dengan timestamp jelas (`WIB`) dan perubahan nyata.
3. **Internal link cluster**: hubungkan halaman kategori ↔ artikel ↔ halaman live agar authority mengalir.
4. **Speed absolut**: Core Web Vitals bagus di jaringan mobile Indonesia.
5. **Trust signal**: ada identitas editorial, sumber data pertandingan, dan halaman kebijakan.

## 2) Perbaikan kritis dari template Anda

- Jangan gunakan **dua dokumen HTML duplikat** pada satu output (mengandung `<html>... </html>` dua kali).
- Hindari data pertandingan statis yang bisa dianggap misleading; pakai data dinamis + jam WIB aktual.
- Kurangi ketergantungan keyword di meta keywords (pengaruh sangat kecil); fokus title, H1, dan body intent.
- Tambahkan bahasa/region signal Indonesia yang kuat.

## 3) Head SEO yang direkomendasikan (Indonesia)

Gunakan komponen ini di `<head>`:

- `meta name="robots" content="index,follow,max-image-preview:large,max-snippet:-1,max-video-preview:-1"`
- `meta property="og:locale" content="id_ID"`
- `link rel="alternate" hreflang="id-ID" href="https://domainanda.com/"`
- `link rel="alternate" hreflang="x-default" href="https://domainanda.com/"`
- `meta name="theme-color" content="#0f172a"`
- `preconnect` ke domain CDN/font penting.

## 4) Structured data (wajib)

Tambahkan JSON-LD minimal:

- `WebSite` + `SearchAction`
- `Organization`
- `BreadcrumbList`
- `NewsArticle` (untuk artikel)
- `SportsEvent` (untuk jadwal/live bila datanya valid)

## 5) Optimasi kecepatan untuk pasar Indonesia

1. **TTFB rendah**: gunakan edge caching di region Asia Tenggara.
2. **Brotli/Gzip aktif** untuk HTML, CSS, JS.
3. **Critical CSS** tetap inline, sisanya minify.
4. **Image**: WebP/AVIF, ukuran tetap (`width/height`) + `loading="lazy"`.
5. **Font**: sistem font dulu (sudah bagus), hindari webfont berat.
6. **JS minimal**: hindari library besar jika tidak wajib.
7. **Cache-Control** ketat untuk asset statis (30 hari+ dengan versioning).

## 6) Strategi konten cepat ranking (khusus ID)

- Buat halaman pilar:
  - `/jadwal-bola-hari-ini/`
  - `/live-score/`
  - `/prediksi-bola/`
  - `/hasil-pertandingan/`
- Terbitkan update singkat tapi rutin (5–20 konten/hari) dengan format konsisten.
- Pakai frasa lokal natural Indonesia:
  - "jam berapa", "siaran langsung", "link nonton", "hari ini WIB".
- Tambahkan FAQ di setiap halaman kategori untuk menangkap long-tail.

## 7) Checklist teknis cepat (harian)

- [ ] Sitemap XML auto-update (artikel + kategori + live).
- [ ] Robots.txt benar, tidak blokir CSS/JS penting.
- [ ] Canonical self-referencing di setiap URL unik.
- [ ] Tidak ada halaman duplikat title/H1.
- [ ] Semua halaman penting bisa dicapai <= 3 klik dari homepage.
- [ ] Cek performa mobile (LCP, INP, CLS).

## 8) Template snippet yang lebih aman (head minimal)

```html
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>{$toptitle}</title>
  <meta name="description" content="{$description}" />
  <link rel="canonical" href="{$web_url}" />
  <meta name="robots" content="index,follow,max-image-preview:large,max-snippet:-1,max-video-preview:-1" />
  <meta property="og:locale" content="id_ID" />
  <link rel="alternate" hreflang="id-ID" href="{$web_url}" />
  <link rel="alternate" hreflang="x-default" href="{$web_url}" />
</head>
```

## 9) Catatan penting soal "ranking cepat"

Tidak ada trik yang dijamin instan. Yang paling cepat biasanya kombinasi:

- halaman sangat cepat,
- update sangat rutin,
- cakupan intent yang tepat,
- internal linking rapih,
- data pertandingan valid & terbaru.

