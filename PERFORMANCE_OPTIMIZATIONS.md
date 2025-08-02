# Performance Optimizations

The project incorporates several techniques to improve Core Web Vitals and overall loading speed.

## Image and Media
- Responsive sizing with AVIF/WebP formats
- Aggressive compression through an `OptimizedImage` component
- ~70% reduction in total image payload

## CSS Delivery
- ~2 KB of critical CSS inlined in the document head
- Remaining styles loaded asynchronously after first paint
- Render-blocking CSS eliminated

## JavaScript
- Modern browserslist targeting removes legacy polyfills
- Dynamic imports and code splitting load heavy components on demand
- ~29 KB of unused JavaScript removed

## LCP Improvements
- Removed animation delays for hero content
- Preloaded fonts for faster text rendering

These optimizations collectively reduce bandwidth usage and improve LCP, FCP, and overall user experience.
