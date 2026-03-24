# Liz Schaefer Designs LLC — GitHub Pages Site

A clean, modern, Etsy-style portfolio and shop landing page for handmade crafts,
t-shirt designs, and custom artwork. Built with pure HTML/CSS — no frameworks required.

🌐 **Live site:** https://liz-schaefer-designs-llc.github.io/liz.schaefer.designs.llc.github.io/

---

## 📁 File Structure

```
liz.schaefer.designs.llc.github.io/
├── index.html          ← Main landing page
├── styles/
│   └── style.css       ← All styles (colors, layout, responsive)
├── media/
│   ├── logo.svg                     ← Hero logo / profile image
│   ├── product-sticker-pack.svg     ← Product placeholder images
│   ├── product-tshirt-design.svg
│   ├── product-original-art.svg
│   ├── product-art-print.svg
│   ├── product-tote-bag.svg
│   ├── product-greeting-cards.svg
│   └── product-custom-logo.svg
└── README.md
```

---

## 🛒 How to Add or Update Products

1. **Add a product image** to the `/media/` folder (JPG, PNG, or SVG recommended).
   - Name it something descriptive, e.g. `product-watercolor-cats.jpg`
   - Aim for square or near-square images (at least 600 × 600 px) for best display.

2. **Open `index.html`** in a text editor.

3. **Find the comment** that reads:
   ```html
   <!-- ADD MORE PRODUCTS HERE -->
   ```

4. **Copy an existing `<article class="product-card">` block** and paste it above
   the comment, then update these five fields:

   | Field | Where to edit |
   |---|---|
   | Product image | `src="media/YOUR-IMAGE.jpg"` and `alt="..."` |
   | Product name | `<h3 class="product-name">...</h3>` |
   | Description | `<p class="product-desc">...</p>` |
   | Price | `<p class="product-price">$XX.XX</p>` |
   | PayPal link | `href="https://paypal.me/YOUR_USERNAME"` |
   | Venmo link | `href="https://venmo.com/YOUR_USERNAME"` |

5. **Save the file** and push to GitHub — the site updates automatically.

---

## 🎨 How to Change the Logo / Hero Image

Replace `media/logo.svg` with your own image (PNG or JPG works too).
Then update the `src` attribute in `index.html`:

```html
<img src="media/your-logo.png" alt="Liz Schaefer Designs LLC logo" class="hero-logo" />
```

---

## 🎨 How to Change Colors

Open `styles/style.css` and edit the CSS variables at the top of the file:

```css
:root {
  --turquoise: #3DBDB5;   /* Primary color */
  --coral:     #FF6B6B;   /* Accent color  */
  --cream:     #FFF8F2;   /* Page background */
  /* ... */
}
```

Change any hex values and save — all elements that use those variables will update instantly.

---

## 🔗 How to Update Payment Links

In each product card in `index.html`, find:

```html
<a href="https://paypal.me/LizSchaeferDesigns" ...>🅿 Buy with PayPal</a>
<a href="https://venmo.com/LizSchaeferDesigns"  ...>💙 Pay with Venmo</a>
```

Replace the `href` values with your actual PayPal.me and Venmo profile URLs.
You can also use PayPal's "Buy Now" button generator for fixed-price items.

---

## 📱 Social Media Links

In `index.html`, find the footer section and replace the `href="#"` placeholders
with your real social media URLs:

```html
<a href="https://etsy.com/shop/YourShop">🛍 Etsy</a>
<a href="https://instagram.com/yourhandle">📸 Instagram</a>
<!-- etc. -->
```

Also update the email address:
```html
<a href="mailto:hello@lizschaeferdesigns.com">✉ Email</a>
```

---

## 🗂 Future Category Pages

To expand into categories (stickers, shirts, prints, etc.), create additional HTML
pages following the same structure:

```
stickers/index.html
shirts/index.html
prints/index.html
```

Each page can reuse `../styles/style.css` and its own product grid.
Add links to those pages in the `<nav>` of `index.html`.

---

## 🚀 Deploying

This site is hosted on **GitHub Pages** automatically.
Any commit pushed to the default branch will be reflected on the live site within
a few minutes — no build step required.

---

&copy; 2026 Liz Schaefer Designs LLC

