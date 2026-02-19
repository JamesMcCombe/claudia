# Product Design Record: Claudia 2.0 Marketing Website

**Project:** Claudia WhatsApp Shopping Assistant - Marketing Website  
**Audience:** Codex 5.3 AI Agent  
**Objective:** Build a conversion-optimized, culturally-relevant marketing site for LATAM women  
**Timeline:** MVP in one session (4-6 hours development time)  
**Success Metric:** 40%+ click-through rate on WhatsApp CTA

---

## 📋 EXECUTIVE SUMMARY

### What is Claudia?
Claudia is a WhatsApp-native AI shopping assistant for women in Latin America. It compares prices across marketplaces (Mercado Libre, Amazon, Shein, etc.), tracks deals, and enables group shopping—all within WhatsApp. No app download required.

### Why This Website Matters
- **Primary conversion goal:** Get users to add Claudia's WhatsApp number
- **Secondary goal:** Explain value proposition in <10 seconds
- **Context:** LATAM women are time-poor, privacy-conscious, mobile-first shoppers

### Target User
**María, 28, Mexico City:**
- Shops online 2-3x/month
- Uses WhatsApp 50+ times/day
- Juggles work + family (limited "me time")
- Price-sensitive (looks for cuotas sin interés)
- Trusts influencer recommendations > ads
- Skeptical of new apps (too many passwords)

---

## 🎯 CORE PRODUCT FEATURES (Context for Messaging)

### 1. **Cross-Marketplace Price Comparison**
User asks: "Busco labial rojo mate bajo $20"  
Claudia searches Mercado Libre, Amazon MX, Liverpool, Shein  
Returns top 3 with prices, ratings, delivery, installments

### 2. **Multimodal Input**
- **Text:** Natural language search
- **Voice:** Send voice note, Claudia transcribes and responds
- **Image:** Send photo of product, Claudia finds similar items

### 3. **Price Tracking**
User: "Rastrear precio"  
Claudia: Monitors product, sends alert when price drops

### 4. **Daily Deal Alerts**
7 PM (peak shopping time): Sends 1-2 curated deals based on interests

### 5. **Group Shopping**
Share product with friends → 3+ people buy → Everyone gets 15% off

### 6. **Episodic Memory**
Remembers past searches, sizes, brands, shopping lists  
"Tu shampoo favorito bajó a $7!"

### 7. **Referral Program**
Invite friend → Friend spends $100 → Both get $100 credit

### 8. **Premium Tier ($3/month)**
Free: 5 tracked products, 1 daily deal  
Premium: Unlimited tracking, 3 daily deals, early access, voice responses

---

## 🏗️ WEBSITE STRUCTURE & CONTENT

### Page 1: Homepage (Single-Page Marketing Site)

---

#### SECTION 1: HERO (Above the Fold)
**Goal:** Instant clarity + emotional hook + CTA

```
[LAYOUT: Two-column on desktop, stacked on mobile]

LEFT COLUMN (60% width):
  [H1 - 40px, Poppins Bold, Deep Plum]
  "Tu amiga de compras en WhatsApp 🛍️"
  
  [Subheading - 20px, Inter Regular, Gray]
  "Ahorra tiempo y dinero comprando online. 
  Claudia compara precios, rastrea ofertas, y te avisa cuando bajan. 
  Gratis, fácil, directo en WhatsApp."
  
  [CTA PRIMARY - Large button, Coral background]
  "💬 Empezar Gratis en WhatsApp"
  [Below button: Tiny text]
  "Sin descargar apps. Sin dar tu email."
  
  [CTA SECONDARY - Outline button, Coral border]
  "▶️ Ver Demo (30 seg)"
  
  [Trust Signals Row - Small icons + text]
  ✅ 100% Gratis  |  🔒 Sin compartir datos  |  💰 Ahorra $50+/mes

RIGHT COLUMN (40% width):
  [Animated WhatsApp Chat Mockup]
  - iPhone frame with WhatsApp UI
  - Conversation scrolling:
    User: "Busco tenis Nike talla 25"
    Claudia: "🔍 Encontré 12 opciones..."
    [Shows 3 product cards with prices]
    Claudia: "El Nike Revolution está en $980 con envío gratis"
  - Subtle animation: Messages appear, scroll, repeat loop
  - Mobile: Reduce size, center below text
```

