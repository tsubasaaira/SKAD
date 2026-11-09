# Gemini Content Quality Fix

- Uses Gemini structured output (`responseSchema`)
- Requires exactly 3 questions and 3 moves with 3 options each
- Requires a real topic-specific audio/story rather than generic placeholder text
- Rejects placeholders such as Soalan kefahaman / Pilihan 1
- Regenerates once from scratch if content is structurally valid but semantically too generic
- Year and difficulty influence language and audio length
