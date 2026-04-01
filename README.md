 ╔══════════════════════════════════════════════════════════════════════════════╗
		                     🎤  PitchPilot 1.0  🎤               
 ╠══════════════════════════════════════════════════════════════════════════════╣
 ║  A browser-only karaoke pitch trainer that combines:                         ║
 ║    • Spotify's Basic Pitch (ML note detection) — runs fully in-browser       ║
 ║    • AssemblyAI word-level transcription (optional, API key required)        ║
 ║    • Web Audio API real-time microphone pitch detection (autocorrelation)    ║
 ║    • RapidAPI youtube-mp36 bridge for direct YouTube → MP3 downloads         ║
 ║                                                                              ║
 ║  ARCHITECTURE OVERVIEW                                                       ║
 ║  ─────────────────────                                                       ║
 ║  1. User loads audio (file drop OR YouTube URL via RapidAPI)                 ║
 ║  2. "Detect Notes" runs Basic Pitch + AssemblyAI in parallel                 ║
 ║  3. Notes → pill objects rendered on a scrolling canvas timeline             ║
 ║  4. On playback, the RAF loop ticks song time, yncs lyrics + expected note   ║
 ║  5. Mic input is autocorrelated each audio frame → smoothed note name        ║
 ║  6. Sung note vs. expected note → colour feedback on the big karaoke word    ║
 ║                                                                              ║
 ║  DEPENDENCIES (all CDN / ESM — no build step)                                ║
 ║    @spotify/basic-pitch  1.0.1   https://esm.sh/                             ║
 ║    AssemblyAI REST API   v2      https://api.assemblyai.com/                 ║
 ║    youtube-mp36 (RapidAPI)       https://rapidapi.com/ytjar/api/youtube-mp36 ║
 ║                                                                              ║ 
 ║  YOU CAN ALWAYS FIND ME ON GITHUB IF YOU HAVE FURTHER QUESTIONS              ║   
 ║  https://github.com/onlyGod-can-Intimidate-me/PitchPilot                     ║
 ║  coded by John Tsorotes                                                      ║ 
 ╚══════════════════════════════════════════════════════════════════════════════╝