**Copy Notes:**
- "Amiga" = friend (warm, not corporate)
- "Gratis" mentioned 2x (removes barrier)
- "Sin descargar apps" = addresses app fatigue
- Time + money savings = dual value prop

---

#### SECTION 2: SOCIAL PROOF BAR
**Goal:** Legitimacy through logos + usage stats

```
[LAYOUT: Horizontal scroll on mobile, centered row on desktop]

[Gray background, 80px height]

[Text - 16px, Medium, Centered]
"Compara precios en:"

[Logos Row - Grayscale, 40px height]
[Mercado Libre] [Amazon] [Liverpool] [Shein] [Walmart]

[Divider - Vertical line]

[Stats]
"10,000+ usuarias activas" | "⭐ 4.9/5 en reseñas"
```

---

#### SECTION 3: HOW IT WORKS (3 Steps)
**Goal:** Simplicity (remove friction fears)

```
[LAYOUT: 3-column grid on desktop, stacked on mobile]

[Section Title - 32px, Center]
"Cómo funciona Claudia en 3 pasos"

[Each Step - Card with icon, title, description]

STEP 1:
  [Icon - 64px, Coral circle with WhatsApp logo]
  Title: "1. Agrega a Claudia"
  Text: "Guarda este número en tu WhatsApp: +52-XXX-CLAUDIA"
  [Small text: "Funciona en cualquier país de LATAM"]

STEP 2:
  [Icon - 64px, Coral circle with microphone/text/camera icons]
  Title: "2. Escribe, habla, o manda foto"
  Text: "Dile qué buscas. Claudia entiende texto, audio, e imágenes."

STEP 3:
  [Icon - 64px, Coral circle with price tag + dollar sign]
  Title: "3. Ahorra automáticamente"
  Text: "Recibe las mejores ofertas, precios comparados, y alertas de descuentos."

[CTA - Below steps]
"Empezar ahora es gratis →"
```

---

#### SECTION 4: FEATURES GRID (6 Core Features)
**Goal:** Show depth without overwhelming

```
[LAYOUT: 3x2 grid on desktop, 1-column on mobile]

[Section Title - 32px, Center]
"Todo lo que Claudia hace por ti"

[Each Feature - Card: Icon (top), Title, 2-line description]

1. 💸 Compara Precios
   "Busca en 5+ tiendas al mismo tiempo. Encuentra el precio más bajo en segundos."

2. 📸 Búsqueda por Foto
   "Manda una foto de lo que viste. Claudia encuentra productos similares."

3. 🔔 Alertas de Precio
   "Rastrea hasta 5 productos gratis. Te avisa cuando bajan de precio."

4. 🎁 Compras Grupales
   "Invita amigas a comprar juntas. Todas obtienen 15% off."

5. 🗣️ Habla Naturalmente
   "Manda audios. Claudia entiende español coloquial."

6. 🧠 Recuerda Tus Gustos
   "Aprende tu talla, marcas favoritas, y te sugiere ofertas relevantes."

[Below grid - Small text, center]
"¿Quieres más? Upgrade a Premium por $3/mes →"
```

---

#### SECTION 5: DEMO VIDEO
**Goal:** Show product in action (reduces uncertainty)

```
[LAYOUT: Centered, 16:9 video player]

[Video - 30 seconds, auto-play (muted), captions ON]
Content:
- 0-5s: Screen recording of WhatsApp chat opening
- 5-10s: User sends "Busco labial MAC rojo"
- 10-15s: Claudia shows 3 price comparison results
- 15-20s: User taps "Rastrear precio"
- 20-25s: Cut to notification: "Bajó a $15!"
- 25-30s: End screen: "Empieza gratis" + QR code

[Below video]
"👆 Así de fácil. Sin complicaciones."
```

---

#### SECTION 6: TESTIMONIALS (Social Proof)
**Goal:** Real voices = trust

```
[LAYOUT: Horizontal scroll carousel on mobile, 3-column on desktop]

[Section Title - 32px, Center]
"Lo que dicen nuestras usuarias"

[Each Testimonial Card]
[Photo - Circular, 64px, real woman]
[Name + Location - 16px, Bold] "María, CDMX"
[Star Rating] ⭐⭐⭐⭐⭐
[Quote - 18px, Italic]
"Ahorré $120 en mi compra navideña. Claudia encontró ofertas que ni sabía que existían!"

TESTIMONIAL 2:
"Laura, Medellín"
⭐⭐⭐⭐⭐
"Ya no pierdo tiempo buscando en 5 apps diferentes. Claudia lo hace en 10 segundos."

TESTIMONIAL 3:
"Sofia, São Paulo"
⭐⭐⭐⭐⭐
"Me encanta que respeta mi privacidad. Sin apps, sin emails, solo WhatsApp."

[Below carousel]
"Únete a 10,000+ mujeres ahorrando tiempo y dinero"
```

