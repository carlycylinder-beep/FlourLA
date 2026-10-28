# Flour LA, Inc. website
Static site for GitHub Pages at www.flourla.com.

## Files to upload (repo root)
index.html, 404.html, robots.txt, sitemap.xml, CNAME, README.md, the `home` folder (redirects the old Google Sites /home URL) and the `assets` folder (all photos, flat, no subfolders). File names are case-sensitive.

## Deploy
1. Upload everything to the `main` branch. Settings > Pages > Deploy from branch > main / root. Custom domain: www.flourla.com. Enable Enforce HTTPS.
2. DNS: CNAME `www` to `<your-github-username>.github.io`. For the bare domain flourla.com, add the four GitHub Pages A records (see GitHub Docs, "Managing a custom domain for your GitHub Pages site") so it redirects to www.
3. Google Search Console: add the domain, submit https://www.flourla.com/sitemap.xml.

## Contact form
The form posts to FormSubmit and emails carly@flourla.com. The first submission triggers a one-time activation email to that address: click the confirm link. Then send a test inquiry. FormSubmit also emails a private alias string; you can swap it into the form action in place of carly@flourla.com to keep the address out of the page source.

## Adding photos
Use descriptive file names, alt text, width and height, and `loading="lazy"`. Gallery pattern:
<figure style="--r:1.5" tabindex="0"><img src="assets/name.jpg" width="1200" height="800" loading="lazy" alt="Describe the photo"><figcaption>Caption</figcaption></figure>
(inside a `<div class="gal" style="--h:300px">`). Click-to-enlarge works automatically.
