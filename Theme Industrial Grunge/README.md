# Industrial Grunge — AO3 Work Skin

A dark, industrial-inspired AO3 work skin with a restrained palette of charcoal, weathered steel, warm paper, and muted rust. It combines a cinematic reading surface with a large set of reusable story, communication, and in-world document components.

The companion HTML file, **`Theme Industrial Grunge.html`**, is a standalone browser preview and component sampler. The CSS file, **`Theme Industrial Grunge.css`**, is the stylesheet intended for the AO3 Work Skin editor.

## Design direction

The theme contrasts a charcoal industrial surround with warm, pale reading panels. Fine grid-like background lines, inset shadows, narrow borders, and restrained rust accents create a worn, archival atmosphere without making the story text difficult to read.

### Colour palette

| Role | Colour | Hex |
|---|---|---|
| Main background | Charcoal | `#242729` |
| Deep charcoal | Near-black | `#171A1C` |
| Slate | Industrial slate | `#41484B` |
| Mid grey | Weathered grey | `#777D7D` |
| Soft grey | Steel grey | `#A3AAA7` |
| Pale metal | Light grey | `#C1C5C1` |
| Main paper | Warm off-white | `#F2F0E9` |
| Secondary paper | Pale grey-green | `#E8E8E2` |
| Light paper | Soft ivory | `#F8F7F2` |
| Aged paper | Warm beige | `#EDE8D9` |
| Rust accent | Muted rust | `#98634D` |
| Gold accent | Industrial gold | `#C5A34A` |
| Highlight | Pale gold | `#EBE0BC` |
| Blue accent | Muted blue | `#526B82` |
| Positive status | Muted green | `#596B54` |

## Files

- **`Theme Industrial Grunge.css`** — the AO3 Work Skin stylesheet. Copy its CSS into the AO3 Work Skin editor.
- **`Theme Industrial Grunge.html`** — a standalone HTML preview. It embeds the stylesheet and demonstrates the components with sample content. Open it in a browser to inspect the appearance.

The HTML preview is not the file to paste into AO3. The CSS file is the stylesheet; the HTML examples are reusable markup snippets for the body of an AO3 work.

## Installation on AO3

1. Open **Dashboard → Skins → My Work Skins**.
2. Choose **Create Work Skin**.
3. Give the skin a name, such as *Industrial Grunge*.
4. Open `Theme Industrial Grunge.css` in a text editor and copy the stylesheet contents.
5. Paste the CSS into the Work Skin CSS field and save.
6. Open the AO3 work you want to style and select **Industrial Grunge** under its Work Skin setting.
7. Save or preview the work.

To use the special components, copy the relevant HTML structure from the preview or your component snippets into the work's HTML editor. Keep the class names unchanged unless you also update the CSS.

## Layout and reading experience

- The outer work area uses a charcoal background with subtle horizontal and vertical texture.
- The preface, chapter content, and afterword sit on warm off-white panels with a fine inset border.
- Main story text uses a Georgia/Palatino serif stack with generous line spacing.
- The title uses a display serif stack; chapter headings use a separate Baskerville-style stack.
- Links use the muted rust accent.
- Mobile overrides reduce outer and inner padding, scale down large headings, widen chat bubbles, and stack selected metadata and signature elements.

## Component guide

The stylesheet contains general typography and story formatting, communication mock-ups, and dossier/document styling. The HTML preview acts as a visual catalogue of these elements.

### Story structure and typography

