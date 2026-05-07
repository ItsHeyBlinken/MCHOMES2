# Tech Context

## Stack
- Pure HTML/CSS/JS — no build tooling, no framework
- **Entry point:** `index.html` — hub page linking to four full-page design options
- **Design option pages:** `index-dark.html`, `index-light.html`, `index-editorial.html`, `index-architectural.html`

## External Dependencies (CDN)
| Library | Version | Purpose |
|---------|---------|---------|
| Google Fonts | — | Cormorant Garamond + Montserrat |
| AOS | 2.3.1 | Scroll-triggered fade animations |

## Design System
| Token | Value |
|-------|-------|
| `--bg` | `#080807` |
| `--bg-2` | `#101010` |
| `--bg-3` | `#161412` |
| `--gold` | `#c8a96b` |
| `--gold-light` | `#e6d3a8` |
| `--gold-dim` | `#9a7c42` |
| `--white` | `#f4f1eb` |
| `--muted` | `#726a5a` |
| Serif | Cormorant Garamond |
| Sans | Montserrat |

## Key Techniques
- Testimonials infinite scroll: CSS `@keyframes tickerRoll` with `translateX(-50%)`, cards duplicated in HTML for seamless loop
- Gallery lightbox: vanilla JS click handler with CSS overlay
- Nav scroll: `IntersectionObserver`-style scroll listener toggling `.solid` class
- Mobile nav: hamburger button + full-screen drawer overlay
- Video backgrounds: `autoplay muted loop playsinline` on both hero and testimonials

## Deployment
- **Target:** VPS with **Coolify**, deployed from a **standalone GitHub repository** (not mixed with other client work).
- **Type:** Fully static — no build command required. Serve the **repository root** as the web root so `index.html` is the default document and relative paths (`__originals/...`, sibling `.html` files) resolve.
- **Assets:** The `__originals/` directory (images, video, logo) must be in the repo at the same level as the HTML files; if files are large, consider **Git LFS** for the MP4 and high-res JPGs.
- **Coolify:** Use a **static site** resource if offered, or a minimal **nginx** (or Caddy) image that copies the repo into the default public directory — no Node/buildpack needed.
