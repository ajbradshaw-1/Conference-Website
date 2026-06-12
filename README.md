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
| `WORKING PLACEHOLDER` | Conference name (5 spots listed in the comment)        |
| `Speaker TBA`         | Talk assignments as titles arrive                      |
| `Draft</span>`        | Remove pill when speaker list is locked                |
| `LOGO LICENSING`      | Swap Wikimedia logos for official assets               |
| `VENUE DISCREPANCY`   | Confirm Hyde Park Labs vs. Hyatt with PI               |
| `Tentative`           | Sophy hotel + discussion topics — confirm or delete    |
| `MODE TOGGLE`         | Conference History: fill 2 prior editions (Mode A)     |
| `CONFLICT FLAG`       | Unconfirmed remarks-speaker names — review pre-launch  |
| `MAP IMPLEMENTATION`  | Optional 3-pin My Maps upgrade path                    |

To edit: open the file in any text editor, change the text, commit on GitHub
(the pencil icon on the file page works — no git knowledge needed). Pages
republishes automatically in ~1 minute.

## Pre-launch checklist

- [ ] Confirm venue (Hyde Park Labs vs. Hyatt) — see VENUE DISCREPANCY flag
- [ ] Real conference name in all 5 spots; remove Placeholder pill
- [ ] Revert the 3 candidate-name TBA pills (Nadya/David A., Dusan/Tian/
      Shuolong, Quad Club dinner) to plain TBA unless confirmed
- [ ] Official logo files + Moore acknowledgment language from grant office
- [ ] Speaker list cleared for publication; remove Draft pill
- [ ] PI eyeballs speaker affiliations
- [ ] Confirm or delete Sophy hotel listing
