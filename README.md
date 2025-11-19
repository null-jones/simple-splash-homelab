# simple-splash-homelab

A modern, minimal homelab splash page with a clean aesthetic and responsive design.

## Features

- 🌌 **Animated space/stars background** with parallax layers
- 💎 **Glassmorphism design** with semi-transparent cards
- ✨ **Glowing JONESBOX header** with modern Orbitron font
- 📱 **Fully responsive** - works on desktop, tablet, and mobile
- 🎯 **Zero JavaScript** - pure HTML and CSS
- 🔗 **Pre-configured service cards** for common homelab applications

## Quick Start

1. Open `index.html` in a web browser
2. Customize the card links in `index.html` to point to your homelab services
3. Deploy to any static web server (nginx, Apache, GitHub Pages, etc.)

## Customization

### Adding/Removing Cards

Edit `index.html` to add or remove service cards. Each card follows this structure:

```html
<a href="https://your-service.local" class="card" target="_blank">
    <div class="card-icon">🎬</div>
    <h2>Service Name</h2>
    <p>Description</p>
</a>
```

### Changing Colors

Edit `styles.css` to customize colors, spacing, and other visual elements. Key variables:
- Card background: `rgba(255, 255, 255, 0.05)`
- Glow colors: Blue tones in the text-shadow properties
- Background gradient: `#1B2735` to `#090A0F`

## Deployment

### Static Web Server (nginx)

```nginx
server {
    listen 80;
    server_name homelab.local;
    root /path/to/simple-splash-homelab;
    index index.html;
}
```

### GitHub Pages

Push to a GitHub repository and enable GitHub Pages in Settings.

### Docker

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
```

## Screenshots

![Desktop View](https://github.com/user-attachments/assets/2fe3b3a7-450f-4f11-96ea-05ccd1fe026e)

## License

MIT