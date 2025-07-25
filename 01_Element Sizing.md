# Element Sizing:

For element sizing in Tailwind CSS we use :

```sql
class='w-{value}'
class='h-{value}'
```

**👉 Tailwind CSS use fixed units** 

### **Sizes in Tailwind CSS:**

```sql
1 unit= 0.25 rem = 4px
1 rem = 16px
```

So

```sql
class='w-4'  => 1 rem (16px)
```

### **1. Fixed Units (rem-based spacing scale)**

```sql
0	=> 0rem
0.5 => 0.125rem (2px)
1	=> 0.25rem (4px)
1.5	=> 0.375rem (6px)
2	=> 0.5rem (8px)
2.5	=> 0.625rem (10px)
3	=> 0.75rem (12px)
3.5	=> 0.875rem (14px)
4	=> 1rem (16px)
...
```

This is used in:

- `w-{n}`
- `h-{n}`
- `m-{n}`
- `p-{n}`

### **2. Percentage Units:**

Tailwind provides utilities for sizing in **percentages**:

- `w-1/2` = `50%`
- `w-1/3` = `33.3333%`
- `w-full` = `100%`
- `w-screen` = `100vw` (full viewport width)
- `h-screen` = `100vh` (full viewport height)

### **3. Fractional Units**

More granular fractions:

- `w-1/4` = `25%`
- `w-2/5` = `40%`
- `w-3/4` = `75%`

### **4. Arbitrary Values (Custom units)**

When you need **specific sizes**, you can use **square bracket notation**:

- `w-[500px]`
- `h-[30%]`
- `max-w-[600px]`
- `p-[2em]`

### **5. Viewport Units**

- `w-screen`: `100vw`
- `h-screen`: `100vh`
- Or arbitrary: `w-[50vw]`

### **6. Auto and Fit**

- `w-auto`: auto width
- `h-auto`: auto height
- `w-min`: `min-content`
- `w-max`: `max-content`
- `w-fit`: `fit-content`

### **7. Other Units**

Tailwind also includes:

- `w-px`: `1px`
- `m-px`: `1px`
- Arbitrary units (like `em`, `vh`, `%`): `w-[10em]`

***Try this one as example:***

```html
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
```

