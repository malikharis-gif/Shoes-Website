from pathlib import Path

readme = """# SOLE — Premium Footwear Store

A responsive, single-page online shoe store demo built with **HTML, CSS, and vanilla JavaScript**.

## Features

- Premium cream and forest-green color palette
- Google Fonts: Playfair Display and DM Sans
- Responsive layout for desktop, tablet, and mobile
- Hero section and featured product collection
- Product filters: All Shoes, Sneakers, Casual, and Formal
- Add-to-bag interaction with live item count
- Demo cart summary with item prices and total
- Newsletter signup interaction
- Product and lifestyle images from Unsplash

## Project Files

```text
sole-boot-shop/
├── sole_boot_shop.html
└── README.md
```

## How to Run

1. Download `sole_boot_shop.html`.
2. Open the file in a modern web browser (Google Chrome, Microsoft Edge, Firefox, etc.).
3. Browse the products and try the category filters and **Add to bag** buttons.

No installation, server, or build tools are required.

## Customization

Open `sole_boot_shop.html` in a code editor such as Visual Studio Code.

- **Store name:** Search for `SOLE` in the HTML and replace it with your store name.
- **Colors:** Edit the CSS variables inside the `:root` block near the top of the `<style>` section.
- **Products:** Find the `<div class="products" id="products">` section. Update product names, prices, categories, image URLs, and the `addToCart()` values.
- **Images:** Replace the Unsplash image URLs with your own product image URLs.
- **Contact details:** Update the footer and contact section with your business information.

## Important Notes

This is a front-end demo, not a complete e-commerce system.

- Cart contents are kept only in the current browser page session.
- Checkout and online payments are not connected.
- Newsletter signup displays a demo confirmation; it does not save email addresses.
- Product images and Google Fonts require an internet connection.

To launch a real online store, connect the interface to a backend/database, order management, delivery workflow, and a payment provider.

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript
- Google Fonts
- Unsplash images

---

Made with care for every step.
"""
path = Path("/mnt/data/README.md")
path.write_text(readme, encoding="utf-8")
print(f"Created: {path} ({path.stat().st_size:,} bytes)")