---

#### SECTION 7: PRICING (Free vs Premium)
**Goal:** Show free value, upsell premium gently

```
[LAYOUT: Two-column comparison table]

[Section Title - 32px, Center]
"Elige tu plan"

[LEFT COLUMN - Free]
[Badge - "Popular" in green]
Title: "Gratis para Siempre"
Price: "$0/mes"

Features (checkmarks):
✅ Comparación de precios ilimitada
✅ Búsqueda por texto, voz, foto
✅ 5 productos rastreados
✅ 1 alerta de oferta al día
✅ Compras grupales
✅ Programa de referidos ($100 por amiga)

[CTA - Coral button]
"Empezar Gratis"

[RIGHT COLUMN - Premium]
Title: "Premium"
Price: "$3/mes"
[Small text: "Primer mes gratis con código CLAUDIA100"]

Everything in Free +
✅ Productos rastreados ilimitados
✅ 3 alertas diarias (mañana, tarde, noche)
✅ Acceso anticipado a ofertas (30 min antes)
✅ Respuestas por voz (TTS)
✅ Ofertas exclusivas de marcas
✅ Sin anuncios

[CTA - Outline button]
"Probar Premium Gratis"
```

---

#### SECTION 8: REFERRAL CTA (Viral Growth)
**Goal:** Encourage sharing

```
[LAYOUT: Full-width, gradient background (coral to gold)]

[Icon - 128px, Gift box illustration]

[Title - 36px, White, Center]
"Invita amigas. Gana $100."

[Description - 20px, White, Center]
"Por cada amiga que gaste $100+, ambas reciben $100 en crédito.
Sin límite. Mientras más compartes, más ahorras."

[CTA - White button with coral text]
"Ver Cómo Funciona"

[Small text below - White, 14px]
"Ejemplo: Invita 5 amigas = $500 en crédito gratis"
```

---

#### SECTION 9: FAQ (Accordion)
**Goal:** Address objections preemptively

```
[LAYOUT: Single column, centered, max-width 700px]

[Section Title - 32px, Center]
"Preguntas Frecuentes"

[Accordion Items - Click to expand]

Q1: "¿Es realmente gratis?"
A: "Sí, 100% gratis. Ganamos una pequeña comisión cuando compras a través de nuestros links (como Amazon Affiliates), pero nunca te cobramos. Premium es opcional."

Q2: "¿Cómo protege mi privacidad?"
A: "No almacenamos tu número de teléfono ni datos personales. Claudia funciona solo en WhatsApp. No vendemos información a terceros. Lee nuestra [Política de Privacidad]."

Q3: "¿Funciona en mi país?"
A: "Actualmente en México, Colombia, Brasil, Argentina, y Chile. Más países pronto."

Q4: "¿Dónde compara precios?"
A: "Mercado Libre, Amazon, Liverpool, Shein, Walmart, Coppel, y más. Agregamos tiendas nuevas cada semana."

Q5: "¿Cómo uso la búsqueda por voz?"
A: "Manda una nota de voz a Claudia como le hablarías a una amiga. Ej: 'Busco tenis Nike para correr, talla 25, máximo mil pesos.'"

Q6: "¿Puedo confiar en las ofertas?"
A: "Sí. Claudia busca en tiempo real y verifica precios. También incluimos calificaciones de usuarios (⭐) para que compres con confianza."

Q7: "¿Qué es el programa de referidos?"
A: "Invita amigas por WhatsApp. Cuando tu amiga gasta $100+, ambas reciben $100 en crédito para usar en futuras compras. [Ver detalles →]"

Q8: "¿Necesito descargar una app?"
A: "No. Claudia vive 100% en WhatsApp. Solo agrega el número y empieza a chatear."
```

---

#### SECTION 10: FINAL CTA (Conversion Push)
**Goal:** Last chance to convert

