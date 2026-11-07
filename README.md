# Clear Sky — website

One-page static site for Clear Sky, a first surface mirror cleaning service for flight simulators (Killeen, TX; nationwide).

No build step. `index.html` + `styles.css` + `images/`. Open `index.html` in a browser to preview.

## Files

| File | What it is |
|---|---|
| `index.html` | The whole page. Layout and colors are inline (exported from the design canvas). |
| `styles.css` | Base styles, focus states, FAQ arrows, and the phone/tablet breakpoints. |
| `images/` | Mike's four job-site photos. |
| `favicon.svg` | Tab icon. |

## Launch checklist

- [ ] **Domain** — buy at Cloudflare (Domain Registration). Candidates: clearskysim.com, clearskymirrors.com, clearskyvisuals.com.
- [ ] **Hosting** — Cloudflare Pages → Create project → Connect to Git → this repo. Framework preset: *None*. Build command: *(empty)*. Output dir: `/`. Then Custom domains → add the domain. Auto-deploys on every push to `main`.
- [ ] **Email** — Zoho Mail (Forever Free). Add the domain, create `contact@` and `mike@`, add `mike.<lastname>@` as an alias. Paste Zoho's MX / SPF / DKIM records into Cloudflare DNS.
- [ ] **Quote form** — sign up at formspree.io with `contact@`, create a form, copy its ID, and replace `[YOUR_FORM_ID]` in `index.html` (one place, search for it). Submissions arrive by email.
- [ ] **Email on the page** — replace `clearskycrew@outlook.com` (two places in `index.html`) with `contact@<domain>`.
- [ ] **Legal name** — once confirmed, add a footer line: *Clear Sky is a trade name of [Legal Name], a Texas limited liability company.*
- [ ] **Photos** — the two mirror shots are scans of prints. Swap in originals if Mike finds them (`images/before-after.jpg`, `images/clean-mirror.jpg`).

## Editing

Everything is plain HTML. Text changes: edit `index.html`, commit, push. Cloudflare redeploys in under a minute.

Decisions, removed content and the reasoning behind them are in the ClearSky project change log (Claude project doc `website-change-log.md`).
