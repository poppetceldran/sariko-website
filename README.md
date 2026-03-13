# SariKo Website

**SariKo** — Node 1 of Pangea. The Filipino diaspora marketplace for Ho Chi Minh City.

> "Ang iyong tindahan, para sa ating lahat" — Your store, for all of us

## Project Overview

This is a **Next.js 15** website built to showcase SariKo:
- Modern, responsive design optimized for mobile
- Built with React 19 and TypeScript
- Tailored for diaspora community storytelling
- Designed for quick deployment to Vercel

## Color Palette (SariKo Brand)

```
Primary Dark:   #0B1F45 (Deep Navy)
Accent Gold:    #F0A500 (Warm Gold)
Gold Light:     #FFD166 (Hover states)
Text Primary:   #FDFAF4 (Cream)
Secondary:      #7A6E58 (Muted warm tones)
```

## Project Structure

```
sariko-website/
├── app/
│   ├── layout.tsx          # Root layout with metadata
│   ├── page.tsx            # Homepage
│   └── globals.css         # Global styles
├── next.config.js
├── tsconfig.json
├── package.json
└── README.md
```

## Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

```bash
cd sariko-website
npm install
```

### Development

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Production Build

```bash
npm run build
npm start
```

## Deployment (Vercel)

**Recommended hosting:** Vercel (git-native deployment, instant edge caching)

1. Push repo to GitHub
2. Connect to Vercel
3. Deploy (automatic on every push to `main`)

**Cost:** Free tier covers startup traffic. Pro features (~$20/mo) for analytics.

## Pages & Sections

### Homepage (`/`)
- **Hero**: "Discover Filipino sellers near you"
- **Problem**: Invisible sellers, manual payments, chaotic orders
- **Solution**: Verified storefront, local payments, seller dashboard
- **Founding Story**: Teresa Cantuba (Founding Seller #1)
- **Traction**: 1 live seller, 300+ ready buyers, $0 MVP cost, 10 nodes designed
- **Team**: Poppet (CEO, 30+ years diaspora experience) + CMO partnership
- **The Ask**: $500K pre-seed at 8% equity
- **Early Access**: Email signup for launch notification
- **Footer**: Brand info, links, contact

## Customization

### Add New Sections
Edit `app/page.tsx` to add sections. Each section follows:
```tsx
<section style={{ /* section styles */ }}>
  <div className="container">
    {/* content */}
  </div>
</section>
```

### Change Colors
Update CSS variables in `globals.css`:
```css
:root {
  --color-navy-dark: #0B1F45;
  --color-gold: #F0A500;
  /* ... */
}
```

### Modify Content
All content is hardcoded in `page.tsx`. Update strings directly for quick changes.

## Key Features

✅ Mobile-first responsive design  
✅ Dark theme with gold accents (matches app mockups)  
✅ Fast loading (optimized for 4G)  
✅ Accessible typography and contrast  
✅ SEO-ready with metadata  
✅ No external dependencies (minimal bloat)  
✅ Ready for Vercel deployment  

## Next Steps (Phase 2 & 3)

- [ ] Add dedicated pages: `/founders`, `/investors`, `/sellers`
- [ ] Integrate Supabase for email signups
- [ ] Add blog/updates section
- [ ] Embed pitch deck and investor materials
- [ ] Social proof: testimonials from Teresa & early users
- [ ] Gallery: app screenshots from mockups
- [ ] Analytics: Vercel Analytics (free tier)

## Links

- **Live App**: sariko.app
- **Pitch Deck**: (embed or link)
- **Investor Inquiries**: poppet@sariko.app
- **GitHub**: (add when ready)

## License

Confidential. © 2026 SariKo App Co., Ltd.

---

**Built with ❤️ for the Filipino diaspora.**
