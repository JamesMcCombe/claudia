# Claudia 2.0 Marketing Website - Project Package

**Created:** February 18, 2026  
**For:** Codex 5.3 Agent  
**Objective:** Build high-converting marketing site for LATAM women shopping assistant  

---

## 📦 WHAT'S IN THIS PACKAGE

### Core Documents (Read in Order)

#### 1. **CODEX_PROMPT_CLAUDIA_WEBSITE.md** ⭐ START HERE
- **Purpose:** Main instructions for Codex agent
- **Contents:** Mission, tech stack, build checklist, success criteria
- **Read Time:** 10 minutes
- **Use:** Give this to Codex to start building

#### 2. **CLAUDIA_PDR_FOR_CODEX.md** 📋 REFERENCE GUIDE
- **Purpose:** Complete product design record
- **Contents:** All 11 website sections, exact copy, technical specs, animations
- **Read Time:** 30 minutes
- **Use:** Detailed reference for every component and section

#### 3. **CLAUDIA_DESIGN_INSPIRATION.md** 🎨 BRAND GUIDELINES
- **Purpose:** Visual identity, brand personality, cultural considerations
- **Contents:** Color palette, typography, illustrations, tone of voice
- **Read Time:** 20 minutes
- **Use:** Design system reference and brand guard rails

#### 4. **CLAUDIA_WEBSITE_INSPIRATION_ANALYSIS.md** 💡 COMPETITIVE INSIGHTS
- **Purpose:** Deep-dive analysis of 10 winning websites
- **Contents:** What to steal, what to avoid, pattern analysis
- **Read Time:** 25 minutes
- **Use:** Design validation and inspiration when stuck

---

## 🎯 QUICK START FOR JAMES

### Option A: Immediate Build (Fastest)
```bash
# 1. Open your coding environment (Cursor, Windsurf, etc.)
# 2. Start a new Codex 5.3 session
# 3. Paste this prompt:

"Read the file CODEX_PROMPT_CLAUDIA_WEBSITE.md and build the Claudia marketing 
website according to the specifications. Reference CLAUDIA_PDR_FOR_CODEX.md for 
detailed content and CLAUDIA_DESIGN_INSPIRATION.md for brand guidelines. 
Build time: 4-6 hours. Prioritize mobile-first, WhatsApp CTA prominence, and 
Spanish language copy. Deploy to Vercel when complete."

# 4. Let Codex read all 4 documents and build
# 5. Review preview URL when ready
```

### Option B: Guided Build (More Control)
```bash
# 1. Review CLAUDIA_PDR_FOR_CODEX.md yourself (30 mins)
# 2. Make any changes to copy, colors, or structure
# 3. Give Codex the CODEX_PROMPT with your modifications
# 4. Review work-in-progress at each phase
# 5. Iterate on design decisions as Codex builds
```

---

## 📊 WHAT CODEX WILL BUILD

### Homepage Structure (11 Sections)

1. **Hero** - WhatsApp CTA + animated chat mockup
2. **Social Proof** - Marketplace logos + user stats
3. **How It Works** - 3-step visual guide
4. **Features Grid** - 6 core features with icons
5. **Demo Video** - 30-second product showcase
6. **Testimonials** - 3 real user quotes
7. **Pricing** - Free vs Premium comparison
8. **Referral CTA** - Invite friends, earn credits
9. **FAQ** - 8 questions, accordion style
10. **Final CTA** - Last conversion push
11. **Footer** - Links, legal, contact

### Technical Specs
- **Framework:** Next.js 14+ (TypeScript)
- **Styling:** Tailwind CSS (custom Claudia palette)
- **Animations:** Framer Motion
- **Components:** Shadcn/ui (customized)
- **Hosting:** Vercel
- **Analytics:** PostHog

### Performance Targets
- Lighthouse Score: 95+ (mobile)
- Load Time: <2 seconds (3G network)
- Above-fold CTA: 100% visible (mobile)

---

