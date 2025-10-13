# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a static website for GUIX Manresa, a construction company based in Barcelona, Spain. The site showcases the company's services, projects, and contact information.

## Architecture

### Project Structure
- **Static HTML/CSS Website**: Single-page application with no framework dependencies
- **index.html**: Main HTML file containing all page sections (hero, about, services, contact)
- **style.css**: Comprehensive CSS with modern styling, animations, and responsive design
- **Assets**: Image files (.webp, .jpg, .png, .svg) for services portfolio and company branding

### Key Sections
- Header with navigation
- Hero section with company introduction
- About section (mission, vision, values)
- Statistics section
- Services showcase with image galleries
- Home renovation portfolio ("Reformas")
- Contact information
- Footer

### Styling Approach
- Mobile-first responsive design
- CSS Grid and Flexbox for layout
- Custom animations and hover effects
- Blue-based color scheme (#1e40af, #3b82f6)
- Modern gradient backgrounds
- Image optimization with WebP format

## Development Commands

### Local Development
```bash
# Serve the site locally (Python 3)
python -m http.server 8000

# Alternative with Node.js (if you have it installed)
npx serve .

# Alternative with PHP (if available)
php -S localhost:8000
```

### Git Operations
```bash
# Check repository status
git --no-pager status

# View recent changes
git --no-pager log --oneline -10

# Stage changes
git add .

# Commit changes
git commit -m "Update website content"

# Push to remote
git push origin main
```

### File Operations
```bash
# List all files including hidden ones
Get-ChildItem -Force

# Find specific file types
Get-ChildItem -Recurse -Include "*.html", "*.css", "*.js"

# Check file sizes (useful for image optimization)
Get-ChildItem -Recurse | Sort-Object Length -Descending | Select-Object Name, Length
```

## Content Management

### Adding New Service Images
- Images should be optimized (WebP preferred for photos, SVG for logos)
- Service images are 280px width minimum for grid layout
- Update both the HTML img src and alt attributes

### Updating Company Information
- Contact details are in the #contacto section
- Company stats are in the .stats-grid section
- Mission/Vision/Values are in the .about-grid section

### Portfolio Images
- Kitchen images: Cocina.webp, Cocina2.webp, etc.
- Living room images: Sala.webp, Sala2.webp, etc.
- All portfolio images follow the same naming convention

## Responsive Design Considerations
- Navigation collapses on mobile (768px breakpoint)
- Logo switches to mobile version (logo-movil.svg) on small screens
- Grid layouts automatically adjust to screen size
- Hero section height adapts to viewport

## Image Assets
- **Logos**: logo.svg (desktop), logo-movil.svg (mobile)
- **Hero background**: hero.jpg
- **Service images**: Technical images for each construction service
- **Portfolio**: Before/after renovation photos in WebP format

## Browser Compatibility
- Modern browsers supporting CSS Grid and Flexbox
- Graceful degradation for older browsers
- Optimized for mobile-first approach