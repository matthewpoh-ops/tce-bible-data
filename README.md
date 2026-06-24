# tce-bible-data

Static, lazy-loadable Bible data for The TCE Academy Bible reader (tceacademy.org/pages/bible).

- `bible-meta.json` — book list, per-chapter verse counts, attribution (loaded once on init, ~8 KB).
- `bible-book-<slug>.json` — KJV verse text + Treasury of Scripture Knowledge cross-references (packed `bookIndex.chapter.verse`, top 6 per verse) for one book. Loaded on book select.

## Sources & licensing
- **KJV** — King James Version (Authorized Version, 1611). Public domain.
- **Cross-references** — Treasury of Scripture Knowledge (public domain); data from openbible.info (CC-BY).
- **Commentary** (Matthew Henry, public domain) is fetched live from helloao.org and is not stored here.
- **ESV** is fetched live from the Crossway ESV API and is not stored here.

Served via jsDelivr CDN. Migratable to Shopify Files without code change (the reader reads a single base URL).
