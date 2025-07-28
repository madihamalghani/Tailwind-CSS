# Padding & Margin:

**Syntax:**

```css
class = 'p - {value}'
class= 'm - {value}'
```

### All Sides

| Utility | Effect |
| --- | --- |
| `m-4` | `margin: 1rem;` |
| `p-4` | `padding: 1rem;` |

⇒ 1 unit = 0.25 rem

⇒ p-4 = 1 rem

### Individual Sides

| Utility | Side | Margin | Padding |
| --- | --- | --- | --- |
| `t` | top | `mt-4` | `pt-4` |
| `r` | right | `mr-4` | `pr-4` |
| `b` | bottom | `mb-4` | `pb-4` |
| `l` | left | `ml-4` | `pl-4` |

### Horizontal & Vertical

| Utility | Affects | Example |
| --- | --- | --- |
| `mx-4` | left & right margin | `margin-left/right: 1rem` |
| `my-4` | top & bottom margin | `margin-top/bottom: 1rem` |
| `px-4` | left & right padding | `padding-left/right: 1rem` |
| `py-4` | top & bottom padding | `padding-top/bottom: 1rem` |

### Implementation

```css
<main>
        <section class="w-screen h-32 bg-sky-200 text-sky-950 m-4 p-14">
            Fixed units
        </section>
        <section class="w-1/2 h-screen bg-red-300 m-8 text-sky-950 p-4">
            Percentage units
        </section>
        <section class="h-15 mb-4 p-10 w-screen bg-fuchsia-200 text-sky-950">
            Viewport units
        </section>
    </main>
```

**OR**

```css
 <section class="bg-blue-200 text-purple-800 m-4 p-6 w-1/2 h-32">
            <p>Section 1</p>
        </section>

        <section class="bg-green-800 text-green-100 my-6 px-8 w-full h-40">
            <p>Section 2</p>
        </section>

        <section class="bg-yellow-200 text-amber-600 mx-auto py-4 w-5/12 h-24">
            <p>Section 3</p>
        </section>
    </main>
```

**Official Docs Link:**

<aside>

https://tailwindcss.com/docs/margin

https://tailwindcss.com/docs/padding

</aside>
