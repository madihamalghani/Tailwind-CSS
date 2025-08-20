# Responsive Design:

In **Tailwind CSS**, responsiveness is handled using **responsive modifiers (breakpoints)**. These allow you to apply different styles at different screen sizes.

---

### Default Breakpoints in Tailwind

By default, Tailwind provides **mobile-first breakpoints**:

| Prefix | Min Width | Example |
| --- | --- | --- |
| `sm:` | `640px` | `sm:bg-red-500` → applies from 640px and above |
| `md:` | `768px` | `md:bg-red-500` → applies from 768px and above |
| `lg:` | `1024px` | `lg:bg-red-500` → applies from 1024px and above |
| `xl:` | `1280px` | `xl:bg-red-500` → applies from 1280px and above |
| `2xl:` | `1536px` | `2xl:bg-red-500` → applies from 1536px and above |

---

### Example Usage

```html
<div class="text-base sm:text-lg md:text-xl lg:text-2xl xl:text-3xl">
  Responsive Text
</div>
```

- **Default (mobile)** → `text-base`
- **≥640px (sm)** → `text-lg`
- **≥768px (md)** → `text-xl`
- **≥1024px (lg)** → `text-2xl`
- **≥1280px (xl)** → `text-3xl`

---

### Responsive Flexbox Example

```html
<div class="flex flex-col sm:flex-row">
  <div class="p-4 bg-red-300">Box 1</div>
  <div class="p-4 bg-green-300">Box 2</div>
</div>

```

- **Mobile (default)** → stacked vertically (`flex-col`)
- **≥640px (sm)** → side by side (`flex-row`)

---

### Responsive Grid Example

```html
<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
  <div class="bg-blue-300 p-4">1</div>
  <div class="bg-blue-300 p-4">2</div>
  <div class="bg-blue-300 p-4">3</div>
  <div class="bg-blue-300 p-4">4</div>
</div>

```

- **Mobile** → 1 column
- **≥640px (sm)** → 2 columns
- **≥1024px (lg)** → 4 columns

---

⚡ So basically: **you just add breakpoint prefixes (`sm:`, `md:`, `lg:`, etc.) before any class to make it responsive.**
