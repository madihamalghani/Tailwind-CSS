# Flexbox:

**Syntax:**

```jsx
class='flex'
class='flex- {direction}'
```

The `flex-direction` in Tailwind is controlled using:

```

flex-row        => Row (default, left to right)
flex-row-reverse=> Row reversed (right to left)
flex-col        => Column (top to bottom)
flex-col-reverse=> Column reversed (bottom to top)

```

---

### Basic Example

```html

<!-- Row direction (default) -->
<div class="flex flex-row gap-4">
  <div class="bg-red-300 p-4">Item 1</div>
  <div class="bg-blue-300 p-4">Item 2</div>
</div>

```

---

### Use Case

| Class | When to Use |
| --- | --- |
| `flex-row` | Horizontal navigation, cards side by side |
| `flex-col` | Vertical menus, stacked sections |
| `flex-row-reverse` | Right to left layouts |
| `flex-col-reverse` | Stack from bottom to top |

---

### Justify Content

### `justify-content` in Tailwind CSS

`justify-content` controls **horizontal alignment** of **flex or grid items** along the **main axis**.

---

### Tailwind Classes for `justify-content`

| Class | CSS Equivalent | Meaning |
| --- | --- | --- |
| `justify-start` | `justify-content: flex-start` | Align items to the **start** (left) |
| `justify-center` | `justify-content: center` | **Center** items |
| `justify-end` | `justify-content: flex-end` | Align items to the **end** (right) |
| `justify-between` | `justify-content: space-between` | **Even space between**, no outer gap |
| `justify-around` | `justify-content: space-around` | Equal space **around** items |
| `justify-evenly` | `justify-content: space-evenly` | Equal space **between and outside** |

---

### Example (Row Flex):

```html

<div class="flex justify-between bg-gray-100 p-4">
  <div class="bg-red-300 p-2">Box 1</div>
  <div class="bg-blue-300 p-2">Box 2</div>
  <div class="bg-green-300 p-2">Box 3</div>
</div>

```

Try changing `justify-between` to other classes like `justify-center`, `justify-end`, etc., and see the alignment change.

### Items Align

### `align-items` in Tailwind CSS

`align-items` controls the **vertical alignment** of items **inside a flex container** along the **cross axis** (perpendicular to the flex direction).

---

### Tailwind Classes for `align-items`

| Class | CSS Equivalent | Meaning |
| --- | --- | --- |
| `items-start` | `align-items: flex-start` | Align items to the **top** |
| `items-center` | `align-items: center` | **Center** items vertically |
| `items-end` | `align-items: flex-end` | Align items to the **bottom** |
| `items-stretch` | `align-items: stretch` (default) | Stretch to fill height (if no fixed height) |
| `items-baseline` | `align-items: baseline` | Align text baselines |

---

### Example:

```html
<div class="flex h-32 items-center bg-gray-100">
  <div class="bg-red-300 p-2">Box 1</div>
  <div class="bg-blue-300 p-6">Box 2</div>
</div>

```

Here, `items-center` aligns all items vertically in the center of the container with height `h-32`.

---

### Note:

- For **row direction**, `align-items` affects **vertical** alignment.
- For **column direction**, it affects **horizontal** alignment instead.

### Gap:

### `gap` in Tailwind CSS

The `gap` utility in Tailwind adds **spacing between items** in a **Flexbox** or **Grid** layout — both **row** and **column**.

---

## **Basic `gap` Classes**

| Class | Gap Size |
| --- | --- |
| `gap-0` | `0rem` |
| `gap-1` | `0.25rem` (4px) |
| `gap-2` | `0.5rem` (8px) |
| `gap-3` | `0.75rem` (12px) |
| `gap-4` | `1rem` (16px) |
| `gap-5` | `1.25rem` (20px) |
| ... | Up to `gap-96` |

---

## **Directional Gaps**

| Class | Description |
| --- | --- |
| `gap-x-4` | Gap only **horizontally** |
| `gap-y-2` | Gap only **vertically** |

---

## Example – Flex with Gaps:

```html

<div class="flex gap-4">
  <div class="bg-red-300 p-4">Box 1</div>
  <div class="bg-blue-300 p-4">Box 2</div>
</div>

```

## Notes:

- `gap` affects **space between** items, not padding inside.
- Works only with **Flex** or **Grid** layouts.

---

## Flex-Grow:

In **Tailwind CSS**, `flex-grow` controls whether a flex item should **grow** to fill the available space inside a flex container.

---

## Tailwind `flex-grow` Classes

| Class | CSS Equivalent | Meaning |
| --- | --- | --- |
| `flex-grow` | `flex-grow: 1;` | Item **can grow** and take remaining space |
| `flex-grow-0` | `flex-grow: 0;` (default) | Item **will not grow** |

---

## Example: Two Boxes

```html
<div class="flex gap-4">
  <div class="bg-red-300 p-4 flex-grow">I will grow</div>
  <div class="bg-blue-300 p-4">I stay the same</div>
</div>

```

👉 The red box expands to fill extra space, while the blue box keeps its size.

---

## Example: Equal Growth

```html
<div class="flex gap-4">
  <div class="bg-green-300 p-4 flex-grow">Box 1</div>
  <div class="bg-yellow-300 p-4 flex-grow">Box 2</div>
</div>

```

👉 Both boxes grow **equally** and share the space.

---

## Note:

- `flex-grow` works **only inside a `flex` container**.
- If multiple children have `flex-grow`, they share space **proportionally**.
- Use with `flex-shrink` and `flex-basis` (`flex` shorthand) for advanced layouts.

---

## Flex Grow:

In **Tailwind CSS**, `flex-wrap` controls whether **flex items stay on one line** or **wrap onto multiple lines** when they don’t fit in the container.

## Tailwind `flex-wrap` Classes

| Class | CSS Equivalent | Meaning |
| --- | --- | --- |
| `flex-nowrap` | `flex-wrap: nowrap;` (default) | All items stay on **one line**, may overflow |
| `flex-wrap` | `flex-wrap: wrap;` | Items wrap onto **multiple lines** |
| `flex-wrap-reverse` | `flex-wrap: wrap-reverse;` | Items wrap onto multiple lines but in **reverse order** |

---

## Example – Without Wrap (default)

```html
<div class="flex flex-nowrap gap-4 bg-gray-200 p-2">
  <div class="bg-red-300 p-4">1</div>
  <div class="bg-blue-300 p-4">2</div>
  <div class="bg-green-300 p-4">3</div>
  <div class="bg-yellow-300 p-4">4</div>
  <div class="bg-pink-300 p-4">5</div>
</div>

```

👉 All items stay in one row, even if they overflow.

---

## Example – With Wrap

```html
<div class="flex flex-wrap gap-4 bg-gray-200 p-2">
  <div class="bg-red-300 p-4 w-32">1</div>
  <div class="bg-blue-300 p-4 w-32">2</div>
  <div class="bg-green-300 p-4 w-32">3</div>
  <div class="bg-yellow-300 p-4 w-32">4</div>
  <div class="bg-pink-300 p-4 w-32">5</div>
</div>

```

👉 Items move to the **next line** when there’s not enough space.

---

## Note:

- Often used with `gap-*` for clean spacing.
- Useful in **responsive layouts** (like wrapping cards or buttons).

---

<aside>

***Official Website Docs:***

- https://tailwindcss.com/docs/flex-direction
- https://tailwindcss.com/docs/justify-content
- https://tailwindcss.com/docs/align-items
- https://tailwindcss.com/docs/gap
- https://tailwindcss.com/docs/flex-wrap
- https://tailwindcss.com/docs/flex-grow
</aside>
