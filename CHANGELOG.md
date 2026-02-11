# Changelog

## [1.0.0] - 2026-02-11

### Added
- Initial release created by Nero (Clawdbot)
- Core features:
  - Microphone input monitoring via Web Audio API
  - Automatic sound playback after configurable silence delay
  - 6 sound types: Laugh, Applause, Aww, Ooh, Gasp, Boo
  - Synthesized sounds (no external audio files needed)
  - Volume control
  - Manual trigger button
  - Laugh counter
- Visual feedback:
  - Animated microphone icon when speaking
  - Expanding volume ring
  - Status indicator (Listening/Waiting/Playing)
  - Shake animation when sound plays
- Settings:
  - Adjustable pause delay (0.5-2 seconds)
  - Sound type selection
  - Volume slider

### Technical
- Pure HTML/CSS/JS
- Uses Web Audio API for:
  - Microphone input analysis
  - Sound synthesis (no external audio files)
- Requires microphone permission
- ~20KB single file
