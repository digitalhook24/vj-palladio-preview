# VJ Palladio — Client Preview

Two new landing pages are ready for review:

1. **VJ Palladio Kothrud Central** — `vj-palladio-kothrud-central.html`
   Residential: 2 / 3 / 4 BHK premium apartments, Kothrud, Pune.

2. **VJ Indiwork Kothrud Central** — `vj-indiwork-kothrud-central.html`
   Commercial: smart office spaces (265–355 sq.ft.), Kothrud, Pune.

## How to open the preview

After the folder is hosted (e.g., on Netlify), the URLs will be:

- `https://<your-host>/vj-palladio-kothrud-central.html`
- `https://<your-host>/vj-indiwork-kothrud-central.html`

To open locally without hosting, just double-click either `.html` file.

## What works on the preview

- Full visual layout (desktop + mobile).
- All images, sliders, modals, accordions, sticky enquiry bar.
- WhatsApp and Call CTAs (links open WhatsApp / dialer normally).

## What will NOT work on a free static host (Netlify, GitHub Pages, etc.)

- **Enquiry form submissions.** The site uses a PHP mailer (`send.php` + `PHPMailer.php`) which only runs on a server with PHP. On a static preview host the form will appear to submit but won't actually deliver an email.
- This is **not** a bug — once the pages are deployed to the production server (which already runs PHP for the existing pages), forms will work exactly like the rest of the site.

## Quick-deploy options for a shareable URL

- **Easiest, no signup:** Open https://app.netlify.com/drop and drag this folder onto the page. You'll get a public URL valid for 24 hours instantly.
- **Persistent free URL:** Sign in to Netlify with a free account before dropping — the URL becomes permanent and renameable.
- **Production:** Upload these new files (`vj-palladio-kothrud-central.html`, `vj-indiwork-kothrud-central.html`, `images/kothrud-central/`, `images/indiwork-kothrud/`) to the existing production server via FTP / SFTP into the same folder as `index.html`. No CSS/JS changes needed — the shared `css/laviento/*` and `js/laviento/*` are reused.

## Sign-off

Please review both pages and reply with:

- ✅ Approved — proceed to production
- ✏ Changes — list any edits (copy, images, sections to add/remove)

Open items the developer flagged:

- **MAHARERA number for VJ Indiwork Kothrud Central** — the source page lists the same RERA (`PR1260002501660`) as Palladio Kothrud Central, which is likely an error. Please confirm the correct Indiwork RERA.
- Final phone number is currently `+91-9834352875` (used across the site). Confirm if Indiwork should use a different project-specific line.
