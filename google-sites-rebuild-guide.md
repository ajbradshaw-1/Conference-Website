# Google Sites Rebuild Guide
## Cavity Workshop site — transcribing the approved HTML into Google Sites

Use the hosted GitHub Pages version (or index.html in a browser) side-by-side
as the visual spec. Everything below maps each piece of the HTML site to the
specific Google Sites mechanism. Estimated total build time: 2–3 hours.

---

## 1. Site setup (10 min)

1. sites.google.com → **Blank site** (use the new Sites, not classic).
2. Site name: the working title — "Cavity Control of Quantum Materials
   [Placeholder]". Keep the literal "[Placeholder]" text until the PI
   confirms the real name; it serves the same purpose as the pill.
3. **Theme:** right panel → Themes → **Aristotle** (matches the lab wiki).
   Then Customize:
   - Primary color: custom → `#4A7194` (the steel blue). This drives link
     and heading accents.
   - Font: Aristotle's default thin sans is already close to the spec.
4. Create the 6 pages (Pages panel → +): Home, Schedule & Program, Speakers,
   Travel & Local Info, Sponsors, Conference History. Keep them flat (no
   nesting) — this becomes the top navigation automatically.
5. Settings (gear) → Navigation: **Top**, transparent off — the dark header
   bar comes from the banner styling below.

## 2. Hero banner on every page (15 min)

1. On each page, hover the header area → **Change image → Upload** →
   `hero-banner-2400x640.png` (in this package).
2. Header type: **Banner** (not "Large banner" — keep it shallow like the
   HTML version).
3. Title text in the banner: the page name. Click the title text → set to
   the largest heading size. Sites renders banner titles in white
   automatically over dark images.
4. Repeat for all 6 pages — same image, different title. This reproduces the
   "same banner, only the title changes" rule exactly.

## 3. Page-by-page content

Copy text directly from the HTML version in your browser (select + copy
renders cleanly into Sites). Per page:

### Home
- About paragraph: plain text block.
- "At a Glance": insert a **2-column layout**; left column bold labels
  (Dates / Venue / Hotel / Format / Attendance), right column values. Or a
  simple 5×2 table — both read fine.
- Confirmed speakers: one text block, the dot-separated name list, with a
  small-text caveat line ("Working invitation list — names may change…").
- Sponsors: see Sponsors page below; on Home use one centered text block
  "Gordon and Betty Moore Foundation — Primary Sponsor" (large text) above a
  3-column layout with the other three names. Swap names for logo images
  when official files arrive (Insert → Image).

### Schedule & Program
- Program-format bullets: standard bulleted list block.
- Each day: **Insert → Table**. Two columns (Time | Program). Recreate the
  row grammar:
  - Session header rows: bold both cells, light blue-gray cell background
    (table paint-roller tool → closest to `#F2F5F8`).
  - Talk rows: indent the program cell text (space or →) and use gray text.
  - Discussion rows: tint with the lightest blue background.
- TBA pills: Sites has no pill component. Convention: bracketed small caps
  — `[TBA]`, `[TBA: Nadya or David A.]`, `[Tentative]` — in the steel-blue
  text color. Document this convention on a private notes page (see §5).
- Print button: not reproducible. Replacement: generate a PDF of the
  schedule (print the HTML version's Schedule page to PDF using its print
  stylesheet) and add it as **Insert → Drive file** or an attachment link:
  "Download schedule (PDF)".

### Speakers
- Lede + the working-list caveat note: text blocks.
- The list: **2-column layout**, each column a text block; speaker name on
  one line, affiliation on the next line in gray small text, thin divider
  (Sites divider element) between entries — or simply paste the whole
  alphabetical list into two columns of plain text. Resist any urge to add
  photos; the spec forbids them.

### Travel & Local Info
- Venue + Hotels + transit sections: headings + paragraphs + bullets,
  straight transcription. Keep the `[Tentative]` marker on Sophy.
- Map: **Insert → Map** → search "5305 S Harper Ct, Chicago" → place. This
  is native in Sites (better than the iframe hack in the HTML version).
  Sites' map element supports one pin; for the 3-pin version create a
  Google My Map (My Maps → 3 pins: venue, Hyatt, Quad Club) and Insert →
  Embed → its share URL.

### Sponsors
- Moore block: centered section — small-caps "PRIMARY SPONSOR" line, then
  the Moore name in large light text linked to moore.org, on a light gray
  section background (section → change background → light gray ≈ #F6F8FA).
- Until official logo files arrive, keep text marks. When they arrive:
  Insert → Image, Moore's logo sized clearly larger than the other three.
- Reminder: acknowledgment language from the grant office goes here.

### Conference History
- Mode A: two placeholder entries as small text cards (single-cell tables
  or outlined sections). Fill year/name/host when the PI supplies them.

## 4. What is lost vs. the HTML version (accepted trade-offs)

- The exact faceted-SVG banner becomes a PNG (visually identical).
- TBA pills become bracketed colored text.
- Print stylesheet → replaced by an attached schedule PDF.
- Per-talk row styling is approximated with table cell colors.
- Custom footer → use Sites' footer: one line, "Workshop on [name] ·
  Oct 15–17, 2026 · Supported by the Gordon and Betty Moore Foundation."

## 5. Handover & workflow

- Create one unpublished page "EDITOR NOTES" (Pages panel → hide from
  navigation) and paste in the pre-launch checklist from the README plus
  the TBA-pill text convention. This replaces the HTML comments.
- Share the site as editor with: PI, Kristi, Cindy, and a continuing lab
  member. Ownership: transfer to the PI's or a lab Google account before
  you graduate — not your personal/student account, which may be
  deprovisioned.
- Publish settings: **Anyone** can view (public, no UChicago login), search
  visibility off (invitation-only event; no need to be indexed).
- Publish → choose the site address. A custom domain is possible later via
  Settings → Custom domains if the PI wants one.

## 6. Launch-day diff against the spec

Before announcing the URL, walk the GitHub Pages version and the Sites
version side by side, page by page, checking: all 6 pages present, banner
consistent, Moore most prominent on Home + Sponsors, schedule complete and
scannable, all remaining [TBA]s intentional, candidate names
(Nadya/David A./Dusan/Tian/Shuolong) removed unless confirmed, and the
venue question resolved.
