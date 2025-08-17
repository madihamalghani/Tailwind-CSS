# Borders:

**Borders in Tailwind CSS** : they’re super flexible:

---

## 1. **Border Width**

| Class | CSS Equivalent |
| --- | --- |
| `border` | `border-width: 1px;` |
| `border-2` | `border-width: 2px;` |
| `border-4` | `border-width: 4px;` |
| `border-8` | `border-width: 8px;` |
| `border-0` | `border-width: 0;` |

👉 You can also apply to one side:

- `border-t` (top), `border-b` (bottom),
- `border-l` (left), `border-r` (right).

---

## 2. **Border Color**

Use `border-{color}` with Tailwind’s color palette:

```html
<div class="border-2 border-red-500 p-4">Red Border</div>

```

---

## 3. **Border Style**

| Class | CSS Equivalent |
| --- | --- |
| `border-solid` | `border-style: solid;` |
| `border-dashed` | `border-style: dashed;` |
| `border-dotted` | `border-style: dotted;` |
| `border-double` | `border-style: double;` |
| `border-none` | `border-style: none;` |

---

## 4. **Border Radius (Rounded Corners)**

| Class | Effect |
| --- | --- |
| `rounded-none` | No rounding |
| `rounded-sm` | Small radius |
| `rounded` | Default radius |
| `rounded-md` | Medium radius |
| `rounded-lg` | Large radius |
| `rounded-xl` | Extra large radius |
| `rounded-2xl` | Even bigger |
| `rounded-3xl` | Super round |
| `rounded-full` | Fully round (circle) |

👉 Also side-specific:

- `rounded-t-lg` (top only)
- `rounded-b-full` (bottom only)
- `rounded-l-md` (left only)
- `rounded-r-xl` (right only)

---

## 5. **Divide Between Children (Special)**

`divide-{x/y}-{color}` adds a border **between flex/grid children**:

```html
<div class="flex divide-x divide-gray-400">
  <div class="p-4">Item 1</div>
  <div class="p-4">Item 2</div>
</div>

```

---

Example (combined):

```html
<div class="border-4 border-dashed border-blue-500 rounded-xl p-6">
  Stylish Box with border
</div>

```

---

