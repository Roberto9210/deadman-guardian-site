# deadman-guardian-site

The public website for **deadman-guardian**, a NinjaTrader 8 add-on that enforces a personal daily loss
limit. The product repository is private; this repository holds only the site.

Four static pages, one stylesheet, no build step, no dependencies, no JavaScript except six lines on the
contact page that assemble one `mailto:` link. No fonts, images, trackers, analytics or cookies — the pages
load nothing from a third party.

| File | What it is |
|---|---|
| `index.html` | what the tool is, what it does **not** do, and the honest status banner |
| `compatibility.html` | the sixteen-firm table: every rule quoted verbatim and linked, written rulings marked as such |
| `how-it-works.html` | the seal, the ledger, fail-closed — with the limits from SPEC §17 on the same page |
| `contact.html` | one address, no form |
| `404.html`, `robots.txt`, `.nojekyll` | plumbing |

## Where the content comes from

Every claim here is derived from documents in the private repositories, and nothing on the site says
anything they do not:

- `deadman-research/LAUNCH/compatibility.md` and `sales_page.md`
- `deadman-research/FIRM_MATRIX.md` — the sixteen firms, each rule quoted with its source URL
- `deadman-research/FIRM_EMAILS.md` — the written-ruling requests and the replies received
- `deadman-guardian/SPEC.md` §17 (*what this does not protect against*), `README.md`, `nt/STEP3_FINDINGS.md`
  (measured platform behaviour) and `nt/soak/REMOJO_REPORT.md` (soak results)

**The rule for editing this site: no claim without a source in those documents.** If a firm's rule changes,
update `FIRM_MATRIX.md` first, then the page — and keep the retrieval date next to the quote.

Counts on the site are 4 allowed / 1 approval route / 4 asked and awaiting / 7 no — three of those seven
by written ruling (Tradeify and Alpha Futures, 2026-08-20; Take Profit Trader, 2026-08-21).

## Publishing

GitHub Pages, from the default branch, root folder. `.nojekyll` is present so files are served exactly as
committed. No custom domain is configured.

## Status

The tool is in testing: not released, no users, soak in progress on a simulated account. The status banner
on the home page says so and should not be softened before a full session has run on a funded account.

Built by Roberto Rodriguez — <https://github.com/Roberto9210>
