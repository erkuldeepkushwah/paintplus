# Paint Plus 🎨

**Bring Your Walls to Life** — a modern, responsive website for a paint & home-improvement brand, built as a single self-contained HTML page.

🌐 **Live Site:** [https://paintplus.pages.dev](https://paintplus.pages.dev)

---

## About

Paint Plus is a single-page marketing website for a paints, textures and home-improvement business. It showcases product categories, a design catalog, services, an interactive paint cost calculator, and an enquiry form — all with a clean pink-and-orange brand theme.

## Features

- **Responsive design** — works across mobile, tablet and desktop, with a dedicated mobile navigation menu.
- **Hero section** — full-screen banner with the tagline *"Har Rang Kuch Kehta Hai"* and call-to-action buttons.
- **Paints & Textures** — product category cards (Interior, Exterior, Waterproofing, Wood Solutions) that open a detail modal.
- **Catalog** — a grid of 10 catalog designs; clicking any photo opens the full catalog on Google Drive.
- **Home Improvement Services** — highlights of the services offered beyond painting.
- **Paint Cost Calculator** — lets visitors estimate painting cost based on area.
- **Enquiry form** — for booking a consultation.
- **Floating WhatsApp button** — quick chat link on every screen.
- **Popular Tags** — quick links to common product searches.

## Tech Stack

| Layer | Used |
|-------|------|
| Markup | HTML5 |
| Styling | [Tailwind CSS](https://tailwindcss.com/) (via CDN) |
| Icons | [Font Awesome 6](https://fontawesome.com/) (via CDN) |
| Fonts | [Google Fonts – Poppins](https://fonts.google.com/specimen/Poppins) |
| Interaction | Vanilla JavaScript (inline) |
| Hosting | [Cloudflare Pages](https://pages.cloudflare.com/) |

## Project Structure

```
paintplus/
├── index.html      # The complete website (markup, styles, scripts)
├── styles.css      # Optional extra stylesheet
├── script.js       # Optional extra script
└── README.md
```

> The site is self-contained: `index.html` loads Tailwind, Font Awesome and Poppins from CDNs and includes its own styles and scripts. The standalone `styles.css` and `script.js` files are optional and not required for the page to work.

## Getting Started

No build step is needed. To run it locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/erkuldeepkushwah/paintplus.git
   ```
2. Open `index.html` in your browser.

Or serve it with any static server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

The site is deployed on **Cloudflare Pages** and is live at **[paintplus.pages.dev](https://paintplus.pages.dev)**.

To deploy your own copy:

1. Push the repository to GitHub.
2. In the Cloudflare dashboard, go to **Workers & Pages → Create → Pages → Connect to Git**.
3. Select this repository.
4. Leave the build command empty (static site) and set the output directory to `/` (root).
5. Deploy — every push to `main` will publish automatically.

## Customization

- **Catalog link:** the catalog photos point to a Google Drive URL. To change it, search for `drive.google.com` in `index.html` and replace the `href` on the catalog cards.
- **Catalog images:** swap the Unsplash image `src` URLs in the catalog grid with your own photos.
- **Contact details:** phone/WhatsApp links use `wa.me/918349363479`; update these in `index.html` to change the number.
- **Brand colors:** the theme uses Tailwind's `pink` and `orange` palettes; adjust the class names to rebrand.

## License

This project is provided for demonstration purposes. © 2025 Paint Plus Ltd. All rights reserved.
