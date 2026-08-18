# ReLU-TM Lab (GitHub Pages)

Static browser project. No Node.js/server required at runtime.

## Main pages
- `index.html` – entry page + automatic file listing
- `compile-tm.html` – text -> compact structured sparse ReLU-TM (`.tm.gz`), default budget 1 MiB
- `compile-general-tm.html` – finite multi-tape TM JSON -> exact sparse ReLU table model
- `run-tm.html` – loads and runs both model formats

## Included data
- `texts/goethe-faust.txt`
- `texts/alice-wonderland.txt`
- `texts/goethe-ein-gleiches.txt`
- precompiled Faust, Alice, poem and 5-tape PowerMod models in `machines/`

## GitHub Pages
Upload the CONTENTS of this repository folder, not the outer ZIP as one file. Then Settings -> Pages -> Deploy from a branch -> main -> /(root).

GitHub's normal web uploader does not unpack a ZIP into repository files automatically. Unzip locally first, then upload/commit the extracted files.
