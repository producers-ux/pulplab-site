# Pulp Lab — Site

Static site for pulplab.com, hosted on GitHub Pages.

## Structure
- `index.html` — homepage (Lab Report masthead + one line, no more)
- `findings.html` — Findings page
- `work.html` — The Work (case studies: Microsoft/AWH, EVERFORTH/Mayo)
- `backissues.html` — Back Issues (archive THEN/NOW cards, links out to archive.pulplab.com)
- `services.html` — Work with the desk
- `styles.css` — shared stylesheet across every page
- `CNAME` — tells GitHub Pages this repo serves the custom domain pulplab.com

## Deploying
1. Push this repo to GitHub
2. Repo Settings → Pages → enable, source = main branch, root
3. Custom domain: pulplab.com (already set via the CNAME file, but re-enter it in the Pages settings if prompted)
4. At the domain registrar: A records for pulplab.com → GitHub's four IPs
   (185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153),
   CNAME for www → <username>.github.io
5. Once DNS resolves, enable "Enforce HTTPS" in Pages settings

## The old WordPress blog
Not migrated yet. Living at archive.pulplab.com (separate subdomain, separate
hosting, untouched). Back Issues page links out to it directly. Full migration
to Markdown + redirects is a post-Shoppe-Object project.

## To do next
- [ ] Swap ticker headlines for real live post titles once new content exists
- [ ] Swap Back Issues THEN/NOW card copy for exact dated permalinks pulled
      from the real WordPress export (current copy is paraphrased from
      fragments, not verified against the original posts)
- [ ] Full archive migration to Markdown, old URLs redirected