| Class | Purpose |
|---|---|
| `.do-title` | Large standalone story title |
| `.do-subtitle` | Italic subtitle beneath a title |
| `.do-epigraph` | Centered epigraph with attribution |
| `.do-meta`, `.do-chip` | Metadata list and compact tags |
| `.do-chapter` | Chapter heading wrapper |
| `.do-chapter-num` | Small uppercase chapter number |
| `.do-chapter-title` | Chapter title |
| `.do-chapter-sub` | Optional chapter subtitle |
| `.do-chapter-orn` | Decorative chapter marker |
| `.do-book` | Book-style paragraph indentation |
| `.do-justify` | Justified story paragraphs |
| `.do-dialogue` | Dialogue paragraph spacing |
| `.do-thought`, `.do-th`, `.thought`, `.thought-plain` | Thought and italic-aside styles |
| `.do-thought-bar` | Thought passage with a rust-coloured left rule |
| `.do-dropcap`, `.do-lead` | Drop cap and small-cap opening |
| `.do-pov`, `.do-tag` | Point-of-view and scene labels |
| `.do-flashback`, `.do-memory`, `.do-dream` | Flashback, memory, and dream passages |
| `.do-pull` | Centered pull quote |
| `.do-break`, `.do-break-dots`, `.do-break-tide`, `.do-break-line` | Decorative scene breaks |
| `.do-note`, `.do-note-title`, `.do-endnotes`, `.do-footnotes` | Notes and footnote areas |
| `.do-warn`, `.do-warn-title` | Content warning panel |
| `.do-disclaimer` | Small uppercase disclaimer |
| `.do-letter`, `.do-sig` | Letter and right-aligned sign-off |
| `.do-diary`, `.do-date` | Diary entry and date label |
| `.do-poem`, `.do-poem-title` | Narrow poem layout |
| `.do-frame` | Framed passage |
| `.do-center` | Centered text helper |
| `.do-lh` | Industrial-style local heading with optional small subheading |
| `.do-hl`, `.do-hl-sea` | Inline highlight treatments |
| `.do-fnref` | Superscript-style footnote marker |

### Messages and digital interfaces

| Class | Purpose |
|---|---|
| `.do-chat` | Chat conversation panel |
| `.do-chat-head`, `.do-chat-body` | Chat header and message area |
| `.do-day` | Date divider |
| `.do-msg`, `.do-out` | Incoming and outgoing message bubbles |
| `.do-sender`, `.do-s2`, `.do-s3` | Sender labels and alternate sender colours |
| `.do-time`, `.do-tick`, `.do-typing` | Message time, delivery marks, and typing indicator |
| `.do-wa` | WhatsApp-style chat variation |
| `.do-secure` | Secure-channel chat variation |
| `.do-post` | Social-media post card |
| `.do-avatar`, `.do-name`, `.do-handle` | Post identity elements |
| `.do-post-body`, `.do-post-stats` | Post content and engagement line |
| `.do-email` | Email card, including nested replies |
| `.do-email-head`, `.do-email-body` | Email header and body |
| `.do-k`, `.do-v`, `.do-email-subject` | Email metadata labels and values |
| `.do-notify` | Dark notification card |
| `.do-system` | Monospaced system/status message |
| `.do-call`, `.do-missed` | Call notification and missed-call label |
| `.do-voice`, `.do-wave` | Voice-message card and waveform-like text |
| `.do-radio`, `.do-ts`, `.do-cs` | Radio/transmission log and timestamp/callsign labels |
| `.do-bank` | Bank transaction or alert card |
| `.do-bank-alert`, `.do-bank-dark` | Bank alert and dark variants |
| `.do-bank-cr`, `.do-bank-dr` | Credit and debit amount treatments |

### Organisations, records, and official documents

