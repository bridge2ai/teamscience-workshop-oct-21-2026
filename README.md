# Bridge2AI Team Science Workshop

Event page for the Bridge2AI Team Science Workshop (October 21, 2026, Rockville, MD). It has links to the slides and handouts for each module, with the module's facilitator, and lists the Teaming & Collaboration Working Group members who facilitated the workshop.

Site (once GitHub Pages is turned on): https://bridge2ai.github.io/teamscience-workshop-oct-21-2026/

It is a plain static site: `index.html`, `styles.css` and `assets/`. There is no build step.

## Updating a slide or handout link

The PDFs are hosted in the [workshop materials folder on Google Drive](https://drive.google.com/drive/folders/1zIO-xo890ca6Ru7bmvvbqpVBVsGO5-1Y), with one subfolder per module. Each **Slides** / **Handout** button on the module cards, and the **Slides & Handouts** button on the Full Workshop Deck card, links to the file's Drive URL:

```
https://drive.google.com/file/d/<FILE_ID>/view
```

To change one, find the button in `index.html` and replace its `href`. Every Drive file must be shared as **Anyone with the link → Viewer**, or visitors will be asked to request access.
## Previewing locally

Double-click `index.html` to open it in your browser. Or serve the folder:

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

## Publishing with GitHub Pages

1. Make the repository public (Settings → General → Danger Zone → Change visibility).
2. Settings → Pages → Build and deployment → Source: **Deploy from a branch**, Branch: `main`, folder `/ (root)`.
3. The site is served at https://bridge2ai.github.io/teamscience-workshop-oct-21-2026/ a minute or two after each push to `main`.

`.nojekyll` tells GitHub Pages to serve the files as they are, without running Jekyll.
