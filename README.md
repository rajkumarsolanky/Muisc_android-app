# 🎵 Music by Rajkumar Solanky

An offline-first Android music player built around a custom Glassmorphism design system. 
Every glass panel's intensity and every accent color respond in real time — no restart needed. 
Powered by Jetpack Media3 & ExoPlayer for gapless, high-fidelity local playback, with a Room-backed 
library cache for instant app opens.

## ✨ Features
- 💎 **Live Glass Engine** — a custom-built styler that dynamically generates translucent glass 
  drawables at runtime; drag the intensity slider and every panel updates instantly.
- 🌈 **Real-time Accent Theming** — pick cyan, red, purple, or green and watch the whole UI 
  re-tint live, from the mini-player to the seek bar.
- 🎧 **Media3 + ExoPlayer Playback** — background playback via MediaSessionService with full 
  media-notification and lock-screen controls.
- 🔍 **Smart Local Library** — MediaStore-backed scanning with folder exclusion and a 
  small-file filter, cached in Room so re-opening the app is instant.
- ⚡ **Instant Cold Starts** — cached library loads immediately; fresh scans happen silently 
  in the background.

## 🛠️ Tech Stack
- **Language:** 100% Kotlin
- **Playback:** Jetpack Media3 (ExoPlayer + MediaSession)
- **Persistence:** Room + SharedPreferences-backed reactive settings (StateFlow)
- **UI:** Custom View/XML with a runtime GlassStyler + ThemeController, no Compose
- **Min SDK:** API 35 (Android 15) · **Target SDK:** API 36