## 🎨 BRAND IDENTITY SUMMARY

### Colors
```css
Primary: #FF6B6B (Coral - warm, energetic, feminine)
Background: #FFF8F0 (Cream - soft, clean)
Text: #5B3A5F (Deep Plum - readable, sophisticated)
Accent: #F4A460 (Warm Gold - savings badges)
Success: #A8C69F (Sage Green - confirmation)
```

### Typography
```
Headings: Poppins (Bold/SemiBold) - Friendly, modern
Body: Inter (Regular) - Highly readable
Accent: Caveat (Handwritten) - Personal touches
```

### Tone & Voice
- **Informal "tú"** (not formal "usted")
- **Warm, conversational** (like talking to a friend)
- **Short, scannable** (women are time-poor)
- **Emojis sparingly** (🛍️💰✨)

---

## 🌍 CULTURAL CONSIDERATIONS

### LATAM-Specific Elements
- **Language:** Spanish (Mexico variant for launch)
- **Currency:** Pesos ($) with "MXN" clarification
- **Payments:** "Cuotas sin interés" (installments) emphasized
- **Support:** WhatsApp contact (expected, trusted)
- **Imagery:** Real LATAM women (diverse skin tones)

### What to Avoid
❌ US-centric examples (Thanksgiving, USD)  
❌ European minimalism (too cold)  
❌ Generic stock photos (use illustrations or LATAM models)  
❌ Technical jargon (AI, ML, API)  
❌ Long paragraphs (mobile users skim)  

---

## ✅ SUCCESS CRITERIA

### Technical
- [ ] Lighthouse 95+ (mobile)
- [ ] LCP <2s (largest contentful paint)
- [ ] CLS <0.1 (cumulative layout shift)
- [ ] Mobile-first responsive (375px → 1280px)
- [ ] All Spanish copy (no English)

### UX
- [ ] User understands "WhatsApp shopping assistant" in 5 seconds
- [ ] WhatsApp CTA above fold (mobile + desktop)
- [ ] Privacy messaging appears 3+ times
- [ ] "Gratis" (free) mentioned 5+ times

### Design
- [ ] Coral color palette consistent
- [ ] Poppins headings, Inter body
- [ ] Rounded corners (12-16px)
- [ ] Subtle animations (not distracting)
- [ ] Feels warm, approachable (not corporate)

---

## 🚀 NEXT STEPS AFTER BUILD

### 1. Review (You + Team)
- [ ] Test on iPhone (Safari) and Android (Chrome)
- [ ] Click WhatsApp CTA → verify it opens chat
- [ ] Read all Spanish copy → check for naturalness
- [ ] Check mobile layout → CTA above fold?
- [ ] Run Lighthouse → score 95+?

### 2. Iterate (Based on Feedback)
- Adjust colors if needed (stay in palette range)
- Refine copy for local dialect (Mexico vs Colombia vs Brazil)
- Add/remove sections (stick to 11-section structure if possible)
- Optimize images (compress for faster load)

### 3. Launch Prep
- [ ] Choose domain (claudia.app recommended)
- [ ] Set up WhatsApp Business API number
- [ ] Configure PostHog analytics
- [ ] Create og:image (1200x630px social share image)
- [ ] Write social media launch posts
- [ ] Prepare influencer outreach scripts

### 4. Go Live
- [ ] Deploy to production (Vercel)
- [ ] Point domain to Vercel
- [ ] Test end-to-end (landing page → WhatsApp)
- [ ] Launch in Mexico first (validate)
- [ ] Expand to Colombia, Brazil, Argentina, Chile

---

## 📝 PLACEHOLDER DATA (Replace When Ready)

Until you provide actual data, Codex will use:

- **WhatsApp Number:** `+52-555-123-4567`
- **Email:** `hola@claudia.app`
- **Domain:** `claudia.app`
- **User Count:** "10,000+ usuarias activas"
- **Testimonials:** María (CDMX), Laura (Medellín), Sofia (São Paulo)
- **Logo:** Text-based ("Claudia" in Poppins Bold)
- **Marketplace Logos:** Free SVG or text placeholders

