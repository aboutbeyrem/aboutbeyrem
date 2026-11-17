# Beyrem

High-school senior in Tunisia. I build tools for problems I actually have, then measure whether they work.

### 🛡️ [SimpleAV](https://github.com/aboutbeyrem/SimpleAV): when my antivirus kept losing
A file-infecting virus patched 865 programs on my PC and came back after every "removal".
I took it apart byte by byte, found its 12-byte fingerprint and the four persistence tricks
keeping it alive, and wrote a scanner and real-time watcher for exactly that family.
When it came back, SimpleAV caught it: 18 freshly infected programs quarantined on its own.<br>
`PowerShell` · `PE parsing` · `Windows persistence` · `47 tests`

### 🪶 [Aether OS](https://github.com/aboutbeyrem/aether-os): Linux for people scared of Linux
My own Arch-based distribution. A first-boot wizard sets the desktop up for developers, gamers or security work;
Game Ready installs the missing graphics and gaming stack; `please` runs system jobs in plain words, with an AI half
that is treated as untrusted (nothing runs without a yes). Btrfs snapshots to roll back, and Flow, a browser built
from Brave's source. Up to v49 now; recent builds are gated by automated checks and QEMU boot tests.<br>
[Download](https://www.runaether.tn) · `Arch Linux` · `KDE Plasma` · `PyQt6 / QML` · `archiso`

### 🌍 [The Blue Record](https://github.com/aboutbeyrem/The-blue-record): NASA data you can hear
NASA Space Apps 2026 (certificate of participation). Pick a country on a 3D globe and hear live satellite data
(temperature, rain, elevation, vegetation) as sound, so people who can't see a map can still explore it.
Every value is checked against a second NASA source: sea temperature within 0.28 °C (r = 0.999).<br>
[Live](https://the-blue-record.vercel.app) · `WebGL` · `Web Audio` · `NASA GIBS`

### How I work
- **Measure, don't claim.** Every project ships its own numbers, including the bad ones (rain: r = 0.42).
- **Write down the limits.** What a tool can't do goes in the README, not in a footnote.
- **Say how it was built.** I use AI as a pair programmer, and my READMEs say so.

### Contact
[itsbeyrem@gmail.com](mailto:itsbeyrem@gmail.com) · [LinkedIn](https://www.linkedin.com/in/aboutbeyrem/)
