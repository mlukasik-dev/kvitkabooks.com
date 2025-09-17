# kvitkabooks.com

Ukrainian book publisher landing page built with Jekyll and Tailwind CSS v4 for book preorders.

## Project Structure

### Content Files
- **_data/home/book.yaml** - Book details (title, synopsis, pricing, author)
- **_data/home/about.yaml** - Publisher mission and philosophy
- **_data/home/contact.yaml** - Contact info and social links

### Templates
- **index.md** - Homepage entry (uses home layout)
- **_layouts/home.html** - Main page template
- **_includes/home/** - Main page individual components

### Assets
- **assets/css/main.css** - Tailwind CSS v4 imports and @font-face
- **assets/images/** - Book cover with 4/3 ratio (width/height) (`book.png`), author photo (`author.jpg`)
- **assets/svg/** - Logos: `logo.svg` (icon), `logo-text.svg` (text), `logo-full.svg` (complete) and social icons (`instagram.svg`, `threads.svg`, `tiktok.svg`)
- **assets/fonts/** - Fixel Display/Text (sans), Kudry Weird (serif)

### Configuration
- **_config.yml** - Jekyll settings (title: "Видавництво Квітка", url: kvitkabooks.com, lang: uk)

## Brand Guidelines

### Colors

| Color | Hex | Tailwind Class | Usage |
|-------|-----|----------------|--------|
| Deep Green | `#31381C` | `text/bg-[#31381C]` | Primary brand color |
| Golden Book | `#F5DEB3` | `text/bg-[#F5DEB3]` | Secondary brand color |
| Accent Brown | `#4B3226` | `text/bg-[#4B3226]` | Accent elements |
| Golden Pink | `#F6B7BE` | `text/bg-[#F6B7BE]` | Highlights |
| Base Cream | `#FFF8F0` | `text/bg-[#FFF8F0]` | Background |

**Distribution:** 60% base, 25% brand, 10% content, 5% accents

### Typography

| Font | Class | Usage |
|------|-------|--------|
| Fixel Display | `font-fixel-display` | Headlines, titles |
| Fixel Text | `font-fixel-text` | Body text, paragraphs |
| Kudry Weird | `font-kudry` | Book titles, special quotes, decorative |

### Logos
All logos support `fill: currentColor` for color control via Tailwind:
- **Icon only:** 32px min height
- **Text only:** 64px min height
- **Full logo:** 128px min height

## Development

### Commands
```bash
# Start development server
pnpm run dev

# Jekyll runs on http://localhost:4000
```

### Tailwind Config
Custom fonts are configured in `tailwind.config.js`:
```javascript
fontFamily: {
  'fixel-display': ['Fixel Display', 'sans-serif'],
  'fixel-text': ['Fixel Text', 'sans-serif'],
  'kudry': ['Kudry Weird', 'serif'],
}
```

## Key Principles
- **Tailwind-only styling** - No custom CSS beyond @font-face declarations
- **Ukrainian language** - All content in Ukrainian (lang: uk)
- **Highly aesthetic design** - Rich visual experience with careful attention to typography, spacing, and brand expression
- **Mobile-first** - Responsive design starting from mobile