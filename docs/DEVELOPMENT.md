# DEVELOPMENT.md

## v1.0 - Initial Launch (Mar 3 2026)
- Single-file HTML, base64 images, inline SVG/CSS
- Iterated through Nunito/Baloo2 > Fraunces/DM Sans > Playfair Display/Outfit
- Added real doctor headshots, office photos, brand SVG logo

## v1.1 - Polish Pass (Mar 3 2026)
- Removed ALL emojis. Service accents = thin colored bars. About = small dots.
- Fonts: Playfair Display (serif headings) + Outfit (geometric sans body)
- Doctor titles: General Dentist (not Pediatric)
- Copy rewritten from mightysmileslv.com real content
- Reviews use actual parent names from Google
- Subtler shadows, more whitespace, navy-forward palette
- Philosophy: polished not plastic, kid-focused without saying pediatric

## Assets
- Dr Campbell: assets/images/Amanda-cropped-scaled-1-768x1024-1.webp
- Dr Truong: assets/images/Vanna-Truong-scaled-1-768x1024-1.webp
- Lobby: assets/images/2022-06-24.webp
- Waiting room: assets/images/2022-07-20.webp
- Entrance: assets/images/2024-05-06.webp
- Logo SVG: assets/logos/logo.svg

## CSS: vars for colors, .sec/.svc/.doc/.rev classes, 900px/600px breakpoints
## JS: nav scroll shadow + IntersectionObserver reveal only

## Roadmap
- Custom domain
- Google Maps embed
- Appointment form
- SEO meta (OG, Twitter)
- Analytics
- Service subpages
- Blog
- Accessibility audit
- Favicon
- Social links


## v1.2 - Color + Kid-Friendly Pass (Mar 3 2026)
Based on wife feedback + 3 reference sites (Castle Rock Kids, Elevated Pediatric, Sunrise Pediatric):
- REMOVED Medicaid from hero stats AND insurance section (too many Medicaid patients already)
- Hero stat changed to just Most Insurance / Plans accepted
- Hero bg: multi-color gradient (sky-bg > mint-bg > gold-bg > coral-bg) with radial color orbs
- Services bg: mint-to-sky gradient instead of flat gray
- Office bg: gold-to-coral gradient
- CTA bg: sky-mint-gold gradient
- Service icons: colored gradient squares (48px) with white SVG icons instead of thin bars
- Each service icon has unique brand color gradient
- Section labels use different brand colors (sky, mint, coral, gold, navy)
- Overall warmer, more colorful, less sterile/corporate
- Hero headline: A special place for kids to smile (inspired by Castle Rock Kids reference)
- Insurance section: removed Medicaid chip, kept MetLife, Delta, Concordia, Cigna, Aetna, + many more


## v2.0 - Fun & Colorful Redesign (Mar 3 2026)
Complete art direction shift based on wife feedback + competitor analysis.
References: Castle Rock Kids, Elevated Pediatric, Sunrise Pediatric, Coconut Smiles, El Segundo Pediatric.

**Art direction:**
- Fonts: Baloo 2 (rounded display, playful headings) + Nunito (warm, friendly body)
- Colored section backgrounds instead of white: sky-bg, mint-bg, gold-bg
- SVG wave dividers between every section (organic, not boxy)
- Floating blob shapes in hero background (mint, gold, coral, sky circles)
- All border-radius bumped to 24-32px (rounded, soft, kid-friendly)
- Pill-shaped buttons and tags (border-radius: 50px)
- Doctor cards have colored background (sky-bg) with white photo borders
- Service icons: large 56px rounded squares with soft color backgrounds and SVG line icons
- About section features in bordered cards with hover slide effect
- Gold highlight underline on hero keyword
- Bouncy logo animation in hero
- Green pulse animation on hero status dot

**Removed:** Medicaid (hero + insurance), Playfair Display, sterile whitespace
**Added:** Wave dividers, blob shapes, colored backgrounds, rounded everything, fun energy
