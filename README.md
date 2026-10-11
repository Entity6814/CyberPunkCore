# Cyberpunk Core — Neon System HUD

**Author:** Entity6814  
**Type:** Lively web wallpaper  
**Entry point:** `index.html`

An audio-reactive cyberpunk desktop HUD built around a central reactor dial. It combines live track artwork and metadata, a frequency spectrum display, animated particles, configurable neon themes, and system telemetry in a compact glass HUD.

## Features

- Central audio-reactive reactor dial with the current album artwork, track, artist, and album.
- Live audio spectrum with bass, midrange, and treble levels; the preview goes idle when live audio is silent, with Reactor Ring, Wave Scope, and Audio Hills presets plus a rotation toggle.
- Toggle the live audio preview on/off; no synthetic waveform is drawn during silence or when the Lively audio feed goes stale.
- Nebula-inspired constellation, singularity, and warp particle modes, with cursor interactions and adjustable density and speed.
- Seven color themes: Cyber Cyan, Amber Warning, Matrix Emerald, Synthwave Violet, RGB Prism, Solar Gold, and Ice White.
- Lively system telemetry for CPU, memory, and GPU when the system-information plugin provides those values.
- Separate integrated and dedicated GPU rows when the incoming telemetry lists multiple adapters; VRAM appears when explicit used/total fields are provided.
- Top-center CPU, GPU, and memory summaries, plus bottom-center session time, active theme, and particle mode.
- Customizable HUD tile transparency, grid opacity, audio sensitivity, and widget visibility.
- Clock controls for 12/24-hour time, five date layouts, three clock treatments, and adjustable UI font size.
- Six configurable top/bottom center HUD slots, each selectable from CPU, GPU, memory, audio, track, clock, date, session, theme, particle mode, or empty.
- Optional uploaded image or muted looping video background with visibility and opacity controls; the asset is saved in this wallpaper's WebView local database when available.
- Custom video controls for audio enable/mute, volume, loop, play/pause, playback speed, and cover/contain/stretch fit.
- Live desktop clock and pointer coordinates.

## Credits

The Nebula particle-field theme and motion modes were inspired by [Nebulaw-wallpaper](https://github.com/Susbananaa/Nebulaw-wallpaper) by [Susbananaa](https://github.com/Susbananaa). Thank you for the inspiration.

The Lively wallpaper details page's website link points to the Cyberpunk Core project repository.

## Customization

Use Lively's wallpaper properties to change the theme, grid and tile transparency, audio sensitivity, particle settings, and widget visibility. The gear button opens equivalent in-wallpaper controls.

The documented Lively web system-information payload exposes a single `NameGpu` / `CurrentGpu3D` pair and does not document VRAM fields. This wallpaper can display multi-adapter telemetry if the host supplies arrays or indexed fields, but the standard payload alone cannot enumerate both laptop GPUs or report VRAM. See the [Lively system data guide](https://github.com/rocksdanister/lively/wiki/Web-Guide-V-%3A-System-Data/9dbcfc957d65aadee8893f11c121dcdeadc0c22e).

## Install

Import `CyberpunkCore.lively.zip` with Lively's **Add wallpaper → Open** flow. The archive contains the wallpaper entry point, Lively metadata, and customization properties. Keep `LivelyInfo.json` and `LivelyProperties.json` alongside `index.html` when using the unpacked project.
