# LE-RELAX UK — trade website

A static website (plain HTML/CSS, no build step) for UK trade customers, ready for GitHub Pages.
English (en-GB) only. Separate from the Hong Kong site at le-relax.co.

| URL | Page |
|---|---|
| `/` | Home |
| `/products/` and `/products/<range>/` | Full range, 11 product pages |
| `/glass/`, `/about/`, `/trade/` | Glass processing · About · Trade supply |
| `/quote/` | Quick quote: builds an email to the UK team |
| `/contact/` | UK contact, factory and showrooms |
| `/guides/` | Buyer's guides (4 articles) |
| `/privacy/` | Privacy policy (UK GDPR wording) |

## Still to fill in (marked in square brackets on the site)

`[UK phone]`, `[UK email]`, `[UK trade counter address]`, `[Opening hours]`.
Send these to Claude and the site is rebuilt with them everywhere: header button, footer,
contact page, quick quote, enquiry buttons on every product page and the phone action bar.
If the UK team will use WhatsApp, send the UK WhatsApp number too and the buttons switch to WhatsApp.

## Domain (not decided yet)

The site works on any address. Until the domain is chosen, the canonical tags, sitemap and
Google structured data are left out on purpose. Once you pick it (for example `le-relax.co.uk`),
ask Claude to rebuild with the domain: those are added, plus a `CNAME` file for GitHub Pages.

## Put it on GitHub

1. Create a new **public** repository, e.g. `le-relax-uk`.
2. **Add file → Upload files** in two goes (the uploader takes 100 files at a time):
   1. Everything **except** the `assets` folder (about 47 files, including the `media` folder (factory video) and `docs` folder (catalogues)). Commit.
   2. The `assets` folder itself (89 files). Commit.
3. **Settings → Pages**: deploy from branch `main`, folder `/ (root)`.

## Notes

- **Cookie banner (UK law):** Google Analytics runs in Consent Mode. No analytics cookies are set until a visitor taps Accept; the choice is remembered on their device.

- Google Analytics uses the same tag as the Hong Kong site. In Google Analytics you can add this site as a
  second web data stream, or create a separate property for the UK and send Claude the new ID.
- The factory video (`media/factory-reel.mp4` and `.webm`, about 4 MB each) only loads when a visitor scrolls to it,
  and does not autoplay for people who have turned off motion or data saving.
- Window and door pages carry a "For UK projects" note: external windows and doors must meet UK Building Regulations.
