> Versi: v1.0.0 | Status: disetujui | Menggantikan: -

# 40-TECHSTACK — Tumpukan Teknologi (pawonee-design)

Mengacu: Pawonee-TownHall v1.0.0 (https://github.com/Coding-Skuy/Pawonee-TownHall).

## 1. Kondisi saat ini (tercatat)

- React 19.0.0 referensi, TypeScript 5.7.2, token JSON mandiri (sumber: `package.json`, `README.md`). Primer `#E8590C`, latar `#FFF9F2`, teks `#212529`, radius kartu 16 dan tombol 12, rasio gambar 4:3.

## 2. Target standar emas (rencana)

- Token tetap framework-agnostik (JSON). Implementasi referensi mengikuti target web (SvelteKit) saat fase coding; varian KMP Compose menyusul memakai token yang sama.
- Selaras divisi: KMP Kotlin 2.2.20 dan Compose 1.8.2 dan nav3 1.0.0; Rust axum 0.8.4; Python 3.12; web SvelteKit dan Bun terbaru; Postgres 16.x; database `pawonee`; JWT audiens `pawonee`.

## 3. Langkah penyesuaian (rencana — bukan eksekusi sekarang)

1. Kunci versi eksak pada `package.json` saat fase coding dimulai.
2. Selaraskan matriks `VERSIONS.md` di `pawonee-infra-devops` setelah fase coding dimulai.
3. Jalankan pemeriksaan render kartu resep sebelum menaikkan versi.
4. Catat perubahan versi pada dokumen ini dan TownHall Pawonee-TownHall v1.0.0.

## Batasan

- Dokumen versi ini tidak mengubah token, komponen, atau versi terpasang; semua target adalah rencana.
- Tidak ada migrasi framework atau kenaikan versi dalam dokumen ini.
- Model tetap mengikuti `:shared:pantry-resep` milik Pawonee; tidak ada duplikasi model baru.
- Perencanaan BRD, PRD, FSD, dan roadmap repo ini mengacu Pawonee-TownHall v1.0.0 dan tidak diduplikasi di sini.