```
[LAYOUT: Full-width, deep plum background, white text]

[Title - 40px, Center, White]
"Lista para ahorrar tiempo y dinero?"

[Subhead - 20px, Center, Light gray]
"Únete a 10,000+ mujeres comprando más inteligente."

[CTA - Large coral button]
"💬 Empezar Gratis en WhatsApp"

[Below button - Small text, white]
"Toma 10 segundos. Sin descargar nada."

[Trust badges row - Small icons]
🔒 Seguro  |  ⚡ Instantáneo  |  💯 Sin Riesgo
```

---

#### SECTION 11: FOOTER
**Goal:** Compliance + secondary links

```
[LAYOUT: 4-column grid on desktop, stacked on mobile]

COLUMN 1: Logo + Tagline
[Claudia Logo - 120px wide]
"Tu amiga de compras en WhatsApp"

COLUMN 2: Links
Producto
- Cómo Funciona
- Precios
- Premium
- Referidos

COLUMN 3: Soporte
- FAQ
- Contacto
- WhatsApp: +52-XXX
- Email: hola@claudia.app

COLUMN 4: Legal
- Términos de Uso
- Política de Privacidad
- Aviso de Cookies

[Social Media Row - Center, below columns]
[Instagram] [TikTok] [Twitter] [YouTube]

[Copyright - Center, bottom]
© 2026 Claudia. Hecho con 💜 en Ciudad de México.
```

---

## 🎨 DESIGN SPECIFICATIONS

### Color Palette (Exact Hex)
```css
--primary-coral: #FF6B6B
--primary-dark: #E85D75
--background-cream: #FFF8F0
--accent-gold: #F4A460
--text-plum: #5B3A5F
--success-green: #A8C69F
--alert-red: #FF4757
--trust-blue: #4A90E2
--gray-secondary: #6C757D
--white: #FFFFFF
```

### Typography Scale
```css
--font-heading: 'Poppins', sans-serif
--font-body: 'Inter', sans-serif
--font-accent: 'Caveat', cursive

--text-h1: 40px / 1.2 / 700
--text-h2: 32px / 1.3 / 600
--text-h3: 24px / 1.4 / 600
--text-body: 18px / 1.6 / 400
--text-small: 14px / 1.5 / 400
```

### Spacing System (8px base)
```css
--space-xs: 8px
--space-sm: 16px
--space-md: 24px
--space-lg: 32px
--space-xl: 48px
--space-2xl: 64px
```

### Border Radius
```css
--radius-sm: 8px (input fields)
--radius-md: 12px (buttons)
--radius-lg: 16px (cards)
--radius-full: 9999px (pills, avatars)
```

### Shadows
```css
--shadow-sm: 0 2px 8px rgba(0,0,0,0.08)
--shadow-md: 0 4px 12px rgba(0,0,0,0.12)
--shadow-coral: 0 4px 12px rgba(255,107,107,0.3)
```

---

## 📱 RESPONSIVE BREAKPOINTS

```css
/* Mobile-first approach */
--breakpoint-sm: 640px   /* Large phones */
--breakpoint-md: 768px   /* Tablets */
--breakpoint-lg: 1024px  /* Laptops */
--breakpoint-xl: 1280px  /* Desktops */
```

**Priority:** Mobile (375px width) → Tablet (768px) → Desktop (1280px)

---

## 🔧 TECHNICAL REQUIREMENTS

### Framework & Stack
```
- Next.js 14+ (App Router)
- TypeScript
- Tailwind CSS (with custom config)
- Framer Motion (animations)
- Shadcn/ui components (customized)
```

### Performance Targets
```
- Lighthouse Score: 95+ (mobile)
- LCP (Largest Contentful Paint): <2s
- CLS (Cumulative Layout Shift): <0.1
- FID (First Input Delay): <100ms
- Total Bundle Size: <300KB (gzipped)
```

### SEO Setup
```html
<title>Claudia - Tu Asistente de Compras en WhatsApp | Ahorra Tiempo y Dinero</title>
<meta name="description" content="Compara precios en Mercado Libre, Amazon, Shein y más. Gratis, fácil, directo en WhatsApp. Ahorra $50+ al mes sin descargar apps.">
<meta property="og:image" content="/og-image.png" (1200x630)>
<link rel="canonical" href="https://claudia.app">
```

### Analytics (PostHog Events)
```javascript
- page_view (default)
- cta_click (WhatsApp button)
- demo_video_play
- demo_video_complete
- pricing_viewed
- faq_opened (which question)
- referral_link_clicked
```

---

## 🌐 LOCALIZATION PREP

