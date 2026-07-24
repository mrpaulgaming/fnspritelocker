# ✨ Features

> Comprehensive overview of every feature available in **Fortnite Sprite Locker**.

---

## 📖 Overview

Fortnite Sprite Locker is a fully offline web application designed to help Fortnite players organize, track and share their Sprite collection from **Chapter 7 • Season 3**.

Unlike a simple checklist, the application provides a complete collection management experience inspired by Fortnite's official Locker interface.

The project combines a modern user interface, automatic saving, advanced statistics and multiple export options into a lightweight single-page application that runs directly inside your browser.

> 💡 **Tip**
>
> Looking for installation instructions?
> See **INSTALLATION.md**.

---

# 🗂️ Collection Management

Collection Management is the core of Fortnite Sprite Locker.

Every Sprite can be individually tracked, completed and managed without requiring an online account or external database.

The application automatically stores every modification inside your browser using LocalStorage.

Main capabilities include:

- Track every available Sprite
- Manage every available variant
- View completion progress
- Mark Sprites as Mastered
- Automatically save every change
- Restore previous backups
- Share collections using a single URL

---

## 🎮 Sprite Tracking

Each Sprite has its own dedicated page containing every important piece of information.

Displayed information includes:

| Property | Description |
|----------|-------------|
| Name | Official Sprite name |
| Artwork | Main Sprite artwork |
| Rarity | Current rarity |
| Passive Ability | Sprite passive effect |
| Variants | Available collectible variants |
| Spawn Rates | Variant drop chances |
| Completion | Individual progress |
| Mastered | Personal completion flag |

Every Sprite updates independently from the others.

---

### Completion Status

Each Sprite can be in one of several states.

| State | Description |
|-------|-------------|
| Not Started | No variants collected |
| In Progress | At least one variant collected |
| Completed | Every available variant collected |
| Mastered | Manually marked as completed by the user |

The application automatically updates these states whenever variants are added or removed.

---

### Automatic Progress Calculation

Progress is calculated in real time.

Whenever the user changes a variant:

- Sprite completion updates
- Statistics refresh
- Progress bars animate
- Overall completion percentage changes
- LocalStorage is updated automatically

No manual save button is required.

---

# 🎨 Variant System

Variants represent different collectible versions of the same Sprite.

Every Sprite may contain multiple variants.

Currently supported variant types include:

| Variant | Description |
|----------|-------------|
| Basic | Default Sprite |
| Gold | Golden version |
| Gummy | Candy-themed version |
| Galaxy | Cosmic appearance |
| Holofoil | Holographic finish |
| Cube | Cube-inspired version |
| Gem | Crystal variant |

Each variant includes:

- Dedicated artwork
- Spawn rate
- Bonus description
- Individual ownership status

---

## 🖼️ Variant Preview

Hovering a variant automatically previews its artwork without permanently changing the selected Sprite.

This allows players to quickly inspect every available appearance before selecting it.

> 📝 **Note**
>
> Preview images automatically revert back when the pointer leaves the variant button.

---

## ⭐ Mastery System

The Mastery System provides an additional personal milestone beyond simple completion.

Once enabled, a Sprite displays a dedicated crown icon indicating that the player considers it fully mastered.

Mastery is completely independent from variant ownership.

For example:

| Variants | Mastered | Result |
|----------|----------|--------|
| 100% | ❌ | Completed |
| 100% | ✅ | Mastered |
| 60% | ✅ | Personal milestone |

This allows players to define their own collection goals.

---

## 📊 Progress Tracking

Every action performed inside the application immediately updates global statistics.

Tracked information includes:

- Collected Sprites
- Missing Sprites
- Collected Variants
- Missing Variants
- Mastered Sprites
- Overall Completion
- Completion by Rarity

Progress bars animate smoothly after every update, providing immediate visual feedback.

---

# 🖥️ User Interface

The user interface has been carefully designed to recreate the look and feel of Fortnite while remaining lightweight, intuitive and responsive.

Unlike many traditional collection trackers, Fortnite Sprite Locker focuses on minimizing the number of clicks required to manage your collection.

Every major action can be completed within a few seconds.

---

## 🎨 Fortnite-inspired Design

The visual appearance of the application is heavily inspired by Fortnite's Locker.

Some design elements include:

- Fortnite color palette
- Rounded panels
- Animated buttons
- Glow effects
- Smooth transitions
- Dynamic rarity colors
- High-contrast interface
- Responsive layout

