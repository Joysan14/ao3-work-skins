# Cranberry Kiss
### AO3 Work Skin and HTML Preview

**Cranberry Kiss** is a custom Archive of Our Own (AO3) Work Skin with a dark red-velvet reading surface, cranberry accents, rose-pink details, and brushed-metal framing. It pairs an editorial, archival atmosphere with a collection of reusable in-story layouts for letters, journals, messages, reports, transcripts, and other narrative inserts.

The package contains two complementary files:

- **`Theme Cranberries Kiss(1).css`** — the stylesheet to install as an AO3 Work Skin.
- **`Theme Cranberries Kiss(1).html`** — a standalone browser preview with the styling embedded and sample components.

## Design direction

The visual concept is **red velvet and brushed metal**. The outer reading area uses deep plum-burgundy with subtle layered gradients, fine metallic texture, inset framing, and a soft shadow. Warm ivory text is used on dark reading surfaces. Light inserts resemble pale paper, framed with rose-toned borders.

The stylesheet also includes a readability patch to keep story text legible on the dark chapter surface and dark plum text legible inside the light author-note panel.

## Colour palette

| Colour | Hex | Role |
|---|---|---|
| Deep plum / velvet | `#4A1A33` | Main reading surface and dark component variants |
| Cranberry | `#8C1D3B` | Strong accents, top borders, labels, and emphasis |
| Muted rose | `#A94A60` | Secondary accents, links, and decorative details |
| Warm ivory | `#FFF8F7` | Main text on dark surfaces and light paper panels |
| Rose pink | `#E8A5AE` | Borders, fine rules, and soft highlights |
| Brushed silver | `#D6C5D1` | Metallic frame and subtle separators |
| Pale blush | `#F4DADA` | Light table headers and selected soft surfaces |

## Typography

The theme uses system-safe font stacks rather than depending on externally hosted fonts.

- **Georgia / Palatino** for titles, chapter headings, and editorial details.
- **Times New Roman** for narrative passages, letters, and diary entries.
- **Arial** for labels, metadata, and interface-like elements.
- **Courier New** for timestamps, references, transcripts, and archival metadata.

If a preferred font is unavailable on a reader's device, the browser falls back to the next font in the stack.

## Component catalogue

The stylesheet uses the `hgm-` class namespace. The HTML preview demonstrates the component styles and their intended use.

| Component | Main class | Purpose |
|---|---|---|
| Opening title card | `.hgm-open` | Story title, subtitle, epigraph, dedication, and publication-style metadata |
| Chapter heading | `.hgm-chap` | Chapter number, title, subtitle, date, and epigraph |
| Scene separators | `.hgm-sep` | Rules, ornaments, dotted dividers, and cinematic separators |
| Narrative markers | `.hgm-mark` | Flashbacks, memories, time jumps, locations, POV changes, and interludes |
| Narrative text treatments | `.hgm-n-*` | Standard prose, monologue, stream of consciousness, flashbacks, dreams, POV labels, and quotations |
| Letters | `.hgm-letter` | Personal correspondence, formal letters, letterheads, and signatures |
| Diary entries | `.hgm-diary` | Dated journal entries, private notes, margin annotations, and fragments |
| Email | `.hgm-mail` | Sender/recipient fields, subject lines, urgent flags, quoted replies, forwarded messages, and signatures |
| SMS messages | `.hgm-sms` | Contact header, date, incoming and outgoing message bubbles, and timestamps |
| Documents | `.hgm-doc` | Official records, forms, reports, tables, stamps, and signature blocks |
| News articles | `.hgm-news` | Newspaper mastheads, headlines, bylines, datelines, article text, pull quotes, and information boxes |
| Transcripts | `.hgm-tx` | Dialogue transcripts, speaker labels, timestamps, pauses, notes, and numbered lines |
| Case files and records | `.hgm-skel` | Profiles, timelines, case records, inventories, annotations, and archival-style layouts |
| Author notes | `.hgm-an` | Opening, closing, chapter, content, research, and thank-you notes |
| Redaction | `.hgm-redact` | Visually concealed text in document-like inserts |
| Small caps | `.hgm-sc` | A compact typographic emphasis treatment |

