# DharmaCanvas website

A responsive, static Hindu art, culture and creativity discovery website.

## Included
- Responsive homepage and navigation
- Search and category filters
- 12 starter resources across art, drawing, festivals, stories, devotion, downloads and culture
- Original decorative SVG illustrations generated in the site code
- Resource detail modal with steps and cultural context notes
- Save/bookmark resources using browser localStorage
- Share resource action (uses Web Share where available)
- Basic SEO title, description, favicon and privacy placeholder

## Preview locally
Open `index.html` in a modern browser. For best results, run a simple local server:
- VS Code: install Live Server and choose "Open with Live Server"
- Or use Python: `python -m http.server 8000` in this folder, then visit `http://localhost:8000`

## Deploy
Upload the contents of this folder to GitHub Pages, Netlify, Cloudflare Pages or any static hosting provider. No build step or database is required.

## Add or edit content
Open `content/resources.js`. Each resource is one JavaScript object in `window.DHARMA_RESOURCES`.
Fields:
- `id`: unique slug
- `title`, `category`, `type`, `time`, `tag`, `description`
- `art`: illustration key (krishna, diya, rangoli, diwali, ganesha, hanuman, lotus, ramayana, mandala, navratri, sanskrit, temple)
- `intro`, `steps` (array), `note`

To add a new item, copy one object, give it a unique id, and add it inside the array. The category filter buttons currently include: All, Art & Drawing, Festivals, Stories, Devotion, Downloads. Add more filter buttons in `index.html` if you add categories such as Culture.

## Before publishing
1. Choose and verify your final brand/domain name.
2. Replace the placeholder email `hello@dharmacanvas.example`.
3. Add real, original or properly licensed images and downloadable files where indicated. The current illustrations are original decorative SVGs, not photographs or canonical deity depictions.
4. Verify religious facts, transliterations and dates with reliable sources and knowledgeable reviewers. Festival dates should be location-specific and updated annually.
5. Add a full privacy/cookie policy if you add analytics, advertising, affiliate links or user accounts.
6. Set up Search Console and submit a sitemap after publishing.
7. This starter version has no admin login or cloud CMS. Content is edited in `content/resources.js`; do not upload private credentials to this static site.

## Important
The sample content is introductory and educational. Hindu practices and interpretations vary by region, sampradaya, family and text. Review all content before publication, especially ritual instructions and scripture quotations.
