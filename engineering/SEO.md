# SEO Guidelines

## 1. Purpose

This document defines Search Engine Optimization (SEO) standards for PINTECHRA web projects.

The objective is to make websites discoverable, understandable, and accessible to search engines while maintaining a high-quality user experience.

SEO must be considered during planning, design, development, and deployment.

## 2. Core Principles

- Create useful and relevant content.
- Maintain clear information architecture.
- Use semantic HTML.
- Provide descriptive page metadata.
- Ensure pages can be discovered and crawled.
- Optimize performance and mobile usability.
- Avoid manipulative SEO practices.
- Prioritize users over search engine manipulation.

SEO should improve discoverability without compromising content quality.

## 3. Page Titles

Every important page should have a unique and descriptive title.

Requirements:

- Describe the page accurately.
- Include the primary topic naturally.
- Keep titles concise and meaningful.
- Avoid keyword stuffing.
- Avoid duplicate titles across important pages.
- Include the brand name when appropriate.

Example:

```html
<title>IoT Digital Clock | PINTECHRA</title>
```

## 4. Meta Descriptions

Provide a meaningful meta description for important pages.

Requirements:

- Summarize the page content.
- Explain its value to potential visitors.
- Use natural language.
- Avoid keyword stuffing.
- Avoid duplicate descriptions.
- Make descriptions relevant to each page.

Example:

```html
<meta
  name="description"
  content="Explore PINTECHRA's IoT digital clock with real-time display and remote configuration."
/>
```

Search engines may generate a different search-result snippet when appropriate.

## 5. Heading Structure

Use headings to organize content logically.

- Use one clear primary page heading.
- Maintain a logical heading hierarchy.
- Use headings to describe actual content sections.
- Avoid selecting heading levels only for visual appearance.
- Do not skip levels without a structural reason.

Use CSS to control visual heading sizes.

## 6. Semantic HTML

Use meaningful HTML elements.

Examples:

- `<header>` for introductory content.
- `<nav>` for navigation.
- `<main>` for primary content.
- `<article>` for independent content.
- `<section>` for thematic sections.
- `<footer>` for footer content.

Semantic structure helps browsers, assistive technologies, and search engines understand page content.

## 7. URL Structure

URLs should be clear and understandable.

Requirements:

- Use descriptive paths.
- Prefer lowercase characters.
- Use hyphens to separate words.
- Avoid unnecessary parameters.
- Avoid excessively deep URL structures.
- Maintain consistent routing conventions.

Example:

```text
/products/iot-digital-clock
```

Use redirects when URLs change to preserve relevant existing links.

## 8. Image SEO

Images should be optimized for users and search engines.

- Use descriptive filenames when practical.
- Provide appropriate alternative text.
- Optimize image dimensions and file sizes.
- Use modern image formats when beneficial.
- Avoid keyword stuffing in alternative text.
- Provide captions when they add useful context.

Example:

```html
<img
  src="/images/iot-digital-clock.webp"
  alt="PINTECHRA IoT digital clock display"
/>
```

## 9. Internal Linking

Create useful connections between related pages.

- Use descriptive anchor text.
- Link to relevant content.
- Maintain logical navigation.
- Avoid broken internal links.
- Ensure important pages are reachable.
- Avoid excessive or irrelevant links.

Internal links should help visitors understand and navigate the website.

## 10. Technical SEO

Consider the following technical requirements:

### Sitemap

- Provide an XML sitemap when appropriate.
- Include canonical URLs for indexable pages.
- Keep the sitemap updated.
- Avoid listing pages that should not be indexed.

### Robots.txt

- Provide a valid robots.txt file when appropriate.
- Do not accidentally block important website resources.
- Remember that robots.txt is not a security mechanism.

### Canonical URLs

Use canonical tags when duplicate or similar URLs may exist.

Example:

```html
<link
  rel="canonical"
  href="https://example.com/products/iot-digital-clock"
/>
```

Replace example URLs with the actual production URL.

### Indexing

- Ensure important pages are indexable.
- Use `noindex` only when intentionally required.
- Avoid accidental indexing restrictions.
- Verify the production website after deployment.

## 11. Structured Data

Use structured data when it accurately describes the page.

Possible schema types include:

- Organization.
- WebSite.
- Product.
- BreadcrumbList.
- Article.
- LocalBusiness.

Requirements:

- Use appropriate schema types.
- Provide accurate information.
- Follow official structured data guidelines.
- Do not invent ratings, reviews, prices, or product availability.
- Validate structured data before deployment.

Structured data does not guarantee rich search results.

## 12. Social Sharing Metadata

Provide social sharing metadata where appropriate.

Consider:

- Open Graph title.
- Open Graph description.
- Open Graph image.
- Open Graph URL.
- Twitter Card metadata.

Social metadata should accurately represent the page being shared.

## 13. Mobile and Performance SEO

Search visibility is affected by the overall quality of the website.

Ensure that:

- Pages work well on mobile devices.
- Content remains accessible.
- Layouts do not break at smaller widths.
- Loading performance is optimized.
- Core Web Vitals are considered.
- Important content is not unnecessarily hidden.

Refer to the Responsive Design and Performance guidelines.

## 14. Content Quality

Content must provide genuine value.

- Write clear and accurate information.
- Use relevant terminology naturally.
- Avoid duplicated or thin content.
- Keep important information updated.
- Use descriptive section headings.
- Do not generate content solely to manipulate rankings.
- Clearly distinguish factual claims from promotional statements.

Content should serve the actual needs of visitors.

## 15. SEO Testing and Monitoring

Use suitable tools to evaluate SEO.

Recommended tools:

- Google Search Console.
- Google Analytics when appropriate.
- Lighthouse.
- PageSpeed Insights.
- Rich Results Test.
- Schema Markup Validator.

Check:

- Indexing status.
- Crawl errors.
- Broken links.
- Metadata.
- Structured data.
- Mobile usability.
- Performance.
- Search appearance.

SEO should be monitored after deployment, not only during development.

## 16. AI SEO Requirements

AI coding agents must:

1. Understand the website's purpose and audience.
2. Create relevant page titles and descriptions.
3. Maintain semantic HTML structure.
4. Use descriptive and accessible image text.
5. Avoid keyword stuffing.
6. Implement technical SEO appropriately.
7. Use accurate structured data.
8. Avoid inventing business or product information.
9. Verify URLs and metadata.
10. Never guarantee search ranking improvements.

SEO recommendations must be based on actual project content.

## 17. SEO Quality Checklist

- [ ] Important pages have unique titles.
- [ ] Meta descriptions are relevant.
- [ ] Heading hierarchy is logical.
- [ ] Semantic HTML is used.
- [ ] URLs are descriptive.
- [ ] Images are optimized.
- [ ] Alternative text is appropriate.
- [ ] Internal links are useful.
- [ ] Sitemap is configured when appropriate.
- [ ] Robots.txt is configured correctly.
- [ ] Canonical URLs are handled when needed.
- [ ] Structured data is accurate when implemented.
- [ ] Social sharing metadata is provided when appropriate.
- [ ] Mobile usability is verified.
- [ ] Technical SEO checks have been performed.

## 18. Final Principle

Good SEO starts with a well-structured website and genuinely useful content.

Build for people first, then make it easy for search engines to understand and discover the experience.
