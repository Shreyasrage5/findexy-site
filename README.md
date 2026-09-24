# Findexy website

Small static landing page for [Findexy](https://apps.microsoft.com/store/detail/9NST54J4R5SC), a Windows file search app by Shrez Labs.

## Files

- `index.html` — homepage, features, screenshots, Free/Pro comparison, and Store buttons
- `privacy.html` — privacy policy
- `support.html` — support contact and quick answers
- `style.css` — responsive site styling
- `images/` — Findexy logo and Store screenshots
- `sitemap.xml` — homepage, privacy, and support URLs for search engines
- `robots.txt` — repository copy of crawler guidance (see note below)

No build tools or external JavaScript are required. Open `index.html` locally to preview it.

## Publish with GitHub Pages

In this repository, open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select **main** and **/(root)**, then save. The expected address is:

https://shreyasrage5.github.io/findexy-site/

The Microsoft Store button points to product ID `9NST54J4R5SC`. The support address is `findexy.support@gmail.com`, matching Findexy 3.5.14.

## Search indexing setup

1. In [Google Search Console](https://search.google.com/search-console), add the URL-prefix property `https://shreyasrage5.github.io/findexy-site/` (including the trailing slash). Complete ownership verification using the exact HTML file or meta tag Google gives you.
2. Submit `https://shreyasrage5.github.io/findexy-site/sitemap.xml` under **Sitemaps**, then use **URL Inspection → Request indexing** for the homepage.
3. In [Bing Webmaster Tools](https://www.bing.com/webmasters/), import the verified Google Search Console property or add and verify the same site directly. Submit the sitemap there too.

The pages already have canonical URLs. Search engines decide when or whether to index them; submission does not guarantee ranking or immediate inclusion.

**GitHub Pages note:** this project is hosted below `/findexy-site/`. Crawlers normally check `https://shreyasrage5.github.io/robots.txt` at the host root, not this repository's `/findexy-site/robots.txt`. The project file is therefore informational and its sitemap directive may not be discovered as a host-level robots directive. Submit the sitemap directly in the webmaster tools as above. A host-root robots file would require control of the root Pages site.
