# Pictogrammatica — exhibition build

The student app with the guided tour, served by GitHub Pages.

`index.html` is `Pictogrammatica_II.html` renamed. Nothing else is needed:
the app is one file, and `.nojekyll` tells Pages to serve it as it is.

## Publish

1. Upload `index.html`, `.nojekyll` and this README to the root of the repository
   (Add file → Upload files, then Commit).
2. Settings → Pages → Build and deployment → Source: **Deploy from a branch**;
   Branch: **main**, folder **/ (root)** → Save.
3. Wait a minute or two. The address appears at the top of the Pages settings:
   `https://<username>.github.io/<repository>/`

## Addresses worth knowing

- `…/` — the app. The tour opens by itself on a device's first visit.
- `…/?tour` — opens the tour every time. Use this one for a QR code, so a
  shared laptop shows the tour to each new visitor.
- `…/?pack=<url>` — loads a sentence pack from a URL (a file in this repository
  works: `?pack=mypack.json`). Combine with `&tour`.

## Updating

Upload the new `index.html` over the old one and commit. Pages republishes on
its own; a hard refresh (Ctrl/Cmd+Shift+R) shows the new copy.
