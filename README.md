# 🛍️ Zenly — Modern E-commerce Website

Zenly is a sleek React + Tailwind starter for an e-commerce website.  
It comes with product catalog, search, filters, animated cart drawer, and a demo checkout flow.

---

## ✨ Features
- 🔎 Product search, filters, sorting  
- 🛒 Cart drawer with quantity update, discounts, and shipping  
- 📱 Responsive & mobile-friendly (with bottom search bar)  
- 🎨 Clean UI built with **Tailwind CSS** + **shadcn/ui** + **lucide-react**  
- ⚡ Smooth animations using **Framer Motion**  
- 💰 INR currency formatting (India-ready)

---

## 🧱 Tech Stack
- React (Vite or Next.js)  
- Tailwind CSS  
- shadcn/ui components  
- lucide-react icons  
- framer-motion animations  

---

## 🚀 Quick Start

### 1. Create a new React app (Vite example)
```bash
npm create vite@latest zenly -- --template react
cd zenly
npm install
```

### 2. Install dependencies
```bash
npm install framer-motion lucide-react
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

### 3. Configure Tailwind
`tailwind.config.js`
```js
export default {
  content: ["./index.html", "./src/**/*.{js,jsx,ts,tsx}"],
  theme: { extend: {} },
  plugins: [],
}
```

`src/index.css`
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### 4. Add Zenly code
Replace `src/App.jsx` with the provided Zenly component code.

### 5. Run dev server
```bash
npm run dev
```


---

## 🛒 Catalog Customization
Inside the code, edit the `CATALOG` array:
```js
const CATALOG = [
  { id: "z-101", name: "Zenly Air Earbuds", price: 3499, category: "Audio", tags: ["bestseller"], image: "your-image.jpg", blurb: "Your description" },
  // add more…
];
```

- `category` automatically generates filter tabs  
- `tags` show as product badges  
- `price` is in INR  

---

## 💸 Demo Pricing Logic
- **Shipping:** Free above ₹5,999, else ₹79  
- **Discount:** 10% off orders above ₹4,999  

---

## 📁 Suggested Project Structure
```
src/
  App.jsx        # Zenly component
  index.css      # Tailwind styles
  main.jsx
  components/    # (Optional split into smaller parts)
  data/          # (Optional product JSON)
```

---

## 🌐 Deployment
- **Vercel / Netlify:** Push repo → Import → Done  
- **Static build:** `npm run build` then serve `dist/`

---

## 🖼️ Branding
- Replace “Z” avatar in navbar with your logo  
- Update gradient colors in hero text  
- Swap product images with your own  

---

## ⚠️ Notes
- Current checkout is **demo only** (no real payments).  
- Connect to a backend (Stripe, Razorpay, Firebase, Supabase, etc.) for production.  
- Replace demo Unsplash images and text before launch.  

---

### 💡 License
This starter is MIT licensed. Use freely for learning, hacking, or building your own store.
