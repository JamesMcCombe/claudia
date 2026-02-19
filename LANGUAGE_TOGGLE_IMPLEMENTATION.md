# Language Toggle Implementation

**Default:** Spanish (es)  
**Secondary:** English (en)  
**Toggle Location:** Top-right corner of header

---

## UI Design

### Toggle Button (Desktop)

```
┌─────────────────┐
│ 🇪🇸 ES  │  EN  │
└─────────────────┘
```

**Active state:** Bold + underline  
**Inactive state:** Gray text  
**Hover:** Subtle highlight

### Toggle Button (Mobile)

```
┌──────┐
│ ES ▾ │
└──────┘
```

Dropdown on tap:
- 🇪🇸 Español
- 🇺🇸 English

---

## Implementation (Next.js)

### 1. i18n Configuration

**File:** `next.config.js`

```javascript
module.exports = {
  i18n: {
    locales: ['es', 'en'],
    defaultLocale: 'es',
    localeDetection: true
  }
}
```

---

### 2. Content Structure

**Directory:**
```
/locales
  /es
    common.json
    hero.json
    features.json
    pricing.json
  /en
    common.json
    hero.json
    features.json
    pricing.json
```

---

### 3. Example Content Files

**`/locales/es/hero.json`**
```json
{
  "headline": "Nunca Pierdas una Llamada",
  "subheadline": "Claudia es tu recepcionista AI que atiende llamadas 24/7",
  "cta": "Prueba Gratis"
}
```

**`/locales/en/hero.json`**
```json
{
  "headline": "Never Miss a Call Again",
  "subheadline": "Claudia is your AI receptionist that answers calls 24/7",
  "cta": "Start Free Trial"
}
```

---

### 4. Language Switcher Component

**File:** `components/LanguageToggle.tsx`

```typescript
import { useRouter } from 'next/router'
import { useState } from 'react'

export default function LanguageToggle() {
  const router = useRouter()
  const { locale, pathname, asPath, query } = router
  const [isOpen, setIsOpen] = useState(false)

  const changeLanguage = (newLocale: string) => {
    router.push({ pathname, query }, asPath, { locale: newLocale })
    setIsOpen(false)
    
    // Save preference
    localStorage.setItem('preferredLanguage', newLocale)
  }

  return (
    <div className="relative">
      {/* Desktop */}
      <div className="hidden md:flex items-center gap-2">
        <button
          onClick={() => changeLanguage('es')}
          className={`px-3 py-1 text-sm ${
            locale === 'es' 
              ? 'font-bold text-white border-b-2 border-cyan-400' 
              : 'text-gray-400 hover:text-gray-200'
          }`}
        >
          🇪🇸 ES
        </button>
        <span className="text-gray-600">|</span>
        <button
          onClick={() => changeLanguage('en')}
          className={`px-3 py-1 text-sm ${
            locale === 'en' 
              ? 'font-bold text-white border-b-2 border-cyan-400' 
              : 'text-gray-400 hover:text-gray-200'
          }`}
        >
          EN
        </button>
      </div>

      {/* Mobile */}
      <div className="md:hidden">
        <button
          onClick={() => setIsOpen(!isOpen)}
          className="px-4 py-2 bg-slate-800 rounded flex items-center gap-2"
        >
          <span>{locale === 'es' ? '🇪🇸 ES' : '🇺🇸 EN'}</span>
          <svg className="w-4 h-4" fill="currentColor" viewBox="0 0 20 20">
            <path fillRule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" />
          </svg>
        </button>
        
        {isOpen && (
          <div className="absolute right-0 mt-2 w-40 bg-slate-800 rounded shadow-lg">
            <button
              onClick={() => changeLanguage('es')}
              className="w-full px-4 py-2 text-left hover:bg-slate-700"
            >
              🇪🇸 Español
            </button>
            <button
              onClick={() => changeLanguage('en')}
              className="w-full px-4 py-2 text-left hover:bg-slate-700"
            >
              🇺🇸 English
            </button>
          </div>
        )}
      </div>
    </div>
  )
}
```

---

### 5. Using Translations

**File:** `pages/index.tsx`

```typescript
import { useTranslation } from 'next-i18next'
import { serverSideTranslations } from 'next-i18next/serverSideTranslations'

export default function Home() {
  const { t } = useTranslation('hero')

  return (
    <section>
      <h1>{t('headline')}</h1>
      <p>{t('subheadline')}</p>
      <button>{t('cta')}</button>
    </section>
  )
}

export async function getStaticProps({ locale }) {
  return {
    props: {
      ...(await serverSideTranslations(locale, ['hero', 'common']))
    }
  }
}
```

---

### 6. Auto-Detection

**File:** `middleware.ts`

```typescript
import { NextRequest, NextResponse } from 'next/server'

export function middleware(request: NextRequest) {
  const preferredLang = request.cookies.get('preferredLanguage')?.value
  const acceptLanguage = request.headers.get('accept-language')
  
  // Priority: Cookie > Browser > Default (es)
  if (preferredLang) {
    return NextResponse.next()
  }
  
  // Detect Spanish preference
  if (acceptLanguage?.includes('es')) {
    const response = NextResponse.redirect(new URL('/es', request.url))
    response.cookies.set('preferredLanguage', 'es')
    return response
  }
  
  return NextResponse.next()
}
```

---

## Testing Checklist

- [ ] Toggle works on desktop
- [ ] Dropdown works on mobile
- [ ] All pages translate correctly
- [ ] CTAs translate properly
- [ ] Forms handle both languages
- [ ] SEO meta tags change with language
- [ ] URL structure: `/es/` and `/en/`

---

## SEO Considerations

**URL Structure:**
```
https://claudia.ai/          → Redirects to /es/ or /en/
https://claudia.ai/es/       → Spanish version
https://claudia.ai/en/       → English version
```

**Hreflang Tags:**
```html
<link rel="alternate" hreflang="es" href="https://claudia.ai/es/" />
<link rel="alternate" hreflang="en" href="https://claudia.ai/en/" />
<link rel="alternate" hreflang="x-default" href="https://claudia.ai/es/" />
```

---

## Accessibility

- Use `lang` attribute on HTML: `<html lang="es">` or `<html lang="en">`
- ARIA labels for screen readers
- Keyboard navigation for toggle

---

**Implementation Priority:** Phase 1 MVP
