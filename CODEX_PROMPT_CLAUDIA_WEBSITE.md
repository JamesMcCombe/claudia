# Codex 5.3 Prompt: Build Claudia Marketing Website

## 🎯 MISSION

Build a high-converting, mobile-first marketing website for **Claudia** - a WhatsApp-native AI shopping assistant for women in Latin America.

**Primary Goal:** Drive WhatsApp CTA clicks  
**Target Audience:** Women 18-45 in Mexico (expanding to LATAM)  
**Success Metric:** User understands value in 5 seconds, clicks WhatsApp CTA in <30 seconds  

---

## 📚 CONTEXT DOCUMENTS (READ FIRST)

You have two comprehensive reference documents in the workspace:

1. **`CLAUDIA_DESIGN_INSPIRATION.md`**
   - Brand personality & voice
   - Color palette & typography
   - Visual style & cultural considerations
   - Competitive website inspirations
   - Component style guidelines

2. **`CLAUDIA_PDR_FOR_CODEX.md`**
   - Full website structure (11 sections)
   - Exact content & copy for each section
   - Technical specifications
   - Animation guidelines
   - Success criteria

**Read both documents thoroughly before starting.** They contain all the details you need.

---

## 🛠️ TECHNICAL STACK

```bash
# Initialize Next.js project
npx create-next-app@latest claudia-marketing-site \
  --typescript \
  --tailwind \
  --app \
  --no-src-dir \
  --import-alias "@/*"

# Install dependencies
cd claudia-marketing-site
npm install framer-motion
npm install @radix-ui/react-accordion @radix-ui/react-dialog
npm install lucide-react
npm install posthog-js
```

### Tailwind Config (Custom Colors)
```javascript
// tailwind.config.ts
module.exports = {
  theme: {
    extend: {
      colors: {
        coral: {
          DEFAULT: '#FF6B6B',
          dark: '#E85D75',
        },
        cream: '#FFF8F0',
        gold: '#F4A460',
        plum: '#5B3A5F',
        sage: '#A8C69F',
      },
      fontFamily: {
        heading: ['Poppins', 'sans-serif'],
        body: ['Inter', 'sans-serif'],
        accent: ['Caveat', 'cursive'],
      },
    },
  },
}
```

---

## 📋 BUILD CHECKLIST (In Order)

### Phase 1: Setup & Structure (30 mins)
- [ ] Initialize Next.js 14+ with TypeScript & Tailwind
- [ ] Configure custom colors, fonts, spacing in tailwind.config
- [ ] Add Google Fonts (Poppins, Inter, Caveat) to app/layout.tsx
- [ ] Create component structure:
  ```
  /app
    /page.tsx (homepage - all sections here)
    /layout.tsx (root layout, fonts, meta)
  /components
    /Hero.tsx
    /SocialProofBar.tsx
    /HowItWorks.tsx
    /FeaturesGrid.tsx
    /DemoVideo.tsx
    /Testimonials.tsx
    /Pricing.tsx
    /ReferralCTA.tsx
    /FAQ.tsx
    /FinalCTA.tsx
    /Footer.tsx
  /public
    /images (placeholders for now)
  ```

### Phase 2: Core Sections (2 hours)
- [ ] **Hero Section** (most important!)
  - Two-column layout (text left, mockup right)
  - H1: "Tu amiga de compras en WhatsApp 🛍️"
  - Primary CTA: Coral button → WhatsApp link
  - Animated WhatsApp chat mockup (looping conversation)
  - Trust signals row below CTAs
  
- [ ] **Social Proof Bar**
  - Marketplace logos (grayscale, 40px height)
  - Stats: "10,000+ usuarias activas"
  
- [ ] **How It Works** (3 steps)
  - Icon + Title + Description cards
  - Mobile: stacked, Desktop: 3-column grid
  
- [ ] **Features Grid** (6 features)
  - Icon + Title + 2-line description
  - 3x2 grid (desktop), 1-column (mobile)

### Phase 3: Conversion Elements (1.5 hours)
- [ ] **Demo Video Section**
  - 16:9 video player (placeholder for now)
  - Centered, max-width 900px
  
- [ ] **Testimonials Carousel**
  - 3 testimonial cards (photo, name, location, quote, stars)
  - Horizontal scroll (mobile), 3-column (desktop)
  
- [ ] **Pricing Table**
  - Two-column comparison (Free vs Premium)
  - Checkmark features list
  - CTA buttons for each
  
