# 🎮 Fortnite Sprite Locker

> **Documentation • Customization Guide**

---

<p align="center">

🏠 [README](../README.md) •
🚀 [Installation](INSTALLATION.md) •
🎮 [Usage](USAGE.md) •
✨ [Features](FEATURES.md) •
📤 [Share & Export](SHARE_AND_EXPORT.md) •
🎨 **Customization** •
📂 [Project Structure](PROJECT_STRUCTURE.md) •
⚙️ [Technical](TECHNICAL.md) •
❓ [FAQ](FAQ.md) •
🗺️ [Roadmap](ROADMAP.md)

</p>

---

# 🎨 Customization Guide

Fortnite Sprite Locker has been designed to be easily customizable.

Whether you want to add new Sprites, introduce future Fortnite seasons, change the visual style, or adapt the project for another collectible system, every major component can be modified independently.

No build tools or frameworks are required.

Everything is contained inside a single HTML application with external assets.

---

# 📚 Contents

- Adding Sprites
- Adding Variants
- Replacing Images
- Editing Rarity Colors
- Customizing the Interface
- Editing Statistics
- Background Music
- Preparing Future Seasons
- Best Practices

---

# 🆕 Adding New Sprites

Adding a new Sprite only requires two steps.

1. Add the Sprite object inside the JavaScript data array.
2. Add the corresponding images inside:

```text
assets/sprites/
```

A typical Sprite contains:

- Name
- Rarity
- Passive Ability
- Available Variants
- Spawn Rates
- Internal ID

Once added, the application automatically includes it in:

- Sidebar
- Locker View
- Grid View
- Statistics
- Export
- Share Collection

No additional configuration is required.

---

## Naming Convention

Every Sprite should use a unique identifier.

Example:

```text
water
fire
earth
storm
```

Avoid spaces and special characters.

---

# 🖼️ Sprite Images

Each Sprite image should follow the naming convention used throughout the project.

Example:

```text
water_basic.png

water_gold.png

water_gummy.png

water_galaxy.png

water_holo.png

water_cube.png

water_gem.png
```

The application automatically loads images using these filenames.

Changing the naming convention requires updating the image loading logic.

---

## Image Format

Recommended format:

| Property | Value |
|----------|-------|
| Format | PNG |
| Background | Transparent |
| Resolution | 512×512 or higher |
| Aspect Ratio | 1:1 |

Transparent backgrounds provide the best visual integration with the rarity cards.

---

# 🌈 Adding New Variants

Variants are defined inside each Sprite object.

Example:

```javascript
variants: [
    "basic",
    "gold",
    "galaxy"
]
```

Every new variant should include:

- Image
- Display name
- Button color
- Internal identifier

If additional logic is required, update the variant rendering system accordingly.

---

## Variant Colors

Each variant has an associated button style.

Current variants include:

| Variant | Theme |
|----------|-------|
| Basic | Gray |
| Gold | Gold |
| Gummy | Pink |
| Galaxy | Blue |
| Holofoil | Cyan |
| Cube | Purple |
| Gem | White |

Additional colors can be added by extending the CSS.

---

# ⭐ Editing Rarities

Rarity colors are controlled through CSS classes.

Typical rarity classes include:

```text
rarity-common

rarity-rare

rarity-epic

rarity-legendary

rarity-mythic
```

Each class controls:

- Border color
- Background
- Hover glow
- Shadows
- Accent colors

Changing these values immediately affects both Locker View and Grid View.

---

# 🎨 Customizing the Interface

The application's appearance can be modified without touching the JavaScript logic.

Most visual changes are controlled by CSS.

Examples include:

- Colors
- Fonts
- Buttons
- Panels
- Animations
- Shadows
- Rounded corners
- Spacing

This separation allows developers to redesign the interface while preserving functionality.

---

## Theme Colors

Most interface colors are grouped together, making global theme changes straightforward.

You can easily create:

- Light Theme
- Dark Theme
- Custom Fortnite Themes
- Seasonal Themes

---

# 🔊 Background Music

Background music can be replaced by simply changing the audio file inside:

```text
assets/audios/
```

Supported browser audio formats include:

- MP3
- OGG
- WAV

Keep file sizes small to reduce loading times.

---

# 📊 Statistics

Statistics are generated dynamically.

Adding a new Sprite automatically updates:

- Total Sprites
- Completion Percentage
- Missing Sprites
- Collected Variants
- Rarity Statistics

Manual adjustments are generally unnecessary.

---

# 🔍 Search & Filters

Search functionality automatically indexes every Sprite.

When adding new content:

- Search updates automatically.
- Filters continue to work.
- Statistics refresh correctly.

No configuration changes are normally required.

---

# 🚀 Preparing Future Seasons

Fortnite Sprite Locker was designed with future expansion in mind.

Possible improvements include:

- Chapter 7 Season 4
- Additional Sprite families
- Event-exclusive Sprites
- Limited-time variants
- Custom user collections

Keeping Sprite data separate from interface logic makes future updates significantly easier.

---

# 💡 Best Practices

For the best customization experience:

- Keep image filenames consistent.
- Use transparent PNG files.
- Avoid changing internal IDs.
- Backup your project before major edits.
- Test new Sprites in both Locker and Grid View.
- Verify PNG Export after adding assets.

---

# ⚠️ Common Mistakes

### Missing Images

If an image cannot be found, the application may display a placeholder or fallback image.

Ensure every filename matches the expected naming convention exactly.

---

### Duplicate IDs

Never reuse an existing Sprite ID.

Duplicate identifiers can cause incorrect statistics and broken save data.

---

### Broken Variants

If a variant button appears but no image loads:

- Verify the filename.
- Check the variant ID.
- Confirm the image exists in the correct folder.

---

# 📚 Related Documentation

- ✨ [Features](FEATURES.md)
- 🎮 [Usage](USAGE.md)
- 📂 [Project Structure](PROJECT_STRUCTURE.md)
- ⚙️ [Technical](TECHNICAL.md)

---

<div align="center">

**Customize it. Expand it. Make it your own.**

</div>