The objective is to make the application feel like a natural extension of the game itself.

---

## 🏠 Main Layout

The interface is divided into several logical areas.

```text
+-----------------------------------------------------------+
| Header                                                    |
| Logo | Search | Filters | Share | Menu                    |
+----------------------+------------------------------------+
| Sidebar              |                                    |
| Sprite List          |        Locker / Grid View          |
|                      |                                    |
|                      |                                    |
+----------------------+------------------------------------+
| Statistics Bar                                           |
+-----------------------------------------------------------+
```

Each section has a specific purpose and automatically updates whenever the collection changes.

---

## 📌 Header

The header provides quick access to the application's most important tools.

Available controls include:

| Control | Purpose |
|----------|---------|
| Search | Find Sprites instantly |
| Filters | Display only specific Sprites |
| Share | Generate a shareable collection link |
| Menu | Export, Import and Settings |
| Layout Toggle | Switch between Locker and Grid View |

The header remains accessible throughout the entire application.

---

## 📂 Sidebar

The sidebar contains the complete Sprite list.

Features include:

- Quick navigation
- Completion indicators
- Mastered indicators
- Selected Sprite highlighting
- Smooth scrolling

Selecting a Sprite immediately updates the main content area.

> 💡 **Tip**
>
> The sidebar automatically scrolls to keep the selected Sprite visible.

---

# 📦 Locker View

Locker View is the primary way to inspect individual Sprites.

Unlike Grid View, this mode focuses on detailed information.

Every Sprite card contains:

- Official artwork
- Sprite name
- Passive ability
- Rarity
- Variant selector
- Completion percentage
- Spawn rates
- Mastered status

---

## 🖼️ Artwork Preview

The artwork section automatically updates according to the selected variant.

For example:

```text
Water Sprite

Basic
⬇

Image changes

⬇

Galaxy

Image changes again
```

Hovering over a variant previews it instantly without modifying your collection.

---

## 🎭 Variant Buttons

Variant buttons provide quick access to every available appearance.

Supported colors include:

| Variant | Button Color |
|----------|--------------|
| Basic | Gray |
| Gold | Gold |
| Gummy | Pink |
| Galaxy | Blue |
| Holofoil | Cyan |
| Cube | Purple |
| Gem | White |

Every button updates automatically depending on ownership.

---

## ⭐ Mastered Indicator

Sprites marked as Mastered display a dedicated visual indicator.

Benefits include:

- Easy identification
- Improved collection overview
- Statistics integration
- Sidebar indicator

Mastered status can be toggled independently from variant ownership.

---

## 📊 Completion Bar

Every Sprite includes an animated progress bar.

The bar updates automatically whenever:

- a variant is collected;
- a variant is removed;
- hidden variants become available.

Animations are intentionally subtle to keep the interface responsive.

---

# 🔲 Grid View

Grid View offers a compact overview of the entire collection.

Instead of displaying one Sprite at a time, every Sprite is shown simultaneously.

This layout is ideal for:

- browsing the collection;
- checking completion status;
- comparing rarities;
- locating missing Sprites.

---

## 🧩 Grid Cards

Each card contains:

- Artwork
- Name
- Completion percentage
- Mastered indicator
- Rarity background

Cards automatically resize depending on screen size.

---

## 🌈 Dynamic Rarity Colors

Each rarity has its own visual identity.

| Rarity | Theme |
|---------|-------|
| Rare | Blue |
| Epic | Purple |
| Legendary | Orange |
| Mythic | Gold |

Both the border and background adapt automatically.

Hover effects also change according to rarity.

---

## 📱 Responsive Grid

The number of columns changes automatically.

Example:

| Device | Columns |
|----------|---------|
| Desktop | 5–7 |
| Tablet | 3–4 |
| Mobile | 2 |

No manual resizing is required.

---

## ⚡ Performance

Only the visible cards are updated when changes occur.

This minimizes unnecessary DOM operations and keeps animations smooth even with large collections.

---

# 🎯 User Experience

Several quality-of-life improvements have been implemented throughout the application.

Highlights include:

- Instant visual feedback
- Automatic saving
- Smooth animations
- Minimal clicks
- Responsive layout
- Consistent color system
- Fast navigation
- Clear information hierarchy

The goal is to make managing a Sprite collection as enjoyable as collecting the Sprites themselves.

---