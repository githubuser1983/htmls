# ReLU-TM Lab – mobile v2

Static GitHub Pages project. No Node.js/server required at runtime.

## Fixes in v2
- Text TMs are variable-order (1..N), so short prompts such as `Faust` or `Alice` no longer fail merely because they are shorter than the maximum context order.
- Unknown long contexts back off deterministically to the longest known suffix.
- Text compilation, general-TM compilation, and long TM execution run in Web Workers so the Chrome UI stays responsive on phones.
- PowerMod opens with its native five-tape example prefilled and can be stepped or run to HALT.

## Main pages
- `index.html`
- `compile-tm.html` – text -> compact variable-order sparse ReLU-TM, default budget 1 MiB
- `compile-general-tm.html` – finite multi-tape TM JSON -> exact sparse ReLU table model
- `run-tm.html` – generic runner for both formats

## GitHub Pages update
Upload the extracted files/folders into the repository root and choose overwrite/replace when GitHub reports same filenames. Commit the changes. The existing Pages deployment from `main` / root will redeploy automatically after the commit.
