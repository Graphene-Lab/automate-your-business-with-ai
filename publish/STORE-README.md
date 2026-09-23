# Store-ready material and publishing notes

This folder holds the versions of the book prepared for distribution through
self-publishing and distribution stores, driven by **DistroBook**
(`https://github.com/Andrea-Bruno/DistroBook`).

## What is here

| File | What it is |
|---|---|
| `store/cover-ebook-1600x2400.png` | Ebook cover, 2:3 ratio, upscaled. Accepted by most ebook stores. |
| `store/cover-ebook-1600x2560.png` | Ebook cover, 1.6:1 ratio (KDP style), padded with a color sampled from the cover edge. |
| `../publish/*.pdf`, `../publish/*.epub` | The book itself, six languages. |

The original covers live in `../assets/` at 1024x1536. The `store/` copies are
resized because stores want a larger, separate cover image, sent on its own and not
embedded only in the book file.

## Cover requirements by store

| Store | Cover | Notes |
|---|---|---|
| Amazon KDP (ebook) | 1.6:1, min 1600x2560 | Use `cover-ebook-1600x2560.png`. |
| Kobo / Apple / most ebook stores | ~1.5:1, 1600x2400+ | Use `cover-ebook-1600x2400.png`. |
| Lulu / IngramSpark (print) | Full wraparound PDF (back + spine + front) | **Not generated.** A print cover must be designed per trim size; a front-only image is not enough. |

## How DistroBook is used

The manifest for this book is `DistroBook/manifests/ayb-en.json` (English edition).
Run from the DistroBook folder:

```bash
# Check the files
dotnet run --project src/DistroBook.Cli -c Release -- validate --config manifests/ayb-en.json

# Plan the publish, send nothing
dotnet run --project src/DistroBook.Cli -c Release -- publish --config manifests/ayb-en.json --dry-run --agent-mode
```

Other languages: copy `ayb-en.json`, change the `language`, the file paths, and the
cover, then repeat.

## Important constraints (read before publishing)

### 1. License allows commercial sale
The book is **CC BY-SA 4.0** (Attribution-ShareAlike, with **no** NonCommercial
clause). This is a free/libre license that **allows selling** — printed copies to
cover paper and printing, and the ebook at any price. Anyone who redistributes or
adapts it must give credit and share derivatives under the same license. The
manifest price is a normal retail price and can be changed freely.

### 2. ISBN (one per language AND per format)
Source: **Latvijas Nacionālā bibliotēka** (National Library of Latvia) — the ISBN
agency for Latvia. Cost: **3.00 EUR per title**, or an annual publisher
subscription (**15.00 EUR up to 10 titles**).

The ISBN rule is per **edition** and per **format**:
- Each language is a separate edition → its own ISBN.
- Each format (paperback, hardcover, EPUB, PDF) of the same edition → its own ISBN.

For this book in six languages:
- **Ebook only**: 6 ISBNs → 15 EUR subscription (cheaper than 6 × 3 = 18 EUR).
- **Ebook + paperback**: 12 ISBNs → use the subscription tier above 10 titles.

Getting the ISBN is a human step (apply at the National Library of Latvia, pay).
Once you have each ISBN, put it in the matching manifest (`isbn` field) and in
`secrets/ayb.json` under `isbn_plan`. Ebook-only stores can sometimes publish
without an ISBN using their own free ID.

### 3. Account registration is a human step
Every store needs a real account. Signup needs things an automated tool cannot do:
- Email verification (a link in your inbox) and CAPTCHA.
- Acceptance of the store's Terms of Service.
- A **tax form** (US W-8BEN for non-US authors) and **bank details** for royalties.

These are legally the author's to complete. DistroBook publishes to accounts that
already exist; it does not create them.

### 4. Live API endpoints are not yet verified
DistroBook is verified as a planner (dry-run, validation, orchestration). The real
publish endpoints for the "contact-only" stores (PublishDrive, Bookmundo, and
others) must be confirmed against each store's real API before a live run. Until
then, use `--dry-run`.

## Author data

The author's personal data and the pre-generated account passwords are kept in
`DistroBook/secrets/ayb.json`. That file is **gitignored** and never committed.
Fill in the registration email there before signing up.
