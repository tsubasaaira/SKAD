# Fix Gemini schema repair

- Gemini hanya jana kandungan Stesen 1-3.
- Metadata guru seperti tajuk, tahun, kesukaran, SK/SP, objektif, sokongan dan EMK dikekalkan terus daripada borang.
- Output Gemini dinormalisasi sebelum validasi.
- Jika schema masih gagal, sistem membuat satu pusingan auto-repair dengan Gemini.
- Jika masih gagal, mesej ralat memaparkan field yang tidak sah.
