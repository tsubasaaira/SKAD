# Fix build Gemini TTS

Pembetulan untuk ralat TypeScript Cloudflare:

1. `Map` daripada `lucide-react` kini dialias sebagai `MapIcon`, supaya `new Map()` tidak bertembung dengan ikon React.
2. Cache TTS menggunakan `new globalThis.Map<string,string>()`.
3. Ditambah type compatibility `ActivityWithAudio` untuk `audioMode`, `audioRecording`, dan `audioRecordingName` supaya build kekal serasi walaupun repo pernah mempunyai `lib/activity.ts` versi lama.
4. `lib/activity.ts` dalam pakej ini juga mengandungi field audio baharu dan perlu di-upload bersama `app/skuad-app.tsx`.

Fail penting untuk replace:
- app/skuad-app.tsx
- lib/activity.ts
- functions/api/skuad.ts
