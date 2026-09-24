# Cavity Workshop Website — Deploy & Maintain

Single-file static site (`index.html`) — no build step, no dependencies.
`hero-banner-2400x640.png` is the exported hero banner for the Google Sites
rebuild (not used by index.html, which has the banner inline as SVG).

## Deploy to GitHub Pages (~10 minutes, one time)

1. Log in to github.com → **New repository**. Name it e.g. `cavity-workshop`.
   Public. Don't add any template files.
2. On the new repo page, click **uploading an existing file** and drag in
   `index.html`. Commit to `main`.
3. Repo **Settings → Pages** → under "Build and deployment", Source =
   **Deploy from a branch**, Branch = `main`, folder = `/ (root)`. Save.
4. Wait ~1 minute. The public URL appears at the top of the Pages settings:
   `https://<your-username>.github.io/cavity-workshop/`
5. Send that URL to anyone — no login needed to view.

## Making updates (for whoever inherits this)

Every anticipated update has an HTML comment next to it inside `index.html`.
Search the file for these markers:

| Search for            | To update                                              |
| --------------------- | ------------------------------------------------------ |
| `LOGO LICENSING`      | Swap Wikimedia logos for official assets               |
| `MODE TOGGLE`         | Conference History: prior editions (Mode A is live)    |
| `${TBA}`              | Remaining TBA slots (remarks, acknowledgment text)     |
| `VENUE PHOTOS`        | Venue photo sources, licenses, and how to swap them    |

To edit: open the file in any text editor, change the text, commit on GitHub
(the pencil icon on the file page works — no git knowledge needed). Pages
republishes automatically in ~1 minute.

## Pre-launch checklist

- [x] Confirm venue (Hyde Park Labs)
- [x] Real conference name in all spots; remove Placeholder pill
- [x] Revert candidate-name TBA pills to plain TBA
- [x] Speaker list cleared for publication; remove Draft pill
- [x] Confirm or delete Sophy hotel listing (removed; all guests at Hyatt Place)
- [x] Venue photos added (Wikimedia Commons + hydeparklabs.com, credited)
- [ ] Welcome remarks speaker (David invited, awaiting confirmation)
- [ ] Concluding remarks speaker
- [ ] Moore acknowledgment language from grant office (Sponsors page)
- [ ] Official logo files from Moore / UChicago / PME comms offices
- [ ] 2025 edition dates on Conference History page
- [ ] Official HPL meeting-space photo, if the venue provides one
- [ ] PI eyeballs speaker affiliations
- [ ] Remove "draft agenda" note from Schedule once program is final
