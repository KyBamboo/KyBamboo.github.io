# APEX hub — static site

A dependency-free personal project hub + the privacy policy for the radio app.
Two files, no build step, no framework.

```
apex-hub/
├── index.html     ← the hub / landing page
├── privacy.html   ← GROL & Commercial Radio Prep privacy policy
└── README.md
```

## Preview locally
Just double-click `index.html` — it opens in any browser. That's it.

## Put it online (free hosting, ~2 minutes)
Any of these serve static files for free. Pick one:

**Cloudflare Pages** (recommended — free, fast, easy custom domains)
1. cloudflare.com → Pages → *Upload assets* → drag this whole folder in → Deploy.
2. Pages → your project → *Custom domains* → add `apex.navy` (or whatever you buy).
   Cloudflare walks you through the DNS records. Done.

**GitHub Pages**
1. Push this folder to a repo → Settings → Pages → Source = your branch.
2. Settings → Pages → *Custom domain* → `apex.navy`, then add the CNAME/A records
   at your registrar as GitHub instructs.

**Netlify** — netlify.com → drag the folder onto the "deploy" box → add domain.

## Wire up the domain
When you buy the domain (registrar/Cloudflare Registrar/Porkbun/etc.), point it at whichever
host above per that host's DNS instructions. No servers to run — it's just files.

## For the Google Play listing
After it's live, your **privacy-policy URL** is:

```
https://<your-domain>/privacy.html
```

Paste that into Play Console → App content → Privacy policy. That unblocks publishing.

## Editing
- **Rename the brand:** change the `APEX` wordmark near the top of `index.html`
  (and the `<title>`).
- **Add a project:** copy any `<article class="card"> … </article>` block.
- **Private/undecided projects** (the "sneak trap", the patient project) are stubbed in an
  HTML comment near the bottom of `index.html` — uncomment and fill in, or delete.
- **Contact email:** search for `hello@example.com` in both HTML files and replace it
  (or remove the line if you'd rather not list one).
