# Website Cinta - Spesifikasi

## 1. Project Overview

- **Nama Project**: Website Cinta Personal
- **Tipe**: Single-page website interaktif untuk pacar
- **Fungsi**: Website romantis dengan desain Pinterest-style, menampilkan foto, pesan cinta, dan elemen interaktif
- **Target User**: Pacar пользователя

---

## 2. UI/UX Specification

### Layout Structure

- **Header**: Fixed navigation dengan logo/name, navigasi smooth scroll
- **Hero Section**: Full-screen dengan animated text intro dan floating hearts
- **Gallery Section**: Pinterest-style masonry grid untuk foto-foto
- **Love Letter Section**: Kartu pesan cinta yang bisa dibalik
- **Timeline Section**: Momen special bersama (interactive timeline)
- **Footer**: Pesan最后的 dan kontrol musik (opsional)

### Responsive Breakpoints
- Mobile: < 768px (1 column)
- Tablet: 768px - 1024px (2 columns)
- Desktop: > 1024px (3-4 columns)

### Visual Design

**Color Palette**:
- Primary Green: `#2D5A27` (Deep forest green)
- Secondary Green: `#4A7C45` (Leaf green)
- Accent Green: `#7CB342` (Light green)
- Primary Pink: `#E91E63` (Hot pink)
- Soft Pink: `#F48FB1` (Light pink)
- Blush Pink: `#FCE4EC` (Very light pink)
- Background: `#FFF8F0` (Warm cream)
- Text Dark: `#2C1810` (Dark brown)
- White: `#FFFFFF`

**Typography**:
- Headings: 'Playfair Display', serif (elegant, romantic)
- Body: 'Quicksand', sans-serif (modern, readable)
- Accent Text: ' Dancing Script', cursive (for love notes)
- Font sizes: 
  - H1: 3.5rem
  - H2: 2.5rem
  - H3: 1.8rem
  - Body: 1.1rem

**Spacing**:
- Section padding: 80px vertical
- Card padding: 24px
- Grid gap: 20px

**Visual Effects**:
- Glassmorphism cards (blur background)
- Gradient overlays pada foto
- Floating animation untuk elemen decorative
- Particle effects (hearts floating)
- Smooth hover transitions (0.3s ease)
- Box shadows yang soft dan romantic

### Components

1. **Navigation Bar**
   - Translucent dengan blur
   - Logo/name pacar
   - Smooth scroll links
   - Hover: underline animation

2. **Hero Section**
   - Full viewport height
   - Animated title dengan typed effect
   - Subtitle dengan fade in
   - Floating hearts particles
   - Scroll down indicator

3. **Gallery Cards** (Pinterest-style)
   - Variable heights (masonry)
   - Image dengan gradient overlay
   - Hover: zoom effect + show caption
   - Click: lightbox modal
   - Heart icon overlay

4. **Love Letter Cards**
   - Flip animation (3D transform)
   - Front: tanggal/judul
   - Back: pesan cinta
   - Hover: lift effect

5. **Timeline Items**
   - Vertical line
   - Date markers
   - Photo + description
   - Scroll-triggered fade in

6. **Interactive Elements**
   - Clickable hearts (like/save)
   - Drag & drop photo (if possible)
   - Quiz tentang kita
   - Animated reactions

---

## 3. Functionality Specification

### Core Features

1. **Photo Gallery**
   - Masonry layout dengan placeholder images
   - Lightbox modal saat klik
   - Caption dan likes
   - Hover effects

2. **Love Letters**
   - Flipable cards
   -_multiple pesan special
   - Animated reveal

3. **Interactive Elements**
   - Floating hearts (canvas/particles)
   - Click untuk buat heart baru
   - Smooth animations

4. **Personalization**
   - Ganti nama pacar di kode
   - Tambah foto sendiri
   - Edit pesan cinta

### User Interactions
- Scroll animations (fade in, slide up)
- Hover effects pada semua cards
- Click untuk flip cards
- Click heart untuk like
- Smooth scroll navigation

### Edge Cases
- Image load failure: show placeholder
- Mobile: simpler animations
- Graceful degradation

---

## 4. Acceptance Criteria

- [ ] Website load tanpa error
- [ ] Desain sesuai Pinterest-style (masonry grid)
- [ ] Warna hijau dan pink terlihat jelas
- [ ] Semua hover effects bekerja
- [ ] Flip cards berfungsi
- [ ] Floating hearts animations aktif
- [ ] Responsive di mobile
- [ ] Smooth scroll bekerja
- [ ] Gallery lightbox berfungsi
- [ ] Semua fonts dan images load benar

---

## 5. Cara Penggunaan

1. Buka file `index.html` di browser
2. Edit nama pacar di bagian JavaScript (variable `namaPacar`)
3. Ganti foto di folder `img/` (gunakan nama yang sama)
4. Edit pesan cinta di array `loveLetters`
5. Customization lainnya di JavaScript

---

## 6. Catatan

- Foto placeholder sudah disediakan (dari Unsplash)
- Semua libraries dari CDN (tidak perlu install)
- Offline bisa dengan download semua assets