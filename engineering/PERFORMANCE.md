# Web Performance Guidelines

## 1. Purpose

This document defines performance standards for PINTECHRA web projects.

The objective is to build websites that load quickly, respond smoothly, and use system resources efficiently.

Performance must be considered throughout design, development, testing, and deployment.

## 2. Core Principles

- Optimize for real users and real devices.
- Prioritize loading speed and responsiveness.
- Avoid unnecessary resources.
- Reduce JavaScript complexity.
- Optimize images and media.
- Minimize expensive rendering operations.
- Measure before optimizing.
- Preserve visual quality while improving performance.

A fast website should not sacrifice usability or functionality.

## 3. Core Web Vitals

Use Google's Core Web Vitals as important performance indicators.

| Metric | Good Target |
|---|---:|
| Largest Contentful Paint (LCP) | ≤ 2.5 seconds |
| Interaction to Next Paint (INP) | ≤ 200 milliseconds |
| Cumulative Layout Shift (CLS) | ≤ 0.1 |

Targets should be evaluated at the 75th percentile of real-user visits when field data is available.

Laboratory tests are useful but do not fully represent real-world performance.

## 4. Image Optimization

Images are often a major source of page weight.

Requirements:

- Use appropriately sized images.
- Avoid unnecessarily large image files.
- Prefer WebP or AVIF when appropriate.
- Preserve visual quality.
- Use responsive images when beneficial.
- Define image dimensions to prevent layout shifts.
- Lazy-load offscreen images.
- Prioritize important above-the-fold images.

Do not lazy-load the main image responsible for the initial Largest Contentful Paint.

## 5. JavaScript Optimization

JavaScript should remain efficient and purposeful.

- Remove unused code.
- Avoid unnecessary dependencies.
- Split code when beneficial.
- Avoid excessive client-side rendering.
- Minimize expensive computations.
- Avoid unnecessary event listeners.
- Use efficient state updates.
- Load non-essential scripts only when needed.

Do not introduce complex JavaScript for simple interactions.

## 6. CSS Optimization

Maintain efficient styling.

- Remove unused CSS when possible.
- Avoid unnecessarily complex selectors.
- Reduce excessive visual effects.
- Avoid expensive animations.
- Reuse design tokens.
- Keep styles organized.
- Avoid excessive DOM complexity.

Use CSS animations thoughtfully, especially for weaker devices.

## 7. Font Optimization

Fonts affect both loading speed and visual stability.

- Limit the number of font families.
- Use only necessary font weights.
- Prefer optimized font formats such as WOFF2.
- Consider self-hosting when appropriate.
- Use `font-display` strategies carefully.
- Provide suitable fallback fonts.

Do not load multiple font variations without a clear design requirement.

## 8. Network and API Performance

External requests must be efficient.

- Avoid unnecessary API calls.
- Handle network failures.
- Use caching where appropriate.
- Avoid duplicate requests.
- Load data only when needed.
- Use pagination for large datasets.
- Consider debouncing frequent user input.
- Provide clear loading states.

Do not block the entire interface while unrelated data is loading.

## 9. Rendering Performance

Keep interface updates efficient.

- Avoid unnecessary component re-renders.
- Keep the DOM reasonably simple.
- Avoid expensive layout calculations.
- Use efficient rendering patterns.
- Avoid excessive animations and transitions.
- Reserve space for asynchronously loaded content.
- Keep scrolling smooth.

Use optimization techniques only when they provide measurable benefits.

## 10. Third-Party Resources

External libraries and services can affect performance.

- Evaluate dependencies before installation.
- Avoid unnecessary third-party scripts.
- Load external resources responsibly.
- Review the impact of analytics and tracking tools.
- Use reputable content delivery networks when appropriate.
- Avoid excessive embedded content.

Every external resource should provide meaningful value.

## 11. Caching and Delivery

Use appropriate delivery strategies.

Consider:
- Browser caching.
- Asset caching.
- Compression.
- CDN delivery.
- Cache invalidation.
- Static asset optimization.

Caching must not cause users to receive outdated or incorrect content.

## 12. Performance on Low-End Devices

Websites should remain usable on modest hardware.

- Avoid excessive background effects.
- Limit expensive blur and shadow effects.
- Keep animations lightweight.
- Reduce unnecessary JavaScript execution.
- Optimize image dimensions.
- Avoid memory-intensive components.
- Test on mobile devices where possible.

Visual quality must remain balanced with practical performance.

## 13. Performance Testing

Use suitable tools to evaluate performance.

Recommended tools include:

- Lighthouse.
- PageSpeed Insights.
- Chrome DevTools.
- WebPageTest.
- Real User Monitoring when available.

Measure:
- Initial loading.
- Interaction responsiveness.
- Layout stability.
- Resource sizes.
- JavaScript execution.
- Network requests.
- Mobile performance.

Record important findings before and after significant optimization work.

## 14. AI Performance Requirements

AI coding agents must:

1. Inspect existing performance issues before optimizing.
2. Avoid unnecessary dependencies.
3. Optimize images and media appropriately.
4. Avoid excessive JavaScript and CSS.
5. Preserve existing functionality.
6. Consider low-end devices.
7. Avoid premature optimization.
8. Use measurable evidence where possible.
9. Explain significant performance trade-offs.
10. Never claim performance improvements without verification.

## 15. Performance Quality Checklist

- [ ] Images are appropriately optimized.
- [ ] Fonts are loaded efficiently.
- [ ] JavaScript is reasonably lightweight.
- [ ] CSS is organized and efficient.
- [ ] Unnecessary network requests are avoided.
- [ ] Loading states are handled properly.
- [ ] Layout shifts are minimized.
- [ ] Animations remain efficient.
- [ ] Low-end devices are considered.
- [ ] Performance has been measured where possible.

## 16. Final Principle

Performance is part of user experience.

Build websites that feel fast, remain responsive, and use resources responsibly across different devices and network conditions.
