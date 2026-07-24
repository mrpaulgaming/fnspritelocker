# 🎮 Fortnite Sprite Locker

> **Documentation • Technical Documentation**

---

<p align="center">

🏠 [README](../README.md) •
🚀 [Installation](INSTALLATION.md) •
🎮 [Usage](USAGE.md) •
✨ [Features](FEATURES.md) •
⚙️ **Technical**

</p>

---

# ⚙️ Technical Documentation

This document explains the internal architecture of Fortnite Sprite Locker.

It is intended for developers who want to understand how the application works, contribute to the project or customize its behavior.

Unlike the user guides, this document focuses on the implementation rather than the interface.

---

# 📚 Contents

- Application Architecture
- Data Flow
- Rendering Engine
- State Management
- LocalStorage
- Image Loading
- Statistics Engine
- Export System
- Share Collection
- Performance Optimizations
- Browser Compatibility
- Future Improvements

---

# 🏗️ Application Architecture

Fortnite Sprite Locker is a **Single Page Application (SPA)** built without frameworks.

Everything runs inside a single HTML document.

```
Browser

↓

index.html

↓

CSS
JavaScript

↓

User Interface

↓

LocalStorage
```

The application does not require:

- Node.js
- npm
- React
- Vue
- Angular
- Backend servers
- Databases

This keeps deployment extremely simple.

---

# 📂 Project Organization

The application is divided into logical components.

```
Application

├── Data
├── Rendering
├── Events
├── Statistics
├── Export
├── Sharing
├── Storage
└── UI
```

Each module has a specific responsibility.

---

# 📦 Data Layer

Sprite information is stored as JavaScript objects.

Each object contains all information required to render the interface.

Typical properties include:

- ID
- Name
- Artwork
- Passive Ability
- Rarity
- Variants
- Spawn Rates

This data acts as the application's "database".

---

# 🔄 Application Flow

The application's lifecycle is straightforward.

```
Page loads

↓

Load Sprite Data

↓

Load LocalStorage

↓

Merge Saved Progress

↓

Render Interface

↓

Wait for User Input

↓

Update State

↓

Save Automatically

↓

Re-render Changed Components
```

Only the necessary parts of the interface are refreshed after each action.

---

# 🎨 Rendering Engine

Rendering is entirely dynamic.

Whenever the user performs an action:

- DOM elements are updated.
- Statistics refresh.
- Progress bars animate.
- Sidebar indicators change.
- Export data is refreshed.

The page never reloads.

---

## Incremental Updates

Instead of rebuilding the entire interface, only affected components are refreshed.

Examples:

Changing a variant updates:

- Current Sprite
- Statistics
- Sidebar
- Progress bars

Grid View updates only visible cards.

This minimizes unnecessary DOM operations.

---

# 🧠 State Management

The application's state consists of:

- Owned variants
- Mastered Sprites
- Selected Sprite
- Filters
- View mode
- User preferences

Whenever a value changes:

```
User Action

↓

State Update

↓

Interface Update

↓

LocalStorage Save
```

This guarantees consistency throughout the application.

---

# 💾 LocalStorage

Persistent data is stored using the browser's LocalStorage API.

Advantages include:

- Offline support
- Fast access
- No server required
- Automatic saving

Typical stored data:

```
{
    variants,
    mastered,
    filters,
    layout,
    preferences
}
```

The application restores this data automatically when opened again.

---

# 🖼️ Image Loading

Images are loaded dynamically.

```
Sprite ID

↓

Variant

↓

Filename

↓

assets/sprites/

↓

Display
```

Example:

```
water

↓

gold

↓

water_gold.png
```

Fallback images may be displayed if a file is missing.

---

# 📊 Statistics Engine

Statistics are calculated dynamically.

No values are permanently stored.

Whenever data changes:

```
Owned Variants

↓

Recalculate

↓

Update Statistics

↓

Render Progress
```

Examples:

- Total completion
- Missing Sprites
- Missing variants
- Completion by rarity
- Mastered Sprites

---

# 📤 Export System

PNG Export is generated using **html2canvas**.

Workflow:

```
Current Interface

↓

Temporary Export Layout

↓

html2canvas

↓

PNG Image

↓

Download
```

The export system automatically scales content for improved image quality.

---

# 🔗 Share Collection

The Share Collection feature works entirely offline.

Workflow:

```
Collection Data

↓

JSON

↓

Encode

↓

URL

↓

Clipboard
```

When another user opens the link:

```
URL

↓

Decode

↓

Restore Data

↓

Render Collection
```

No external servers are involved.

---

# ⚡ Performance Optimizations

Several optimizations have been implemented.

## Lazy Updates

Only affected UI components are refreshed.

---

## Efficient Rendering

DOM modifications are minimized.

---

## Automatic Saving

Saving occurs only when necessary.

---

## Lightweight Assets

PNG assets are optimized for quick loading.

---

## No Framework Overhead

Because the application uses vanilla JavaScript, startup time remains extremely fast.

---

# 🌐 Browser Compatibility

Fortnite Sprite Locker supports every modern browser.

| Browser | Supported |
|-----------|-----------|
| Chrome | ✅ |
| Edge | ✅ |
| Firefox | ✅ |
| Opera | ✅ |
| Safari | ✅ |

Older browsers may lack support for certain modern JavaScript features.

---

# 🔒 Privacy

User data never leaves the browser.

No analytics.

No accounts.

No tracking.

No cloud synchronization.

Every collection remains entirely local unless explicitly shared.

---

# 🚀 Future Improvements

Possible technical improvements include:

- Service Worker
- Progressive Web App
- IndexedDB support
- Cloud synchronization
- Dynamic asset loading
- Modular JavaScript architecture

These improvements are being evaluated for future releases.

---

# 💡 Developer Tips

If you plan to contribute:

- Keep rendering functions independent.
- Avoid hardcoding Sprite data.
- Reuse existing utility functions.
- Preserve naming conventions.
- Test both Locker View and Grid View.
- Verify exports before committing.

---

# 📚 Related Documentation

- ✨ [Features](FEATURES.md)
- 🎮 [Usage](USAGE.md)
- 🎨 [Customization](CUSTOMIZATION.md)
- 📂 [Project Structure](PROJECT_STRUCTURE.md)

---

<div align="center">

**Built with simplicity, optimized for performance.**

</div>