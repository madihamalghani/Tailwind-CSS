# Animations:

Tailwind CSS comes with **built-in animations and transitions** + the ability to extend with your own custom animations.

---

## 1. Built-in Animations (Utilities)

Tailwind gives you a few **ready-made animations**:

- `animate-spin` → rotates element (like a loader)
- `animate-ping` → pulse effect with fading out circle
- `animate-pulse` → smooth fading in/out (like skeleton loading)
- `animate-bounce` → bouncing effect (like arrows pointing down)

Example:

```html
<div class="w-10 h-10 bg-blue-500 rounded-full animate-bounce"></div>

```

---

## 2. Transitions

You can animate changes between states using transition utilities:

- `transition` → enables transition on all properties
- `transition-colors` → animates only colors (bg, text, border)
- `transition-transform` → animates transforms (scale, rotate, translate)
- `duration-500` → 500ms duration
- `ease-in`, `ease-out`, `ease-in-out` → easing functions

Example (hover effect):

```html
<button class="bg-blue-500 text-white px-4 py-2 rounded
               transition-colors duration-300 hover:bg-blue-700">
  Hover me
</button>

```

---

## Transform Animations

Tailwind supports transforms that you can combine with transitions:

- `scale-110` → enlarge
- `rotate-45` → rotate
- `translate-x-4` → move
- `skew-y-6` → skew

Example:

```html
<div class="w-20 h-20 bg-red-500 transform transition
            duration-500 hover:scale-110 hover:rotate-12">
</div>

```

---

## 4. Custom Keyframe Animations

You can define your **own animations** in `tailwind.config.js`:

```jsx
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      keyframes: {
        wiggle: {
          '0%, 100%': { transform: 'rotate(-3deg)' },
          '50%': { transform: 'rotate(3deg)' },
        },
      },
      animation: {
        wiggle: 'wiggle 1s ease-in-out infinite',
      },
    },
  },
}

```

Then use it:

```html
<div class="w-16 h-16 bg-green-500 animate-wiggle"></div>

```

---

✨ So basically:

- Use **built-in ones** (`spin`, `bounce`, etc.)
- Use **transition + transform** for hover/focus effects
- Create **custom animations** in `tailwind.config.js` for anything unique
