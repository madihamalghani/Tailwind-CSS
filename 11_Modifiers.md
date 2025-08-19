# Modifiers:

These are **prefixes** you attach to utilities to control **state, screen size, or conditions**.

---

## **1. State Modifiers** (Pseudo-classes)

Used for **hover, focus, active, etc.**

| Modifier | Effect |
| --- | --- |
| `hover:` | Styles when element is hovered |
| `focus:` | When focused (like inputs/buttons) |
| `active:` | While being clicked |
| `visited:` | For visited links |
| `disabled:` | Disabled elements |
| `checked:` | Checked radio/checkbox |
| `first:` / `last:` | First or last child |
| `odd:` / `even:` | Alternate rows (tables/lists) |

Example:

```html
<button class="bg-blue-500 hover:bg-blue-700 focus:ring-2 focus:ring-blue-300 text-white px-4 py-2 rounded">
  Click Me
</button>

```

---

## **2. Responsive Modifiers (Breakpoints)**

Tailwind uses **mobile-first** design.

Modifiers apply styles at **specific screen widths**.

| Modifier | Min Width |
| --- | --- |
| `sm:` | ≥ 640px |
| `md:` | ≥ 768px |
| `lg:` | ≥ 1024px |
| `xl:` | ≥ 1280px |
| `2xl:` | ≥ 1536px |

Example:

```html
<p class="text-sm md:text-lg lg:text-2xl">
  This text gets bigger on larger screens.
</p>
```

---

## **3. Dark Mode Modifier**

Tailwind supports dark mode out of the box.

| Modifier | Effect |
| --- | --- |
| `dark:` | Apply styles in dark mode |

Example:

```html
<div class="bg-white text-black dark:bg-black dark:text-white">
  Dark mode ready!
</div>

```

---

## **4. Motion / Preference Modifiers**

For accessibility or system preferences:

| Modifier | Effect |
| --- | --- |
| `motion-safe:` | Applies only if animations are allowed |
| `motion-reduce:` | Applies if user prefers reduced motion |
| `print:` | Styles when printing |

---

## Summary

- **State modifiers** → `hover:`, `focus:`, `active:`, `disabled:`, etc.
- **Responsive modifiers** → `sm:`, `md:`, `lg:`, etc.
- **Dark mode modifier** → `dark:`
- **Other preferences** → `motion-safe:`, `print:`

---

👉 Modifiers **stack together**:

```html
<button class="bg-blue-500 hover:bg-blue-700 md:hover:bg-green-500 dark:bg-gray-800">
  Responsive + Hover + Dark mode
</button>
```

---

