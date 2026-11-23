# Grand Line Elegance
### AO3 Work Skin · Sanji x Zoro palette

A dark, cinematic AO3 work-skin theme built around midnight navy, parchment, antique gold, muted crimson, and brushed silver. The design pairs a velvet-like reading surface with light document panels, giving story prose and in-universe artefacts distinct visual treatments.

> **Theme identity:** Grand Line Elegance  
> **Fandom-inspired palette:** Sanji x Zoro  
> **Format:** Standalone HTML preview with embedded CSS  
> **Primary wrapper:** `#workskin`  
> **Component namespace:** `.hgm-*`

---

## Design direction

The theme uses a dark navy reading environment with subtle layered gradients and fine texture. Opening and chapter panels sit against the dark background, while letters, diaries, emails, reports, transcripts, and other paper-based artefacts use parchment surfaces with dark ink for readability.

The overall mood is restrained and cinematic rather than brightly themed. Gold provides the principal highlight; crimson marks important details; silver adds a cool metallic counterpoint.

## Colour palette

| Colour | Hex | Intended use |
|---|---|---|
| Midnight navy | `#10121B` | Main page and dark surfaces |
| Slate navy | `#202333` | Panels, headers, and contrast surfaces |
| Warm parchment | `#E8DFC9` | Light document panels |
| Ivory | `#F0E5DC` | Main light text on dark backgrounds |
| Antique gold | `#D4AF62` | Highlights, links, ornaments |
| Aged gold | `#B99A52` | Borders and secondary metallic details |
| Muted crimson | `#A63D4F` | Accent borders, flags, emphasis |
| Deep wine | `#702F45` | Message bubbles and secondary accents |
| Brushed silver | `#C7D0D8` | Fine borders and cool metallic details |
| Pale metal | `#C5BBA8` | Outer frame and subtle separators |
| Forest green | `#243D32` | Limited legacy/variant accent |

The final Grand Line overrides take precedence over earlier component declarations. If you customise the palette, edit the final override section as well as any earlier component rules that you want to change.

## Components

The stylesheet uses reusable HTML classes. The preview demonstrates the components with sample content.

### Story structure

- `.hgm-open` — story opening/title panel.
  - `.hgm-open--minimal` — restrained opening treatment.
  - `.hgm-open--cinematic` — dark cinematic variation.
- `.hgm-chap` — chapter heading with number, title, subtitle, date, and optional epigraph.
  - `.hgm-chap--ornament`
  - `.hgm-chap--left`
  - `.hgm-chap--cinematic`
- `.hgm-sep` — section dividers.
  - `.hgm-sep--rule`
  - `.hgm-sep--ornament`
  - `.hgm-sep--dots`
  - `.hgm-sep--cine`
- `.hgm-mark` — narrative markers for POV, flashbacks, memories, time jumps, locations, and interludes.

### Narrative text

- `.hgm-n-std` — standard narrative block, with optional `.hgm-n-std--dropcap` and `.hgm-n-std--lead`.
- `.hgm-n-mono` — inset reflective or monologue-style passage.
- `.hgm-n-stream` — italic stream-of-consciousness passage.
- `.hgm-n-flash` — flashback passage; `.hgm-n-flash--memory` gives it a memory treatment.
- `.hgm-n-dream` — dream sequence.
- `.hgm-n-pov` — point-of-view and location label.
- `.hgm-n-quote` — featured quotation; `.hgm-n-quote--scripture` provides a left-aligned variant.
- Inline helpers: `.hgm-n-em`, `.hgm-n-soft`, `.hgm-n-loud`, `.hgm-n-strike`.

### Letters and communications

- `.hgm-letter` — letter, with sender, place, date, recipient, salutation, body, closing, signature, and postscript elements.
  - `.hgm-letter--formal` — formal letter treatment.
- `.hgm-diary` — journal or diary entry.
  - `.hgm-diary--fragment`
  - `.hgm-diary--aged`
  - `.hgm-diary--dark`
- `.hgm-mail` — email layout with metadata, subject, urgency flag, quoted text, forwarded message, signature, and legal note.
  - `.hgm-mail--urgent`
  - `.hgm-mail--chapter`