**Provide These ASAP:**
1. Real WhatsApp Business number (for CTA links)
2. Actual domain name (for deployment)
3. Logo design (or confirm text-only is OK)
4. Real testimonials (or approve placeholders)
5. Demo video (or confirm placeholder rectangle)

---

## 💎 DESIGN DECISIONS CODEX CAN MAKE

Codex has **creative freedom** to decide:

✅ Exact shades of coral/plum (within palette range)  
✅ Illustration style (flat, semi-flat, geometric)  
✅ Animation timing (balance delight vs performance)  
✅ Micro-copy refinements (keep it conversational)  
✅ Layout tweaks (optimize for content flow)  
✅ Icon selection (Lucide React or custom SVGs)  

Codex should **ask approval** before:

⚠️ Changing core message (e.g., "shopping assistant" → something else)  
⚠️ Adding new sections (stick to 11-section structure)  
⚠️ Switching tech stack (Next.js is required)  
⚠️ Using paid assets (free resources only)  

---

## 🤝 WORKING WITH CODEX

### Give This Prompt to Codex
```
I need you to build the Claudia marketing website. 

Please read these 4 files in order:
1. CODEX_PROMPT_CLAUDIA_WEBSITE.md (main instructions)
2. CLAUDIA_PDR_FOR_CODEX.md (detailed specs)
3. CLAUDIA_DESIGN_INSPIRATION.md (brand guidelines)
4. CLAUDIA_WEBSITE_INSPIRATION_ANALYSIS.md (design inspiration)

Build a mobile-first, Spanish-language marketing site that converts LATAM 
women to add Claudia's WhatsApp number. Prioritize clarity, trust signals, 
and a prominent WhatsApp CTA.

Target build time: 4-6 hours
Deliverable: Deployed Vercel preview URL + Lighthouse report

Ask questions if anything is unclear. Otherwise, start building!
```

### What to Expect
- **Phase 1 (30 min):** Setup & structure
- **Phase 2 (2 hours):** Core sections (hero → features)
- **Phase 3 (1.5 hours):** Conversion elements (pricing, FAQ, testimonials)
- **Phase 4 (1 hour):** Polish & animations
- **Phase 5 (30 min):** SEO & deploy

### Review Points
- After hero section → Check WhatsApp CTA prominence
- After features grid → Verify mobile layout
- After full build → Run Lighthouse, test on real device

---

## 📊 ESTIMATED TIMELINE

### Codex Build: 4-6 hours
- **MVP (Priority 1):** 2 hours
  - Hero + How It Works + Features + FAQ
- **Conversion (Priority 2):** 2 hours
  - Social proof + Testimonials + Pricing + Final CTA
- **Polish (Priority 3):** 1-2 hours
  - Animations + Demo video + Referral CTA

### Your Review: 1-2 hours
- Mobile testing (iPhone, Android)
- Copy review (Spanish naturalness)
- CTA functionality (WhatsApp link works?)
- Lighthouse check (score 95+?)

### Iteration: 1-3 hours
- Color tweaks
- Copy refinements
- Layout adjustments
- Image optimization

**Total:** 6-11 hours from start to launch-ready

---

## 🎯 CRITICAL SUCCESS FACTORS

### Non-Negotiables
1. **Mobile-first** (70%+ users on phones)
2. **WhatsApp CTA above fold** (primary conversion)
3. **Privacy messaging** (appears 3+ times)
4. **LATAM cultural relevance** (not a translated US site)
5. **Fast load time** (<2s on 3G)

### Nice-to-Haves
- Demo video (can be placeholder initially)
- Testimonial carousel (can start with 3 static cards)
- Country selector (can add post-launch)
- Dark mode (optional, launch light-only)

---

## ❓ FAQ FOR JAMES

