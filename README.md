# JFFI Monthly Newsletter Template

A reusable browser preview and production-safe HTML email for Jesus Foundation Family International. The design uses a JFFI-aligned palette: deep navy, royal blue, ministry gold, warm white and clear neutral text.

## Files

- `index.html` is the polished browser preview. It includes Desktop/Mobile preview controls and the complete monthly content structure.
- `styles.css` contains the browser-only responsive design system.
- `newsletter-email.html` is the email-safe version for Gmail, Outlook, Apple Mail and Mailchimp workflows. It is JavaScript-free, web-font-free, table-based, and keeps critical styles inline with a small mobile media query.
- `assets/` contains named placeholders for supplied or approved imagery.

## Preview

Open `index.html` directly in a browser, or run a local static server from this folder, for example:

```text
python -m http.server 8000
```

Then visit `http://localhost:8000/`. Open `newsletter-email.html` separately to inspect the production markup.

## Monthly updates

In both HTML files, search for `ACL:` and the bracketed placeholders. Update the month, hero theme, introduction, verse, reflection, pastoral message, event cards, announcement, testimony and image references. The persistent links are listed in the opening comment of `index.html`; confirmed URLs should not be replaced with `#`.

Replace the files in `assets/` with approved images while keeping the organised filenames: `jffi-logo.png`, `hero-worship.jpg`, `pastor-chibuzor.jpg`, `event-1.jpg`, `event-2.jpg`, `event-3.jpg`, and `testimony.jpg`. Add meaningful `alt` text when adding real images. The current preview uses accessible, local CSS placeholders so it does not hotlink imagery.

## Testing and sending

Check every CTA in a browser, especially the Zoom, website, social, `tel:` and `mailto:` links. Preview at 320px, 375px, 768px and desktop widths and look for overflow. Send `newsletter-email.html` to a test list before publishing, checking Gmail web/mobile, Outlook and Apple Mail.

HTML email support varies. Avoid relying on JavaScript, web fonts, CSS grid, flexbox or background images in the production file. Outlook may render some spacing and font details differently. For Mailchimp, paste the contents of `newsletter-email.html` into a custom HTML/code block or import it as a template, then replace the unsubscribe and preferences placeholders with Mailchimp's merge tags before sending. Do not send the literal placeholders in a live campaign.

## Theme colors

- Deep navy: `#071C35`
- Royal blue: `#1456A0`
- Ministry gold: `#D8A84E`
- Warm white: `#F7F4EC`
- Neutral text: `#172331`
