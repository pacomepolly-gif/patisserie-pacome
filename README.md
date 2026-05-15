# 🥐 La Pâtisserie Française

A beautiful recipe website for French pastry, built with Next.js. Ready to deploy on Vercel in minutes.

---

## 🚀 Deploy in 3 steps

### Step 1 — Create accounts (free)
- [github.com](https://github.com) — create a free account
- [vercel.com](https://vercel.com) — sign up with your GitHub account

### Step 2 — Upload to GitHub
1. Go to github.com → click **"New repository"**
2. Name it `patisserie-francaise` → click **Create**
3. Upload ALL the files from this folder into the repository

### Step 3 — Deploy on Vercel
1. Go to [vercel.com/new](https://vercel.com/new)
2. Click **"Import"** next to your GitHub repository
3. Click **Deploy** — that's it! ✅

Your site will be live at: `https://patisserie-francaise.vercel.app`

---

## 📁 Project structure

```
patisserie/
├── pages/
│   ├── index.js          ← Public homepage with all recipes
│   ├── admin.js          ← Private admin to add recipes
│   ├── _app.js
│   └── recette/
│       └── [id].js       ← Individual recipe page
├── components/
│   └── Nav.js
├── lib/
│   └── recipes.js        ← All recipe data (edit this!)
├── styles/
│   └── globals.css
└── package.json
```

---

## ✏️ Add a new recipe

### Option A — Via the Admin page
1. Go to `yoursite.vercel.app/admin`
2. Password: `patisserie2024` (change this in `pages/admin.js`!)
3. Fill in the form → copy the generated code
4. Paste it into `lib/recipes.js` in the `recipes` array
5. Push to GitHub → Vercel redeploys automatically

### Option B — Edit directly
Open `lib/recipes.js` and add a new object to the `recipes` array following the same format.

---

## 🔐 Change the admin password
Open `pages/admin.js` and change line:
```js
const ADMIN_PASSWORD = 'patisserie2024';
```

---

## 🎨 Customize
- **Colors**: Edit CSS variables at the top of `styles/globals.css`
- **Site name**: Search and replace "La Pâtisserie" across files
- **Recipes**: Edit `lib/recipes.js`
