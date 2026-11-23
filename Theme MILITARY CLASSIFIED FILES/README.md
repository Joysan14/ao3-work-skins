# Military Classified Files — AO3 Work Skin

A dark, archival-style AO3 Work Skin designed to make fanfiction feel like a classified dossier, institutional record, or recovered case file. It combines a deep military-green interface with warm parchment reading panels, restrained brass details, redacted text, official stamps, communications, and document-style inserts.

## Files

| File | Purpose |
|---|---|
| `Theme MILITARY CLASSIFIED FILES.css` | The AO3 Work Skin stylesheet. Add this to an AO3 Work Skin. |
| `Theme MILITARY CLASSIFIED FILES.html` | A standalone browser preview containing the stylesheet and sample markup for the components. |

The HTML file is a preview, not the stylesheet to paste into AO3. The CSS file is the one to install.

## Design direction

The visual language is inspired by classified government files, military administration, police records, intelligence briefings, and paper archives.

- **Outer frame:** dark charcoal-green with subtle grid lines, vignette shading, and an inset border.
- **Reading panels:** warm parchment with fine aged-brass borders and layered paper-like shadows.
- **Typography:** traditional serif body text paired with uppercase sans-serif labels and monospaced technical details.
- **Accents:** muted olive, brass, steel-grey, and controlled red for alerts or sensitive classifications.
- **Document styling:** file labels, reference numbers, metadata, status markers, redactions, signatures, and classification stamps.

## Colour palette

The following colours are used in the stylesheet:

| Colour | Hex | Use |
|---|---|---|
| Deep charcoal | `#1D221E` | Outer preview background |
| Military charcoal-green | `#252C26` | Main Work Skin frame and dark panels |
| Dark olive | `#343D32` | Headers, banners, and selected accents |
| Olive-grey | `#454B35` | Borders, links, and classification details |
| Moss green | `#59634A` | Decorative rules and secondary accents |
| Warm parchment | `#E8E1CE` | Main reading surfaces |
| Aged brass | `#B5AA8B` | Borders, metadata accents, and stamps |
| Pale ivory | `#F4F0E5` | Light cards and document surfaces |
| Soft ivory | `#F9F7F0` | Highlighted text and light details |
| Dark ink | `#252724` | Main text on light surfaces |
| Muted grey | `#414747` | Secondary text and labels |
| Steel grey | `#777C78` | Fine rules and subdued details |
| Alert red | `#8B3737` | Warnings, incidents, and urgent status |
| Blue signature ink | `#1F3F8F` | Blue handwritten-style signatures |
| Red signature ink | `#A12B2B` | Red handwritten-style signatures |

## Main layout and reading typography

The stylesheet styles the standard AO3 work structure:

- `.preface` — work title, byline, summary, and notes.
- `#chapters` — chapter content and chapter preface.
- `.afterword` — end notes and closing material.
- `.userstuff` — story text and embedded content.

The main reading panels use a maximum width of approximately 760px, parchment backgrounds, generous padding, and a Georgia/Palatino serif stack. The default paragraph style has no first-line indent. Add `.do-book` to a wrapper when you want traditional book-style paragraph indents. `.do-justify` provides justified text.

The work title uses a display serif stack, while chapter headings use a Baskerville-style serif stack. Small labels and metadata use Arial/Helvetica; technical timestamps and file references use Courier New.

## Component reference

All component selectors are scoped to `#workskin`.

### Story and literary formatting

