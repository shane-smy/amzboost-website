# AMZ Boost website

Static marketing site for AMZ Boost — Amazon agency, Ipswich, Suffolk.

No build step. Plain HTML and one stylesheet, served straight from the repo root
by GitHub Pages. Edit a file, commit, and the live site updates within a minute.

## Pages

| File | Targets |
|---|---|
| `index.html` | Amazon agency UK |
| `services.html` | Amazon agency services UK |
| `amazon-account-management.html` | Amazon account management agency UK |
| `amazon-ppc-management.html` | Amazon PPC agency UK |
| `amazon-listing-optimisation.html` | Amazon listing optimisation UK |
| `amazon-profit-reporting.html` | Amazon profit reporting |
| `amazon-international-expansion.html` | Amazon international expansion |
| `results.html` | Case studies |
| `about.html` | About, local SEO for Ipswich / Suffolk |
| `insights.html` | Content hub |
| `contact.html` | Account review enquiries |

`styles.css` holds the whole design system. Brand colours are CSS custom
properties at the top of the file: ultramarine `#0e2096` and cyan `#00eafa`,
taken from the existing amzboost identity. Ledger green and oxblood are used
only on figures inside statement blocks, where they carry accounting meaning.

## Before launch

- Canonical URLs and `sitemap.xml` point at `https://www.amzboost.co.uk/`. While
  the site is on a `github.io` address those canonicals send search engines to
  the real domain, which is intended — no change needed until the domain moves.
- Blocks marked with a dashed border and a red tag need real content: client
  logos, case study narratives, quotes, team bios, contact details and the
  Amazon partner badge.
- The contact form has no backend. Formspree, Basin or a Cloudflare Worker will
  deliver it to an inbox.

## Custom domain

Add a `CNAME` file containing `www.amzboost.co.uk`, then point the DNS record at
GitHub Pages and enable HTTPS in the repository settings.
