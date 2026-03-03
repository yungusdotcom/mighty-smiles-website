# DEVELOPMENT.md - Mighty Smiles Website

## Build History

### v1.0.0 - Initial Launch (March 3, 2026)

**Design decisions:**
- Single-file HTML with all assets inlined (base64 images, inline SVG, inline CSS)
- No build tools, no frameworks, no bundlers
- Fraunces serif for headings (warm, editorial character)
- DM Sans for body (clean, modern)
- Brand colors from official logo SVG

**Iterations:**
1. v0.1 - Initial build with Nunito + Baloo 2, emoji tooth character, placeholder photos
2. v0.2 - Replaced emojis with actual SVG brand logo (nav, hero, footer)
3. v0.3 - Added real doctor headshots and office interior photos
4. v0.4 - Full redesign: cleaner layout, brighter colors, circular doctor photos, office gallery
5. v1.0 - Font upgrade: Fraunces + DM Sans. Removed Smile Squad. Tightened typography.

## Asset Management

All images base64-encoded in index.html. Source files in assets/ for reference:

| Asset | File | Section |
|-------|------|---------|
| Dr. Campbell | assets/images/dr-amanda-campbell.webp | Doctors |
| Dr. Truong | assets/images/dr-vanna-truong.webp | Doctors |
| Lobby | assets/images/office-lobby.webp | About + Office |
| Waiting room | assets/images/office-waiting-room.webp | About + Office |
| Entrance | assets/images/office-entrance.webp | Office |
| Logo SVG | assets/logos/Mighty_Smile_Logo_full_color.svg | Nav, Hero |

## CSS Architecture

Single style block with CSS custom properties.

**Section classes:** .hero, .about, .services, .doctors, .office, .reviews, .insurance, .cta
**Card classes:** .svc, .doc, .rev, .ins-chip
**Shared:** .section, .section-header, .section-label, .section-title, .section-sub
**Utilities:** .reveal (scroll anim), .btn, .btn-sky, .btn-outline

**Breakpoints:** 900px (mobile nav, single column) | 600px (simplify grids)

## JavaScript

Two features only:
1. Nav shadow on scroll
2. IntersectionObserver scroll reveal on .reveal elements

No frameworks. No dependencies.

## Brand Colors

| Color | Hex | Usage |
|-------|-----|-------|
| Sky | #40bcd9 | Primary, CTAs, links |
| Navy | #3768af | Headings, text accents |
| Mint | #77c59a | Secondary, success |
| Gold | #fac35c | Highlights, stars |
| Coral | #f38b95 | Warm accents |
| Rose | #d26092 | Accent |
| Purple | #b7679d | Accent |

## Planned Future Work

- [ ] Custom domain setup
- [ ] Google Maps embed
- [ ] Online appointment request form
- [ ] SEO meta tags (Open Graph, Twitter Cards)
- [ ] Google Analytics
- [ ] Individual service pages
- [ ] Blog/news section
- [ ] Accessibility audit
- [ ] Favicon from brand logo