| Class | Purpose |
|---|---|
| `.do-title` | Large centred story title |
| `.do-subtitle` | Italic subtitle |
| `.do-epigraph` | Centred epigraph with optional citation |
| `.do-meta` | Story metadata arranged as label/value pairs |
| `.do-chip` | Small metadata tag |
| `.do-chapter` | Decorative chapter-heading block |
| `.do-chapter-num` | Chapter number or label |
| `.do-chapter-title` | Chapter title |
| `.do-chapter-sub` | Chapter subtitle |
| `.do-chapter-orn` | Decorative chapter ornament |
| `.do-dialogue` | Dialogue paragraph spacing |
| `.do-thought` | Italic internal thought |
| `.do-th` | Short italic aside |
| `.do-thought-bar` | Internal thought with a vertical accent rule |
| `.do-dropcap` | Large decorative first letter |
| `.do-lead` | Small-cap opening phrase |
| `.do-pov` | Centred point-of-view label |
| `.do-tag` | Small uppercase section label |
| `.do-flashback` | Flashback panel |
| `.do-memory` | Memory or recollection panel |
| `.do-dream` | Dream sequence panel |
| `.do-pull` | Centred pull quote |
| `.do-break` | Decorative scene break |
| `.do-break-dots`, `.do-break-tide`, `.do-break-line` | Alternative scene-break styles |
| `.do-note` | Author or contextual note |
| `.do-warn` | Content warning panel |
| `.do-disclaimer` | Small disclaimer text |
| `.do-hl`, `.do-hl-sea` | Inline highlight treatments |
| `.do-fnref`, `.do-footnotes` | Footnote reference and footnote area |
| `.do-center` | Centred content |
| `.do-label` | Small component label |

### Letters, diaries, and literary inserts

| Class | Purpose |
|---|---|
| `.do-letter` | Letter or written correspondence |
| `.do-sig` | Right-aligned letter sign-off |
| `.do-diary` | Diary or journal entry |
| `.do-date` | Date/time label |
| `.do-poem` | Narrow, inset poem layout |
| `.do-poem-title` | Poem title |

### Digital communications

| Component | Purpose |
|---|---|
| `.do-chat` | General messaging conversation |
| `.do-chat.do-wa` | WhatsApp-inspired variation |
| `.do-chat.do-secure` | Dark encrypted or secure-channel conversation |
| `.do-chat-head` | Conversation header |
| `.do-chat-body` | Message area |
| `.do-day` | Date separator |
| `.do-msg` | Incoming message |
| `.do-msg.do-out` | Outgoing message |
| `.do-sender` | Sender label |
| `.do-s2`, `.do-s3` | Alternate sender colours |
| `.do-time` | Message timestamp |
| `.do-tick` | Read/delivery tick marks |
| `.do-typing` | Typing indicator |
| `.do-post` | Social-media post card |
| `.do-avatar` | Initial/avatar placeholder |
| `.do-name`, `.do-handle` | Display name and username |
| `.do-post-body` | Post text |
| `.do-post-stats` | Engagement figures |
| `.do-email` | Email card, including nested replies |
| `.do-email-head` | Email metadata header |
| `.do-k`, `.do-v` | Email field label and value |
| `.do-email-subject` | Email subject |
| `.do-email-body` | Email message body |
| `.do-notify` | Notification card |
| `.do-system` | Monospaced system or terminal message |
| `.do-call` | Call notification |
| `.do-missed` | Missed-call emphasis |
| `.do-voice` | Voice-message card |
| `.do-wave` | Audio waveform decoration |
| `.do-radio` | Radio or dispatch transcript |
| `.do-ts` | Radio timestamp |
| `.do-cs` | Radio callsign/speaker |

### Banking notifications

The `.do-bank` component provides a compact banking-app notification card.

| Class | Purpose |
|---|---|
| `.do-bank` | Standard banking notification |
| `.do-bank-app` | Bank/app name row |
| `.do-bank-icon` | Decorative app icon placeholder |
| `.do-bank-time` | Notification time |
| `.do-bank-title` | Transaction or alert heading |
| `.do-bank-amt` | Transaction amount |
| `.do-bank-cr` | Credit/received amount |
| `.do-bank-dr` | Debit/sent amount |
| `.do-bank-bal` | Balance or supporting information |
| `.do-bank-alert` | Alert/declined-payment variation |
| `.do-bank-dark` | Dark card variation |

You can combine variants, for example `do-bank do-bank-alert do-bank-dark`.

### Documents, dossiers, and records

