# BNHR Training Tools

Small tools for running a training session, published with GitHub Pages at https://bnhr.xyz/training-tools/.

## Layout

One folder per tool, named after the tool, so its address is `https://bnhr.xyz/training-tools/<folder>/`. Tool folders carry no date, unlike workshops, because a tool is used again and again. Each folder is self-contained, with its own fonts, logos and icon, so a change to one tool or to the brand never changes another.

| Folder | Tool |
|---|---|
| `voluntold/` | Voluntold: picks a name at random from a list typed, pasted or loaded from a `.txt` file, keeps the picked names out of the draw, and lists who has been picked. Enter or Space picks when the cursor isn't in the names. First made for the Learn Geospatial Data Management and Engineering course (`tools/voluntold.html` there) |

`index.html` lists the tools: add a line there for each new folder. `assets/` holds the index page's logos, icon and fonts. `.nojekyll` tells GitHub Pages to serve the files as they are.

## Brand

The pages use the BNHR 2026 brand: the core-light colorway, or core-dark when the system is set to dark; a navy header with the horizontal logo; Albert Sans 800 headlines in sentence case with the orange highlight block; Atkinson Hyperlegible Next text and Atkinson Hyperlegible Mono labels; and the straight footer band with the square logo, `bnhr.xyz` and the tagline. Fonts, logos and colors are copied from the brand's web kit (`branding/web-2026`): each folder's `fonts.css` keeps only the faces its pages use. Copy them again from the kit when it changes, and never edit a copy.

## Privacy

The tools run in the browser and send nothing anywhere: no accounts, no analytics of their own, and no requests outside this site. Every repository on `bnhr.xyz` shares the browser's storage, so a tool that saves anything in the browser uses a key that starts with `training-tools/<folder>/`. Voluntold saves nothing: its names go when the page closes.

## Publishing

Pushes to `main` publish the site (Settings → Pages → Deploy from a branch: `main`, root). The site takes the `bnhr.xyz` custom domain from the main site, `benhur07b.github.io`, so it needs no CNAME file of its own; add `training-tools` to that site's `reserved-paths.json`.
