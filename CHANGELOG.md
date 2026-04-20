# Changelog

All notable changes to Cast are documented here.

## v1.0.0 — 2026-04-20

Initial release.

### Features

- **7 randomness modes:** Number, Dice, Coin, Picker, Password, Color, Shuffle — each with its own focus view tuned to what the mode does.
- **Tactile delight:** per-mode cast animations, system-sound-backed audio (Pop / Basso / Glass / Bottle / Morse / Hero / Purr), and Force Touch haptics — all toggleable from Settings.
- **Apple Shortcuts integration:** 7 `AppIntents` discoverable in Siri, Spotlight, and Shortcuts.app.
- **Cryptographically-secure password generation** using `SystemRandomNumberGenerator`. Passwords are never persisted to disk.
- **Help popovers:** a `?` button on every focus view explains the mode, lists tips, and shows keyboard shortcuts.
- **Live-switchable UI language:** 8 languages bundled (English, French, German, Spanish, Portuguese (BR), Japanese, Korean, Chinese Simplified). Language picker in Settings with a confirm-to-restart flow.
- **Live-switchable theme:** Auto / Light / Dark picker in Settings. Applies immediately, no relaunch.
- **Accessibility-first:** VoiceOver labels + hint text on every card with per-mode result summaries. Reduce Motion auto-downgrades animations to subtle.
- **Keyboard shortcuts:** `Space` to cast, `Cmd+1…7` to jump between modes, `Cmd+C` to copy, `Esc` / `Cmd+[` to return home, `Cmd+,` for Settings, `Cmd+?` for help.
- **macOS 14+ native.** Apple Silicon + Intel. Zero third-party runtime dependencies.
- **Built-in update checker** via the GitHub Releases API. No Sparkle.

### Hardware caveat

Haptic feedback requires a Force Touch trackpad (MacBook Pro 2015+, MacBook Air 2018+, Magic Trackpad 2+). On desktop Macs or non-Force-Touch trackpads, macOS silently ignores haptic requests — sounds and animations continue to work. An `info` affordance next to the Haptics toggle explains this in-app.

### Notes for translators

The 8 bundled translations were produced machine-assisted against the Apple Style Guides per locale. Native-speaker refinements via PR against `languages/*.xml` are very welcome — see `CONTRIBUTING.md`.
