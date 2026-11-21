# Beyrem Oueslati

Hey, I'm Beyrem Oueslati 👋 A student in Tunisia who got hacked once and decided to build my way out. Here's what came of it.

---

## 🛡️ [SimpleAV](https://github.com/aboutbeyrem/SimpleAV): when my antivirus kept losing

A file from a friend's hijacked Discord account brought in two things: Blank Grabber, an account stealer I caught
and wiped, and a file infector I missed. The infector patched 865 programs and came back after every "removal".
I took it apart byte by byte, found its 12-byte fingerprint and the four persistence tricks
keeping it alive, and wrote a scanner and real-time watcher for exactly that family.
When it came back, SimpleAV caught it: 18 freshly infected programs quarantined on its own.

`PowerShell` · `PE parsing` · `Windows persistence` · `47 tests`

---

## 💡 [Porchlight](https://github.com/aboutbeyrem/porchlight): a calm guard for your home network

After SimpleAV I wanted to stop the next attack at the door. Porchlight is a Windows tray app that watches the home
network and tells you, in plain words, what to fix next. It only looks: no logins, no password guessing.
**[Download it at porchlight-beryl.vercel.app](https://porchlight-beryl.vercel.app)**

<a href="https://github.com/aboutbeyrem/porchlight"><img src="https://raw.githubusercontent.com/aboutbeyrem/porchlight/main/docs/app-overview.png" alt="Porchlight saying Your home is mostly safe, with the next step lit up and a small map of the home network" width="100%"></a>

- **Who's here:** names each device from what it announces (the router's DNS, service names, mDNS) and asks
  "Is it yours?" when someone new joins.
- **Something pretending:** catches a device answering as the router (ARP spoofing), fake copies of your Wi-Fi,
  and the repeated drops of a "kick-off" (deauthentication) attack, live.
- **One step at a time:** the next fix, lit up, and "I did it, check again" to prove it worked.
- **Tested at home first:** its first look found an FTP server and SMBv1 still on in our router, and WPS on the extender.
- **Trust:** signed updates, no account, no telemetry, and a page listing every connection it makes.

`Rust` · `Tauri` · `Windows Wi-Fi API` · `150 tests`

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
- **Snap Layouts:** `Super+Z` tiles the active window into one of six layouts, with a gold preview.
- **Release process:** up to v49 so far, built with `archiso`; recent builds pass an automated gate and QEMU
  boot tests before they ship.

`Arch Linux` · `KDE Plasma` · `PyQt6 / QML` · `Bash` · `archiso`

---

## 🌊 [Flow](https://github.com/aboutbeyrem/Flow): Aether's own browser

Compiled from source on top of Brave (Chromium 149), rebranded at the source so it feels like part of the OS.

<a href="https://github.com/aboutbeyrem/Flow"><img src="https://raw.githubusercontent.com/aboutbeyrem/Flow/main/docs/new-tab-light.png" alt="Flow new tab" width="100%"></a>

- **Rebranded at the source:** a build overlay rewrites names, the `aether://` scheme, about pages, logos and
  colours inside Brave's source tree, then the whole browser is compiled (~520 MB).
- **Survives updates:** the overlay is idempotent, so it re-applies cleanly to each new Brave release.
- **One surgical change for the new tab:** Brave builds its new tab through one function; Flow swaps that single
  chokepoint instead of patching dozens of files.
- **Make the new tab yours:** `Ctrl+Shift+E` lets you drag everything around, edit your sites and set an image or
  video background. Brave's `Ctrl+Space` command palette stays on.
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
- **Say how it was built.** The ideas and decisions are mine; AI coding agents (Claude Code) are my tools, and I say so.

### Contact
[aboutbeyrem.com](https://www.aboutbeyrem.com) · [itsbeyrem@gmail.com](mailto:itsbeyrem@gmail.com) · [LinkedIn](https://www.linkedin.com/in/aboutbeyrem/)