### Q: Can I change the color palette?
**A:** Yes, but stay in the warm spectrum (coral/terracotta). Avoid cold colors (blue, gray) or overly bright (hot pink, neon). Test on mobile before committing.

### Q: Do I need a demo video?
**A:** Not for MVP. Codex will create a placeholder (gray rectangle with text). You can film a real demo later and swap it in.

### Q: What if I don't have a WhatsApp Business number yet?
**A:** Use a placeholder (`+52-555-123-4567`). Update it before launch. Just do a find-and-replace.

### Q: Should I launch in multiple countries at once?
**A:** No. Start with Mexico (largest market, easiest Spanish). Validate conversion, then expand to Colombia, Brazil, etc.

### Q: How do I test on mobile if I'm building on desktop?
**A:** Chrome DevTools (Cmd+Opt+I) → Device toolbar (Cmd+Shift+M) → Select iPhone 12 Pro. Or use Vercel preview URL on your real phone.

### Q: What if I want to add a section (e.g., "Press Mentions")?
**A:** Ask Codex to add it, but keep the core 11 sections. Insert new section logically (e.g., after testimonials). Don't disrupt the conversion flow.

---

## 🚨 COMMON PITFALLS TO AVOID

❌ **Overdesigning** - Keep it simple, fast, clear  
❌ **Translation errors** - Write natively in Spanish, don't use Google Translate  
❌ **US assumptions** - Remember: LATAM ≠ USA (culture, currency, logistics)  
❌ **Desktop-first** - Mobile is 70%+ of users, design for 375px first  
❌ **Slow load times** - LATAM has slower networks, optimize images  
❌ **Hiding the CTA** - WhatsApp button must be above fold, always visible  
❌ **Ignoring trust signals** - Privacy concerns are HIGH, address explicitly  

✅ **Do this instead:**
- Ship MVP fast, iterate based on real user behavior
- Test on real phones (not just Chrome DevTools)
- Get native Spanish speakers to review copy
- Optimize for mobile networks (3G, not 5G)
- Make privacy/free messaging prominent

---

## 📞 SUPPORT

If Codex gets stuck or you need clarification:

1. **Check the reference docs** (PDR, Design Inspiration, Analysis)
2. **Review the inspiration sites** (Nubank, Glossier, Rare Beauty links in Analysis doc)
3. **Look at 21st.dev components** (https://21st.dev/community/components)
4. **Ask Walter** (me!) for design validation or copy review

---

## 🎉 READY TO BUILD!

You now have everything Codex needs to build a world-class marketing site for Claudia:

✅ Complete technical specifications  
✅ Exact content and copy  
✅ Brand guidelines and color palette  
✅ 10 website inspirations analyzed  
✅ Success criteria and performance targets  
✅ Cultural considerations for LATAM  

**Next Step:** Give Codex the prompt from the "Working with Codex" section above.

**Build Time:** 4-6 hours  
**Outcome:** Deployed Vercel site ready for user testing  
**Goal:** 40%+ WhatsApp CTA click-through rate  

---

## 📂 FILE MANIFEST

```
WORKSPACE ROOT
├── README_CLAUDIA_WEBSITE_PROJECT.md (this file)
├── CODEX_PROMPT_CLAUDIA_WEBSITE.md (start here for build)
├── CLAUDIA_PDR_FOR_CODEX.md (detailed reference)
├── CLAUDIA_DESIGN_INSPIRATION.md (brand guidelines)
└── CLAUDIA_WEBSITE_INSPIRATION_ANALYSIS.md (competitive analysis)
```

All files are in: `/Users/zeus/.openclaw-walter/workspace/`

---

**LET'S BUILD SOMETHING THAT MAKES LATAM WOMEN SAY:**  
**"¡Esto es exactamente lo que necesito!" 💎🛍️**

---

*Created by Walter, The Incubator Agent*  
*Research time: 6 hours | Documentation time: 2 hours*  
*Based on: 20+ Spanish sources, 10 competitive sites, LATAM market research*
