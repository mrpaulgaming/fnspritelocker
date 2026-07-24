# 🎮 Fortnite Sprite Locker

> **Documentation • Usage Documentation**

---

<p align="center">

🏠 [README](../README.md) •
🚀 [Installation](INSTALLATION.md) •
🎮 **Usage** •
✨ [Features](FEATURES.md) •
📤 [Share & Export](SHARE_AND_EXPORT.md) •
🎨 [Customization](CUSTOMIZATION.md) •
📂 [Project Structure](PROJECT_STRUCTURE.md) •
⚙️ [Technical](TECHNICAL.md) •
❓ [FAQ](FAQ.md) •
🗺️ [Roadmap](ROADMAP.md)

</p>

---


# 📖 Overview

Fortnite Sprite Locker is designed to be simple enough for new users while providing advanced features for dedicated collectors.

Everything happens inside a single page, allowing you to navigate, manage and export your collection without ever leaving the application.

No installation, login or internet connection is required.

---

## 📚 In This Guide

This document covers:

- Navigating the interface
- Managing your Sprite collection
- Collecting variants
- Using filters and search
- Tracking your progress
- Exporting and sharing
- Backing up your collection

> 💡 **Tip**
>
> Looking for a detailed explanation of every feature?
> See **FEATURES.md**.

---

# 🚀 Getting Started

Using Fortnite Sprite Locker only takes a few seconds.

1. Open **index.html** in your browser.
2. Wait for the application to load.
3. Select a Sprite from the sidebar.
4. Start tracking your collection.

Your progress is automatically saved.

No setup is required.

---

# 🗂️ Managing Your Collection

Collection management is the primary purpose of Fortnite Sprite Locker.

Each Sprite can be individually tracked and customized.

---

## Selecting a Sprite

Choose any Sprite from the left sidebar.

The main panel immediately updates with:

- Sprite artwork
- Passive ability
- Available variants
- Spawn rates
- Completion progress
- Mastery status

---

## Collecting Variants

Every Sprite includes one or more collectible variants.

To mark a variant as collected:

1. Select the desired Sprite.
2. Locate the Variant section.
3. Click the desired variant.
4. The application instantly updates your collection.

Collected variants are highlighted automatically.

---

## Removing Variants

Variants can be removed at any time.

Simply click an owned variant again.

The following elements update automatically:

- Completion percentage
- Statistics
- Progress bars
- Overall completion
- Saved data

No confirmation dialog is required.

---

# ⭐ Mastering a Sprite

Mastery is a personal milestone.

Unlike variant ownership, it is completely optional.

To mark a Sprite as Mastered:

1. Open the Sprite.
2. Enable the **Mastered** option.
3. A crown icon will appear.

Mastered Sprites are also highlighted throughout the application.

---

# 🖥️ Navigating the Interface

Fortnite Sprite Locker offers two viewing modes.

---

## Locker View

Locker View displays detailed information for one Sprite at a time.

Ideal for:

- Reading abilities
- Viewing variants
- Managing completion
- Inspecting artwork

---

## Grid View

Grid View displays every Sprite simultaneously.

Useful when you want to:

- Compare progress
- Browse rarities
- Locate missing Sprites
- View your entire collection

Switch between the two layouts using the Layout button.

---

# 🔍 Search

Searching is instant.

Simply type part of a Sprite name into the search box.

Matching Sprites are displayed immediately.

The search updates as you type.

Examples:

```text
water

↓

Water Sprite

Crystal Water Sprite
```

Search is not case-sensitive.

---

# 🎯 Filters

Filters allow you to display only the Sprites you're interested in.

Available filters include:

| Filter | Description |
|----------|-------------|
| Rarity | Display specific rarities |
| Hide Completed | Hide fully completed Sprites |
| Hide Mastered | Hide mastered Sprites |
| Show Unreleased | Display unreleased content |
| Group by Rarity | Organize the collection |

Filters can be combined.

Example:

```text
Epic

+

Hide Completed

↓

Only incomplete Epic Sprites
```

---

# 📊 Statistics

The Statistics panel updates automatically.

Displayed information includes:

- Total Sprites
- Collected Sprites
- Missing Sprites
- Mastered Sprites
- Completion Percentage
- Variants Collected
- Progress by Rarity

No manual refresh is necessary.

---

# 💾 Automatic Saving

Every change is automatically saved using LocalStorage.

Saved information includes:

- Collected variants
- Mastered Sprites
- Filters
- View mode
- Preferences

Closing the browser will not erase your progress.

---

# 📤 Exporting Your Collection

The application includes multiple export options.

Available exports:

- Entire Collection
- Missing Sprites
- Current Sprite
- JSON Backup

For a detailed explanation, see **SHARE_AND_EXPORT.md**.

---

# 🔗 Sharing Your Collection

Collections can be shared using a unique URL.

The generated link contains your collection data.

Another user can simply open the link to view your progress.

No account is required.

---

# 📱 Mobile Experience

Fortnite Sprite Locker is fully responsive.

Supported devices include:

| Device | Supported |
|----------|-----------|
| Desktop | ✅ |
| Laptop | ✅ |
| Tablet | ✅ |
| Mobile | ✅ |

The layout automatically adapts to different screen sizes.

---

# 💡 Tips & Best Practices

### Keep regular backups

Although LocalStorage is reliable, exporting a JSON backup is recommended.

---

### Use Grid View for quick browsing

Grid View is significantly faster when searching for missing Sprites.

---

### Use Locker View for detailed management

Locker View provides additional information not visible in Grid View.

---

### Share your progress

Generate a Share Collection link to compare your collection with friends.

---

# ❗ Troubleshooting

## My progress disappeared

Check whether your browser data has been cleared.

If available, restore your collection using a JSON backup.

---

## Images are missing

Verify that every image exists inside:

```text
assets/sprites/
```

---

## Share links do not work

Ensure the complete URL has been copied.

Some messaging applications may shorten long links.

---

## Export fails

Verify that every required image has loaded before exporting.

---

<div align="center">

**Happy Sprite Hunting! 🎮**

</div>