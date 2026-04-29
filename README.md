<p align="center">
  <img width="1070" height="559" alt="112f942f1b8c81f2785f5446ef8026bd" src="https://github.com/user-attachments/assets/d95e4b4c-a78b-42c8-a040-e158c1ed04fe" />
</p>

```text
███╗   ██╗███████╗████████╗███████╗██╗███╗   ██╗
████╗  ██║██╔════╝╚══██╔══╝██╔════╝██║████╗  ██║
██╔██╗ ██║█████╗     ██║   █████╗  ██║██╔██╗ ██║
██║╚██╗██║██╔══╝     ██║   ██╔══╝  ██║██║╚██╗██║
██║ ╚████║███████╗   ██║   ██║     ██║██║ ╚████║
╚═╝  ╚═══╝╚══════╝   ╚═╝   ╚═╝     ╚═╝╚═╝  ╚═══╝
```

<p align="center">
  <img src="https://img.shields.io/github/stars/ya0903/NetFin?style=for-the-badge&color=E50914&labelColor=0b0b0b&logo=github&logoColor=white" alt="GitHub Stars" />
  <img src="https://img.shields.io/badge/Jellyfin-10.9%2B-0b0b0b?style=for-the-badge&labelColor=000000&color=2b2b2b" alt="Jellyfin 10.9+" />
  <img src="https://img.shields.io/badge/Type-Theme-E50914?style=for-the-badge&labelColor=000000&color=E50914" alt="Theme Type" />
</p>

# 🎬 NetFin Theme for Jellyfin

<p align="center">
  <img src="https://img.shields.io/badge/Jellyfin-Theme-0f1117?style=for-the-badge" alt="Jellyfin Theme" />
  <img src="https://img.shields.io/badge/Style-Cinematic-darkred?style=for-the-badge" alt="Cinematic Style" />
  <img src="https://img.shields.io/badge/UI-Modern-black?style=for-the-badge" alt="Modern UI" />
</p>

A sleek cinematic Jellyfin theme inspired by modern streaming platforms.  
NetFin focuses on immersion, clarity and smooth visual flow while keeping media artwork as the centrepiece of the interface.

Designed for users who want Jellyfin to feel like a premium streaming service.

---

## 🎨 Theme Colour Palette

<p align="center">
  <img src="https://placehold.co/120x40/000000/000000.png" alt="#000000" />
  <img src="https://placehold.co/120x40/0d0d0d/0d0d0d.png" alt="#0d0d0d" />
  <img src="https://placehold.co/120x40/1a0000/1a0000.png" alt="#1a0000" />
  <img src="https://placehold.co/120x40/660000/660000.png" alt="#660000" />
  <img src="https://placehold.co/120x40/cc0000/cc0000.png" alt="#cc0000" />
  <img src="https://placehold.co/120x40/ffffff/ffffff.png" alt="#ffffff" />
</p>

<p align="center">
  <sub>Primary tones used throughout NetFin, black, deep charcoal, dark crimson, red accent and clean white text.</sub>
</p>

---

## ✨ Overview

NetFin transforms Jellyfin with:

- 🎥 Deep cinematic dark visuals  
- 🧭 Clean modern layouts  
- ✨ Smooth refined hover effects  
- 📐 Balanced spacing across all screens  
- 🔍 Improved readability for titles and metadata  
- 🧼 Minimal clutter for distraction-free browsing  

The result is an elegant, professional interface that enhances both browsing and playback.

---

## 🧩 Key Features

- 🏠 Modernised home and library layouts  
- 🎞 Smooth poster scaling and hover animations  
- 🎬 Enhanced film and TV show detail pages  
- 🧭 Clean navigation bars and side menus  
- ✍ Consistent typography across all devices  
- 🎮 Refined buttons and playback controls  
- 🌗 Improved contrast for metadata visibility  
- 🔗 Unified design language across phone, desktop and TV  

---

## ⚙ Installation

