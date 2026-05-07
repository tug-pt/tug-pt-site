# TUG-PT Website Migration Summary

## Migration Completed: TUG-PT (Static HTML) → TUG-PT2 (Jekyll)

### ✓ Content Migrated

All 8 pages have been successfully converted from static HTML to Jekyll markdown format:

1. **index.md** — Homepage with hero section and feature rows
2. **sobre.md** — About page (mission, history)
3. **noticias-eventos.md** — News & Events section with named anchors
4. **publicacoes.md** — Publications/Resources
5. **aprender-tex.md** — Learning guide with quick references
6. **comunidade.md** — Community info (participation, collaboration)
7. **modelos.md** — LaTeX templates by institution
8. **adesao.md** — Membership & Contact information
9. **contactos.md** — Additional contact details

### ✓ Assets Migrated

- **Logo**: logo.svg, logo.png ✓
- **Icons**: 8 icon sets (SVG + PNG fallbacks) ✓
- **CSS**: 
  - Original style.css copied as assets/css/tug-pt.css ✓
  - main.scss (Jekyll template CSS) present ✓

### ✓ Configuration

- **_config.yml**: Navigation updated with all 9 pages
- **Gemfile**: Updated for Ruby 2.6 compatibility (Jekyll 4.1.0)
- **Layouts**: Using minimal-mistakes Jekyll theme with single page layout
- **Front Matter**: All pages include title, permalink, layout, and author_profile fields

### ✓ Features Preserved

- Full Portuguese content and localization
- Navigation structure with active page highlighting
- Named anchors for sections (e.g., #noticias, #eventos)
- All links converted to Jekyll permalinks
- Brand colors and styling (--primary: #142C4B, --accent: #F28C28)
- Responsive design via minimal-mistakes theme

### Navigation Structure

All pages are accessible via:
- `/` — Homepage
- `/sobre/` — About
- `/noticias-eventos/` — News & Events
- `/publicacoes/` — Publications
- `/aprender-tex/` — Learn TeX
- `/comunidade/` — Community
- `/modelos/` — Templates
- `/adesao/` — Membership
- `/contactos/` — Contacts

### To Build and Deploy

```bash
cd /Users/jml/LOCAL/Repos/TUG-PT2

# Install dependencies (may require Ruby 3.0+)
bundle install

# Build the site
bundle exec jekyll build

# Preview locally
bundle exec jekyll serve

# Output will be in _site/ directory
```

### Notes

- The site uses the minimal-mistakes Jekyll theme for styling and responsiveness
- Custom CSS from the original site is available at assets/css/tug-pt.css if additional customization is needed
- All icons are available as SVG (preferred) with PNG fallbacks
- The structure supports future expansion with blog posts, events calendar, etc.

---
**Migration Date**: May 2026
**Source**: TUG-PT/tug-pt-site/
**Target**: TUG-PT2/
