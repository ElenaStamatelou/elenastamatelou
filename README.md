# elenastamatelou.com — simple version

Temporary one-page site (November 2026). It will be replaced by the final website
(Learn / For researchers / Signatomics / Blog, see `ideas_future/10-product-map.md`).

## Contents
- `index.html` — the page: links to signatomics, the periodontitis questionnaire, LinkedIn and GitHub,
  plus a "Coming soon" note about the final website.
- `CNAME` — tells GitHub Pages to serve this at elenastamatelou.com.

## Links used
- signatomics: https://signatomics.elenastamatelou.com
- Periodontitis questionnaire: https://elenastamatelou.github.io/perio-screening-questionnaire-based-tool/
- LinkedIn: https://www.linkedin.com/in/elenistamatelou/
- GitHub: https://github.com/ElenaStamatelou

## Put it online (GitHub Pages, same as signatomics)
1. Create a public repo on GitHub, e.g. `ElenaStamatelou/elenastamatelou.com`, and push these files.
2. Repo → Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. In Cloudflare (DNS for elenastamatelou.com lives there), add, with proxy status **DNS only** (grey cloud):
   - four `A` records, name `@` → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `CNAME` record `www` → `elenastamatelou.github.io`
   (Keep the existing `signatomics` CNAME record as it is.)
4. Back in Settings → Pages, tick "Enforce HTTPS" once the certificate is ready.

## When the final website is ready
Replace this folder's content (or point the domain to the new site) and remove the "Coming soon" note.
