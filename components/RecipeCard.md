# Spesifikasi Kartu Resep Pawonee

## Anatomi

1. Gambar hidangan (rasio 4:3).
2. Lencana "KURASI" bila resep berasal dari bank grade-2.
3. Nama resep (maksimal 2 baris, elipsis).
4. Baris meta: durasi menit, level pedas 0–5, estimasi biaya rupiah.
5. Tombol aksi "Lihat Resep".

## Varian

- `ringkas`: gambar + nama + meta satu baris (daftar rekomendasi).
- `penuh`: ringkas + 3 bahan pertama + tombol aksi (detail/terpilih).

## Aksesibilitas

- Kontras teks terhadap latar minimal 4.5:1.
- Level pedas tidak hanya mengandalkan warna; tulis angka "pedas 3/5".
- Area sentuh tombol minimal 44×44 dp.

## Data

Kolom kartu dipetakan 1:1 dari modul `:shared:pantry-resep` milik Pawonee:
`nama`, `menit`, `levelPedas`, `estimasiBiaya`, `grade`.