- [ ] **Referral CTA**
  - Full-width gradient background (coral to gold)
  - Large title + CTA
  
- [ ] **FAQ Accordion**
  - 8 questions (see PDR for content)
  - Click to expand/collapse
  - Use Radix Accordion

### Phase 4: Polish & Animations (1 hour)
- [ ] **Framer Motion Animations**
  - Hero: Staggered fade-ins (H1 → Subhead → CTAs)
  - Features: Fade up on scroll (once per viewport)
  - WhatsApp mockup: Messages type in, loop
  
- [ ] **Hover States**
  - Buttons: lift 2px, darken 10%
  - Cards: lift 8px, shadow intensifies
  
- [ ] **Responsive Testing**
  - Test on 375px (iPhone), 768px (iPad), 1280px (desktop)
  - Ensure WhatsApp CTA above fold on all sizes

### Phase 5: SEO & Deploy (30 mins)
- [ ] **Meta Tags** (app/layout.tsx)
  ```tsx
  export const metadata = {
    title: 'Claudia - Tu Asistente de Compras en WhatsApp | Ahorra Tiempo y Dinero',
    description: 'Compara precios en Mercado Libre, Amazon, Shein y más. Gratis, fácil, directo en WhatsApp.',
    openGraph: {
      images: ['/og-image.png'],
    },
  }
  ```
  
- [ ] **PostHog Analytics**
  ```tsx
  // Track CTA clicks
  onClick={() => {
    posthog.capture('whatsapp_cta_click', { location: 'hero' })
    window.open('https://wa.me/52XXXXXXXXXX', '_blank')
  }}
  ```
  
- [ ] **Deploy to Vercel**
  ```bash
  git init
  git add .
  git commit -m "Initial Claudia marketing site"
  vercel deploy
  ```

---

## 🎨 DESIGN GUIDELINES (Quick Reference)

### Colors
```css
Primary: #FF6B6B (coral)
Background: #FFF8F0 (cream)
Text: #5B3A5F (plum)
Accent: #F4A460 (gold)
Success: #A8C69F (sage)
```

### Typography
```
Headings: Poppins (Bold/SemiBold)
Body: Inter (Regular)
Sizes: H1=40px, H2=32px, Body=18px
```

### Spacing
```
Mobile-first: 16px base padding
Sections: 64px vertical spacing
Cards: 16px border-radius
Buttons: 12px border-radius
```

---

## 💬 COPY GUIDELINES (Spanish, Mexico)

### Tone
- **Informal "tú" form** (not "usted")
- **Conversational, warm, friendly**
- **Short sentences** (busy women skim)
- **Emojis sparingly** (🛍️💰✨)

### Key Phrases to Use
- "Gratis" (free) - mentioned multiple times
- "Sin descargar apps" (no app download)
- "Ahorra tiempo y dinero" (save time and money)
- "Directo en WhatsApp" (directly in WhatsApp)
- "Sin compartir datos" (no data sharing)

### Key Phrases to AVOID
- "Descargar app" (download app)
- "Crear cuenta" (create account)
- "Dar tu email" (give email)
- Technical jargon (API, AI, ML)

---

## ⚡ QUICK WINS (If Short on Time)

**Priority 1 (Must-Have):**
- Hero with WhatsApp CTA above fold
- How It Works (3 steps)
- Features Grid (6 items)
- FAQ (8 questions)
- Footer

**Priority 2 (Should-Have):**
- Social proof bar
- Testimonials
- Pricing table
- Final CTA

**Priority 3 (Nice-to-Have):**
- Demo video
- Referral CTA
- Animations

---

## 📱 MOBILE-FIRST APPROACH

### Critical Mobile Checks
1. **WhatsApp CTA above fold** (375px viewport)
2. **Tap targets ≥48px** (buttons, accordions)
3. **Font size ≥16px** (body text - prevents zoom on iOS)
4. **Fast scroll** (no janky animations)
5. **Load time <2s** (test on simulated 3G)

### Mobile Layouts
- **Hero:** Stack text above mockup
- **How It Works:** Vertical stack (1 column)
- **Features:** Vertical stack (1 column)
- **Testimonials:** Horizontal scroll carousel
- **Pricing:** Stack columns (Free on top)

---

## 🚨 GOTCHAS TO AVOID

