# Built-in Theme:

## *Simple HTML + CDN*

***In HTML with tailwind link:***

```html
   <head>
    <title> Add dark mode </title>   
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        // Enable dark mode class
        tailwind.config = {
            darkMode: 'class',
        }
     </script>
```

and after this you can add dark colors like this in class:

```html
   <!-- Navbar -->
    <nav class="bg-white dark:bg-gray-900 shadow-md px-6 py-4 flex justify-between items-center mb-8">
        <!-- Logo -->
        <div class="text-2xl font-bold text-gray-900 dark:text-white">
            My UI Kit
        </div>

        <!-- Links -->
        <ul class="flex space-x-6 font-medium">
            <li><a href="#buttons" class="text-gray-700 dark:text-gray-300 hover:text-blue-500">Buttons</a></li>
            <li><a href="#forms" class="text-gray-700 dark:text-gray-300 hover:text-blue-500">Forms</a></li>
            <li><a href="#cards" class="text-gray-700 dark:text-gray-300 hover:text-blue-500">Cards</a></li>
            <li><a href="#loaders" class="text-gray-700 dark:text-gray-300 hover:text-blue-500">Loaders</a></li>
        </ul>

        <!-- Theme Switcher Button -->
        <button id="theme-toggle" class="px-4 py-2 rounded-lg bg-gray-200 dark:bg-gray-700 text-gray-900 dark:text-gray-100 
                        hover:scale-105 transition-all duration-300">
            Toggle Theme
        </button>
    </nav>
```

**dark:** shows the corresponding color etc in dark theme

---

## HTML and Tailwind Config file:

### 1. Setup in `tailwind.config.js`

```jsx
module.exports = {
  darkMode: "class", // important!
  content: ["./*.html"],
  theme: {
    extend: {},
  },
  plugins: [],
}

```

---

### 2. Example in HTML

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <script>
      function toggleDark() {
        document.documentElement.classList.toggle("dark");
      }
    </script>
    <link href="output.css" rel="stylesheet" />
  </head>
  <body class="bg-white dark:bg-gray-900 text-black dark:text-white min-h-screen flex items-center justify-center">
    <div class="text-center">
      <h1 class="text-3xl font-bold">Hello Tailwind!</h1>
      <button onclick="toggleDark()" class="mt-4 px-4 py-2 bg-gray-200 dark:bg-gray-800 rounded-lg">
        Toggle Dark Mode
      </button>
    </div>
  </body>
</html>

```

---

## *Tailwind & React:*

### 1. Configure Tailwind

In your `tailwind.config.js`, enable class-based dark mode:

```jsx
/** @type {import('tailwindcss').Config} */
module.exports = {
  darkMode: "class", // or 'media'
  content: ["./src/**/*.{js,jsx,ts,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

```

---

### 2. Apply Dark Classes in React

For example, in `App.jsx`:

```jsx
import { useState } from "react";

function App() {
  const [darkMode, setDarkMode] = useState(false);

  return (
    <div className={darkMode ? "dark" : ""}>
      <div className="min-h-screen bg-white dark:bg-gray-900 text-black dark:text-white flex flex-col items-center justify-center">
        <h1 className="text-3xl font-bold">Hello Tailwind!</h1>
        <buttononClick={() => setDarkMode(!darkMode)}
          className="mt-4 px-4 py-2 bg-gray-200 dark:bg-gray-800 rounded-lg"
        >
          Toggle Dark Mode
        </button>
      </div>
    </div>
  );
}

export default App;

```

 Here:

- If `dark` class is present on parent `<div>`, dark styles apply.
- You can toggle manually.

---

So difference is only in **state handling**:

- In React → manage with `useState`.
- In plain HTML/JS → just toggle the `dark` class on `<html>` or `<body>`.