| Class | Purpose |
|---|---|
| `.do-doc` | Official document or report |
| `.do-doc-label` | Document category label |
| `.do-doc-title` | Document heading |
| `.do-ref` | Reference or file number |
| `.do-docmeta` | Document metadata row |
| `.do-sect` | Section heading inside a document |
| `.do-sigline` | Printed signature line |
| `.do-lh` | Institutional letterhead |
| `.do-photo` | Photograph placeholder |
| `.do-dossier` | Label/value personnel or case details |
| `.do-status` | General status marker |
| `.do-status-open` | Open/active status |
| `.do-status-closed` | Closed status |
| `.do-status-hold` | On-hold status |
| `.do-dist` | Distribution information |
| `.do-chainlist` | Chain-of-custody or sequence list |
| `.do-receipt` | Receipt-style insert |
| `.do-cert` | Certificate or formal award |
| `.do-frame` | Framed document or insert |
| `.do-news` | Newspaper/news document variation |
| `.do-dateline` | News dateline |
| `.do-transcript` | Transcript text |
| `.do-spk` | Transcript speaker label |
| `.do-missing` | Missing-record marker |

### Document variants

The stylesheet includes specialised document variants that can be combined with `.do-doc`:

- `.do-d-personnel` — personnel file.
- `.do-d-service` — service record.
- `.do-d-intel` — intelligence document.
- `.do-d-brief` — briefing document.
- `.do-d-field` — field report.
- `.do-d-incident` — incident report.
- `.do-d-medical` — medical record.
- `.do-d-inv` — investigation file.
- `.do-d-interrog` — interrogation record.
- `.do-d-casualty` — casualty report.
- `.do-d-chain` — chain-of-custody record.
- `.do-d-corr` — correspondence file.

### Classification labels, stamps, and redactions

The `.do-class` and `.do-stamp` components provide official-looking classification bars and status stamps.

Available classification variants:

- `.do-class-ts` / `.do-stamp-ts` — Top Secret.
- `.do-class-s` / `.do-stamp-s` — Secret.
- `.do-class-c` / `.do-stamp-c` — Confidential.
- `.do-class-rs` / `.do-stamp-rs` — Restricted.
- `.do-class-dc` / `.do-stamp-dc` — Declassified.
- `.do-class-fouo` / `.do-stamp-fouo` — For Official Use Only.

Additional stamp variants include `.do-stamp-y` for a pending-style stamp and `.do-stamp-r` for a red outlined status such as denied.

Redaction helpers:

- `.do-redact` — inline redaction.
- `.do-redact-name` — name-sized redaction.
- `.do-redact-block` — full-width block redaction.

### Signatures and organisation branding

The signature and banner add-ons are included in the main stylesheet.

**Handwritten-style signatures**

- `.do-sign` — signature treatment.
- `.do-sign-blue`, `.do-sign-red`, `.do-sign-black` — ink colours.
- `.do-sign-light` — light ink for dark backgrounds.
- `.do-sign-sm`, `.do-sign-lg` — size variations.
- `.do-initials` — compact initials.
- `.do-sign-flat` — removes the rotation.
- `.do-signature` — signature block with printed name.
- `.do-signature-right`, `.do-signature-center` — alignment options.
- `.do-signature-line` — printed name and role line.
- `.do-signature-blue`, `.do-signature-red` — matching signature-line accents.
- `.do-signature-x` — sign-here marker.

**Compact organisation banner**

- `.do-brand` — compact emblem/name/tagline card.
- `.do-brand-mark` — emblem or initials.
- `.do-brand-body` — name and tagline wrapper.
- `.do-brand-name` — organisation name.
- `.do-brand-tag` — department or motto.
- `.do-brand-ref` — reference or establishment detail.
- `.do-brand-blue`, `.do-brand-red`, `.do-brand-black` — colour variations.

**Wide organisation banner**

- `.do-banner` — full-width title-card banner.
- `.do-banner-name` — organisation name.
- `.do-banner-tag` — motto or department.
- `.do-banner-est` — establishment date or identifying line.
- `.do-banner-blue`, `.do-banner-red`, `.do-banner-black` — colour variations.

## Mobile behaviour

The stylesheet includes compact-layout overrides for narrow screens. These reduce the outer frame and reading-panel padding, scale down titles and chapter headings, widen message bubbles, and simplify metadata rows so labels and values stack vertically. Signature lines and document details also become more flexible, while photo placeholders stop floating beside text.