❌ **Don't** use generic stock photos (use illustrations or LATAM models)  
❌ **Don't** make copy too long (women are time-poor)  
❌ **Don't** hide the WhatsApp CTA (it's the whole funnel)  
❌ **Don't** translate from English (write natively in Spanish)  
❌ **Don't** use cold colors (blues, grays) - keep it warm  

✅ **Do** prioritize mobile (70%+ users)  
✅ **Do** mention "gratis" early and often  
✅ **Do** add trust signals (privacy, security)  
✅ **Do** use natural Spanish (not Google Translate)  
✅ **Do** test on real devices (iPhone, Android)  

---

## 🎯 SUCCESS CRITERIA

### Technical
- [ ] Lighthouse score 95+ (mobile)
- [ ] LCP (Largest Contentful Paint) <2s
- [ ] CLS (Cumulative Layout Shift) <0.1
- [ ] No console errors
- [ ] Works on Chrome, Safari, Firefox (mobile + desktop)

### UX
- [ ] User understands "WhatsApp shopping assistant" in 5 seconds
- [ ] WhatsApp CTA visible without scrolling (mobile)
- [ ] All copy in Spanish (no English)
- [ ] Privacy messaging appears 3+ times
- [ ] Site feels warm, approachable (not corporate)

### Design
- [ ] Coral color palette consistent
- [ ] Poppins headings, Inter body
- [ ] Rounded corners (12-16px)
- [ ] Subtle shadows (no harsh borders)
- [ ] Mobile-first responsive

---

## 🤖 YOUR CREATIVE FREEDOM

### You Decide
- **Exact shades** of coral/plum (within palette range)
- **Illustration style** (flat, semi-flat, geometric)
- **Animation timing** (balance delight vs performance)
- **Micro-copy** (write conversationally in Spanish)
- **Layout tweaks** (optimize for content flow)
- **Icon selection** (use Lucide React or custom SVGs)

### Get Approval Before
- Changing core message (e.g., "shopping assistant" → something else)
- Adding new sections (stick to 11-section structure)
- Switching tech stack (Next.js required)
- Using paid assets (use free resources only)

---

## 📦 DELIVERABLES

When complete, provide:

1. **Vercel Preview URL** (deployed site)
2. **GitHub Repo Link** (if pushed to Git)
3. **Lighthouse Report** (screenshot or link)
4. **Mobile Screenshot** (375px viewport)
5. **Desktop Screenshot** (1280px viewport)
6. **Summary:**
   - What you built
   - Design decisions you made
   - Any deviations from PDR (with reasoning)
   - Recommended next steps

---

## 🚀 READY TO BUILD?

### Your Mission (TL;DR)
Build a mobile-first, Spanish-language marketing site that makes LATAM women say:  
**"¡Esto es exactamente lo que necesito!"** (This is exactly what I need!)

### Key Principles
1. **Clarity over creativity** - User gets value prop in 5 seconds
2. **Mobile-first** - 70%+ users are on phones
3. **Trust-first** - Privacy concerns are high
4. **LATAM-native** - Not a translated US site
5. **Fast** - Every second of load time costs conversions

### What Success Looks Like
✅ User lands → Sees "WhatsApp shopping assistant" → Clicks "Empezar Gratis" → Opens WhatsApp → Done in <30s

---

**NOW GO BUILD IT! 🛠️**

Reference `CLAUDIA_PDR_FOR_CODEX.md` for detailed section content.  
Reference `CLAUDIA_DESIGN_INSPIRATION.md` for brand guidelines.  

**Questions? Ask before starting. Otherwise, ship fast and iterate.** 🚀

---

## 📞 PLACEHOLDER DATA

Until James provides actual data, use:

- **WhatsApp Number:** `+52-555-123-4567` (placeholder)
- **Email:** `hola@claudia.app`
- **Domain:** `claudia.app`
- **Launch Country:** Mexico
- **Testimonial Names:** María (CDMX), Laura (Medellín), Sofia (São Paulo)
- **Logo:** Text-based for now ("Claudia" in Poppins Bold, coral color)
- **Marketplace Logos:** Find free SVGs or use text placeholders
- **Demo Video:** Gray rectangle placeholder (16:9, "Video Demo - 30 segundos")

Replace all placeholders once James provides real assets.

---

**Estimated Build Time:** 4-6 hours for full MVP  
**Priority:** Hero + How It Works + Features + FAQ = Core MVP (2 hours)  
**Stretch:** Testimonials + Pricing + Animations = Polish (2 hours)

**LET'S SHIP IT! 💎🛍️**