| Class | Purpose |
|---|---|
| `.do-banner` | Large organisation banner |
| `.do-banner-blue`, `.do-banner-red`, `.do-banner-black` | Banner colour variants |
| `.do-banner-name`, `.do-banner-tag`, `.do-banner-est` | Banner name, tagline, and establishment line |
| `.do-brand` | Compact organisation/brand strip |
| `.do-brand-blue`, `.do-brand-red` | Compact brand colour variants |
| `.do-brand-mark`, `.do-brand-body`, `.do-brand-name`, `.do-brand-tag`, `.do-brand-ref` | Brand mark, identity, and reference details |
| `.do-doc` | General document panel |
| `.do-doc-label`, `.do-doc-title`, `.do-docmeta`, `.do-ref`, `.do-sect` | Document labels, title, metadata, reference, and section heading |
| `.do-d-brief`, `.do-d-casualty`, `.do-d-chain`, `.do-d-corr`, `.do-d-field`, `.do-d-incident`, `.do-d-intel`, `.do-d-interrog`, `.do-d-inv`, `.do-d-medical`, `.do-d-personnel`, `.do-d-service` | Document border/background variants |
| `.do-dossier` | Definition-list dossier layout |
| `.do-photo` | Placeholder/photo block in a dossier |
| `.do-status`, `.do-status-open`, `.do-status-hold`, `.do-status-closed` | Record status labels |
| `.do-redact`, `.do-redact-name`, `.do-redact-block` | Inline, name-level, and block redaction |
| `.do-missing` | Missing-record marker |
| `.do-chainlist` | Chain-of-custody or event list |
| `.do-dist` | Distribution line |
| `.do-class` and `.do-class-*` | Document classification bars |
| `.do-stamp` and `.do-stamp-*` | Compact status/classification stamps |
| `.do-sign`, `.do-sign-blue`, `.do-sign-red` | Script-like signature text |
| `.do-signature`, `.do-signature-line`, `.do-signature-entry`, `.do-signature-sheet` | Signature blocks and signature sheet |
| `.do-news`, `.do-dateline` | News-style document and dateline |
| `.do-transcript`, `.do-spk` | Transcript and speaker label |
| `.do-receipt` | Narrow receipt with aligned table values |
| `.do-cert` | Certificate-style panel |

## Variant notes

- **Chat:** `.do-chat` is the default dark-header conversation. Add `.do-wa` for the lighter WhatsApp-inspired variation, or `.do-secure` for the secure-channel treatment.
- **Bank cards:** `.do-bank-alert` changes the top rule to the rust accent. `.do-bank-dark` switches the card to a dark surface. These can be combined.
- **Documents:** Add one `.do-d-*` class to `.do-doc` to change the document's border treatment. The preview includes personnel, service, intelligence, brief, field, incident, medical, investigation, interrogation, casualty, chain-of-custody, and correspondence examples.
- **Classification:** The `.do-class-*` and `.do-stamp-*` variants cover Top Secret, Secret, Confidential, Restricted, Declassified, and For Official Use Only treatments.
- **Signatures:** Use `.do-signature-blue` or `.do-signature-red` for the left-border accent; `.do-sign-blue` and `.do-sign-red` colour the script-like name.

## Responsive behaviour

The stylesheet includes mobile adjustments at `max-width: 600px`. These:
- reduce the reading panel padding and title sizes;
- remove floats from dossier labels and email metadata;
- allow chat bubbles to use more of the available width;
- reduce padding in letters, documents, and certificates;
- stack signature entries and adjust brand reference labels.

The preview is a standalone browser page. AO3's own page layout and sanitisation can affect the final result, so check the selected Work Skin on both desktop and mobile after installation.

## Compatibility and implementation notes

- The component-support section is explicitly written to avoid CSS Grid, `gap`, external font imports, and scripts.
- Font declarations use system font stacks with fallbacks. The preview does not load external font files.
- The stylesheet scopes its rules under `#workskin` to limit effects to the work content.
- Some styles rely on ordinary HTML elements such as `div`, `span`, `p`, `dl`, `dt`, `dd`, `table`, and `hr`. Preserve the documented nesting and class names when reusing snippets.
- The HTML preview contains sample fiction and fictional interface content to demonstrate appearance; replace it with your own story material.

## Customisation

- Change the colour values in the CSS to retheme the interface. Update related variants together so the chat, document, banner, and status components remain visually consistent.
- Adjust the main reading width by changing the `max-width` on `.preface`, `#chapters`, and `.afterword`.
- Adjust the overall reading density through the padding, `font-size`, and `line-height` declarations on those panels.
- Keep the mobile overrides near the end of the stylesheet in sync with any desktop changes.

## Scope

This README describes the supplied CSS and HTML preview files. It documents the selectors and examples present in those files; it does not claim that the skin has been independently tested or approved by AO3.
