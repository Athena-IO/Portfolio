# README

```javascript
//  █████╗ ████████╗██╗  ██╗███████╗██╗   ██╗ █████╗ 
// ██╔══██╗╚══██╔══╝██║  ██║██╔════╝██║   ██║██╔══██╗
// ███████║   ██║   ███████║█████╗  ██║   ██║███████║
// ██╔══██║   ██║   ██╔══██║██╔══╝  ╚██╗ ██╔╝██╔══██║
// ██║  ██║   ██║   ██║  ██║███████╗ ╚████╔╝ ██║  ██║
// ╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚══════╝  ╚═══╝  ╚═╝  ╚═╝
//
//                     ATHENA-IO
//    Intelligent, clean, and elegant portfolio site
//             Crafted by Mehdi Fazzli
// -----------------------------------------------------
```

---

## 👋 Introduction
Hey there! I’m **Mehdi Fazzli** — a front-end and app developer passionate about clean UI, smooth UX, and meaningful design.  
**ATHENA-IO** is my personal portfolio project — a space where I showcase my skills, experiments, and creative journey as a developer.

---

## 🚀 What’s Inside
- A personal introduction and skills overview  
- Showcased projects with demos and GitHub links  
- Technical breakdowns for each project  
- Simple setup and build instructions  

---

## 🧭 Interests
- **Front-end Development:** Vue 3 / Nuxt 3 / React  
- **Software Engineering:** architecture, testing, performance  
- **Game Development (future):** gameplay systems, C++ logic  
- **UI/UX Design:** minimal, clean, animated interfaces  

---

## 🛠️ Tech Stack
- **Languages:** JavaScript (ES6+), TypeScript  
- **Frameworks:** Vue 3, Nuxt 3, React  
- **Tools:** Vite, Webpack, Tailwind CSS, Pinia  
- **Backend (sample):** Node.js, Express, Firebase  
- **Deployment:** Vercel, Netlify  

---

## 📂 Featured Projects
### 1. **ATHENA-IO — Portfolio**
A personal portfolio built with **Nuxt 3** and **@nuxt/content**, featuring markdown-based project pages, automatic sitemap generation, and smooth animations.  
**Highlights:**
- Dynamic content loading  
- SEO-friendly structure  
- Deployed on **Vercel**

```bash
# install dependencies
npm install

# run in development mode
npm run dev

# build for production
npm run build && npm run start
```

---

### 2. **Perfume Lab**
A concept site for creating and showcasing fictional perfumes.  
**Stack:** Nuxt 3, Pinia, Tailwind CSS, Composition API  

### 3. **Mini Game Demo (Unity / WebGL)**
A simple 2D game where the player collects points and fights enemies.  
**Tech:** Unity, C#, WebGL export  

---

## ⚙️ Configuration Tips
If your sitemap generator has a hostname setting, remember to change it:
```js
const sitemap = new SitemapStream({
  hostname: "https://athena-io.vercel.app", // or your custom domain
});
```

Or use an environment variable:
```js
const baseUrl = process.env.SITE_URL || "http://localhost:3000";
```

---

## 📫 Contact
- **Email:** your.email@example.com  
- **LinkedIn:** https://linkedin.com/in/your-profile  
- **GitHub:** https://github.com/your-username  

---

## 📜 License
Released under the **MIT License** — free to use, modify, and share.

---

## ✨ Final Note
If you like this project, consider starring it ⭐ or sharing it.  
Thanks for visiting **ATHENA-IO** — built with code, creativity, and caffeine ☕
