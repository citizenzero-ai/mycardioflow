# MyCardioFlow → Lightspeed eCom (E-Series / Instant Site)

Instant Site doesn't accept uploaded themes. You rebuild the page from:
- native Instant Site parts (header, footer, product grid, cart and checkout, so your real catalog works), plus
- the custom code sections in this kit for the branded homepage sections.

## 1. Host the images and video (do this first)
Instant Site custom code can't use local files, so the images need public URLs.
This kit is set up to be its own GitHub Pages site.
1. Create a GitHub repo and upload the **contents** of this kit folder to the repo root
   (`index.html`, `preview.html`, `custom.css`, `.nojekyll`, `img/`, `sections/`, `README.md`).
   Keep `img/` at the root. The section files expect `/img/` there.
2. Turn on GitHub Pages: Settings > Pages > Deploy from a branch > main > /(root) > Save.
3. After 1–2 minutes:
   - https://YOUR-USERNAME.github.io/YOUR-REPO/ shows the styled homepage preview
   - https://YOUR-USERNAME.github.io/YOUR-REPO/img/tread.jpg shows the treadmill
4. In every file in `sections/`, find and replace
   `https://YOUR-USERNAME.github.io/YOUR-REPO/img/` with your real URL.

(Alternative: upload each image to Lightspeed's own media/image fields and paste those URLs instead.)

`preview.html` loads `custom.css` and the same images, so what you see there is what the
pasted sections will look like. If you edit a section, make the same edit in `preview.html`.

## 2. Pick a base theme
Retail POS > Online > Webstore (or Website) > Edit Site > Settings > Themes.
Choose a clean, minimal theme and click Publish.

## 3. Brand fonts and colors
Settings > Fonts & Styles:
- Colors: background #F8F3EB, text #1D2024, accent/buttons #F8671A
- Fonts: pick the closest to Bricolage Grotesque (headings) and Hanken Grotesk (body)
Then open Advanced custom CSS and paste ALL of `custom.css`. Publish.

## 4. Header and logo
Edit the Header section and upload `img/logo-lockup-light.png`.
Menu links: Treads, Bikes, Rowers, Membership, Financing (link them to your store categories).

## 5. Build the homepage (top to bottom)
For each file in `sections/`, add a section of type Custom code / HTML, paste the file's contents, and save.
1. 01-hero.html (you can delete the theme's default cover section)
2. 02-product-strip.html (update each link to its product page)
3. Native Store / Featured products section: this is your real, shoppable product grid
4. 03-value-props.html
5. 04-testimonials.html
6. 05-membership.html
7. 06-apparel-banner.html
8. 07-journal.html
Footer: use the native footer and add the dark logo and your links.

## 6. Products
Add Tread, Tread+, Bike, Bike+ and Row+ in your catalog with the product images from `img/`.
Product pages and the cart are Lightspeed's own, styled by your Fonts & Styles settings.

## Notes
- Placeholder links to update before publishing: `href="/products"` (hero button, product strip,
  apparel button) and `href="#"` ("Take a tour", "Explore membership", the three journal cards).
- The hero video plays muted and loops (browsers require mute for autoplay).
- If a section looks unstyled, the CSS from step 3 is missing or wasn't published.
- Lightspeed support doesn't troubleshoot custom code. Keep this kit so you can re-paste anything.
