# Hifdh

A beautiful mobile app (Expo + React Native) for memorizing the Quran and learning meanings in English/Swahili.

## Highlights

- Liquid glass UI with gradients, animations, tab navigation
- Surah list and detail with per-ayah audio (AB speed control)
- English/Swahili localization with toggle
- Search across translations, downloads for offline audio
- Word-by-word view with token modal (morphology stub)
- SRS memorize flow with add-to-deck and review
- Bookmarks and notes per ayah

## Tech

- Expo SDK 53, TypeScript, expo-router
- expo-av, expo-blur, expo-linear-gradient, react-native-reanimated
- i18next + react-i18next + expo-localization
- AsyncStorage + zustand for caching and prefs

## Getting started

1. Install deps:

```bash
npm install
```

2. Run:

```bash
npm run android   # or npm run web
```

3. Build web preview:

```bash
npx expo export --platform web
```

## Configuration

- Reciters can be selected in Settings
- Language can be toggled in the header
- AMOLED theme in Settings affects background style

## Deployment (GitHub Pages)

A workflow publishes the web build to `gh-pages`. Configure Settings → Pages → Branch: `gh-pages`.

## Notes

- Word-by-word morphology is a stub; replace with a licensed dataset when available.
- Audio and text are fetched from public APIs and may have rate limits.