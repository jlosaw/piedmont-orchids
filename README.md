# Piedmont Orchids — collection explorer prototype

A working static site for GitHub Pages: searchable/filterable collection cards, plant profiles, and expandable parentage trees. No hosting fees or database server required.

## Preview locally

From this directory run `python -m http.server 8000` and open http://localhost:8000. Double-clicking `index.html` will not work in many browsers because the site loads `plants.json` using fetch.

## Publish free with GitHub Pages

1. Create a **public** GitHub repository, for example `piedmont-orchids`.
2. Upload the contents of this folder to the repository root.
3. In repository **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. The site will appear at `https://YOUR-USERNAME.github.io/piedmont-orchids/` after GitHub builds it.

## Current scope and data limitations

- **44 verified-ID sample records** from the conversation, not a full import of the 101-plant catalog.
- **39 actual archived images**, resized for the web. Some earlier catalog photos were unavailable or not confidently mapped to an ID; those entries show a placeholder.
- The full 101-plant catalog and all historical photographs have **not** been reconstructed in this prototype.
- Missing parents are shown as unknown. Parentage that the owner distrusts is flagged in notes.
- Some historic names/registrations/awards remain unverified. Do not interpret this demo as an RHS-authoritative reference.
- Virus status is included as requested. **IMPORTANT: it is currently visible on the public plant profile.** Remove this field from public profiles before publishing if you want it private.
- `plants.json` is the source of truth for the prototype. Add records by copying the same field structure and putting photos in `assets/`.

## Next enhancements

Full import with source-of-truth catalog review, multiple photos per plant, true recursive ancestor lookup from an independently verified RHS pedigree dataset, photo-date bloom calendar, breeding project pages, private maintenance data, and a lightweight editing interface.
