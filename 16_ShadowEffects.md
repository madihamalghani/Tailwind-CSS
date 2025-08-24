# Shadow:

In **Tailwind CSS**, shadows are added with the `shadow-*` utility classes.

They control how much blur and spread the shadow has.

---

### Common Shadow Classes

- `shadow-none` → removes shadow
- `shadow-sm` → small shadow
- `shadow` → normal (default) shadow
- `shadow-md` → medium shadow
- `shadow-lg` → large shadow
- `shadow-xl` → extra large shadow
- `shadow-2xl` → very strong shadow

---

### Example

```html
<div class="p-6 shadow-lg bg-white rounded-xl">
  Large shadow box
</div>

```

---

### Colored Shadows

You can combine shadows with **color utilities**:

```html
<div class="shadow-lg shadow-blue-500/50 p-6 rounded-xl">
  Shadow with blue tint
</div>

```

Here `shadow-blue-500/50` means **blue shadow at 50% opacity**.

---

By default, Tailwind gives you only a set of **predefined shadow levels** (the ones I listed: `shadow-sm`, `shadow-md`, `shadow-lg`, etc. and `drop-shadow-*`).

But you’re not limited to just those. You can:

---

### 1. Use Default Shadows

Already built in → `shadow-sm`, `shadow-md`, … `shadow-2xl`

For drop shadows → `drop-shadow-sm`, … `drop-shadow-2xl`

---

### 2. Add **Colored Shadows**

You can combine with colors & opacity:

```html
<div class="shadow-lg shadow-purple-500/40 p-6 rounded-xl">
  Purple Glow
</div>

```

---

### 3. Use **Arbitrary Values**

If you want a **custom shadow**, Tailwind lets you write inline values:

```html
<div class="shadow-[0_10px_30px_rgba(0,0,0,0.4)] p-6 rounded-xl">
  Custom Shadow
</div>

```

👉 This means: `x=0, y=10px, blur=30px, color=rgba(0,0,0,0.4)`

---

### 4. Extend in `tailwind.config.js`

If you want to **reuse your own custom shadows everywhere**, you can define them:

```jsx
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      boxShadow: {
        'glow': '0 0 20px rgba(34,197,94,0.7)', // green glow
        'soft': '0 4px 12px rgba(0,0,0,0.1)',   // soft shadow
      }
    }
  }
}

```

Then use:

```html
<div class="shadow-glow p-6 rounded-xl">Custom Glow Shadow</div>

```

---
