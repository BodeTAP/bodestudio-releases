# BodeStudio Pro — Official Public Releases & Distribution Portal

Welcome to the official public distribution channel for **BodeStudio Pro** (Universal YouTube Ambience Video Automation Engine).

BodeStudio Pro is an agency-grade Windows desktop application engineered for YouTube ambience, lofi, relaxing, and meditation channel creators.

---

## 📥 Download Latest Official Release

| Release Version | Target Platform | Architecture | Installer Size | Direct Download | Release Notes |
|---|---|---|---|---|---|
| **v3.6.0 (Latest)** | Windows 10 / Windows 11 | x64 (64-bit) | 124.01 MB | [Download Setup Installer (.exe)](https://github.com/BodeTAP/bodestudio-releases/releases/download/v3.6.0/BodeStudioPro_v3.6.0_Setup.exe) | [Changelog v3.6.0](https://github.com/BodeTAP/bodestudio-releases/releases/tag/v3.6.0) |

---

## 📖 Official Documentation & User Guides

- 🇮🇩 **[Panduan Pengguna Lengkap (Bahasa Indonesia)](PANDUAN_PENGGUNA.md)**: Panduan instalasi, aktivasi lisensi, alur kerja pembuatan video ambience, setup YouTube OAuth, dan troubleshooting.
- 🇬🇧 **[Official User Manual & Quick-Start Guide (English)](USER_MANUAL.md)**: Full guide for international agency clients and individual creators.

---

## ⚡ Core Capabilities

- **100% Forward Seamless Crossfade Loop**: Industrial forward-only crossfade dissolve algorithm. Zero reverse / ping-pong playback.
- **Smart Audio Shuffle Engine**: Minimum 60% pool cooldown distance between consecutive plays. Zero repeating tracks in short intervals.
- **EBU R128 Broadcast Audio Mastering**: Calibrated to exact `-14 LUFS` (`loudnorm=I=-14:TP=-1.5:LRA=11`) with Fast Stream-Copy bypass toggle.
- **AI Metadata & C2PA Scrubber**: Removes C2PA, Google AI, and SynthID tags (`-map_metadata -1 -bitexact`) to safeguard monetization and organic reach.
- **Multi-Vendor GPU Acceleration**: Auto-detects NVIDIA NVENC, Intel QuickSync (QSV), AMD AMF, and DirectX Media Foundation.
- **YouTube Resumable Auto-Uploader**: Direct chunked background upload to YouTube Studio with automatic chapter markers, tags, and 1080p thumbnail cover grabber.
- **In-App Auto-Updater**: Instant version checking, background download telemetry, and seamless in-place upgrade.

---

## 💻 System Requirements

- **OS**: Windows 10 (Build 19041+) or Windows 11 64-bit.
- **RAM**: 8 GB RAM minimum (16 GB recommended for 1080p 60fps / 4K).
- **GPU**: NVIDIA GeForce GTX 1050+ / Intel UHD Graphics 620+ / AMD Radeon RX 500+ with hardware encoder support.
- **Storage**: ~500 MB free disk space for application installation.

---

## 📜 Release Notes

### v3.6.0 (Latest Release)
- **Custom Audio Spectrum Overlay (Batch Render)**: Added two reactive visualizer styles (**Capsule Glow** and **Silky Wave**) with free color picker, Rainbow gradient mode, scale/opacity sliders, and interactive drag-and-drop positioning directly on the preview monitor.
- **Auto-Persistent User Settings**: Automatically saves and restores the user's last render session preferences (channel preset, duration, resolution, quality preset, LUFS, micro-crop, loop transitions, spectrum, watermark, and YouTube upload config) across restarts.
- **Strict 2-Pass VBR for NVIDIA NVENC**: Enforced `-rc vbr -2pass 1` on `h264_nvenc` so short video loops strictly obey Saver/Ultra-Saver bitrate budgets without file size bloat.
- **Live Broadcast Initialization & HUD Fixes**: Resolved `max_duration` `NameError` when launching 24/7 RTMP live streams and hardened Windows `drawtext` path escaping.

### v3.5.0
- **Multi-Scene Dynamic Assembly**: Native support for sequencing multiple video clips into a single seamlessly looped project. Full drag-and-drop / scan batch ingestion with individual sub-clip inspection, duration trim, and scene tab switching.
- **Granular Horizontal Video Flip**: Per-video and per-scene horizontal mirroring (`hflip`) to evade copyright fingerprinting and repurpose video assets. Each individual scene clip can now be mirrored independently or inherited from parent queue items.
- **Shorts Visual Crop Simulator with Real-Time Mirroring**: Upgraded 9:16 vertical crop preview modal with live smartphone simulator supporting flipped clips without visual offset desynchronization or black-screen rendering.
- **Ultra-Responsive Studio Layout**: Streamlined workstation UI accommodating compact laptop and minimum window resolutions (~1100x700px) with adaptive icon-only toolbars, zero-wrap queues, and space-budgeted footer telemetry.
- **Synchronized Monitor & Inspector Context**: Multi-scene sub-clips dynamically drive the central video monitor, transport controls, and preview generators.

### v3.4.0
- **Loop Transition Engine & Direct Cut**: Full suite of forward loop transitions including smooth linear alpha crossfade, fade through black, fade through white, wipe left/right, slide up/down, smooth left/right, and direct cut passthrough.
- **GPU-Accelerated Instant Loop Preview**: Sub-second preview generation engine utilizing GPU acceleration and 720p draft Lanczos scaling, allowing creators to inspect seam smoothness in real time.
- **Real-Time Storage Estimator**: Pre-render disk capacity calculator estimating output gigabytes across batch queues based on target duration, bitrate quality presets, and target resolution.
- **Corrupt Render Output Auto-Cleaner**: Automated validation and recovery utility identifying and deleting damaged or truncated MP4 files resulting from disk-full errors, recovering space without breaking queues.
- **Zero Noise Crossfade Blend**: True linear alpha mixing replacing legacy binary threshold dithering, eliminating 100% of particle noise dots on moving elements (steam, rain, embers, smoke).
- **Unified Reactive Invalidation**: Fully reactive state synchronization ensuring zero stale preview playback across video queue switching, preset switching, cropping, and watermark adjustments.

### v3.3.1
- **Automatic Disk Cache Pruning**: Intermediate video loops and concat lists in `.cache` are automatically deleted upon video completion or cancellation. Added manual `clean_disk_cache` utility.
- **Admin Keygen CLI Utility**: Official isolated CLI tool (`admin_keygen.py`) for the software owner to instantly generate and verify customer offline licenses (`--hwid`, `--tier`, `--name`).
- **Resilient YouTube API Uploader**: Added pre-flight token refresh buffer and clear human-readable diagnostics for Daily Quota Limits (10,000 units/day) and upload channel restrictions.
- **Cancelable Shorts 9:16 Generator**: Upgraded vertical teaser generator with non-blocking subprocess loop and instant process tree kill (<100ms) on cancel.
- **Workstation UI Version Sync**: Dynamic Header badge and IPC telemetry updated to v3.1.2.

### v3.1.1
- **Eliminated OS Pipe Buffer Deadlock**: Resolved render freeze at 0% during forward loop creation by switching to non-blocking pipe buffer draining (`communicate` with timeout).
- **Instant Render Cancelation**: Aborting active renders terminates the complete FFmpeg process tree in <100ms (`taskkill /F /T /PID`).
- **Worker Thread Return Contract Safety**: Guarded all exception and cancellation handlers against `TypeError` unpacking crashes.
- **Public In-App Auto-Updater Channel**: Routed update queries to public distribution manifests with live download telemetry.

### v3.1.0
- **Official Inno Setup Windows Installer Pipeline**: Single-file setup installer (`BodeStudioPro_Setup.exe`) with auto-launch and desktop shortcuts.
- **Official Flame Orange Studio Branding**: Multi-resolution `.ico` icon bundle for taskbar, desktop, and window titles.
- **Container-Aware Responsive Preview Layout**: Fluid resizing of live canvas player for narrow windows and multi-monitor setups.
- **In-App Auto-Updater**: In-place download and automatic upgrade without losing offline license activations.
- **Smart Audio Engine Cooldown**: Hardened anti-duplicate track spacing ensuring at least 60% pool cooldown window.

---

*Copyright (c) 2026 BodeStudio Engineering Team. All rights reserved.*
