> Versi: v1.0.0 | Status: disetujui | Menggantikan: -

# 60-BLAST-RADIUS — Batas Context (pawonee-design)

Mengacu: Pawonee-TownHall `platform/versions/v1.0.0` (https://github.com/Coding-Skuy/Pawonee-TownHall/tree/main/platform/versions/v1.0.0), beku 2026-10-07. Baris Pawonee townhall-roadmap §2: point of concern "12 resep inti; serapan ≥1.500 g"; batas context "G2-V/U/S; porsi 1–8 jiwa; DB `pawonee`; JWT audiens `pawonee`". Rujukan lintas divisi: KONTEKS §8/§9.

## 1. Boleh disentuh repo ini

- `tokens/`, `components/*.md`, flow, aset desain, README (link Figma).
- Spesifikasi RecipeCard, halaman publik bagi, dan cetak 1 halaman.

## 2. Dilarang

- Menambah kode aplikasi/server.
- Mengubah flow besar tanpa PRD/FSD versi baru di TownHall.
- Mendefinisikan ulang data kartu di luar `:shared:pantry-resep` (`nama`, `menit`, `levelPedas`, `estimasiBiaya`).
- Menyentuh DB divisi lain (DB per service; Titeny hanya read-only ke DB sumber).
- Memakai komoditas non-pilot (kentang/wortel/tomat/kol) untuk klaim pasokan agregasi Lumbung; hanya cabai, bawang, kangkung (KONTEKS §4).
- Menambah resep ke-13, mengubah definisi G2, atau mengubah audiens JWT tanpa PR TownHall + ADR.

## 3. Kontrak yang diproduksi

- Token dan pemetaan Compose/CSS.
- Spesifikasi RecipeCard, flow 6 layar + 5 rute web.

## 4. Kontrak yang dikonsumsi

- Model data kartu dari `:shared:pantry-resep` (pemilik Pawonee).
- PRD 10/20/30 dan FSD 10 sebagai sumber flow.

## 5. Dampak bila berubah

- Perubahan token/komponen memengaruhi `pawonee-app-kmp`, `pawonee-web`, dan tampilan ringkasan Pedaree.

## Batasan

- Dokumen ini hanya memetakan batas dan risiko; tidak mengubah kode atau konfigurasi.
- Keputusan lintas divisi dirujuk ke `KONTEKS-LINTAS-DIVISI.md` dan TownHall Pawonee v1.0.0.
