# BodeStudio Pro 3.3.0 — Official User Manual & Quick-Start Guide
### *Universal YouTube Ambience Video Automation Engine*

Welcome to **BodeStudio Pro 3.3.0**! This software is engineered specifically for YouTube creators, lofi/ambience music producers, and automated video agency owners looking to produce long-form broadcast-quality ambience videos (1 to 3+ hours) with maximum rendering throughput and monetization protection.

---

## TABLE OF CONTENTS

1. [Chapter 1: System Requirements & Installation](#chapter-1-system-requirements--installation)
2. [Chapter 2: License Activation Guide](#chapter-2-license-activation-guide)
3. [Chapter 3: Studio Workspace Overview](#chapter-3-studio-workspace-overview)
4. [Chapter 4: Step-by-Step Ambience Creation Workflow](#chapter-4-step-by-step-ambience-creation-workflow)
5. [Chapter 5: Broadcast Standards & Golden Rules](#chapter-5-broadcast-standards--golden-rules)
6. [Chapter 6: YouTube Studio Automation (Upload, SEO, & Chapters)](#chapter-6-youtube-studio-automation-upload-seo--chapters)
7. [Chapter 7: In-App Auto-Updater Engine](#chapter-7-in-app-auto-updater-engine)
8. [Chapter 8: Troubleshooting & FAQ](#chapter-8-troubleshooting--faq)

---

## CHAPTER 1: SYSTEM REQUIREMENTS & INSTALLATION

### 1.1. Recommended Hardware Specifications
* **Operating System**: Windows 10 (64-bit) Build 19041+ or Windows 11.
* **Processor (CPU)**: Intel Core i5 / AMD Ryzen 5 (8th Generation or newer).
* **Memory (RAM)**: 8 GB minimum (16 GB recommended for 1080p 60fps / 4K).
* **Graphics Card (GPU)**:
  * NVIDIA: GeForce GTX 1050 or newer (NVENC accelerated).
  * Intel: Intel UHD Graphics 620 or newer (QuickSync / QSV accelerated).
  * AMD: Radeon RX 500 series or newer (AMF accelerated).
* **Storage**: At least 1 GB free disk space for application runtime.

### 1.2. Installation Steps
1. Download the official setup installer: `BodeStudioPro_v3.1.1_Setup.exe`.
2. Double-click the installer to launch the Inno Setup wizard.
3. **Windows Defender SmartScreen Note**:
   If the blue *"Windows protected your PC"* banner appears (standard for newly released independent software):
   * Click **"More info"**.
   * Click **"Run anyway"**.
4. Choose your installation destination directory (Default: `C:\Program Files\BodeStudio Pro`).
5. Check *"Create a desktop shortcut"* if desired.
6. Click **Install**. Ultra-compressed binaries will extract in seconds.
7. Click **Finish** to immediately launch BodeStudio Pro.

---

## CHAPTER 2: LICENSE ACTIVATION GUIDE

BodeStudio Pro utilizes a cryptographic **Hardware ID (Machine ID)** locking system.

### 2.1. Activating Your Lifetime License
1. Launch BodeStudio Pro.
2. In the top Header Bar, click the license status badge (e.g. `TRIAL` or key icon).
3. The **Software License Activation** modal will open.
4. Locate your **Machine ID** (Format: `XXXX-XXXX-XXXX-XXXX`).
5. Click **Copy** next to your Machine ID and send it to your license vendor/administrator.
6. Your vendor will issue your official **Serial Key** (Format: `BODE-TIER-HWID-SIGNATURE`).
7. Paste the Serial Key into the input field and click **Activate License Now**.
8. Once verified, your status will instantly elevate to **LIFETIME ACTIVE** with your purchased tier (`PERSONAL` or `AGENCY`).

> **NOTE**: Your license verification file is safely stored at `%APPDATA%\BodeStudioPro\license.dat`. Reinstalling or updating the application **will never delete or reset your license**.

---

## CHAPTER 3: STUDIO WORKSPACE OVERVIEW

BodeStudio Pro features a CapCut-style 3-panel docked workspace:

```
+-----------------------------------------------------------------------------------------+
| [B] BodeStudio Pro  [Preset: Nocturnal Cruise v]   [QSV Active] [PERSONAL] [Update] [-][#][X] |
+-----------------------+---------------------------------+-------------------------------+
| PANEL 1: MEDIA BIN    | PANEL 2: ADAPTIVE MONITOR       | PANEL 3: INSPECTOR & MASTERING|
|                       |                                 |                               |
| * Raw Video Queue     | * Real-time Video Canvas        | * Target Duration (~1 hr, etc)|
| * Music Audio Pool    | * Safe Guides & Shorts 9:16     | * Resolution & Quality Preset |
| * Add Assets Buttons  | * Loop Indicator (No Reverse)   | * EBU R128 (-14 LUFS) Master  |
|                       | * Play, Seek, Mute, Volume      | * Watermark / Channel Logo    |
|                       |                                 | * YouTube Metadata & Upload   |
+-----------------------+---------------------------------+-------------------------------+
```

* **Left Panel (Media Bin)**: Manages your short video clips and audio pool tracks.
* **Center Panel (Adaptive Monitor)**: Real-time preview player with safe guides, vertical 9:16 Shorts framer, and container-aware responsive collapsing.
* **Right Panel (Inspector & Mastering)**: Controls duration, resolution, -14 LUFS mastering, ambient SFX layers, watermark logos, and YouTube upload automation.

---

## CHAPTER 4: STEP-BY-STEP AMBIENCE CREATION WORKFLOW

### Step 1: Select or Create a Channel Preset
1. From the top Header, select your channel preset from the dropdown (e.g., `Nocturnal Cruise`).
2. To create a new channel, click the **Channel Preset Slider** icon to configure custom folders and branding.

### Step 2: Import Raw Video Clips
1. In the Left Panel under *Video Queue*, click **Add**.
2. Select your raw video clips (`.mp4`, `.mov`, `.mkv`). The engine automatically inspects duration, resolution, and framerate.

### Step 3: Populate Music Pool
1. Under *Music Collection*, click **Add Track** or **Folder**.
2. Import your royalty-free ambient/lofi songs (`.mp3`, `.wav`, `.flac`, `.aac`).

### Step 4: Configure Duration & Audio Mastering
1. In the Right Panel:
   * Select **Target Duration**: `~1 Hour Organic`, `~2 Hours`, or `~3 Hours`.
   * Enable **Broadcast Standard -14 LUFS (EBU R128)** for stable, YouTube-compliant loudness.
   * *(Optional)* Enable **Ambient SFX Layer** (e.g., rain, crackling fireplace, ocean waves) and calibrate volume (recommended: 15% - 25%).

### Step 5: Content Protection & Watermarking
1. Under Card 2:
   * Toggle **Watermark / Channel Logo** and choose your transparent PNG logo.
   * Select corner alignment (e.g. *Top-Right*), opacity (70%), and pixel width.
   * Keep **AI Metadata Scrubber** checked to purge C2PA and generative tags.

### Step 6: Thumbnails & YouTube Shorts
1. Check **Auto Thumbnail 1080p** for instant high-resolution cover extraction.
2. Check **Generate YouTube Shorts (9:16)**:
   * Set Shorts duration (e.g. 45s).
   * Use the **Preview Frame Shorts** button on the player to adjust the horizontal crop focal point.

### Step 7: Export Video
1. Click the prominent orange **Export Video** button in the top right.
2. Monitor real-time GPU encoder metrics, speed multipliers, and ETA.
3. Upon completion, a pleasant two-tone chime sounds, and your output folder is ready to open.

---

## CHAPTER 5: BROADCAST STANDARDS & GOLDEN RULES

BodeStudio Pro is built on 5 fundamental engineering directives:

1. **100% Forward Seamless Crossfade Loop**: Zero reverse or ping-pong playback. Video always advances forward naturally.
2. **Smart Audio Shuffle Engine**: Enforces a minimum 60% cooldown window across the music pool. No songs ever repeat in short proximity.
3. **AI Metadata Scrubber**: Strips C2PA, SynthID, and generative EXIF tags (`-map_metadata -1 -bitexact`).
4. **Broadcast Audio Mastering**: Normalized to `-14 LUFS` EBU R128 (`loudnorm=I=-14:TP=-1.5:LRA=11`).
5. **Fast Stream-Copy Architecture**: Loops and logos burn at the short clip stage (10-30s), allowing 1-3 hour assembly to finish via stream copy (`-c:v copy`) in ~45 seconds!

---

## CHAPTER 6: YOUTUBE STUDIO AUTOMATION

1. **Connect Channel**: Click **YouTube** in the Header Bar to authorize via Google OAuth 2.0.
2. **Automatic Timestamps & Chapters**: Track titles and timestamps (`00:00 - Track A`) are automatically populated from `_chapters.txt`.
3. **Smart Title & SEO Tags**: Generates high-converting titles and 500 characters of optimized tags 100% offline.
4. **Privacy Status**: Set uploads as `Draft / Private`, `Unlisted`, `Public`, or `Scheduled`.
5. **Auto-Upload**: Enable the auto-upload toggle to automatically send videos to YouTube immediately following render completion.

---

## CHAPTER 7: IN-APP AUTO-UPDATER ENGINE

1. **Silent Detection**: The app quietly checks for updates on startup.
2. **Visual Notification**: When a new version is released, the **Update** button glows in pulsing Flame Orange.
3. **One-Click Upgrade**: Click **Update**, review changelogs, click **Download Update**, and finally click **Install & Restart** for a seamless in-place upgrade.
4. **Zero Data Loss**: Your license and presets remain 100% intact.

---

## CHAPTER 8: TROUBLESHOOTING & FAQ

* **SmartScreen Warning on Install?** Click *More info* -> *Run anyway*. This is expected for new releases.
* **GPU Encoder shows CPU?** Update your NVIDIA GeForce or Intel Graphics drivers to activate hardware acceleration.
* **Moving License to another PC?** Contact support with your proof of purchase to transfer your HWID license.

---

*Copyright (c) 2026 BodeStudio Engineering Team. All rights reserved.*