### Initial Launch: Mexico (Spanish)
- Currency: MXN ($)
- Phone format: +52 XX-XXXX-XXXX
- Marketplaces: Mercado Libre MX, Amazon MX, Liverpool, Coppel
- Colloquialisms: "Tú" form, Mexican Spanish idioms

### Future: Brazil (Portuguese)
- Domain: claudia.app/br
- Currency: BRL (R$)
- Marketplaces: Mercado Livre, Amazon BR
- Language: Portuguese (BR variant)

### Scalable Structure
```
/locales/es-MX.json
/locales/pt-BR.json
/locales/es-CO.json
```

---

## ⚙️ COMPONENT LIBRARY GUIDELINES

### Using 21st.dev Components
**Recommended Components to Adapt:**
1. **Hero Section:** 21st.dev "Hero with App Mockup"
2. **Feature Grid:** 21st.dev "Feature Cards with Icons"
3. **Pricing Table:** 21st.dev "Pricing Comparison"
4. **FAQ:** 21st.dev "Accordion FAQ"
5. **Testimonials:** 21st.dev "Testimonial Carousel"

**Customizations Required:**
- Change color scheme to Claudia palette (coral/plum)
- Replace icons with custom illustrations
- Adjust spacing for mobile (80% of users)
- Add LATAM-specific elements (WhatsApp green accents, peso signs)

### Custom Components to Build
1. **WhatsApp Chat Mockup** (animated, looping conversation)
2. **Marketplace Logo Bar** (horizontal scroll with logos)
3. **Savings Calculator** (referral math: 5 friends = $500)
4. **Country Selector** (dropdown with flags)

---

## 🎬 ANIMATION SPECIFICATIONS

### Hero Animations
```javascript
// H1 fades in
{ opacity: 0 → 1, y: 20 → 0, duration: 0.6s, ease: "easeOut" }

// Subhead follows (stagger 200ms)
{ delay: 0.2s, ... same as H1 }

// WhatsApp mockup slides in from right
{ x: 100 → 0, opacity: 0 → 1, duration: 0.8s, delay: 0.4s }

// Chat messages type in (loop)
Message 1 appears → wait 1s → Message 2 appears → wait 1.5s → scroll up → repeat
```

### Scroll-Triggered
```javascript
// Features fade up as they enter viewport
{ 
  initial: { opacity: 0, y: 30 },
  whileInView: { opacity: 1, y: 0 },
  viewport: { once: true },
  transition: { duration: 0.5 }
}
```

### Button Hovers
```css
.button-primary:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-coral);
  transition: all 0.2s ease;
}
```

---

## 🚨 CRITICAL SUCCESS FACTORS

### Non-Negotiable Elements
1. **WhatsApp CTA must be above the fold** (mobile + desktop)
2. **Privacy messaging appears 3+ times** (hero, FAQ, footer)
3. **Mobile optimization is primary** (test on real device)
4. **Load time <2s** (LATAM 3G networks)
5. **Spanish language is native, not translated** (no awkward phrasing)

### Avoid These Mistakes
❌ Generic stock photos (use LATAM women or illustrations)  
❌ Long paragraphs (busy women skim)  
❌ Hidden pricing (transparency builds trust)  
❌ US-centric examples (Thanksgiving, dollars)  
❌ Forcing email signup (WhatsApp is the funnel)

---

## 📊 CONVERSION OPTIMIZATION

### A/B Test Ideas (Post-Launch)
- CTA text: "Empezar Gratis" vs "Hablar con Claudia"
- Hero image: Chat mockup vs Real woman shopping
- Testimonial format: Text quotes vs Video clips
- Referral reward: $100 vs 500 pesos (localization)

### Exit Intent Popup (Optional)
```
Trigger: User moves mouse to close tab
Content: 
"¡Espera! ⏰"
"Ahorra 10 minutos hoy. Prueba Claudia gratis."
[WhatsApp button]
```

---

## ✅ DEFINITION OF DONE

**Codex Agent Deliverables:**
- [ ] Fully responsive Next.js site (mobile + desktop)
- [ ] All 11 sections implemented with content
- [ ] WhatsApp CTA buttons functional (wa.me link)
- [ ] Animated hero mockup (looping conversation)
- [ ] FAQ accordion (8 questions, clickable)
- [ ] Pricing table (free vs premium comparison)
- [ ] Footer with all links
- [ ] PostHog analytics integrated
- [ ] SEO meta tags configured
- [ ] Lighthouse score 95+ (mobile)
- [ ] Deployed to Vercel (preview URL)

