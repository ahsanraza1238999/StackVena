# StackVena Landing Page

A clean, responsive landing page for StackVena — a full-stack web development and AI integration agency.

---

## Files

```
/
├── index.html       # Main landing page (HTML + CSS + JS)
├── favicon.svg      # Browser tab icon (square-cropped logo mark)
├── logo-full.svg    # Logo with company name (used in navbar & footer)
└── logo-icon.svg    # Icon-only logo (source file)
```

---

## How to Run

No build tools or dependencies required. Just open `index.html` in a browser.

**With a local server (recommended):**
```bash
# Using VS Code Live Server extension — right-click index.html → Open with Live Server

# Or using Python
python -m http.server 5500

# Or using Node
npx serve .
```

Then visit `http://localhost:5500`

---

## Customization

### Change Logo Size

In `index.html`, find these two CSS rules:

```css
/* Navbar logo */
.nav__logo img {
  height: 52px; /* change this */
}

/* Footer logo */
.footer__logo img {
  height: 38px; /* change this */
}
```

`width: auto` is already set — the logo scales proportionally.

### Change Nav Bar Height

```css
:root {
  --nav-h: 80px; /* change this */
}
```

### Change Colors

All colors are CSS variables at the top of the stylesheet inside `:root {}`:

```css
--accent:   #3b7cf4;  /* primary blue */
--accent-2: #00c9ff;  /* cyan highlight */
--accent-3: #7b5ea7;  /* purple */
--bg:       #06080f;  /* page background */
--text:     #e8ecf4;  /* primary text */
--text-2:   #8892a4;  /* secondary text */
```

### Change Content

All page content (headings, descriptions, team info, email) is plain HTML inside `index.html`. Search for the text you want to update and edit it directly.

---

## Sections

| Section | ID |
|---|---|
| Hero | `#home` |
| Services | `#services` |
| Why Us | *(no anchor)* |
| Platforms | *(no anchor)* |
| Founders / About | `#about` |
| Contact | `#contact` |

---

## Tech Stack

- Plain HTML5, CSS3, and vanilla JavaScript
- No frameworks, no dependencies, no build step
- Fonts loaded from Google Fonts (Syne + DM Sans)

---

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). Requires JavaScript for scroll animations and the mobile menu.
