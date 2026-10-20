# SoundCraft PWA

Deploys at https://cptnope.github.io/soundcraft/ after GitHub Actions succeeds.

Phone-only UI provides Edit, Mix, Tracks and Clips views plus New, Open, Save, Audio import, add track and transport buttons. Phones start with a lightweight blank session; use `?demo` for the sample session. Desktop layout stays intact.

The GitHub Pages workflow builds the WASM browser app and packages a PWA, without running the full Rust workspace test suite. Existing source tests are preserved; FreeBSD, Nix, packaging, Windows ARM64, and release workflows are manual-only.

Offline caching covers static application assets, not user sessions or audio files. Back up your projects through Save/Export. WebAudio playback on phones requires a user gesture.
