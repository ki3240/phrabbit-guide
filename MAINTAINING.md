# Maintaining versioned manuals

- Root locale pages and `/versions/4.2.0/<locale>.html` include the same source
  from `_includes/manuals/4.2.0/`. Edit that source once for the current guide.
- `_includes/manuals/4.1.0/` and `versions/4.1.0/` are the released 4.1.0 manual
  (published `e63d51f`); leave them unchanged.
- `versions/4.0.0/` preserves the five released locale sources and their 46
  referenced screenshots byte-for-byte from commit `45d90b7`. Its page version
  comes from `_config.yml` defaults, so the original front matter stays intact.
- `_data/guide_versions.yml` controls selection order and the current guide.
  `_data/guide_ui.json` localizes the current/past version labels.
- Dev shows the final publication display: the current guide is labeled
  “Published” and older guides “Previous version”. There is no preview status
  or preview notice; publication timing is controlled by which remote is used.
- 4.2.0 is published: `origin/main` and `dev/main` both serve it (released
  2026-11-12, `51bc624`). Prepare the next version on `dev/main` only and push
  origin only after that app version is approved; existing Support URLs stay
  unchanged and versioned URLs remain available.
- For the next guide version, add its include sources, wrapper pages and
  version-local images, point root wrappers at it, and add its version entry.
  Retain the previous version's source and assets. Bug-fix-only releases with
  unchanged usage do not require a separate manual.
- Verify all five languages on root and versioned URLs, version/language links,
  images, section anchors, search, mobile contents, light and dark appearance.
  The existing `privacy-policy.html` remains the current policy for all versions.
