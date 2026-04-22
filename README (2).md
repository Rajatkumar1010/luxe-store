# LUXE — Premium Ecommerce Website

A fully responsive, single-file luxury fashion ecommerce website built with pure HTML, CSS, and JavaScript. No frameworks, no dependencies, no build tools required.

## 🔗 Live Demo

> Deploy to [GitHub Pages](https://pages.github.com/) for a free live URL (see steps below).

## ✨ Features

- **Custom animated cursor** with a smooth trailing ring effect
- **Sticky navigation** with blur backdrop and cart badge counter
- **Hero section** with floating product animation and scroll CTAs
- **Scrolling marquee** banner
- **Category grid** with hover zoom and overlay effects
- **Product grid** (8 items) with quick-add to cart, wishlist button, and sale/new/hot badges
- **Sale promo banner** with statistics
- **Customer testimonials** section
- **Newsletter signup** form
- **Toast notifications** for cart and form actions
- **Scroll-triggered fade-in** animations using IntersectionObserver
- **Fully responsive** — works on mobile, tablet, and desktop
- **Zero dependencies** — one `.html` file is all you need

## 📁 Project Structure

```
luxe-ecommerce/
├── index.html      ← The entire website (HTML + CSS + JS)
└── README.md
```

## 🚀 How to Deploy on GitHub Pages

1. **Create a new GitHub repository** (e.g. `luxe-store`)
2. **Upload** `index.html` and `README.md` to the repo
3. Go to **Settings → Pages**
4. Under *Source*, select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder
6. Click **Save**
7. Your site will be live at: `https://<your-username>.github.io/luxe-store/`

## 🛠 Local Development

No setup needed. Just open the file in your browser:

```bash
# Clone your repo
git clone https://github.com/<your-username>/luxe-store.git
cd luxe-store

# Open directly in browser
open index.html
```

Or use the VS Code **Live Server** extension for hot reload.

## 🎨 Customization

All styles use CSS variables at the top of the file — easy to rebrand:

```css
:root {
  --ink: #0d0d0d;       /* Main dark color */
  --cream: #f5f0e8;     /* Page background */
  --gold: #c8a96e;      /* Accent color */
  --rust: #b84a2e;      /* Sale badge color */
  --muted: #7a7065;     /* Secondary text */
}
```

To change the brand name, search for `LUXE` in `index.html` and replace with your store name.

## 📄 License

Free to use for personal and commercial projects.
