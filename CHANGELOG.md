# Changelog

## [1.3.0] - 2026-02-11

### Added
- **5 different laugh track variants** (laugh2-laugh6)
  - Alternates between clips to avoid repetition
  - Never plays the same clip twice in a row
- Sound variant system for future expansion

### Changed
- Replaced single laugh.mp3 with higher quality laugh tracks

## [1.2.0] - 2026-02-11

### Added
- **Randomized audio playback** to prevent repetitive sound
  - Random pitch shift: ±100 cents (±1 semitone)
  - Random playback speed: ±10%
- **Crossfade looping** for extended playback
  - Smooth 300ms crossfade between segments
  - No audible cuts when sound loops
- Full Web Audio API integration for audio manipulation

### Technical
- Switched from HTML5 Audio to AudioBufferSourceNode for pitch/speed control
- Added detune and playbackRate randomization
- Implemented segment scheduling with gain envelope crossfading
- Audio context persists between start/stop for faster response

## [1.1.0] - 2026-02-11

### Changed
- **Replaced synthesized sounds with real audio clips** from Mixkit (free, royalty-free)
- Added /sounds folder with 6 MP3 files:
  - laugh.mp3 - Crowd laughter
  - applause.mp3 - Audience applause
  - aww.mp3 - Crowd aww reaction
  - ooh.mp3 - Crowd ooh reaction
  - gasp.mp3 - Dramatic gasp
  - boo.mp3 - Crowd booing
- Added loading indicator for audio files
- Improved audio playback (using HTML5 Audio instead of Web Audio synthesis)

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
