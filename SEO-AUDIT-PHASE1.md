# Phase 1 SEO Audit & Deployment Notes — drmuhammadadil.com

## What this patch fixes
- Refines homepage title, meta description and canonical.
- Adds Open Graph and Twitter metadata.
- Adds Person + ProfilePage + WebSite structured data.
- Connects the entity to the official Bacha Khan University faculty page, ORCID, Google Scholar and ResearchGate.
- Adds a direct University Profile link.
- Adds SEO metadata and CollectionPage schema to Gallery.
- Improves Blog title/description and adds Blog schema.
- Replaces the two placeholder/sample blog articles with substantive indexable articles.
- Adds ScholarlyArticle schema to both articles.
- Marks the reusable post template `noindex,follow`.
- Removes the template from sitemap.xml.
- Adds `lastmod`, `changefreq` and `priority` to sitemap.xml.
- Adds a crawlable 404 page with `noindex`.

## Important issue that remains
The Gallery still loads its legacy gallery HTML from a GitHub revision at runtime. It works for visitors,
but Phase 2 should move the photos into normal `/images/gallery/` files and render them directly in `gallery.html`.

## Google Search Console — immediately after deployment
1. Verify the Domain property `drmuhammadadil.com`.
2. Submit `https://drmuhammadadil.com/sitemap.xml`.
3. Request indexing for:
   - https://drmuhammadadil.com/
   - https://drmuhammadadil.com/blog/
   - https://drmuhammadadil.com/blog/posts/seerah-research-modern-age.html
   - https://drmuhammadadil.com/blog/posts/teaching-islamic-studies-today.html
   - https://drmuhammadadil.com/gallery.html
4. Do NOT request indexing for `/blog/posts/post-template.html`.

## First 30-day KPI
- All 5 indexable URLs discovered and indexed.
- Branded query impressions for `Dr Muhammad Adil`.
- Non-branded impressions begin for Seerah and Islamic Studies article topics.
- Zero canonical or robots errors in Search Console.
