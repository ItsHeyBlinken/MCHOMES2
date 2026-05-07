# Active Context

## Session: 2026-05-06

### Completed
- Created `index-dark.html` — dark version (near-black + gold #c8a96b); **filename was `index.html` until hub became default `index.html` for hosting**
- Created `index-light.html` — light version (warm ivory #f8f4ee + gold + dark charcoal text)
  - Google Fonts: Cormorant Garamond (headings) + Montserrat (body/UI)
  - Hero: full-screen video background (`__originals/480p/mp4/file.mp4`)
  - Stats band: 100+ projects, 15+ years Best Builder, D Magazine, CGB
  - About section: portrait photo + credentials
  - Services: 3-tile grid (New Construction / Renovation / Commercial)
  - Gallery: 12-image CSS Grid mosaic with lightbox
  - Testimonials: infinite CSS scroll ticker (translateX(-50%) loop) with video BG
  - Communities served strip
  - Contact: split layout with form + contact details
  - Footer: brand, nav, services, contact columns
  - AOS scroll animations throughout
  - Mobile responsive with hamburger drawer

### Assets Used
- All 12 JPG home photos from `__originals/`
- `__originals/480p/mp4/file.mp4` — hero and testimonials video BG
- `5e6802_7a8624b937a1423e994a9b5bce92623a~mv2_d_4537_5671_s_4_2.jpg` — about section hero photo
- `5e6802_53eb3d45e9ff4f179b5e9d3f834a6519~mv2.png` — available (35KB PNG, not currently placed; may be logo)

### Libraries (CDN)
- AOS 2.3.1 — scroll animations
- Google Fonts — Cormorant Garamond, Montserrat

## Session: 2026-05-07

### Completed
- `index-editorial.html` — client option C: editorial / magazine rhythm (see plan). Testimonials as static grid (same 10 quotes). Stats embedded in hero copy column.
- `index-architectural.html` — client option D: structural / architectural rhythm. Testimonials as vertical stack. Stats in hero plinth beside headline.
- **Hosting filenames:** dark classic is `index-dark.html`; hub (design options menu) is `index.html` (replaced prior `variants.html`). Hub links to `index-dark.html` for Option A.
- **Hub redesign:** `index.html` restyled as agency client presentation—dark hero (Fraunces + Outfit), top bar, lettered option cards, `<details>` for technical hosting note, professional footer.

### Next Steps / Open Questions
- **Hosting:** GitHub repo → Coolify on VPS; static root deploy; include `__originals/` (see `techContext.md` → Deployment)
- Verify `5e6802_53eb3d45` PNG content — if it's the MCH logo, add to nav/footer
- Decide if a contact form backend (Formspree, Netlify Forms, etc.) is needed
- Confirm fax number on footer
- Client review and feedback
