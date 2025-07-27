# Color System:

You can see the official website color docs, where different color choices with shades are given:

https://tailwindcss.com/docs/colors

- 50 → Lightest shade
- 950→ darkest shade

### Implementation of Colors :

```css
  <div class="bg-sky-200"></div>
  <div class="bg-sky-300"></div>
  <div class="bg-sky-400"></div>
  <div class="bg-sky-200 text-sky-900"></div>
```

Shades you can use:

```css

50

100

200

300

400

500

600

700

800

900

950
```

Try to run this one:

```html
<!doctype html>
<html>
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <script src="https://cdn.tailwindcss.com"></script>
    </head>
    <body>
        <main> 
            <section class="w-screen h-32 bg-sky-200 text-sky-950">
                Fixed units
            </section>
            <section class="w-screen h-screen bg-red-300 text-sky-950">
                Percentage units
            </section>
            <section class="h-1/2 w-screen bg-fuchsia-200 text-sky-950">
                Viewport units
            </section>
        </main>
    </body>
</html>

```

