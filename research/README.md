# Research publications

Static blog-style publications served by the existing GitHub Pages site. No build
or external runtime is needed. Homepage → research/index.html → article.

## Files
- `index.html`: publication listing.
- `burbank-resident-priorities.html`: HT-RP-001, exploratory research brief.
- `research.css`: responsive, accessible and print styling shared by research pages.
- `catalog.json`: machine-readable publication metadata, evidence scope and section URLs.

## Add or update a publication
1. Use semantic HTML: article, a single h1, section IDs, source references and
   visible questions and answers. Keep all content available without scripts.
2. Give each publication a stable slug, ID, actual publication date, version,
   named author or organization, evidence type, and peer-review status. Do not
   invent credentials, affiliations, sample sizes, metrics, or peer review.
3. Separate primary-source facts, supplied observations and recommendations.
   Cite source URLs beside claims; include precise page or section locators.
4. State sampling limits, missing data, and corrections. For HT-RP-001 the raw
   capture was not reviewed; its year and timezone are unspecified. Do not infer
   citywide priorities, percentages or sentiment from it. Keep the platform
   described as social media. Preserve the conflicting city response counts.
5. Add the paper to this index, catalog.json, ../sitemap.xml, ../llms.txt and the
   research section of ../agents.html (the homepage .skills destination).
6. Set unique canonical, description, Open Graph and sharing metadata. Use
   Article and BreadcrumbList JSON-LD; FAQPage entries must match visible answers.
   Structured metadata aids parsing but does not guarantee search rich results.
7. Check JSON, local links and fragments, unique IDs, heading order, keyboard
   focus, narrow-screen table scrolling, print styling and browser layout.

Serve from the repository root with `python3 -m http.server 8765` and visit
`http://localhost:8765/research/`. Keep edits local until publication is requested.
