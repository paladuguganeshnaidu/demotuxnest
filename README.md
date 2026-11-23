# TuxNest Demo

Production-ready demo site for TuxNest — deployed via GitHub Pages.

## Live Site
🌐 **https://paladuguganeshnaidu.github.io/demotuxnest/**

## Features
- Responsive, accessible homepage with semantic HTML5
- Modern CSS with custom properties (CSS variables)
- Mobile-first responsive design
- SEO optimized with meta tags, Open Graph, Twitter Cards, JSON-LD structured data
- GitHub Actions auto-deploy on push to `main`
- Custom 404 page with consistent styling
- PWA support with manifest.json
- Accessibility compliant (WCAG 2.1 AA)
- Dark/light mode support via `prefers-color-scheme`
- Reduced motion support via `prefers-reduced-motion`
- High contrast mode support
- Print stylesheet

## Project Structure
```
demotuxnest/
├── index.html          # Main homepage
├── 404.html            # Custom 404 page
├── styles.css          # All styles
├── favicon.svg         # SVG favicon
├── manifest.json       # PWA manifest
├── robots.txt          # Search engine directives
├── sitemap.xml         # XML sitemap
├── .nojekyll           # Disable Jekyll processing
└── .github/workflows/
    └── pages.yml       # GitHub Pages deployment
```

## Local Development
```bash
# Serve locally with Node.js
npx serve .

# Or with Python
python -m http.server 8000

# Or with PHP
php -S localhost:8000
```

Then open http://localhost:8000

## Deployment
Automatic via GitHub Actions on every push to `main`.

The workflow (`.github/workflows/pages.yml`):
1. Checks out the repository
2. Configures GitHub Pages
3. Uploads the entire repository as an artifact
4. Deploys to GitHub Pages

## Customization
### Colors
Edit CSS custom properties in `styles.css`:
```css
:root {
  --accent: #00d4aa;        /* Primary brand color */
  --bg: #0d0d14;            /* Background */
  --fg: #e8e8f0;            /* Foreground text */
  /* ... more variables */
}
```

### Content
Edit `index.html` to update:
- Hero section text and stats
- Feature cards
- Platform cards
- Code preview
- Testimonials
- Footer links

### SEO
Update in `index.html`:
- `<title>` and `<meta name="description">`
- Open Graph tags (`og:title`, `og:description`, `og:image`)
- Twitter Card tags
- JSON-LD structured data

Update `sitemap.xml` with your URLs.

## Performance
- No external JavaScript frameworks
- Minimal CSS (~15KB gzipped)
- System fonts with Google Fonts preconnect
- Optimized SVG icons inline
- No render-blocking resources

## Accessibility
- Semantic HTML5 elements
- Skip to main content link
- ARIA labels and roles
- Focus visible states
- Color contrast ratios (WCAG AA)
- Reduced motion support
- High contrast mode support
- Keyboard navigable

## Browser Support
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## License
MIT License — see [LICENSE](https://github.com/paladuguganeshnaidu/tuxnestdesktop/blob/main/LICENSE) for details.

---
Built for the [TuxNest ecosystem](https://github.com/paladuguganeshnaidu/tuxnestdesktop).