# Claudia Sites Comparison

## Overview
Both sites were built by **GPT-5.3-Codex** model, but through different tools:

### Port 3000: `/Users/zeus/Desktop/dev/claudia/claudia-site`
- **Tool**: Codex via Browser Extension (?)
- **Next.js**: 16.1.6 (latest)
- **React**: 19.2.3 (latest)
- **Tailwind**: 4.0 (latest)
- **Built**: Feb 18, 11:42 PM

### Port 3001: `/Users/zeus/Desktop/dev/claudia-codex/claudia-site`
- **Tool**: Codex CLI
- **Next.js**: 14.2.35
- **React**: 18.2.0
- **Tailwind**: 3.4.17
- **Built**: Feb 18, 11:39 PM

## Tech Stack Comparison

| Feature | Port 3000 | Port 3001 |
|---------|-----------|-----------|
| Next.js | 16.1.6 | 14.2.35 |
| React | 19 | 18 |
| Tailwind | 4 | 3 |
| Framer Motion | 12.34.1 | 11.18.2 |
| PostHog | 1.350.0 | 1.221.0 |
| Radix UI | ✅ | ✅ |
| Lucide Icons | ✅ | ✅ |

## Component Structure

### Port 3000 (Newer Stack)
```
components/
├── demo-video.tsx
├── faq.tsx
├── features-grid.tsx
├── final-cta.tsx
├── footer.tsx
├── header.tsx
├── hero.tsx
├── how-it-works.tsx
├── posthog-provider.tsx
├── pricing.tsx
├── referral-cta.tsx
├── reveal.tsx
├── section-heading.tsx
├── social-proof-bar.tsx
├── sticky-cta.tsx
├── testimonials.tsx
├── whatsapp-button.tsx
└── whatsapp-mockup.tsx
```

### Port 3001 (Codex CLI)
```
components/
├── analytics/
├── sections/
│   ├── DemoVideo.tsx
│   ├── FAQ.tsx
│   ├── FeaturesGrid.tsx
│   ├── FinalCTA.tsx
│   ├── FloatingWhatsAppCTA.tsx
│   ├── Footer.tsx
│   ├── Hero.tsx
│   ├── HowItWorks.tsx
│   ├── Pricing.tsx
│   ├── ReferralCTA.tsx
│   ├── SocialProofBar.tsx
│   ├── Testimonials.tsx
│   └── TopNav.tsx
└── ui/
```

## Key Differences

### 1. Organization
- **Port 3000**: Flat component structure
- **Port 3001**: Organized into sections/ and ui/ folders

### 2. Dependencies
- **Port 3000**: Latest bleeding-edge (Next 16, React 19, Tailwind 4)
- **Port 3001**: Stable versions (Next 14, React 18, Tailwind 3)

### 3. File Naming
- **Port 3000**: kebab-case (hero.tsx)
- **Port 3001**: PascalCase (Hero.tsx)

## Questions

1. **Which tool built Port 3000?**
   - Not Factory Droid (that failed)
   - Not Codex CLI (that's Port 3001)
   - Did you run Codex extension separately in ~/Desktop/dev/claudia/?

2. **Visual Comparison Needed**
   - Both should look similar (same PDR, same model)
   - Need to compare actual rendered output
   - Check mobile responsiveness
   - Check Spanish copy quality

## Next Steps

1. **Visit both sites**
   - http://localhost:3000
   - http://localhost:3001

2. **Compare**
   - Visual design accuracy
   - Mobile responsiveness
   - Spanish copy
   - Animation smoothness
   - WhatsApp CTA conversion flow

3. **Run Lighthouse**
   ```bash
   npx lighthouse http://localhost:3000 --view
   npx lighthouse http://localhost:3001 --view
   ```

4. **Pick the winner** based on:
   - Code quality
   - Organization
   - Performance
   - Visual accuracy to PDR

## Notes
- Both are Next.js (you mentioned one wasn't - both are!)
- Port 3000 has NEWER dependencies (could be better or more unstable)
- Port 3001 (Codex CLI) has better folder organization
