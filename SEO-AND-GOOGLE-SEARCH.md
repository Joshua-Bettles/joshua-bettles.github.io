# SEO and Google Search setup

This site is configured for `https://joshua-bettles.github.io/`.

## Files added

- `robots.txt`: allows search crawlers and points them to the sitemap.
- `sitemap.xml`: lists the four canonical HTML pages.
- `index.html`: the canonical homepage, with title, description, canonical URL, social sharing metadata and Person structured data (JSON-LD).
- Each section page has its own title, description, canonical URL and Open Graph/Twitter metadata.

## Deploy

Commit and push the **contents** of this ZIP to the root of the `Joshua-Bettles/joshua-bettles.github.io` repository (or whichever repository publishes `joshua-bettles.github.io`). Keep `robots.txt` and `sitemap.xml` at repository root. After deployment, check these URLs in a browser:

- https://joshua-bettles.github.io/
- https://joshua-bettles.github.io/robots.txt
- https://joshua-bettles.github.io/sitemap.xml
- https://joshua-bettles.github.io/publications/
- https://joshua-bettles.github.io/blog/
- https://joshua-bettles.github.io/cv/

## Add the site to Google Search Console

1. Open [Google Search Console](https://search.google.com/search-console/).
2. Add a **URL prefix** property: `https://joshua-bettles.github.io/`. (A Domain property generally requires DNS verification, which isn't available for the `github.io` subdomain.)
3. Choose **HTML file** verification. Download the exact verification file Google gives you. Its filename and contents contain a unique token, so do not make up or rename it.
4. Put that downloaded file in the repository root, next to `index.html`, `robots.txt` and `sitemap.xml`, and push the change to GitHub Pages.
5. Visit the exact verification URL shown by Search Console to make sure it loads, then click **Verify** in Search Console. Keep the file on the site afterward.
6. In Search Console, open **Sitemaps**, enter `sitemap.xml`, and submit it.
7. Use **URL inspection** for `https://joshua-bettles.github.io/` and choose **Request indexing**. Repeat for key pages if useful.

Google may take days or longer to crawl and index the pages. These steps improve discoverability but cannot guarantee ranking or inclusion in search results. Submitting a sitemap is a hint, not a guarantee.

## Optional HTML-tag verification

If Search Console offers the HTML tag method instead, it will provide a line similar to this:

```html
<meta name="google-site-verification" content="YOUR_UNIQUE_TOKEN" />
```

Place the exact line Google gives you inside the `<head>` of the root `index.html`, commit and push, then click Verify. Replace the example token with Google's real token; don't publish the placeholder as if it verifies ownership.

## SEO code examples

### `robots.txt`

```text
User-agent: *
Allow: /
Sitemap: https://joshua-bettles.github.io/sitemap.xml
```

### `sitemap.xml`

```xml
<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  <url><loc>https://joshua-bettles.github.io/</loc></url>
  <url><loc>https://joshua-bettles.github.io/publications/</loc></url>
  <url><loc>https://joshua-bettles.github.io/blog/</loc></url>
  <url><loc>https://joshua-bettles.github.io/cv/</loc></url>
</urlset>
```

### Homepage `<head>` essentials

The root `index.html` already contains these. Keep the canonical URL absolute and update the description if the homepage copy changes.

```html
<title>Joshua Bettles | Robotics Researcher at The University of Manchester</title>
<meta name="description" content="Joshua Bettles is a postgraduate robotics researcher at The University of Manchester, researching robotic inspection, radiological surveying, coverage path planning and mobile manipulation.">
<meta name="robots" content="index, follow, max-image-preview:large">
<link rel="canonical" href="https://joshua-bettles.github.io/">
```
