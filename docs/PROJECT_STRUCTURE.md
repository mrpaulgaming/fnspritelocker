# 🎮 Fortnite Sprite Locker

> **Documentation • Project Structure**

---

<p align="center">

🏠 [README](../README.md) •
🚀 [Installation](INSTALLATION.md) •
🎮 [Usage](USAGE.md) •
✨ [Features](FEATURES.md) •
📤 [Share & Export](SHARE_AND_EXPORT.md) •
🎨 [Customization](CUSTOMIZATION.md) •
📂 **Project Structure** •
⚙️ [Technical](TECHNICAL.md) •
❓ [FAQ](FAQ.md) •
🗺️ [Roadmap](ROADMAP.md)

</p>

---

# 📂 Project Structure

This document explains the purpose of every important folder and file included in Fortnite Sprite Locker.

Understanding the project organization makes it much easier to customize, maintain and extend the application.

---

# 📚 Contents

- Root Directory
- Assets Folder
- Documentation
- Screenshots
- Main Application
- Data Organization
- File Naming Conventions
- Recommended Structure
- Best Practices

---

# 🌳 Complete Structure

```text
fortnite-sprite-locker/
│
├── README.md
├── README.it.md
├── LICENSE
├── CONTRIBUTING.md
├── CHANGELOG.md
│
├── index.html
│
├── assets/
│   ├── sprites/
│   ├── icons/
│   ├── ui/
│   └── audios/
│
├── screenshots/
│
└── docs/
    ├── FEATURES.md
    ├── INSTALLATION.md
    ├── USAGE.md
    ├── SHARE_AND_EXPORT.md
    ├── CUSTOMIZATION.md
    ├── PROJECT_STRUCTURE.md
    ├── TECHNICAL.md
    ├── FAQ.md
    ├── ROADMAP.md
    └── CHANGELOG.md
```

---

# 📄 Root Directory

The root directory contains the files required to run and document the project.

| File | Purpose |
|------|---------|
| `index.html` | Main application |
| `README.md` | Main documentation |
| `README.it.md` | Italian documentation |
| `LICENSE` | Project license |
| `CONTRIBUTING.md` | Contribution guidelines |

Only `index.html` is required to run the application.

---

# 🖥️ Main Application

The entire application lives inside:

```text
index.html
```

It contains:

- HTML structure
- CSS styles
- JavaScript logic
- Rendering engine
- LocalStorage management
- Export system
- Share system

This design keeps deployment extremely simple.

---

# 🎨 assets/

The `assets` directory contains every resource used by the application.

```text
assets/

├── sprites/
├── icons/
├── ui/
└── audios/
```

---

## 🖼️ sprites/

Contains every Sprite image.

Typical files:

```text
water_basic.png
water_gold.png
water_gummy.png
water_galaxy.png
water_holo.png
water_cube.png
water_gem.png
```

Every Sprite variant is stored independently.

Transparent PNG images are recommended.

---

## 🎯 icons/

Contains interface icons.

Examples include:

- Logo
- Favicon
- Buttons
- Small UI icons

These assets are reused throughout the application.

---

## 🎨 ui/

Contains visual interface resources.

Typical assets include:

- Backgrounds
- Decorative elements
- Crowns
- Panels
- UI textures

Keeping these assets separate improves project organization.

---

## 🎵 audios/

Stores optional background music.

Supported formats include:

- MP3
- OGG
- WAV

Audio files should be optimized for quick loading.

---

# 📸 screenshots/

This folder is dedicated exclusively to documentation.

Example:

```text
screenshots/

main-interface.png

locker-view.png

grid-view.png

filters.png

statistics.png

export.png

share.png

mobile.png
```

These images are referenced inside the README and documentation.

They are **not** used by the application itself.

---

# 📚 docs/

The `docs` folder contains the complete project documentation.

| File | Description |
|------|-------------|
| FEATURES.md | Complete feature overview |
| INSTALLATION.md | Installation guide |
| USAGE.md | User guide |
| SHARE_AND_EXPORT.md | Export & sharing |
| CUSTOMIZATION.md | Customization guide |
| PROJECT_STRUCTURE.md | This document |
| TECHNICAL.md | Technical documentation |
| FAQ.md | Frequently Asked Questions |
| ROADMAP.md | Planned improvements |
| CHANGELOG.md | Version history |

---

# 🗂️ Data Organization

Sprite information should remain separated from visual assets.

```
Sprite Data

↓

Rendering

↓

Images

↓

User Interface
```

Separating responsibilities makes future updates significantly easier.

---

# 🏷️ Naming Conventions

The project follows consistent naming rules.

Folders:

```text
assets

screenshots

docs
```

Images:

```text
water_basic.png

water_gold.png

storm_galaxy.png
```

Documentation:

```text
FEATURES.md

TECHNICAL.md

USAGE.md
```

Using consistent names makes maintenance easier.

---

# 🧹 Keeping the Project Organized

When adding new content:

✅ Place Sprite artwork inside `assets/sprites`

✅ Place documentation images inside `screenshots`

✅ Keep Markdown files inside `docs`

✅ Avoid mixing application assets with documentation assets

A clean folder structure helps contributors quickly understand the project.

---

# 🚀 Recommended Workflow

When introducing a new Sprite:

```
Create Sprite Data

↓

Add Images

↓

Test Rendering

↓

Verify Statistics

↓

Test Export

↓

Update Documentation
```

Following the same workflow helps reduce bugs and keeps the project consistent.

---

# 💡 Best Practices

- Keep assets organized by purpose.
- Use descriptive filenames.
- Remove unused images.
- Compress PNG files when possible.
- Avoid duplicate assets.
- Keep documentation updated when adding new features.

---

<div align="center">

**A well-organized project is easier to understand, maintain and expand.**

</div>