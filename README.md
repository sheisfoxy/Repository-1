# GadgetFix Reviews

A static website reviewing household gadgets, built with plain HTML, CSS, and JavaScript. No build step, no dependencies, no database.

Live at https://sheisfoxy.github.io/gadgetfix/

## Structure

```
index.html          Homepage (hero, featured products, why-trust-us, CTA)
about.html           About page + Amazon affiliate disclosure
css/styles.css        Shared styles
js/script.js          Mobile nav toggle
images/                Product photos and favicon
```

## Affiliate links

Each "View on Amazon" button on the homepage links to the real product page
with the `gadgetfix09-20` Associates tag attached. To update one (e.g. if a
product listing changes), find its `<a class="btn btn-amazon" ...>` in
`index.html` and swap the `href`. Keep `rel="nofollow sponsored noopener"` on
every affiliate link — it's what Amazon and search engines expect for
paid/affiliate outbound links.

## Hosting on GitHub Pages

Already configured: **Settings → Pages** is set to deploy from the
`claude/gadgets-review-site-y5t7kz` branch, root folder. Any push to that
branch redeploys automatically within a minute or two.
