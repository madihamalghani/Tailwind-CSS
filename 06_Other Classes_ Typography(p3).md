# Other Classes /Typography (p3):

## Letter Spacing:

In Tailwind CSS, **letter spacing** is controlled using the `tracking-{size}` utility classes.

### Available Letter Spacing Classes

| Class | Letter Spacing |
| --- | --- |
| `tracking-tighter` | -0.05em |
| `tracking-tight` | -0.025em |
| `tracking-normal` | 0em |
| `tracking-wide` | 0.025em |
| `tracking-wider` | 0.05em |
| `tracking-widest` | 0.1em |

---

### Example:

```html

<p class="tracking-wider text-lg">
  This text has wider letter spacing.
</p>

```

---

## Line Height

In **Tailwind CSS**, **line height** is controlled using the `leading-{size}` utility classes.

---

### Common `leading-{}` Classes

| Class | Line Height |
| --- | --- |
| `leading-none` | 1 |
| `leading-tight` | 1.25 |
| `leading-snug` | 1.375 |
| `leading-normal` | 1.5 |
| `leading-relaxed` | 1.625 |
| `leading-loose` | 2 |

---

### Numeric Values (customizable via config)

You can also use values like:

| Class | Line Height |
| --- | --- |
| `leading-3` | .75rem |
| `leading-4` | 1rem |
| `leading-5` | 1.25rem |
| `leading-6` | 1.5rem |
| `leading-7` | 1.75rem |
| `leading-8` | 2rem |
| `leading-9` | 2.25rem |
| `leading-10` | 2.5rem |

---

### Example:

```html
<p class="text-base leading-relaxed">
  This paragraph has relaxed line height.
</p>

```

---

## Line Clamp

In **Tailwind CSS**, **line clamping** (truncating text after a certain number of lines) is handled using the `line-clamp-{n}` utility — but it's part of the **Tailwind Typography plugin** or **line-clamp plugin**, which you may need to enable if it’s not working by default.

### What Is Line Clamping?

It limits the number of lines displayed in a block of text and adds an ellipsis (`...`) when the text overflows.

### Available Classes[1-6 OR NONE]

| Class | Effect |
| --- | --- |
| `line-clamp-1` | Show 1 line, truncate rest with `...` |
| `line-clamp-2` | Show 2 lines |
| `line-clamp-3` | Show 3 lines |
| ... | Up to `line-clamp-6` by default |
| `line-clamp-none` | Disable clamping |

---

### Example:

```html

<p class="line-clamp-2 text-ellipsis overflow-hidden">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean euismod bibendum laoreet. Proin gravida dolor sit amet lacus accumsan.
</p>
```

---

### How to Enable Line Clamp (if not working)

1. Install the plugin (if not already):
    
    ```bash
    
    npm install -D @tailwindcss/line-clamp
    
    ```
    
2. Add it to `tailwind.config.js`:
    
    ```jsx
    
    module.exports = {
      content: ["./src/**/*.{html,js}"],
      theme: {
        extend: {},
      },
      plugins: [
        require('@tailwindcss/line-clamp'),
      ],
    }
    
    ```
    

---

**Official Website Docs Link:**

<aside>

- https://tailwindcss.com/docs/letter-spacing
- https://tailwindcss.com/docs/line-height
- https://tailwindcss.com/docs/line-clamp
</aside>

**Other Typography classes are also present**