**Bonus (If Time Permits):**
- [ ] Demo video embedded (30s placeholder or real)
- [ ] Testimonials carousel (3+ quotes)
- [ ] Referral calculator widget
- [ ] Dark mode toggle
- [ ] Country selector (flag dropdown)

---

## 🤖 INSTRUCTIONS FOR CODEX AGENT

### Your Mission
Build a high-converting, culturally-relevant marketing website for Claudia, a WhatsApp shopping assistant targeting LATAM women. Prioritize mobile-first design, trust signals, and a clear path to the WhatsApp CTA.

### Creative Freedom
You have full autonomy to:
- Choose exact shades within the color palette
- Design the WhatsApp chat mockup animation
- Write micro-copy (keep it conversational, warm, Spanish)
- Select illustration style (flat, semi-flat, geometric)
- Optimize layout for content flow
- Add delightful interactions (hover states, transitions)

### Design Principles to Follow
1. **Mobile-first:** 70%+ users are on phones
2. **Trust-first:** Privacy concerns are high, address early
3. **Clarity over creativity:** User should understand value in 5 seconds
4. **LATAM cultural relevance:** Colors, language, examples feel local
5. **Speed:** Every second of load time costs conversions

### Reference Materials
- Design inspiration: `CLAUDIA_DESIGN_INSPIRATION.md`
- Component library: 21st.dev/community/components
- Color psychology: Nubank (approachable), Glossier (minimal), Rare Beauty (authentic)

### What "Good" Looks Like
✅ User lands on page → Immediately understands "WhatsApp shopping assistant"  
✅ Sees "Gratis" and "Sin descargar apps" → Barrier removed  
✅ Clicks "Empezar Gratis" → Taken to WhatsApp chat with Claudia  
✅ Entire flow takes <30 seconds from landing to WhatsApp  
✅ Site feels like talking to a smart friend, not a corporation

### Technical Constraints
- **Framework:** Next.js 14+ (App Router, TypeScript)
- **Styling:** Tailwind CSS (custom config for Claudia palette)
- **Components:** Shadcn/ui (customized) + Framer Motion (animations)
- **Hosting:** Vercel (edge, LATAM CDN)
- **Performance:** Lighthouse 95+, LCP <2s

### Development Workflow
1. **Setup:** Initialize Next.js project with Tailwind + TypeScript
2. **Config:** Add custom colors, fonts, spacing to tailwind.config
3. **Layout:** Build mobile-first (375px → 1280px)
4. **Sections:** Implement hero → social proof → how it works → ... → footer
5. **Animations:** Add Framer Motion for hero, scroll-triggered features
6. **Analytics:** Integrate PostHog event tracking
7. **SEO:** Configure meta tags, og:image, sitemap
8. **Test:** Run Lighthouse, check mobile rendering
9. **Deploy:** Push to Vercel, share preview URL

### Questions to Consider
- Should the hero mockup show a real conversation or generic placeholder?
- Animated illustrations or static icons for features?
- Video auto-play or click-to-play?
- Dark mode toggle or launch light-only?

### Success Criteria
**MVP Definition:**
- Page loads in <2s (3G network)
- WhatsApp CTA above fold (mobile + desktop)
- All content in Spanish (no English fallbacks)
- 95+ Lighthouse score (mobile)
- User can understand value prop in 5 seconds

**Stretch Goals:**
- Animated testimonials carousel
- Interactive referral calculator
- Country-specific landing pages (/mx, /br, /co)

---

## 📞 CONTACT & NEXT STEPS

**Questions for James:**
1. WhatsApp number to link to? (placeholder: +52-555-CLAUDIA)
2. Domain preference? (claudia.app, hola-claudia.com)
3. Primary launch country? (Mexico recommended)
4. Want real demo video or placeholder?

**After Codex Builds V1:**
1. Review on mobile device (iPhone 12/13, Android)
2. Test WhatsApp CTA click → opens chat
3. Check Spanish copy for naturalness
4. Iterate on colors/spacing
5. Deploy to production domain

---

**Remember:** This site isn't selling software—it's inviting a friend to help you shop smarter. Design accordingly. 🛍️💜

**Build Time Estimate:** 4-6 hours for full MVP  
**Let's ship it! 🚀**
