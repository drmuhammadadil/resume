# WEBSITE HANDOVER — Dr. Muhammad Adil

This website is a static HTML site hosted on **GitHub** and deployed automatically through **Cloudflare Pages**.

## How publishing works
1. Edit files in the GitHub repository.
2. Commit the changes to the `main` branch.
3. Cloudflare Pages detects the new commit and deploys automatically.
4. The live site updates at `https://drmuhammadadil.com/`.

---

## Main files and folders
- `/index.html` → homepage
- `/gallery.html` → gallery page
- `/blog/index.html` → blog homepage
- `/blog/posts/` → individual blog posts
- `/images/gallery/` → upload future gallery photos here
- `/images/blog/` → upload blog featured images here
- `/images/books/` → upload future book cover images here
- `/images/profile/` → profile / headshot images
- `/templates/` → reusable code snippets

---

## Workflow 1 — Edit text on the homepage
1. Open `index.html`.
2. Change the text.
3. Commit with a clear message, for example: `Update biography`.
4. Wait for Cloudflare Pages to deploy.

## Workflow 2 — Add a new gallery image
1. Upload the image into `/images/gallery/`.
2. Open `gallery.html`.
3. Duplicate one existing gallery card or use `/templates/gallery-card-snippet.html`.
4. Change:
   - image path
   - alt text
   - title/caption
   - optional description
5. Commit with a message such as: `Add conference gallery photo`.

### Gallery filename examples
- `conference-islamabad-2026.jpg`
- `award-ceremony-2026.jpg`
- `seminar-peshawar-2026.jpg`

---

## Workflow 3 — Publish a new blog post
1. Upload the featured image into `/images/blog/`.
2. Duplicate `/blog/posts/post-template.html`.
3. Rename it, for example: `seerah-research-modern-age.html`.
4. Edit:
   - page title
   - meta description
   - canonical URL
   - visible article title
   - publication date
   - article text
   - featured image path
5. Open `/blog/index.html`.
6. Duplicate one existing blog card or use `/templates/blog-card-snippet.html`.
7. Change:
   - image path
   - date
   - title
   - short summary
   - article link
8. Commit with a message such as: `Publish new Seerah article`.

---

## Workflow 4 — Add a new book
1. Upload the cover image to `/images/books/`.
2. Open `index.html`.
3. Find the Books section.
4. Duplicate one existing book card.
5. Update the cover image, title, and description.
6. Commit with a message such as: `Add new book`.

---

## Best practices
- Use **one task = one commit**.
- Use clear commit messages.
- Keep images optimized.
- Recommended blog image size: **1200 × 675 px**.
- Recommended gallery image size: **1200–1800 px wide**.
- Prefer filenames like `event-name-year.jpg`, not `IMG_0098.jpg`.

---

## What not to change during normal publishing
The owner normally does **not** need to change:
- Cloudflare DNS
- nameservers
- custom domain settings
- Cloudflare redirect rules
- SSL settings
- GitHub ↔ Cloudflare connection

---

## If something goes wrong
1. Open **Cloudflare → Workers & Pages → Deployments** and check the latest deployment.
2. If the deployment failed, read the error.
3. If the site looks broken after a content change, compare the last edited file in GitHub and restore the previous version if necessary.

---

## Android publishing tip
For uploading/replacing files, use **Chrome with Desktop Site enabled** rather than the GitHub Android app. It is much easier for file uploads.
