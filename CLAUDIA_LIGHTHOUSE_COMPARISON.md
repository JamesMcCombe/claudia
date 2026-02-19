# Claudia Lighthouse Comparison - Bake-Off Results

## Summary
Both sites were built by **GPT-5.3-Codex**, but through different tools and with different Next.js versions.

## Lighthouse Scores

### Port 3000 - Score: **71/100** ✅ WINNER
- **Tool**: Unknown (appears to be Codex via browser extension in ~/Desktop/dev/claudia/)
- **Next.js**: 16.1.6 (latest - React 19, Tailwind 4)
- **Location**: `/Users/zeus/Desktop/dev/claudia/claudia-site`
- **Built**: Feb 18, 11:42 PM NZDT

### Port 3001 - Score: **54/100**
- **Tool**: Codex CLI
- **Next.js**: 14.2.35 (stable - React 18, Tailwind 3)
- **Location**: `/Users/zeus/Desktop/dev/claudia-codex/claudia-site`
- **Built**: Feb 18, 11:39 PM NZDT

## Performance Breakdown (Port 3000 - Score 71)

### Core Web Vitals
- **First Contentful Paint (FCP)**: 2.4s
- **Largest Contentful Paint (LCP)**: 7.2s ⚠️ (needs improvement)
- **Total Blocking Time (TBT)**: 164ms ✅
- **Cumulative Layout Shift (CLS)**: Good ✅
- **Speed Index**: 2.9s

### Key Issues Found
1. **LCP is slow** (7.2s) - main performance bottleneck
2. **Server response time**: 68ms ✅ (good)
3. **Back/Forward Cache**: Not enabled (4 blockers found)
4. **JavaScript Issues**:
   - 214KB unminified JavaScript
   - 392KB unused JavaScript
5. **Legacy JavaScript**: 14.5KB of polyfills not needed for modern browsers

### What's Working Well
- ✅ HTTPS enabled
- ✅ No console errors
- ✅ Good server response time (68ms)
- ✅ Mobile-responsive
- ✅ All accessibility checks passed
- ✅ SEO fundamentals in place

## Key Differences

| Aspect | Port 3000 (71) | Port 3001 (54) |
|--------|----------------|----------------|
| **Next.js** | 16.1.6 | 14.2.35 |
| **React** | 19.2.3 | 18.2.0 |
| **Tailwind** | 4.0 | 3.4.17 |
| **Organization** | Flat component structure | Organized (sections/ ui/) |
| **File Naming** | kebab-case | PascalCase |
| **Dependencies** | Bleeding edge | Stable |
| **Lighthouse Score** | 71 | 54 |

## Winner Analysis

**Port 3000 wins by 17 points** (71 vs 54)

### Why Port 3000 Won
1. **Newer Next.js 16** with better optimizations
2. **React 19** performance improvements
3. **Tailwind 4** optimizations
4. Better build output despite bleeding-edge stack

### Why Port 3001 Lost
- Older dependencies (Next 14, React 18)
- Potentially different build configuration
- May have different optimization settings

## Recommendations

### Immediate (Port 3000)
1. **Fix LCP (7.2s → <2.5s target)**:
   - Optimize hero image loading
   - Preload critical resources
   - Check font loading strategy

2. **Reduce unused JavaScript (392KB)**:
   - Use dynamic imports for non-critical code
   - Code split by route
   - Remove unused dependencies

3. **Enable Back/Forward Cache**:
   - Fix WebSocket usage
   - Remove `Cache-Control: no-store` from main resource
   - Optimize for BFCache compatibility

### Next Steps
1. Run detailed comparison of both implementations
2. Check mobile responsiveness manually
3. Test WhatsApp CTA conversion flow
4. Compare Spanish copy quality
5. Decide if Port 3000's newer stack is worth the bleeding-edge risk

## Verdict

**Port 3000 is the winner** but has room for optimization. The newer Next.js 16 + React 19 + Tailwind 4 stack provides better baseline performance.

### Action Items
1. ✅ Use Port 3000 as the production candidate
2. 🔧 Optimize LCP (hero image, fonts)
3. 🔧 Reduce JavaScript bundle size
4. 🔧 Enable Back/Forward Cache
5. 📊 Retest after optimizations (target: 85+ score)

### Target Metrics
- Performance: 85+ (currently 71)
- LCP: <2.5s (currently 7.2s)
- TBT: <200ms (currently 164ms ✅)
- CLS: <0.1 (currently good ✅)

## Bake-Off Conclusion

While Codex CLI (Port 3001) has better code organization (sections/, PascalCase), the implementation using newer Next.js 16 (Port 3000) delivers better actual performance.

**Recommendation**: Use Port 3000 as base, but adopt Port 3001's folder organization pattern for maintainability.
