# CLAUDIA - Updated Codex Build Prompt

**Includes:** English content + Language toggle implementation

---

## 🎯 Prompt for Codex 5.3

Copy this **complete prompt** into Codex:

```
You are building CLAUDIA - an AI receptionist SaaS website for Latin American businesses.

CONTEXT:
This repository contains complete documentation including Spanish content, English translations, and language toggle implementation.

YOUR TASK:
1. Read these files IN ORDER:
   - START_HERE.md (navigation & overview)
   - README_CLAUDIA_WEBSITE_PROJECT.md (project overview)
   - CLAUDIA_PDR_FOR_CODEX.md (complete requirements)
   - ENGLISH_CONTENT.md (English translations)
   - LANGUAGE_TOGGLE_IMPLEMENTATION.md (bilingual setup)
   - CLAUDIA_DESIGN_INSPIRATION.md (design references)

2. Build a bilingual landing page with:
   - Spanish as default language
   - English toggle in top-right corner
   - i18n implementation (Next.js)
   - Dark theme (midnight blue + cyan)
   - Mobile-first responsive design

3. Key Components to Build:
   - Hero section with headline + CTA
   - Demo video section
   - Features grid (4-6 features)
   - Pricing table (3 tiers)
   - Testimonials (social proof)
   - FAQ section
   - Footer with links
   - Language toggle component

4. Technical Stack:
   - Next.js 14 (App Router)
   - next-i18next for translations
   - Tailwind CSS
   - TypeScript
   - Dark mode only

5. Content Structure:
   /locales
     /es  → Spanish content (default)
     /en  → English content (from ENGLISH_CONTENT.md)

6. Language Toggle:
   - Desktop: ES | EN buttons (top-right)
   - Mobile: Dropdown selector
   - Saves preference to localStorage
   - Auto-detects browser language

IMPORTANT FEATURES:
✅ Spanish-first (default language)
✅ English toggle functional
✅ "Empezar Gratis" CTA (Spanish)
✅ "Start Free Trial" CTA (English)
✅ WhatsApp integration mention
✅ Mobile-responsive
✅ Fast loading (<2s)
✅ Dark theme

DESIGN SPECS:
- Colors: Midnight Blue (#0B1220), Electric Cyan (#00E5FF)
- Font: Inter (clean, modern)
- Spacing: Generous whitespace
- Images: Use placeholder images initially
- Icons: Use Heroicons or similar

BUILD STEPS:
1. Set up Next.js project with i18n
2. Create language toggle component
3. Add Spanish content to /locales/es/
4. Add English content to /locales/en/
5. Build all landing page sections
6. Style with Tailwind (dark theme)
7. Test language switching
8. Optimize for mobile
9. Deploy to Vercel

TESTING:
- Toggle switches language correctly
- All text translates (no missing keys)
- Mobile displays dropdown
- Desktop shows ES | EN buttons
- Page loads fast on mobile
- Dark theme looks good

Create a BUILD_LOG.md documenting:
- Setup steps
- Translation structure
- Component architecture
- How to add new content
- Deployment instructions

Start by confirming you've read the documentation, then begin building.
```

---

## 📊 What Codex Will Build

**Directory Structure:**
```
claudia/
├── app/
│   ├── [locale]/
│   │   ├── layout.tsx
│   │   └── page.tsx
│   └── layout.tsx
├── components/
│   ├── LanguageToggle.tsx
│   ├── Hero.tsx
│   ├── Features.tsx
│   ├── Pricing.tsx
│   ├── Testimonials.tsx
│   └── FAQ.tsx
├── locales/
│   ├── es/
│   │   ├── common.json
│   │   ├── hero.json
│   │   ├── features.json
│   │   └── pricing.json
│   └── en/
│       ├── common.json
│       ├── hero.json
│       ├── features.json
│       └── pricing.json
├── public/
│   └── images/
├── styles/
│   └── globals.css
├── next.config.js (with i18n)
├── tailwind.config.js
└── package.json
```

---

## ✅ Success Criteria

**After build, verify:**
- [ ] Default language is Spanish
- [ ] Language toggle appears in top-right
- [ ] Clicking toggle switches all content
- [ ] Mobile shows dropdown selector
- [ ] All CTAs translate correctly
- [ ] Forms handle both languages
- [ ] URLs show `/es/` and `/en/`
- [ ] Dark theme looks polished
- [ ] Mobile-responsive (375px+)
- [ ] Page loads <2s on 3G

---

## 🚀 Deploy Instructions

**After Codex completes:**

```bash
# Install dependencies
npm install

# Test locally
npm run dev
# Open http://localhost:3000

# Test language toggle
# Click ES/EN in header
# Verify all content switches

# Deploy to Vercel
vercel --prod
```

---

## 📝 Adding New Content

To add new translated content:

1. Add to Spanish: `/locales/es/[section].json`
2. Add to English: `/locales/en/[section].json`
3. Use in component: `const { t } = useTranslation('[section]')`
4. Reference: `t('key')`

Example:
```json
// /locales/es/hero.json
{
  "headline": "Nunca Pierdas una Llamada"
}

// /locales/en/hero.json
{
  "headline": "Never Miss a Call Again"
}
```

```tsx
// Component
const { t } = useTranslation('hero')
<h1>{t('headline')}</h1>
```

---

**Ready to build!** 🚀

Paste the prompt above into Codex 5.3 and start the build.
