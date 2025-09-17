# Inset:

In CSS, `inset` is a shorthand for setting all four positioning properties

### What `inset-0` means?

```css
top: 0;
right: 0;
bottom: 0;
left: 0;

```

So in **Tailwind**,

```html
inset-0

```

is equivalent to:

```css
top: 0;
right: 0;
bottom: 0;
left: 0;

```

---

### When is it used?

It’s commonly used with **absolute** or **fixed** positioned elements to make them **fill their parent**.

Example:

```html
<div class="relative w-64 h-40 bg-gray-200">
  <div class="absolute inset-0 bg-sky-500 opacity-30"></div>
</div>

```

 Explanation:

- The outer `div` is `relative` (so the absolute element is positioned inside it).
- The inner `div` is `absolute inset-0`, meaning it will **stretch from top 0 to bottom 0 and left 0 to right 0** → fully covering the parent.
- Then we added `bg-sky-500 opacity-30` so you see it as a **semi-transparent overlay**.

---

**Shortcut memory**:

- `inset-0` → Fill parent completely.
- `inset-x-0` → Stretch only horizontally (`left: 0; right: 0;`).
- `inset-y-0` → Stretch only vertically (`top: 0; bottom: 0;`).
