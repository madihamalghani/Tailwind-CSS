# CRA + Tailwind Connect:

After installing react:

## Step 1: Install Tailwind

Go inside your CRA project folder and run:

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p

```

This will create:

- `tailwind.config.js`
- `postcss.config.js`

## Step 2: Configure Tailwind

Open `tailwind.config.js` and replace with this:

```jsx
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",   //  tells Tailwind where to look
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

```

---

## Step 3: Add Tailwind to your CSS

Open `src/index.css` and clear everything. Then add:

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

```

---

## Step 4: Use Tailwind in React Components

Now in `src/App.js` try this:

```jsx
function App() {
  return (
    <div className="h-screen flex items-center justify-center bg-gray-100">
      <button className="px-4 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue-600">
        Click Me
      </button>
    </div>
  );
}

export default App;

```

---

## Step 5: Start your project

Run:

```bash
npm start

```

Open [http://localhost:3000](http://localhost:3000/) → You’ll see a Tailwind-styled button 

---

Now Tailwind is fully working with Create React App.
