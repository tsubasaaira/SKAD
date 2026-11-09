# Gemini hard repair

Backend kini membaiki output Gemini secara deterministic sebelum validasi akhir.
- note/audio dipanjangkan jika terlalu pendek
- questions dijamin tepat 3
- moves dijamin tepat 3
- setiap soalan dijamin mempunyai 3 pilihan dan answer 0-2
- speaking, ideas, frame, examples dan assessment diberi fallback mengikut topik

Fail utama berubah: `functions/api/skuad.ts`.
