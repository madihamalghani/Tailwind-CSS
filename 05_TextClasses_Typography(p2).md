# Text Classes/Typography(p2):

### **Text Alignment Classes:**

**Syntax**

```css
class='text-{value}'
```

| Class | Description |
| --- | --- |
| `text-left` | Aligns text to the **left** (default) |
| `text-center` | Aligns text to the **center** |
| `text-right` | Aligns text to the **right** |
| `text-justify` | Justifies the text |
| `text-start` | Aligns to start (based on direction — useful in RTL languages) |
| `text-end` | Aligns to end (opposite of start) |

---

### Examples:

```html
<p class="text-left">This text is left aligned</p>

<p class="text-center">This text is centered</p>

<p class="text-right">This text is right aligned</p>

<p class="text-justify">This is some justified text that adjusts spacing to align evenly on both sides of the paragraph box.</p>

```

---

## **Font Size Classes:**

Tailwind provides a range of text sizes from very small to very large:

| Class | Approx Size (px) | Description |
| --- | --- | --- |
| `text-xs` | 12px | Extra Small |
| `text-sm` | 14px | Small |
| `text-base` | 16px | Normal / default |
| `text-lg` | 18px | Large |
| `text-xl` | 20px | Extra Large |
| `text-2xl` | 24px | 2x Large |
| `text-3xl` | 30px | 3x Large |
| `text-4xl` | 36px | 4x Large |
| `text-5xl` | 48px | 5x Large |
| `text-6xl` | 60px | 6x Large |
| `text-7xl` | 72px | 7x Large |
| `text-8xl` | 96px | 8x Large |
| `text-9xl` | 128px | 9x Large |

---

### Example Usage:

```html

<p class="text-xs">This is extra small text</p>
<p class="text-base">This is base (normal) text</p>
<p class="text-2xl">This is 2x large text</p>
<p class="text-6xl">This is huge text</p>

```

---

### ✨ You can also combine it:

```html

<p class="text-3xl font-bold text-center text-blue-600">
  Tailwind Font Size Example
</p>
```

## **Text Decoration Classes**

These classes control underlines, overlines, line-throughs, and how text decorations behave.

### **1. Basic Text Decorations**

| Class | Description |
| --- | --- |
| `underline` | Adds an underline |
| `overline` | Adds a line above text |
| `line-through` | Adds a line through text |
| `no-underline` | Removes underline |

 **Example:**

```html
<p class="underline">This text is underlined</p>
<p class="line-through">This text has a line through it</p>
<p class="overline">This text has an overline</p>
<p class="no-underline">No underline here</p>
```

---

### **2. Decoration Style**

| Class | Description |
| --- | --- |
| `decoration-solid` | Solid line (default) |
| `decoration-double` | Double line |
| `decoration-dotted` | Dotted underline |
| `decoration-dashed` | Dashed underline |
| `decoration-wavy` | Wavy underline |

👉 **Example:**

```html
<p class="underline decoration-dotted">Dotted underline</p>
<p class="underline decoration-wavy">Wavy underline</p>
```

---

### **3. Decoration Color**

| Class | Description |
| --- | --- |
| `decoration-red-500` | Red underline |
| `decoration-blue-600` | Blue underline |
| `decoration-yellow-400` | Yellow underline |

👉 **Example:**

```html
<p class="underline decoration-dashed decoration-pink-500">Stylish dashed pink underline</p>
```

---

### **4. Decoration Thickness**

| Class | Description |
| --- | --- |
| `decoration-0` | No thickness |
| `decoration-2` to `decoration-8` | Thicker lines |

👉 **Example:**

```html

<p class="underline decoration-4 decoration-green-500">Thicker green underline</p>

```

---

## Want to Try a Cool Combo?

```html

<p class="underline decoration-wavy decoration-blue-600 decoration-2">
  Stylish Tailwind Underline!
</p>
```

## **Text Transform Classes**

| Class | What It Does |
| --- | --- |
| `uppercase` | Transforms **all letters to UPPERCASE** |
| `lowercase` | Transforms **all letters to lowercase** |
| `capitalize` | **Capitalizes the first letter** of each word |
| `normal-case` | **Removes** any transformation (resets to normal text) |

---

### 💡 Examples:

```html

<p class="uppercase">this becomes uppercase</p>
<!-- Output: THIS BECOMES UPPERCASE -->

<p class="lowercase">THIS BECOMES LOWERCASE</p>
<!-- Output: this becomes lowercase -->

<p class="capitalize">this is capitalized</p>
<!-- Output: This Is Capitalized -->

<p class="normal-case uppercase">reset to normal case</p>
<!-- Output: reset to normal case -->

```

---

### Combine with Other Classes

You can also combine text transform with:

- `text-xl`, `font-bold`, `text-center`
- `tracking-wide` (letter spacing)
- `decoration-*` (underline styles)

Example:

```html

<p class="capitalize text-blue-600 font-semibold text-lg">
  welcome to my website
</p>
<!-- Output: Welcome To My Website -->

```

---