### Variants

Several components include modifier classes for alternate presentations. Examples include:

- `.hgm-open--minimal` and `.hgm-open--cinematic`
- `.hgm-chap--ornament`, `.hgm-chap--left`, and `.hgm-chap--cinematic`
- `.hgm-diary--fragment`, `.hgm-diary--aged`, and `.hgm-diary--dark`
- `.hgm-doc--fraternity` and `.hgm-doc--file`
- `.hgm-news--campus` and `.hgm-news--editorial`
- `.hgm-tx--readable`, `.hgm-tx--numbered`, and `.hgm-tx--dark`
- `.hgm-skel--dark` and `.hgm-skel--archival`

Use the base class together with the modifier class. For example:

```html
<div class="hgm-open hgm-open--cinematic">
  ...
</div>
```

## Installation on AO3

1. Open **AO3 → My Dashboard → Skins**.
2. Select **Create Work Skin**.
3. Give the skin a name, such as **Cranberry Kiss**.
4. Open `Theme Cranberries Kiss(1).css` in a text editor.
5. Copy the complete CSS and paste it into the Work Skin CSS field.
6. Save the Work Skin.
7. Open the Work Skin's preview, then apply it to a test work to check the result.
8. In the work's **Associations** or **Post** settings, select the saved Work Skin where AO3 provides the option.

The HTML preview is **not** the file to paste into AO3. Install the `.css` file. The `.html` file is for viewing the design in a regular browser.

## Using the HTML preview

Open `Theme Cranberries Kiss(1).html` in a modern browser. It is a standalone preview, with its CSS embedded in the document and sample markup included.

Use it to inspect the visual treatment and compare component variants before adding the corresponding HTML to an AO3 work. The preview is a demonstration page, not an AO3 upload file.

## Mobile and responsive behaviour

The stylesheet includes a mobile breakpoint at **700px**. At narrower widths it:

- reduces the outer reading-area margins and padding;
- reduces the size and spacing of title treatments;
- adjusts the padding of letters, diaries, emails, documents, news panels, transcripts, and case files;
- allows document signature blocks to stack vertically;
- changes selected metadata fields from floated columns to stacked labels and values; and
- constrains component widths and allows long text to wrap.

The CSS also limits images and tables to the available reading width to reduce horizontal overflow.

## Readability and contrast

The theme is designed around two main reading contexts:

- **Dark chapter surface:** story prose, chapter headings, narrative treatments, and markers use warm ivory text.
- **Light insert panels:** letters, diary entries, emails, documents, news panels, transcripts, case files, and author notes use dark plum text.

The final readability overrides are important. If you customise colours, preserve this contrast relationship rather than changing text and background colours independently.

## Customisation notes

- Change the palette by updating the colour values in the CSS, including the later override sections. Later rules can take precedence over earlier declarations.
- Keep the `hgm-` class names intact when using the supplied component HTML.
- Keep the outer `#workskin` scoping for AO3 compatibility.
- When adding a new component to a work, copy its matching HTML structure from the preview and replace only the sample content.
- Test changes on both desktop and mobile layouts.
- Avoid relying on external fonts or scripts for core presentation.

## File contents

| File | Description |
|---|---|
| `Theme Cranberries Kiss(1).css` | AO3 Work Skin stylesheet, including the component system, red-velvet visual overrides, mobile adjustments, and readability corrections |
| `Theme Cranberries Kiss(1).html` | Standalone HTML preview with embedded styling and sample markup |

## Credits and use

This is a custom fan-created styling resource for AO3 works. It is not an official AO3 theme or an AO3 product. Adapt the sample text and component content to suit your own work.

---

*Theme: Cranberry Kiss · Style direction: Red Velvet + Brushed Metal · Platform: Archive of Our Own*
