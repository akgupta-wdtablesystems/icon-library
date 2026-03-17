# Icon Library

A unified icon library containing pixel-perfect, scalable SVG assets used across our product ecosystem. This repository supports design consistency, improves developer handoff, and simplifies usage by offering clean folder structures, variants, and clear naming conventions.

---

## Table of Contents

- [Overview](#overview)
- [Folder Structure](#folder-structure)
- [Icon Categories](#icon-categories)
  - [Actions](#actions)
  - [Navigation](#navigation)
  - [Communication](#communication)
  - [Status](#status)
  - [Media](#media)
  - [UI](#ui)
  - [App Icons](#app-icons)
- [Using Icons](#using-icons)
  - [Direct SVG embed](#direct-svg-embed)
  - [As an `<img>` tag](#as-an-img-tag)
  - [CSS background-image](#css-background-image)
- [Manifest File](#manifest-file)
- [Naming Conventions](#naming-conventions)
- [Contributing](#contributing)

---

## Overview

This library was migrated from the `common-ui-v2` repository and serves as the single source of truth for all SVG icon assets. Every icon is:

- **24 × 24 px** viewBox (app icons use **48 × 48 px**)
- Rendered with `stroke="currentColor"` so they inherit the CSS `color` property
- Optimised for crisp rendering at common display sizes (16 px, 20 px, 24 px, 32 px)
- Grouped into logical categories for easy discovery

---

## Folder Structure

```
icon-library/
├── manifest.json               ← machine-readable index of every icon
├── README.md
└── src/
    └── assets/
        ├── icon/               ← app / brand icons (logos, splash)
        │   ├── app-icon.svg
        │   ├── app-icon-dark.svg
        │   ├── app-icon-round.svg
        │   ├── logo.svg
        │   └── logo-light.svg
        └── icons/              ← UI icons, organised by category
            ├── actions/
            ├── communication/
            ├── media/
            ├── navigation/
            ├── status/
            └── ui/
```

---

## Icon Categories

### Actions

> Path: `src/assets/icons/actions/`

| Icon | File | Tags |
|------|------|------|
| ➕ add | `add.svg` | plus, create, new, insert |
| ➖ remove | `remove.svg` | minus, subtract, decrease |
| ✕ close | `close.svg` | x, dismiss, cancel, exit |
| ✔ check | `check.svg` | checkmark, tick, done, confirm |
| 🔍 search | `search.svg` | find, magnifier, lookup |
| ✏️ edit | `edit.svg` | pencil, write, modify |
| 🗑️ delete | `delete.svg` | trash, bin, remove |
| ⬇️ download | `download.svg` | save, export, pull |
| ⬆️ upload | `upload.svg` | send, import, push |
| 📋 copy | `copy.svg` | duplicate, clone, clipboard |
| 🔽 filter | `filter.svg` | funnel, refine, narrow |
| ↕️ sort | `sort.svg` | order, arrange, list |

### Navigation

> Path: `src/assets/icons/navigation/`

| Icon | File | Tags |
|------|------|------|
| 🏠 home | `home.svg` | house, main, dashboard |
| ↑ arrow-up | `arrow-up.svg` | up, north, ascending |
| ↓ arrow-down | `arrow-down.svg` | down, south, descending |
| ← arrow-left | `arrow-left.svg` | left, west, back, previous |
| → arrow-right | `arrow-right.svg` | right, east, forward, next |
| ∧ chevron-up | `chevron-up.svg` | caret, collapse |
| ∨ chevron-down | `chevron-down.svg` | caret, expand, dropdown |
| ‹ chevron-left | `chevron-left.svg` | caret, back, previous |
| › chevron-right | `chevron-right.svg` | caret, forward, next |
| ☰ menu | `menu.svg` | hamburger, nav, sidebar |
| 🔍 search | `search.svg` | find, magnifier, lookup |

### Communication

> Path: `src/assets/icons/communication/`

| Icon | File | Tags |
|------|------|------|
| ✉️ mail | `mail.svg` | email, envelope, inbox |
| 📞 phone | `phone.svg` | call, telephone, contact |
| 💬 message | `message.svg` | chat, bubble, comment |
| 🔔 bell | `bell.svg` | notification, alert, alarm |
| 🔗 share | `share.svg` | send, distribute, broadcast |
| 👤 user | `user.svg` | person, account, profile |
| 👥 users | `users.svg` | people, team, group |

### Status

> Path: `src/assets/icons/status/`

| Icon | File | Tags |
|------|------|------|
| ℹ️ info | `info.svg` | information, help, hint |
| ⚠️ warning | `warning.svg` | alert, caution, danger |
| ❌ error | `error.svg` | fail, invalid, problem |
| ✅ success | `success.svg` | done, complete, confirmed |
| ⏳ loading | `loading.svg` | clock, pending, wait |
| 🔒 lock | `lock.svg` | secure, private, protected |
| 🔓 unlock | `unlock.svg` | open, public, accessible |

### Media

> Path: `src/assets/icons/media/`

| Icon | File | Tags |
|------|------|------|
| ▶️ play | `play.svg` | start, run, video, audio |
| ⏸️ pause | `pause.svg` | halt, wait, hold |
| ⏹️ stop | `stop.svg` | end, finish, halt |
| 🎥 video | `video.svg` | camera, film, record |
| 🖼️ image | `image.svg` | photo, picture, gallery |
| 📶 wifi | `wifi.svg` | wireless, internet, network |

### UI

> Path: `src/assets/icons/ui/`

| Icon | File | Tags |
|------|------|------|
| ⚙️ settings | `settings.svg` | gear, preferences, options |
| ❤️ heart | `heart.svg` | love, like, favorite |
| ⭐ star | `star.svg` | favorite, rating, bookmark |
| 📅 calendar | `calendar.svg` | date, schedule, event |
| 📄 file | `file.svg` | document, page, text |
| 📁 folder | `folder.svg` | directory, collection |
| 🛡️ shield | `shield.svg` | security, protect, safe |
| 🔄 refresh | `refresh.svg` | reload, sync, update |
| 🚫 ban | `ban.svg` | block, prohibit, restrict |
| … more-horizontal | `more-horizontal.svg` | ellipsis, overflow, dots |
| ⋮ more-vertical | `more-vertical.svg` | ellipsis, kebab, dots |

### App Icons

> Path: `src/assets/icon/`

| File | Description |
|------|-------------|
| `app-icon.svg` | Default application icon – rounded-square shape |
| `app-icon-dark.svg` | Dark-mode variant of the application icon |
| `app-icon-round.svg` | Circular variant of the application icon |
| `logo.svg` | Horizontal lockup logo for light backgrounds |
| `logo-light.svg` | Horizontal lockup logo for dark backgrounds |

---

## Using Icons

### Direct SVG embed

Copy the SVG source directly into your HTML for maximum flexibility:

```html
<!-- The icon inherits the text color of its parent element -->
<span style="color: #0066cc;">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"
       fill="none" stroke="currentColor" stroke-width="2"
       stroke-linecap="round" stroke-linejoin="round"
       width="24" height="24">
    <circle cx="11" cy="11" r="8"/>
    <line x1="21" y1="21" x2="16.65" y2="16.65"/>
  </svg>
</span>
```

### As an `<img>` tag

Reference the SVG file directly:

```html
<img src="src/assets/icons/actions/search.svg"
     alt="Search"
     width="24"
     height="24" />
```

> **Note:** When used as `<img>`, `currentColor` will not inherit from CSS. Use the inline embed approach if you need dynamic colour control.

### CSS background-image

```css
.icon-search {
  display: inline-block;
  width: 24px;
  height: 24px;
  background: url('src/assets/icons/actions/search.svg') center / contain no-repeat;
}
```

---

## Manifest File

The [`manifest.json`](./manifest.json) at the root of the repository provides a machine-readable index of every icon. It is intended for use by:

- **Build tools** that auto-generate icon sprite sheets or component imports
- **Design tools** (Figma plugins, Storybook addons) that need to enumerate available assets
- **Documentation generators** that render a live icon catalogue

### Structure

```json
{
  "name": "icon-library",
  "version": "1.0.0",
  "totalIcons": 59,
  "categories": [
    {
      "name": "actions",
      "description": "Icons representing user actions and interactions",
      "path": "src/assets/icons/actions",
      "icons": [
        {
          "name": "add",
          "file": "add.svg",
          "path": "src/assets/icons/actions/add.svg",
          "tags": ["plus", "create", "new", "insert"]
        }
      ]
    }
  ],
  "appIcons": {
    "description": "Application and brand icons",
    "path": "src/assets/icon",
    "icons": [ ... ]
  }
}
```

---

## Naming Conventions

| Rule | Example |
|------|---------|
| All lowercase, hyphen-separated | `arrow-left.svg` ✅  `ArrowLeft.svg` ❌ |
| Descriptive, not decorative | `delete.svg` ✅  `icon-37.svg` ❌ |
| No size suffix in filename | `search.svg` ✅  `search-24.svg` ❌ |
| Variant suffix for alternates | `app-icon-round.svg`, `logo-light.svg` |

---

## Contributing

1. **Add the SVG file** to the appropriate category folder under `src/assets/icons/` (or `src/assets/icon/` for brand/app icons).
2. **Follow the naming conventions** above.
3. **Update `manifest.json`** – add an entry in the correct category, including a meaningful `tags` array.
4. **Ensure the SVG**:
   - Uses `viewBox="0 0 24 24"` (or `48 48` for app icons)
   - Sets `stroke="currentColor"` and `fill="none"` (unless a filled variant is intentional)
   - Does **not** hard-code colours – rely on `currentColor` for theming support
5. **Open a Pull Request** with a brief description of the new icon and its intended use case.

