# Display and Position:

In **Tailwind CSS**, `display` and `position` utilities help you control how elements behave in the layout.

---

## **Display Utilities**

| Class | CSS Equivalent | Description |
| --- | --- | --- |
| `block` | `display: block` | Block-level element |
| `inline-block` | `display: inline-block` | Inline with block capabilities |
| `inline` | `display: inline` | No block layout, flows inline |
| `flex` | `display: flex` | Enables Flexbox |
| `inline-flex` | `display: inline-flex` | Flex inside inline container |
| `grid` | `display: grid` | Enables CSS Grid |
| `inline-grid` | `display: inline-grid` | Grid inside inline container |
| `hidden` | `display: none` | Hides the element |
| `table`, `table-row`, `table-cell` | mimic table layouts |  |

### Example:

```html

<div class="flex justify-between">
  <p>Left</p>
  <p>Right</p>
</div>
```

---

## 2. **Position Utilities**

| Class | CSS Equivalent | Description |
| --- | --- | --- |
| `static` | `position: static` | Default positioning |
| `relative` | `position: relative` | Position relative to itself |
| `absolute` | `position: absolute` | Positioned relative to nearest parent with `relative` |
| `fixed` | `position: fixed` | Positioned relative to viewport |
| `sticky` | `position: sticky` | Sticks to a position when scrolling |

**Offset helpers (for absolute/fixed/sticky):**

| Class | Description |
| --- | --- |
| `top-0`, `bottom-0` | Align to top/bottom |
| `left-0`, `right-0` | Align to left/right |
| `inset-0` | `top`, `right`, `bottom`, and `left` all `0` |

### Example:

```html

<div class="relative">
  <div class="absolute top-0 right-0">
    I'm placed at the top right corner.
  </div>
</div>

```

---

**Official Website Links:**

<aside>

- https://tailwindcss.com/docs/display
- https://tailwindcss.com/docs/position
- https://tailwindcss.com/docs/top-right-bottom-left
</aside>
