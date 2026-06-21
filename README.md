# Volt & Byte – Premium Electronics Website

A cutting-edge, single-page e‑commerce experience for a premium electronics retailer. **Volt & Byte** combines a futuristic cyberpunk aesthetic with practical shopping features — including product browsing, cart management, wishlist, comparison tool, and interactive services — all built with vanilla HTML, CSS, and JavaScript.

---
<img width="1882" height="896" alt="image" src="https://github.com/user-attachments/assets/349f3761-2a7a-46de-b167-dedc490eff62" />

---
## Overview

**Volt & Byte** is a conceptual premium electronics brand website that offers a futuristic, dark‑themed shopping experience. The site showcases:

- Next‑gen laptops, desktops, components, and gaming gear
- Interactive browsing with carousels, filtering, and quick‑view
- Smart shopping tools: wishlist, comparison, trade‑in estimator
- A fully functional cart with local storage persistence
- A cyberpunk aesthetic with glowing cyan accents, particle animations, and 3D product mockups

All data is static (JavaScript‑driven), making it perfect for **brand showcases**, **portfolio projects**, or as a foundation for a full e‑commerce platform.

---

## Features

| Feature                     | Description                                                                                      |
|-----------------------------|--------------------------------------------------------------------------------------------------|
| **Hero with Typing Effect** | Animated headline with a blinking cursor and particle background.                                |
| **3D Laptop Mockup**        | Floating, rotating 3D laptop with glowing keyboard (desktop only).                               |
| **Product Carousel**        | Horizontal scrollable product cards with hover tilt, wishlist, compare, and quick‑view.          |
| **Shop by Category**        | Visual category tiles with matrix‑rain animations.                                               |
| **Deals & Countdown**       | Flash deal section with a countdown timer and discounted product cards.                          |
| **Services Cards**          | Flip‑over cards for Trade‑In, Extended Warranty, and Tech Support.                               |
| **Trade‑In Calculator**     | Estimate device trade‑in value with a smooth counter animation.                                  |
| **Shopping Cart**           | Slide‑out panel with quantity controls, removal, subtotal, and localStorage persistence.         |
| **Wishlist**                | Heart‑icon toggle with count badge and localStorage persistence.                                 |
| **Product Comparison**      | Compare up to 4 products side‑by‑side with spec highlighting.                                    |
| **Product Quick‑View**      | Modal with image gallery, full specs, add‑to‑cart, and compare actions.                          |
| **Search Overlay**          | Full‑screen search with live suggestions; shortcut `Ctrl+K` (or `Cmd+K`).                       |
| **Dark / Light Theme**      | Toggleable "Matrix" (dark) and "Lab" (light) modes; preference saved in `localStorage`.         |
| **Scroll Progress Bar**     | Thin glowing bar at the top showing scroll progress.                                             |
| **Live Chat Bubble**        | Floating chat button with quick‑action options (demo).                                          |
| **Newsletter Signup**       | Email subscription with toast feedback.                                                         |
| **Contact Form**            | Validated contact form with toast notification.                                                  |
| **Responsive Design**       | Fully responsive across desktop, tablet, and mobile devices.                                    |
| **Accessibility**           | ARIA labels, semantic HTML, keyboard navigation (Escape to close modals/overlays).              |
| **PWA Ready**               | Inline service worker and manifest for basic offline support.                                   |
| **Keyboard Shortcuts**      | `Ctrl+K` / `Cmd+K` to open search. `Escape` to close modals, panels, and overlays.              |
| **Persistent Data**         | Cart, wishlist, compare list, and theme stored in `localStorage`.                               |

---

## Technology Stack

