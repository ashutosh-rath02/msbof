# The Fundamentals of Business by Michael Scott

A page-turning 3D digital book (Three.js, no build step). Season 1 is released.

## Run locally

Open `index.html` in a browser, or serve the folder:

    npx serve .

## Add a chapter or season

Everything is data at the top of the script in `index.html`, inside the `BOOK` object.

- Replace a `{ t:'Title', soon:1 }` chapter with `{ t:'Title', pages:[ [blocks], [blocks] ] }`.
- Replace a season's `soon:1` with `chapters:[...]` to open a new season.
- Contents, page numbers, padding and the back cover update automatically.

Block types: `k` kicker, `h1`, `h2`, `p`, `c` centered, `m` maxim, `w` warning, `note` handwritten, `sp` spacer.

## Deploy

Static site, no build command. Import the repo in Vercel, leave the framework as "Other", and deploy.
