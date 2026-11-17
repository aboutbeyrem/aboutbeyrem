# Beyrem

High-school senior in Tunisia. I build tools for problems I actually have, then measure whether they work.

---

## 🛡️ [SimpleAV](https://github.com/aboutbeyrem/SimpleAV): when my antivirus kept losing

A file-infecting virus patched 865 programs on my PC and came back after every "removal".
I took it apart byte by byte, found its 12-byte fingerprint and the four persistence tricks
keeping it alive, and wrote a scanner and real-time watcher for exactly that family.
When it came back, SimpleAV caught it: 18 freshly infected programs quarantined on its own.

`PowerShell` · `PE parsing` · `Windows persistence` · `47 tests`

---

## 🪶 [Aether OS](https://github.com/aboutbeyrem/aether-os): Linux for people scared of Linux

My own Linux distribution, built on Arch and KDE Plasma, for people who have always been too scared to try Linux.
**[Download it at runaether.tn](https://www.runaether.tn)**

<a href="https://github.com/aboutbeyrem/aether-os"><img src="https://raw.githubusercontent.com/aboutbeyrem/aether-os/main/docs/welcome.png" alt="Aether OS first-run welcome" width="100%"></a>

- **Welcome, made yours:** the first-boot wizard asks if you're a developer, a casual user or into cybersecurity, and
  sets the desktop up for that. Light/dark flips the whole OS live.
- **Game Ready:** audits the graphics and gaming stack (Vulkan, Direct3D translation, Steam, Bottles, Heroic) and
  installs what's missing in one click.
- **`please`:** system jobs in plain words. Its AI half is treated as **untrusted**: a separate danger classifier
  blocks destructive commands, and nothing runs without a yes.
- **Timeline:** Btrfs snapshots, so a broken system rolls back.
- **Built like a product:** up to v49 so far, built with `archiso`; recent builds pass an automated gate and QEMU
  boot tests before they ship.

`Arch Linux` · `KDE Plasma` · `PyQt6 / QML` · `Bash` · `archiso`

---

## 🌊 [Flow](https://github.com/aboutbeyrem/Flow): Aether's own browser

Compiled from source on top of Brave (Chromium 149), rebranded down to the engine so it feels like part of the OS.

<a href="https://github.com/aboutbeyrem/Flow"><img src="https://raw.githubusercontent.com/aboutbeyrem/Flow/main/docs/new-tab-light.png" alt="Flow new tab" width="100%"></a>

- **Rebranded at the source:** a build overlay rewrites names, the `aether://` scheme, about pages, logos and
  colours inside Brave's source tree, then the whole browser is compiled (~520 MB).
- **Survives updates:** the overlay is idempotent, so it re-applies cleanly to each new Brave release.
- **One surgical change for the new tab:** Brave builds its new tab through one function; Flow swaps that single
  chokepoint instead of patching dozens of files.
- **Quiet by default:** telemetry, rewards, crypto wallet, VPN and AI chat off; search through DuckDuckGo.

`C++` · `Chromium / Brave` · `GN build` · `JavaScript`

---

## 🌍 [The Blue Record](https://github.com/aboutbeyrem/The-blue-record): NASA data you can hear

Built with my team for the NASA Space Apps Challenge 2026
([participant certificate](https://github.com/aboutbeyrem/The-blue-record/blob/main/docs/nasa-space-apps-2026-certificate.pdf)).
Pick a country on a 3D globe and hear live satellite data (temperature, rain, elevation, vegetation) as sound, so
people who can't see a map can still explore it. Every value is checked against a second NASA source: sea
temperature within 0.28 °C (r = 0.999).

[Live](https://the-blue-record.vercel.app) · `WebGL` · `Web Audio` · `NASA GIBS`

---

### How I work
- **Measure, don't claim.** Every project ships its own numbers, including the bad ones (rain: r = 0.42).
- **Write down the limits.** What a tool can't do goes in the README, not in a footnote.
- **Say how it was built.** I use AI as a pair programmer, and my READMEs say so.

### Contact
[itsbeyrem@gmail.com](mailto:itsbeyrem@gmail.com) · [LinkedIn](https://www.linkedin.com/in/aboutbeyrem/)