- **HTML5** — Semantic markup with ARIA attributes for accessibility.
- **CSS3** — Custom properties (variables), Grid, Flexbox, animations, transitions, and dark/light theming.
- **Vanilla JavaScript (ES6+)** — DOM manipulation, event handling, state management, and localStorage persistence.
- **Google Fonts** — [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) (headings) and [Source Code Pro](https://fonts.google.com/specimen/Source+Code+Pro) (monospace specs).
- **Unsplash** — High‑quality stock images for products and hero background.
- **Service Worker** — Basic offline caching via inline registration.
- **Manifest** — Inline JSON manifest for PWA support.

**No frameworks, no build tools, no dependencies** — everything is self‑contained in one HTML file.

---

## Installation & Usage

### 1. Download the file

Save `Laptop.html` to your local machine.

### 2. Open in a browser

Double‑click the file or open it in your favourite browser (Chrome, Firefox, Edge, Safari).

### 3. Offline support

The page includes a minimal service worker that enables basic offline caching — once loaded, you can revisit without an internet connection.

### 4. Hosting

For live deployment, upload the file to any static hosting service (Netlify, Vercel, GitHub Pages, etc.).

---

## Project Structure

The entire application is contained in a **single HTML file** with well‑organised sections:

```
Laptop.html
├── <head>
│   ├── Meta tags (viewport, description, theme-color)
│   ├── Google Fonts links
│   └── <style> (all CSS — ~800 lines)
├── <body>
│   ├── Loading screen (animated circuit traces)
│   ├── Scroll progress bar
│   ├── Header (fixed, with logo, mega‑menu, search, theme toggle, wishlist, cart)
│   ├── Search overlay (full‑screen with suggestions)
│   ├── Cart overlay & slide‑out panel
│   ├── Comparison overlay (with table)
│   ├── Hero section (particles, typing, 3D laptop)
│   ├── Featured products carousel
│   ├── Shop by category grid
│   ├── Deals section (countdown + deal cards)
│   ├── Services section (flip cards: Trade‑In, Warranty, Support)
│   ├── Store locator & contact form
│   ├── Newsletter & community section
│   ├── Product quick‑view modal
│   ├── Live chat bubble
│   ├── Toast container
│   ├── Back to top button
│   ├── Footer
│   └── <script> (all JavaScript — ~600 lines)
└── (end)
```

---

## Key Components

### Loading Screen

- Animated circuit traces with glowing dots
- Auto‑hides after the page loads (`window.load` event)
- Smooth opacity/visibility transition

### Hero Section with Typing Effect

- Full‑width hero with particle canvas background (golden dots with occasional connections)
- Typing animation: "Power Meets Precision" with blinking cursor
- Call‑to‑action button with ripple effect
- 3D laptop mockup (desktop only): floating, rotating, with glowing keyboard and screen shimmer

### Product Carousel

- Horizontal scrollable track of product cards
- Each card shows:
  - Product image, spec badge, name, CPU/GPU preview, price (with original price if discounted)
  - **Wishlist** heart (♡/❤️)
  - **Compare** button (⚖️)
  - **Quick View** and **Add to Cart** buttons (appear on hover)
- Hover tilt effect (3D parallax)
- Carousel navigation arrows

### Shop by Category

- Grid of 7 category tiles (Laptops, Desktops, Monitors, Peripherals, Components, Audio, Gaming Gear)
- Some tiles have a "matrix rain" background animation
- Hover underline and scale effect

### Deals & Countdown Timer

- Countdown to a fixed future date (3 days from current time)
- Displays days, hours, minutes, seconds
- Products with discount badges (percentage off)
- Deals carousel with same product card design

### Services & Support Cards

Three flip‑over cards:

- **Trade‑In** — select a laptop model to see an animated estimated value
- **Extended Warranty** — peace of mind protection
- **24/7 Tech Support** — real human support

Cards flip on click with a 3D rotation animation.

### Shopping Cart

- Slide‑out panel from the right
- Cart items list with thumbnails, quantity controls (+/−), and remove button
- Subtotal calculation
- Cart count badge in the header with bounce animation on update
- Persistent via `localStorage` (`vb_cart`)

### Wishlist

- Heart icon toggle on each product card
- Wishlist count badge in the header
- Persistent via `localStorage` (`vb_wishlist`)

### Product Comparison Tool

- Compare up to **4 products** side‑by‑side
- Specs compared: CPU, GPU, RAM, Storage, Display, Price
- Different values are highlighted in cyan
- Persistent via `localStorage` (`vb_compare`)
- Floating "Compare" button with count badge

### Product Quick‑View Modal

- Opens on product card click or "Quick View" button
- Displays:
  - Main image with thumbnail strip (click to switch)
  - Product name, rating, price (with discount if applicable)
  - Full specs list (CPU, GPU, RAM, Storage, Display)
  - "Add to Cart" and "Compare" buttons
- Closes with ✕ button, overlay click, or Escape key

### Search Overlay

- Full‑screen overlay with search input
- Live suggestions matching product name, brand, spec badge, or category
- Click a suggestion to open the product modal
- Keyboard shortcut: `Ctrl+K` / `Cmd+K`
- Closes with ✕ button, overlay click, or Escape key

### Dark / Light Theme

- Toggle button in the header (⚡)
- "Matrix" (dark) and "Lab" (light) modes
- All colors controlled by CSS custom properties
- Preference saved to `localStorage` (`vb_theme`)

### Live Chat Bubble

- Floating chat button in the bottom‑left
- Click to open a quick‑action menu
- Demo options: Track Order, Returns, Tech Specs, Price Match
- Closes on outside click

### Trade‑In Calculator

- Inside the Trade‑In service card (back side)
- Dropdown to select a laptop model
- Animated counter displays estimated value
- "Start Trade‑In" button (demo)

---

## Data Model

The site uses static JavaScript data structures for easy modification:

### Products

```javascript
const products = [
  {
    id: 1,
    name: 'Nebula X1 Pro',
    category: 'Laptops',
    brand: 'Volt',
    price: 2499,
    wasPrice: 2799,
    rating: 4.8,
    specBadge: 'RTX 4090',
    cpu: 'Intel i9-14900HX',
    gpu: 'RTX 4090',
    ram: '32GB DDR5',
    storage: '1TB NVMe',
    display: '16" 4K OLED',
    img: 'https://...',
    thumbs: ['https://...', 'https://...']
  },
  // ...
];
```

### Categories

```javascript
const categories = [
  { name: 'Laptops', icon: '💻', bgClass: 'matrix-rain' },
  // ...
];
```

---

## Customization

### Change Colors

Edit the CSS custom properties in the `:root` block:

```css
:root {
  --accent-cyan: #00f0ff;      /* Primary accent */
  --accent-purple: #b347ea;    /* Secondary accent */
  --bg-primary: #0a0a0f;       /* Background */
}
```

### Update Product Data

Modify the `products` array in the JavaScript section — add new products, change prices, images, or specs.

### Add New Categories

Update the `categories` array with new entries.

### Modify Countdown Duration

Change the `endDate.setDate(endDate.getDate() + 3)` line in the `startCountdown()` function.

### Change Trade‑In Values

Update the `<option value="...">` tags inside `#trade-select` with new model names and values.

### Replace Images

All product and category images are from Unsplash. Replace the `img` and `thumbs` URLs with your own.

---

## Browser Support

| Browser          | Version | Support |
|------------------|---------|---------|
| Chrome           | 60+     | ✅ Fully supported |
| Firefox          | 60+     | ✅ Fully supported |
| Safari           | 14+     | ✅ Fully supported |
| Edge             | 79+     | ✅ Fully supported |
| Opera            | 50+     | ✅ Fully supported |
| Internet Explorer| 11-     | ❌ Not supported |

The site uses modern CSS features (Grid, Custom Properties, `backdrop-filter`) and ES6 JavaScript, so it works best in modern browsers.

---

## Performance Considerations

- **Image optimisation** — all images use `loading="lazy"` and are served with `w=400&h=300&fit=crop` parameters.
- **No external dependencies** — everything is self‑contained, reducing network requests.
- **Service Worker** — caches assets for offline access.
- **GPU‑accelerated animations** — uses `transform` and `opacity` for smooth performance.
---

*"Power meets precision."* ⚡