- `.hgm-sms` — text-message conversation with incoming/outgoing bubbles.
  - `.hgm-sms--dark`

### Documents and media

- `.hgm-doc` — formal report or institutional document, including stamps, metadata, tables, and signature lines.
  - `.hgm-doc--fraternity`
  - `.hgm-doc--file`
  - Stamp variants: `.hgm-doc__stamp--confidential`, `--restricted`, `--draft`, `--archived`.
- `.hgm-news` — newspaper or editorial article.
  - `.hgm-news--campus`
  - `.hgm-news--editorial`
- `.hgm-tx` — transcript, interview, or recorded conversation.
  - `.hgm-tx--readable`
  - `.hgm-tx--numbered`
  - `.hgm-tx--dark`
- `.hgm-skel` — case file, investigation record, profile, timeline, or evidence list.
  - `.hgm-skel--dark`
  - `.hgm-skel--archival`

### Author notes and inline utilities

- `.hgm-an` — author note panel.
  - `.hgm-an--open`
  - `.hgm-an--close`
  - `.hgm-an--chapter`
  - `.hgm-an--content`
  - `.hgm-an--research`
  - `.hgm-an--thanks`
- `.hgm-redact` — redacted text treatment.
- `.hgm-sc` — small-cap styling.
- `.hgm-field`, `.hgm-field__k`, `.hgm-field__v` — reusable key/value metadata rows.

---

## Installation on AO3

This HTML file is a **preview**, not the stylesheet to paste into AO3.

1. Open **AO3 → Skins → My Work Skins**.
2. Create a new Work Skin.
3. Copy the CSS from the HTML file's `<style>` section into the Work Skin CSS editor. Do not copy the `<style>` tags themselves.
4. Save the Work Skin.
5. Open the work you want to format and select the saved Work Skin in its **Work Skin** setting.
6. Add the relevant component HTML to the work's chapter or notes using AO3's HTML editor.

The HTML examples in the preview show the required class names and nesting. When using a component in a real work, replace the sample text with your own content while keeping the structural classes.

## Responsive behaviour

The stylesheet includes a breakpoint at `700px`. On narrower screens it reduces outer margins and padding, scales down prominent headings, stacks document signature fields, and adjusts metadata rows and message bubbles to fit smaller widths.

The CSS also constrains the work area, images, and tables to avoid horizontal overflow.

## Customisation

- **Change the overall atmosphere:** edit the final `body` and `#workskin` background rules.
- **Change the metallic accents:** update the gold and silver values in the final override sections.
- **Change the red accent:** update `#A63D4F` and `#702F45`.
- **Change paper panels:** update the shared light-panel rules for `.hgm-letter`, `.hgm-diary`, `.hgm-mail`, `.hgm-sms`, `.hgm-doc`, `.hgm-news`, `.hgm-tx`, and `.hgm-skel`.
- **Change typography:** edit the font stacks in the component rules. The theme uses system serif and sans-serif fonts, so no external font files are required.

Because the stylesheet contains multiple layers of component rules and later theme overrides, remember that later declarations can replace earlier ones. Keep related colour and contrast rules together when making substantial changes.

## Compatibility notes

- The CSS is scoped primarily under `#workskin` so the formatting is intended to affect the work content rather than the entire AO3 site.
- The standalone preview includes page-level styling for `body`; that outer-page appearance is for preview purposes. AO3 controls the surrounding site interface.
- The stylesheet uses conventional layout techniques and includes a mobile breakpoint. Still, check the saved Work Skin on AO3 desktop and mobile before using it on a long work.
- This file has not been independently verified against AO3's live rendering or current CSS restrictions. If AO3 rejects a declaration, remove or replace that declaration in the Work Skin stylesheet.

## File notes

`Theme Grand Line.html` combines the CSS and a full component sampler in one standalone HTML document. It is useful for previewing the visual system and copying component markup. For AO3 installation, extract the CSS from the `<style>` element and use the HTML snippets as the formatting templates.

---

*Grand Line Elegance · Sanji x Zoro palette*
