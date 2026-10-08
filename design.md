# Mediara — Design System & Brand Guidelines

Dokumen ini merupakan panduan identitas visual, token warna, dan pedoman desain untuk **Mediara** (berdasarkan *Concept 2: Futuristic • Innovative • Visionary* dari `mediara colors.png`).

---

## 1. Filosofi & Esensi Brand

* **Brand Statement:** *Technology for Smarter Business*
* **Brand Personality:**
  * **Futuristic:** Mengedepankan teknologi mutakhir, antarmuka modern, dan estetika generasi baru.
  * **Innovative:** Solutif, efisien, dan dirancang untuk akselerasi pertumbuhan bisnis.
  * **Visionary:** Estetika yang profesional, berwawasan ke depan, dan berstandar global.
* **Gaya Visual Utama:**
  * Deep Midnight Canvas (latar gelap kosmik `#020A21`).
  * Neon Ribbon Gradients & Smooth Glows (efek pendaran cahaya dari kombinasi Biru, Cyan, dan Ungu).
  * Glassmorphism & High-contrast typography.

---

## 2. Palet Warna (Mediara Palette Tokens)

Warna resmi Mediara didefinisikan ke dalam 4 nilai inti:

| Token / Variabel | Nilai Hex | Peran & Deskripsi |
| :--- | :--- | :--- |
| `--mediara-dark` | `#020A21` | **Deep Space Navy** — Background utama seluruh halaman web, menciptakan kanvas gelap yang elegan, imersif, dan futuristik. |
| `--mediara-blue` | `#2A6EFD` | **Electric Royal Blue** — Warna korporat modern, memberikan impresi terpercaya, teknologi tinggi, dan kestabilan. |
| `--mediara-cyan` | `#22D3EE` | **Vibrant Neon Cyan** — Warna aksen pendaran cahaya, highlight interaktif, badges, dan gradien masa depan. |
| `--mediara-purple` | `#7B4FFC` | **Radiant Electric Violet** — Warna sekunder gradien ribbon, aksen visual kreatif, dan sentuhan inovasi. |

---

## 3. Sistem Variabel CSS (`:root`)

Semua warna disimpan dalam bentuk CSS variables (`var(...)`) sehingga Anda dapat dengan mudah mengganti warna **Primary**, **Secondary**, maupun **Accent** kapan saja hanya dengan mengubah 1 baris referensi.

```css
:root {
  /* ============================================================
     1. MEDIARA BASE PALETTE
     ============================================================ */
  --mediara-dark: #020A21;       /* Background Gelap Utama */
  --mediara-blue: #2A6EFD;       /* Royal Blue */
  --mediara-cyan: #22D3EE;       /* Neon Cyan */
  --mediara-purple: #7B4FFC;     /* Electric Purple / Violet */

  /* ============================================================
     2. DYNAMIC THEME TOKENS
     Ubah referensi di bawah untuk mengganti peran warna web:
     ============================================================ */
  /* PILIHAN WARNA PRIMARY:
     - Opsi Biru   : var(--mediara-blue)   (Rekomendasi Utama)
     - Opsi Cyan   : var(--mediara-cyan)   (Lebih Cerah & Kontras Tinggi)
     - Opsi Ungu   : var(--mediara-purple) (Lebih Eksentrik & Kreatif)
  */
  --primary: var(--mediara-blue);
  --secondary: var(--mediara-purple);
  --accent: var(--mediara-cyan);

  /* Surface & Canvas Tokens */
  --bodybg: var(--mediara-dark);
  --bodytext: #8E9DB8;
  --card: #06102D;
  --card-light: #0D1A40;
  --card-border: rgba(42, 110, 253, 0.2);
  --title: #FFFFFF;
}
```

### Cara Mengganti Warna Primary:
* **Ingin Primary berwarna Biru:**
  ```css
  --primary: var(--mediara-blue);
  ```
* **Ingin Primary berwarna Cyan:**
  ```css
  --primary: var(--mediara-cyan);
  ```
* **Ingin Primary berwarna Ungu:**
  ```css
  --primary: var(--mediara-purple);
  ```

---

## 4. Gradien Resmi (Official Gradients)

Kombinasi gradien yang terinspirasi dari ribbon logo 3D:

* **Signature Hero Gradient:**
  ```css
  background: linear-gradient(135deg, #7B4FFC 0%, #2A6EFD 50%, #22D3EE 100%);
  ```
* **Glow & Border Gradient:**
  ```css
  background: linear-gradient(90deg, #2A6EFD 0%, #22D3EE 100%);
  ```
* **Card Ambient Glow:**
  ```css
  box-shadow: 0 0 35px rgba(42, 110, 253, 0.15);
  ```

---

## 5. Layanan & Visual Icons

Berdasarkan struktur pada concept visual:
1. **Website Development** — Arsitektur web modern, kustom, dan responsif.
2. **Online Menu** — Katalog digital & menu interaktif untuk F&B/ritel.
3. **Marketplace & E-Commerce** — Transaksi terintegrasi, pembayaran instan, dan sistem POS.
4. **Google Rating** — Optimasi reputasi digital, SEO lokal, dan social proof.
5. **AI Solutions** — Otomasi cerdas, rekomendasi sistem, dan integrasi workflow berbasis AI.

---

## 6. Aset Identitas Brand

* **Brand Mark Logo (`src/assets/images/logo.png`):**
  * Logo Ribbon "M" 3D dengan alur gradien dari ungu (`#7B4FFC`) memutar ke biru (`#2A6EFD`) hingga cyan (`#22D3EE`).
  * Digunakan pada Header, Mobile Sidenav, Footer, dan Favicon.
* **Banner / Open Graph Share Image (`src/assets/images/banner.jpeg`):**
  * Rasio aspek 16:9 berlatar gelap yang memuat Ribbon Logo dan tipografi "mediara SERVICE".
  * Digunakan untuk meta tag preview media sosial (`og:image` dan `twitter:image`).
