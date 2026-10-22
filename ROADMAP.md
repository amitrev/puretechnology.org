# Roadmap: puretechnology.org

Deferred extensions. Each has a trigger — the condition under which it is worth doing — and nothing here is done before its trigger fires. The first version is the manifesto, the page and the signatures; that is complete without any of the items below.

## 1. Compliance badge
**What.** A small SVG ("Pure Technology") that a project puts on its site, linking back to the manifesto. Self-declared; no review, no registry.
**Why.** Spread and backlinks at zero cost; makes signing visible on the signatory's own product.
**Trigger.** The first signatory who is not the maintainer.
**Cost.** One SVG in the repo, light and dark variants, plus three lines in `CONTRIBUTING.md` with the embed snippet. One hour.
**Risk.** Cheap self-declarations. Acceptable: the badge says "we signed", not "we were checked".

## 2. Build step
**What.** Move signatories out of `index.html` into a Markdown or JSON file; a script renders the page; a GitHub Action runs it on push.
**Why.** Reviewing HTML in pull requests stops being tolerable past a certain volume.
**Trigger.** Signature PRs arrive faster than a few per week, or a malformed one breaks the page.
**Cost.** A 30-line script, one Action file. Half a day including testing.

## 3. Translations
**What.** Versions of the text in other languages, each on its own path, each clearly marked as a translation of the English original.
**Why.** Reach, and the text is short enough that volunteers will offer.
**Trigger.** Someone offers one. Do not commission.
**Cost.** Per translation: a review for fidelity and one more HTML file under the same constraints.
**Rule.** Only the English text is signed. Translations link to it.

## 4. Machine-readable declaration
**What.** A small specification — e.g. `/.well-known/pure-technology` or a `<meta>` tag — by which a site or service declares that it holds to the manifesto, so that an agent, browser or directory can read it.
**Why.** Turns the manifesto from a text into a signal that software can act on; fits a world where agents choose which services to use.
**Trigger.** A consumer exists or asks for it — an agent framework, a browser extension, a directory that wants to filter by it. Not before. A spec with no reader is a standard invented for oneself.
**Cost.** Low to write, high to get right: field names and semantics are hard to change once anyone reads them.

## 5. Criteria document
**What.** A separate document, built on the manifesto, that turns each principle into checkable conditions a product can be tested against.
**Why.** The manifesto is a position; some signatories will want a checklist. The second review of the text said exactly this: keep the manifesto short, put the standard elsewhere.
**Trigger.** Signatories ask how to check their own product, or two of them disagree about whether something complies.
**Cost.** The real one: this is where interpretation lives. Expect revisions.
**Rule.** The manifesto never changes to accommodate the criteria. The criteria change.

## 6. Independent verification
**What.** Some way for compliance to be assessed by someone other than the maker.
**Why.** Self-declaration has an obvious conflict of interest; the first analysis raised it.
**Trigger.** Item 5 exists and is being used, and a bad-faith badge has caused visible harm.
**Cost.** Unknown and probably not minimal. This is the one item that may never fit the project's resource constraint; recorded so it is not forgotten, not so it is done.

## Not planned
- A blog, news or commentary around the manifesto. It would need a schedule and a voice; the text does not.
- A directory of compliant products. Curation is a maintenance commitment and the badge covers the need.
- Analytics on the page. Visits can be read from the hosting provider's logs if ever needed.
