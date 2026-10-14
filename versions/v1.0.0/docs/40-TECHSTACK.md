> Versi: v1.0.0 | Status: disetujui | Menggantikan: -

# 40-TECHSTACK — Tumpukan Teknologi (pawonee-design)

Mengacu: Pawonee-TownHall `platform/versions/v1.0.0` (https://github.com/Coding-Skuy/Pawonee-TownHall/tree/main/platform/versions/v1.0.0), beku 2026-10-07. Tidak menduplikasi BRD/PRD/FRD/FSD/SRS; hanya mengunci stack repo ini.

## 1. Matriks stack

| Komponen | Kondisi saat ini (tercatat) | Target terkunci v1.0.0 |
|---|---|---|
| Token | `tokens/tokens.json` | Token framework-agnostik + pemetaan Compose/CSS |
| Komponen | `RecipeCard.md` + `RecipeCard.tsx` (React) | Spesifikasi `.md` sebagai sumber; implementasi di repo klien |
| Desain visual | belum terdaftar | Figma (link terdaftar di README) |
| Web referensi | React | Svelte 5 (setelah migrasi web) |



## Batasan

- Dokumen ini tidak mengubah manifes atau kode; kondisi saat ini dicatat apa adanya dari manifes/README repo.
- Versi dikunci eksak di manifes saat kickoff coding; perubahan versi dicatat di dokumen ini lewat versi dokumen berikutnya dan ADR baru.
- JWT audiens `pawonee`, DB logis `pawonee`, dan `:shared:pantry-resep` milik Pawonee tidak berubah oleh dokumen ini.
