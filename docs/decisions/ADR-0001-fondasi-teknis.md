# ADR-0001 — Fondasi teknis pawonee-design

Status: Diterima | Tanggal: 2026-10-14

## Konteks

Mobile dan web harus tampil konsisten, dan Pedaree menampilkan ringkasan resep dengan gaya kartu yang sama. Sumber kebenaran: Pawonee-TownHall `platform/versions/v1.0.0` (https://github.com/Coding-Skuy/Pawonee-TownHall/tree/main/platform/versions/v1.0.0), beku 2026-10-07; lintas divisi: [KONTEKS-LINTAS-DIVISI.md](https://github.com/Coding-Skuy/ChefGenie-TownHall/blob/main/KONTEKS-LINTAS-DIVISI.md). Tiket fondasi: PWN-DSG-001 (issue #1).

## Keputusan

1. Repo desain tidak berisi kode produk; hanya token, flow, spesifikasi komponen, dan tautan Figma.
2. Token framework-agnostik dengan pemetaan eksplisit ke Compose Multiplatform dan CSS (SvelteKit).
3. Flow dikunci: 6 layar mobile (beranda, stok, rekomendasi, resepDetail, preferensi, riwayat) dan 5 rute web pendamping.
4. Kartu resep selalu menampilkan nama, durasi (menit), level pedas, dan estimasi biaya; lencana grade hanya untuk resep dari bank 12 resep.
5. Perubahan flow besar = PRD/FSD versi baru di TownHall.

## Konsekuensi

- Referensi React `RecipeCard.tsx` harus diganti/ditandai usang saat `pawonee-web` bermigrasi ke Svelte 5.
- Perubahan token memengaruhi tiga konsumen: KMP, web, dan Pedaree.
- Link Figma menjadi artefak wajib di README.