Paste this into **Jellyfin → Dashboard → General → Custom CSS**

```css
@import url("https://cdn.jsdelivr.net/gh/ya0903/NetFin@main/netfin.css");
```

---

## 🖼 Theme Showcase

NOTE: Screenshots contain mediabar plugin and others you can find on **[Awesome Jellyfin](https://github.com/awesome-jellyfin/awesome-jellyfin)**

<details open>
<summary><strong>🔒 Login Screen</strong></summary>

<br>

![Login Screen](https://github.com/user-attachments/assets/69d1e032-e99e-4fdf-af4e-428d7e81252b)

</details>

<details>
<summary><strong>🏠 Home Interface</strong></summary>

<br>

![Home Interface](https://github.com/user-attachments/assets/5eee060a-0c1d-4ab3-8b64-027251973997)

</details>

<details>
<summary><strong>🎞 Library View</strong></summary>

<br>

![Library View](https://github.com/user-attachments/assets/adc6ae25-6687-43b9-aa19-3319794c297b)

</details>

<details>
<summary><strong>🎬 Movie Detail Page</strong></summary>

<br>

![Movie Detail Page 1](https://github.com/user-attachments/assets/192bd752-be1a-462d-a9f2-088f61940f4a)

<br>

![Movie Detail Page 2](https://github.com/user-attachments/assets/93e86e2a-cc57-4af8-9eee-288b975c6ed9)

</details>

<details>
<summary><strong>📂 Sidebar</strong></summary>

<br>

![Sidebar](https://github.com/user-attachments/assets/ee968d48-94dd-4ada-ba43-e83533cc9159)

</details>

---
## 🧪 Experimental Add-Ons

These are optional tweaks you can paste **after** the main NetFin import in Jellyfin’s **Custom CSS** box.

<details>
<summary><strong>Replace the Jellyfin logo with a custom logo</strong></summary>

<br>

This add-on hides the default Jellyfin logo and swaps it for your own image in the header area.

```css
/* Paste this after the NetFin import */

/* Hide default header logo assets */
.headerLogo img,
.headerLogo-withBackground img,
.logoImage,
.headerLogo svg {
  display: none !important;
}

/* Remove any existing pseudo-logo */
.headerLogo::after,
.headerLogo-withBackground::after {
  display: none !important;
}

/* Prepare the title container — NOT during playback */
:not(.osdHeader) .pageTitle,
:not(.osdHeader) .pageTitleWithDefaultLogo,
:not(.osdHeader) .pageTitleWithLogo {
  display: inline-flex !important;
  visibility: visible !important;
  align-items: center !important;
  font-size: 0 !important;
  line-height: 1 !important;
  overflow: visible !important;
  min-height: 1.8em !important;
  margin-left: 8px !important;  /* ← shift whole logo LEFT/RIGHT */
  margin-top: 0px !important;   /* ← shift whole logo UP/DOWN */
  min-width: max-content !important;
  animation: none !important;
  text-shadow: none !important;
  box-shadow: none !important;
  filter: none !important;
}

/* Hide the original title text — NOT during playback */
:not(.osdHeader) .pageTitle > *,
:not(.osdHeader) .pageTitleWithDefaultLogo > *,
:not(.osdHeader) .pageTitleWithLogo > * {
  display: none !important;
}

/* Custom logo image — NOT during playback */
:not(.osdHeader) .pageTitle::before,
:not(.osdHeader) .pageTitleWithDefaultLogo::before,
:not(.osdHeader) .pageTitleWithLogo::before {
  content: "" !important;
  display: inline-block !important;
  width: 150px !important;   /* ← logo width */
  height: 40px !important;   /* ← logo height */
  position: relative !important;
  top: 0px !important;       /* ← fine-tune vertical (+down / -up) */
  left: 0px !important;      /* ← fine-tune horizontal (+right / -left) */
  background: url("PASTE-YOUR-LOGO-URL-HERE") center / contain no-repeat !important;
  animation: none !important;
  text-shadow: none !important;
  box-shadow: none !important;
  filter: none !important;
}

/* No extra text after logo — NOT during playback */
:not(.osdHeader) .pageTitle::after,
:not(.osdHeader) .pageTitleWithDefaultLogo::after,
:not(.osdHeader) .pageTitleWithLogo::after {
  content: none !important;
  display: none !important;
}

/* ── Restore OSD header title during playback ── */
.osdHeader .pageTitle,
.osdHeader .pageTitleWithDefaultLogo,
.osdHeader .pageTitleWithLogo {
  display: flex !important;
  font-size: unset !important;
  visibility: visible !important;
  min-width: unset !important;
  animation: none !important;
  filter: none !important;
}

.osdHeader .pageTitle > *,
.osdHeader .pageTitleWithDefaultLogo > *,
.osdHeader .pageTitleWithLogo > * {
  display: unset !important;
}

.osdHeader .pageTitle::before,
.osdHeader .pageTitle::after,
.osdHeader .pageTitleWithDefaultLogo::before,
.osdHeader .pageTitleWithDefaultLogo::after,
.osdHeader .pageTitleWithLogo::before,
.osdHeader .pageTitleWithLogo::after {
  content: none !important;
  display: none !important;
}
```

### How to use it

1. Upload your logo somewhere publicly accessible  
2. Replace `PASTE-YOUR-LOGO-URL-HERE` with the direct image link  
3. Paste the CSS **after** your NetFin import  
4. Use top and left to finetune logo position  
5. Save and refresh Jellyfin

NETFIN logo is available in NetFin/assets/netfin-logo - https://raw.githubusercontent.com/ya0903/NetFin/main/Assets/netfin-logo.png

</details>
<details>
<summary><strong>Example Home Screen Preview</strong></summary>

<br>

Below is an example of how NetFin looks on the Jellyfin home screen once installed.

<img width="1920" height="915" alt="image" src="https://github.com/user-attachments/assets/5aa445b8-acf0-4c9f-97a2-fa8020ede0c0" />

</details>

<details>
<summary><strong>Mobile Buttons Size Adjustment</strong></summary>

<br>

This add-on adjusts the size of the touch buttons on mobile devices.

```css
/* ================= MOBILE TOUCH FIX ================= */

  /* Top left menu button */
  .headerButton,
  .headerButton.headerButtonLeft,
  .headerButton.headerButtonRight {
      width: 36px !important;
      height: 36px !important;
      min-width: 36px !important;
      min-height: 36px !important;
      margin: 0 6px !important;
  }

  /* Icons inside header buttons */
  .headerButton i,
  .headerButton .material-icons,
  .headerButton .material-icons-round {
      font-size: 26px !important;
  }

  /* Profile picture tap area */
  .headerUserButton {
      width: 36px !important;
      height: 36px !important;
  }

  .headerUserButton img {
      width: 36px !important;
      height: 36px !important;
  }

  /* Cast & group watch buttons */
  .headerCastButton,
  .headerSyncButton {
      width: 36px !important;
      height: 36px !important;
  }
```
### How to use it
1. Copy and paste underneath NetFin import
2. Adjust px for each according to your tastes
3. Save and refresh Jellyfin

</details>

## 🙏 Credits & Inspiration

NetFin is heavily inspired by the incredible work of  
✨ **[ElegantFin by lscambo13](https://github.com/lscambo13/ElegantFin)**

ElegantFin set the benchmark for modern Jellyfin theming by refining layout structure, spacing consistency and overall UI polish across devices.

NetFin builds upon those design principles while introducing its own darker cinematic styling and visual identity.

If you enjoy NetFin, consider supporting the ElegantFin project.

⭐ If you use NetFin, consider starring the repository to support development.
---
Any requests please create an issue thank you

### 🎥 Enjoy your media in cinematic style with NetFin
