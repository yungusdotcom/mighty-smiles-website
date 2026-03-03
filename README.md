# Mighty Smiles Dentistry - Website

Patient-facing website for **Mighty Smiles Dentistry**, a pediatric dental practice in North Las Vegas, NV.

**Live:** [Vercel URL TBD]
**Repo:** https://github.com/yungusdotcom/mighty-smiles-website

---

## Quick Start

```
git clone https://github.com/yungusdotcom/mighty-smiles-website.git
cd mighty-smiles-website
npx serve public
```

Auto-deploys on push to main via Vercel.

## Project Structure

```
mighty-smiles-website/
  public/                    -> Deployed to Vercel
    index.html               -> Full single-page site (self-contained)
  assets/                    -> Source files (NOT deployed, local reference only)
    images/
      dr-amanda-campbell.webp
      dr-vanna-truong.webp
      office-lobby.webp
      office-waiting-room.webp
      office-entrance.webp
    logos/
      Mighty_Smile_Logo_full_color.svg
  docs/
    DEVELOPMENT.md           -> Architecture and dev notes
  vercel.json
  package.json
  .gitignore
  README.md
```

## Architecture

**Single-file static site.** Everything in `public/index.html`:

- All CSS inline (no external stylesheets)
- All images base64-encoded inline (zero external image requests)
- SVG logo inlined directly in markup
- Google Fonts via CDN (Fraunces + DM Sans)
- Zero JS dependencies - vanilla IntersectionObserver for scroll animations

**Why single-file?** Fastest possible load. No build step. No asset pipeline. No broken image links.

## Deployment (Vercel)

| Setting          | Value    |
|------------------|----------|
| Framework        | Other    |
| Output Directory | public   |
| Build Command    | (empty)  |

## Brand Colors

| Color   | Hex       | Usage                    |
|---------|-----------|--------------------------|
| Sky     | #40bcd9   | Primary / CTAs / links   |
| Navy    | #3768af   | Headings / text accents  |
| Mint    | #77c59a   | Success / secondary      |
| Gold    | #fac35c   | Highlights / stars       |
| Coral   | #f38b95   | Warm accents             |
| Rose    | #d26092   | Accent                   |
| Purple  | #b7679d   | Accent                   |

**Fonts:** Fraunces (headings) + DM Sans (body)

## Contact Info (hardcoded)

- **Phone:** (702) 850-8148
- **Address:** 4210 W Craig Rd, Suite #104, North Las Vegas, NV 89032
- **Hours:** Mon, Wed-Fri 8AM-5PM | Tue 9AM-4PM
- **Doctors:** Dr. Amanda Campbell, Dr. Vanna Truong

## Site Sections

1. Hero - Headline, phone CTA, brand logo animation
2. About - Office photos, key differentiators
3. Services - Laser, Preventive, Restorative, Special Needs, Sedation, Hospital
4. Doctors - Circular headshots, bios
5. Office - Photo gallery
6. Reviews - 3 parent testimonials
7. Insurance - Medicaid highlighted + major carriers
8. CTA - Phone, appointment, address, hours
9. Footer

## Updating Content

**Change text:** Edit directly in public/index.html.

**Replace a photo:** Convert new image to base64 and swap the data:image/webp;base64,... string. Source images in assets/images/ for reference.
