# GadgetFix Reviews

A static website reviewing household gadgets, built with plain HTML, CSS, and JavaScript. No build step, no dependencies, no database.

## Structure

```
index.html          Homepage (hero, featured products, why-trust-us, CTA)
about.html           About page + Amazon affiliate disclosure
css/styles.css        Shared styles
js/script.js          Mobile nav toggle + placeholder affiliate link handling
images/                SVG product illustrations and favicon
```

## Adding real Amazon affiliate links

Each "View on Amazon" button is currently a placeholder:

```html
<a href="#" class="btn btn-amazon" data-affiliate-placeholder target="_blank" rel="nofollow sponsored noopener">View on Amazon</a>
```

Once approved for Amazon Associates, replace `href="#"` with your real affiliate
link (and you can drop the `data-affiliate-placeholder` attribute — it only
triggers the "not linked yet" alert in `js/script.js`). Keep `rel="nofollow
sponsored noopener"` on affiliate links; it's what Amazon and search engines
expect for paid/affiliate outbound links.

## Hosting on GitHub Pages

1. Push this repo to GitHub.
2. In the repo, go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to `Deploy from a branch`.
4. Pick the branch (e.g. `main`) and `/ (root)` folder, then save.
5. GitHub will publish the site at `https://<username>.github.io/<repo-name>/`.

No build tools or frameworks are required — it's plain static files.