The HTML preview is useful for checking the components in a browser at desktop and mobile widths. Actual rendering may differ slightly inside AO3 because the site controls the surrounding page layout.

## Installation on AO3

1. Open **AO3 → My Work Skins**.
2. Select **Create Work Skin**.
3. Give it a name, such as `Military Classified Files`.
4. Open `Theme MILITARY CLASSIFIED FILES.css` in a text editor.
5. Copy the entire CSS file into the Work Skin CSS field.
6. Save the Work Skin.
7. Open or edit a work and select the new skin under **Work Skin**.

Use the HTML preview file locally in a browser to inspect the sample components. Do not paste the complete HTML document into the AO3 CSS field.

## Using the components in a work

After installing the Work Skin, add the relevant HTML in the work's HTML editor and use the matching class names. For example:

```html
<div class="do-doc do-d-intel">
  <div class="do-doc-label">Intelligence Report</div>
  <span class="do-ref">Ref: INT/042</span>
  <span class="do-doc-title">Subject Observation</span>
  <div class="do-docmeta">
    <span><b>Filed</b> 12 Oct</span>
    <span><b>Office</b> Field Division</span>
  </div>
  <div class="do-sect">Summary</div>
  <p>Report contents go here.</p>
  <span class="do-stamp do-stamp-s">Secret</span>
</div>
```

For a signature:

```html
<div class="do-signature do-signature-blue">
  <span class="do-sign do-sign-blue">J. Harlan</span>
  <span class="do-signature-line">
    James Harlan
    <small>Chapter President</small>
  </span>
</div>
```

For a wide organisation banner:

```html
<div class="do-banner do-banner-blue">
  <span class="do-banner-name">Raccoon Police Department</span>
  <span class="do-banner-tag">To Protect and to Serve</span>
  <span class="do-banner-est">RACCOON CITY · EST. 1969</span>
</div>
```

For a dark banking alert:

```html
<div class="do-bank do-bank-alert do-bank-dark">
  <p class="do-bank-app">Security Alert</p>
  <p class="do-bank-title">Unusual activity detected</p>
  <p class="do-bank-text">A sign-in attempt was blocked.</p>
  <p class="do-bank-bal">Contact the bank if this was not you.</p>
</div>
```

You can combine compatible modifier classes to create variations. Keep the base component class (such as `.do-doc`, `.do-chat`, `.do-bank`, or `.do-banner`) when using a modifier.

## Customisation

- Change the main dark frame by editing the `#workskin` background colours.
- Change the parchment reading surface by editing the background and border colours on `.preface`, `#chapters`, and `.afterword`.
- Adjust the overall reading width by changing the `max-width` value on those panels.
- Adjust the story's text appearance through the `.userstuff` font and paragraph rules.
- Change signature ink or banner accents by editing the relevant modifier classes.
- Keep contrast strong when changing text and background colours, especially for dark notification panels and classification labels.

## Compatibility notes

- The stylesheet is scoped primarily to `#workskin` so its component styles are intended for work content rather than the entire AO3 interface.
- It uses ordinary HTML elements and CSS classes. The components do not require JavaScript.
- The cursive signature effect uses system font fallbacks. AO3 cannot load arbitrary external web fonts through a Work Skin, so the handwriting appearance can vary by device and operating system.
- The HTML preview is a standalone demonstration. AO3's own page chrome and work layout may affect the final appearance.
- Test long names, wide tables, and lengthy classification labels on mobile before publishing.

## Preview content

The HTML sample uses **The Salt Archive** and its fictional harbour records to demonstrate the components. The sample includes organisation banners, signatures, story typography, letters, diary entries, chats, banking alerts, emails, system notifications, radio messages, classified documents, stamps, and redactions. These are demonstration elements and can be replaced with your own story content.

---

*Documentation based on the supplied `Theme MILITARY CLASSIFIED FILES.css` and `Theme MILITARY CLASSIFIED FILES.html` files. The README describes the supplied implementation and does not claim independent live testing on AO3.*
