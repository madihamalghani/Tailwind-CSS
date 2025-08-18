# Extras:

## 1. **Fill (for SVGs)**

The `fill` utility changes the **fill color of SVG shapes**.

| Class | Effect |
| --- | --- |
| `fill-current` | Inherits `currentColor` (usually text color) |
| `fill-{color}` | Sets fill to a specific color |

[](data:image/svg+xml;utf8,%3Csvg%20class%3D%22w-8%20h-8%20fill-blue-500%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20viewBox%3D%220%200%2020%2020%22%3E%0A%20%20%3Cpath%20d%3D%22M10%2015l-5-5h10l-5%205z%22%3E%3C%2Fpath%3E%0A%3C%2Fsvg%3E%0A)

## 2. **Opacity**

Controls the **transparency** of an element.

| Class | CSS Equivalent |
| --- | --- |
| `opacity-0` | `opacity: 0;` (invisible) |
| `opacity-25` | `opacity: 0.25;` |
| `opacity-50` | `opacity: 0.5;` |
| `opacity-75` | `opacity: 0.75;` |
| `opacity-100` | `opacity: 1;` (default) |

Example:

```html
<button class="bg-blue-500 text-white p-2 opacity-50">
  Disabled Button
</button>
```

---

## 3. **Cursor**

Changes the **mouse cursor style** when hovering.

| Class | Cursor Type |
| --- | --- |
| `cursor-auto` | Default based on element |
| `cursor-pointer` | Pointer (hand icon, usually for links/buttons) |
| `cursor-wait` | Loading/wait cursor |
| `cursor-not-allowed` | Disabled cursor |
| `cursor-text` | Text cursor (I-beam) |
| `cursor-move` | Move cursor |
| `cursor-grab` / `cursor-grabbing` | Grab/drag cursor |

Example:

```html
<button class="bg-green-500 text-white p-2 cursor-not-allowed">
  Disabled
</button>

```

---

## 4. **Screen Reader Utilities (Accessibility)**

These help **show or hide content for screen readers**.

| Class | Effect |
| --- | --- |
| `sr-only` | Hide visually but **accessible** for screen readers |
| `not-sr-only` | Reverses `sr-only` (make it visible again) |

 Example:

```html
<button class="bg-blue-500 text-white p-2">
  <span class="sr-only">Close menu</span>
  ✖
</button>

```

👉 The “✖” is visible, but “Close menu” is what screen readers will announce.

---

With these 4 (`fill`, `opacity`, `cursor`, `sr-only`), you can handle **SVGs, visibility, interactivity, and accessibility** all at once.
