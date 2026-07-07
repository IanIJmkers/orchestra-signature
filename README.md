# Orchestra e-mailhandtekening

A static page where colleagues copy the Orchestra email signature and paste it into Outlook, then edit their own name, function, and phone number.

- **`index.html`** — the shareable copy page (this is what Vercel serves at the root).
- **`signature-source.html`** — the raw signature markup on its own, for reference.

## Deploy on Vercel

No build step — it's a static site.

1. Import this repo in Vercel.
2. Framework preset: **Other** (static).
3. Leave build command and output directory empty. Deploy.

Vercel serves `index.html` at the root URL. Share that URL with colleagues.

## Notes

- The font is **Averta** with Helvetica/Arial fallbacks — it only renders as Averta on machines that have the font installed.
- The logo is embedded as a base64 data URI. Classic Outlook for Windows (Word engine) can strip base64 images; if that happens, host the logo as an `https://` image and swap the `src`.
