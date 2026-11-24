# Phrabbit

This repository contains the Phrabbit landing pages and versioned user guides for iPhone and iPad.

- [Published user manual](https://ki3240.github.io/phrabbit-guide/en)
- [Privacy policy](privacy-policy.html)
- [Maintaining versioned manuals](MAINTAINING.md)

## Pages deployment

The workflow runs on `main` in `ki3240/phrabbit-guide-dev` and
`ki3240/phrabbit-guide`. Set **Settings → Pages → Source** to **GitHub Actions**
in the repository being deployed. The workflow reads that repository's current
Pages URL at build time. The preview uses its project base path and sets
`noindex, nofollow` on HTML pages. Its sitemap has no indexable URLs and its
`llms.txt` omits the production directory. Production uses its GitHub project base
path until a custom domain is connected. After changing the domain, run the
workflow again on `main` to regenerate links and metadata. Configure a custom
domain in the production repository's Pages settings before pointing web DNS
at Pages. After connecting it, check redirects for the existing manual URLs
and check the host-root `robots.txt` and sitemap.

Set the repository variable `PAGES_SUPPORT_EMAIL` after the new address receives
mail. The site uses the existing support address until then.

To build locally, use Jekyll with the GitHub Pages gems. A normal Jekyll build
defaults to preview indexing rules. GitHub Pages builds the workflow artifact
with the environment values supplied by the workflow.
