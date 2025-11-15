# LocalLoop Website

Official website for LocalLoop - South Africa's Hyperlocal Social Network

🌍 **Live Site**: [mhalesto.github.io/localloop.app](https://mhalesto.github.io/localloop.app)
🔗 **Custom Domain** (when configured): [localloop.app](https://localloop.app)

## About LocalLoop

LocalLoop connects communities across South African cities and towns. Share local stories, discover events, find services, and connect with neighbors.

### Features

- 📍 City-based community feeds
- 🎨 AI-powered profile avatars (GPT-4o Vision)
- 📅 Local events calendar
- 🛍️ Community marketplace
- 💬 Real-time discussions
- 🌈 Customizable themes
- 🔔 Smart notifications

## Website Structure

```
├── index.html          # Homepage - main landing page
├── about.html          # About page
├── contact.html        # Contact form
├── privacy.html        # Privacy policy
├── terms.html          # Terms of service
├── 404.html           # 404 error page with Lottie animation
├── styles.css         # Global styles
├── main.jsx           # Main JavaScript (React)
├── logo.svg/png       # LocalLoop logos
├── mockup.svg         # App mockup illustration
├── error-404.json     # Lottie 404 animation
└── screens/           # App screenshots (SVG)
```

## Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with gradients and animations
- **React 18** - UI components (via Babel standalone)
- **Lottie** - Smooth animations
- **Responsive Design** - Mobile-first approach

## Local Development

```bash
# Clone the repository
git clone https://github.com/mhalesto/localloop.app.git
cd localloop.app

# Serve locally
npx serve .
# Or use Python
python3 -m http.server 8000

# Open http://localhost:8000
```

## Deployment

**Automatic**: GitHub Pages deploys from `main` branch automatically.

Every push to `main` triggers a deployment to:
- https://mhalesto.github.io/localloop.app

## Custom Domain Setup

### DNS Configuration for localloop.app

**A Records** (apex domain):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME Record** (www subdomain):
```
www → mhalesto.github.io
```

### GitHub Settings

1. Go to repo **Settings** → **Pages**
2. Add custom domain: `localloop.app`
3. Enable **Enforce HTTPS**
4. Wait for DNS verification (can take 24-48 hours)

## Content Updates

### Updating Text Content
- Edit respective HTML files directly
- Use React JSX components for dynamic sections

### Updating Styles
- Modify `styles.css` for global styles
- Inline styles in HTML for page-specific changes

### Adding Pages
1. Create new `.html` file
2. Link from navigation in `index.html`
3. Follow existing page structure

## Contact Forms

Contact form submissions are handled via:
- FormSpree (if configured)
- Or custom backend endpoint

Update form action in `contact.html` as needed.

## License

© 2024 LocalLoop. All rights reserved.

---

🇿🇦 Proudly built in South Africa
