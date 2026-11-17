# nate-p.com: static rebuild

Plain HTML and CSS. Free to host on GitHub Pages or Cloudflare Pages. There's no build step.

The old Wix URLs keep working: `/resume`, `/projects`, `/contact` and `/post/<slug>` all have matching pages.

## 1. Contact form (free)

1. Sign up at formspree.io and create a form.
2. In `contact.html`, replace `YOUR_FORM_ID` with your form's ID. The free tier is enough for a portfolio.

## 2. Host on GitHub Pages

1. Create a repo, e.g. `Suraporn/nate-p.com`, and push this folder to it.
2. Go to Settings → Pages. Choose "Deploy from a branch", select `main`, then `/ (root)`.
3. Under Custom domain, enter `nate-p.com`. Add a `CNAME` file containing `nate-p.com`. Tick "Enforce HTTPS" once the option appears.

## 3. Move the domain off Wix (do this before it expires)

1. In Wix, go to Domains → nate-p.com. Unlock the domain, turn off auto-renew and get the transfer (EPP/auth) code.
2. In Cloudflare (free account), add the site `nate-p.com`. Then go to Domain Registration → Transfer and paste the code. Cloudflare charges the wholesale price, about $11/yr. The transfer includes one extra year.
3. In Cloudflare DNS, point the domain at GitHub Pages:
   - `A @` → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153 (set to **DNS only**, grey cloud)
   - `CNAME www` → `suraporn.github.io`
4. Cancel the Wix Premium plan only after the site loads at nate-p.com.
