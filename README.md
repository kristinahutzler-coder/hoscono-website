# HOSCONO Insights — Website

Fractional CFO practice website for Kristina van den Berg-Hutzler.

## Pages

| File | URL | Description |
|------|-----|-------------|
| `index.html` | `/` | Homepage — hero, challenge, service selector, logo bar |
| `about.html` | `/about` | About page — bio, career, assignments, human section |
| `contact.html` | `/contact` | Contact page — form, details |

## Assets

| File | Used in |
|------|---------|
| `assets/portrait.jpg` | Homepage hero, About hero, Contact hero |
| `assets/family.jpg` | About — "Beyond the finance function" section |

## Deploy to Vercel (5 minutes)

1. Push this folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → New Project → Import your repo
3. Framework: **Other** (static HTML — no build step needed)
4. Root directory: `/` (leave as default)
5. Click Deploy

That's it. Vercel auto-deploys on every push to main.

## Connect your domain

1. In Vercel → Project → Settings → Domains
2. Add `hosconoinsights.com` (or your chosen domain)
3. Vercel gives you DNS records to add in Transip
4. SSL certificate is automatic

## Contact form

The form in `contact.html` needs a form handler. Recommended: **Formspree**.

1. Go to [formspree.io](https://formspree.io) → create a free account
2. Create a new form → get your form endpoint (e.g. `https://formspree.io/f/xabcdefg`)
3. In `contact.html`, find the `<form>` tag and add:
   ```html
   <form action="https://formspree.io/f/YOUR_ID" method="POST">
   ```
4. Add `name` attributes to each input field (required for Formspree to label them)

## Customise

- **Brand colours**: in `style.css` under `:root`
- **Copy**: edit directly in the HTML files
- **Logo text**: search for `HOSCONO` across all files
- **Photos**: replace `assets/portrait.jpg` and `assets/family.jpg` with new files (keep same names)

## Open items before launch

- [ ] Final brand name (HOSCONO Insights or Konekta) — update all `<title>` tags and nav
- [ ] LinkedIn URL — replace `linkedin.com/in/kristinavandenberqhutzler` in contact.html
- [ ] Formspree endpoint — wire up the contact form
- [ ] Client logo permissions — add real SVG logos to the logo bar in index.html
- [ ] Domain registration on Transip

