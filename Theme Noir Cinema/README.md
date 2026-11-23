# Noir Cinema — AO3 Work Skin

A cinematic, editorial-style AO3 Work Skin built around charcoal, soft ivory, cool slate, and muted burgundy. It combines book-like typography and spacious reading panels with reusable components for story formatting, messages, social posts, notifications, institutional documents, signatures, and dossier-style records.

## Files

| File | Purpose |
|---|---|
| `Theme Noir Cinema.css` | Main stylesheet to install as an AO3 Site Skin / Work Skin. |
| `Theme Noir Cinema.html` | Standalone browser preview demonstrating the stylesheet and its component classes. |

**Use the CSS on AO3.** The HTML file is a visual reference and testing page. It is not uploaded as part of the AO3 Work Skin.

## Design direction

The theme uses a dark cinematic outer frame around pale, paper-like reading surfaces. Serif typography gives the story text a literary feel, while compact sans-serif labels and monospaced text distinguish interface elements and official records.

- Dark charcoal surrounds the work.
- Warm ivory and pale grey form the reading surfaces.
- Slate provides secondary text, rules, and borders.
- Muted burgundy is used for links, warnings, and selected accents.
- Dusty blue and restrained green/gold tones appear in selected document and status variants.

## Colour palette

| Colour | Hex | Main use |
|---|---|---|
| Charcoal | `#24272B` | Outer background, dark panels, message headers |
| Deep black | `#17191C` | Strong contrast, headings, dark stamps |
| Warm ivory | `#F3F1EC` | Main reading surface and light text |
| Soft paper | `#FAF9F6` | Cards, letters, receipts, and light panels |
| Pale grey | `#E7E6E2` | Secondary panels and message backgrounds |
| Slate grey | `#B8BBC0` | Borders, dividers, muted UI details |
| Mid slate | `#747B83` | Secondary rules and accents |
| Charcoal grey | `#41464C` | Secondary text and document labels |
| Ink | `#292B2E` | Main body text |
| Muted burgundy | `#783B42` | Links, warnings, red accents |
| Dusty blue | `#526A7C` | Blue banner, signature, and classification accents |
| Pale rose | `#E3D3D4` | Highlight treatment |
| Pale blue-grey | `#D9DDE1` | Declassified treatment |
| Muted green | `#386B55` | Credit/status accent |

## Reading layout and typography

- The outer `#workskin` uses a charcoal background, inset shading, and generous desktop padding.
- The preface, chapter area, and afterword are styled as centred paper panels with a maximum width of approximately `760px`.
- Main story text uses Georgia with a `1.75` line height.
- Work titles use Cormorant Garamond where available, with serif fallbacks.
- Chapter headings use Libre Baskerville/Baskerville-style serif fallbacks.
- Labels, metadata, timestamps, and interface details use Arial/Helvetica.
- System messages, radio transcripts, receipts, and formal records use Courier New or another monospace fallback.

The stylesheet includes `.do-book` for indented book-style paragraphs and `.do-justify` for justified text.

## Component reference

All classes below are scoped under `#workskin`. Add the relevant class to the HTML you place in an AO3 work's HTML editor.

### Story and editorial formatting

| Class | Purpose |
|---|---|
| `.do-title` | Large centred title |
| `.do-subtitle` | Italic subtitle |
| `.do-epigraph` | Centred quotation with citation |
| `.do-meta` | Definition-list metadata panel |
| `.do-chip` | Compact metadata tag |
| `.do-chapter` | Chapter heading group |
| `.do-chapter-num` | Small uppercase chapter number |
| `.do-chapter-title` | Chapter title |
| `.do-chapter-sub` | Chapter subtitle |
| `.do-chapter-orn` | Decorative chapter marker |
| `.do-dialogue` | Dialogue paragraph spacing |
| `.do-thought`, `.do-th`, `.do-thought-bar` | Internal thought treatments |
| `.do-dropcap` | Large initial letter |
| `.do-lead` | Small-cap opening phrase |
| `.do-pov` | Centred point-of-view marker |
| `.do-tag` | Small uppercase section label |
| `.do-flashback` | Flashback block with left rule |
| `.do-memory` | Shaded memory block |
| `.do-dream` | Dashed dream block |
| `.do-pull` | Centred pull quote |
| `.do-break`, `.do-break-dots`, `.do-break-tide`, `.do-break-line` | Decorative scene breaks |
| `.do-note`, `.do-endnotes` | Notes and endnotes panels |
| `.do-warn` | Content warning panel |
| `.do-disclaimer` | Subtle disclaimer text |
| `.do-letter`, `.do-sig` | Letter and right-aligned sign-off |
| `.do-diary`, `.do-date` | Diary entry and date label |
| `.do-poem`, `.do-poem-title` | Poetry block and title |
| `.do-frame` | Framed passage |
| `.do-hl`, `.do-hl-sea` | Highlight treatments |
| `.do-fnref`, `.do-footnotes` | Footnote marker and footnote area |
| `.do-label`, `.do-center` | Component label and centred alignment helper |

### Messages and digital interfaces

| Class | Purpose |
|---|---|
| `.do-chat` | General chat interface |
| `.do-chat-head` | Chat header |
| `.do-chat-body` | Message area |
| `.do-day` | Date/day divider |
| `.do-msg` | Incoming message |
| `.do-out` | Outgoing message |
| `.do-sender` | Sender label |
| `.do-s2`, `.do-s3` | Alternate sender colours |
| `.do-time` | Message timestamp |
| `.do-tick` | Read/delivery marks |
| `.do-typing` | Typing indicator |
| `.do-wa` | WhatsApp-style colour variant |
| `.do-secure` | Secure-channel chat variant |
| `.do-post` | Social-media post card |
| `.do-avatar`, `.do-name`, `.do-handle` | Social profile details |
| `.do-post-body`, `.do-post-stats` | Post text and engagement line |
| `.do-email` | Email panel; supports nested replies |
| `.do-email-head`, `.do-email-body` | Email header and message body |
| `.do-k`, `.do-v`, `.do-email-subject` | Email metadata labels and values |
| `.do-notify` | General notification |
| `.do-system` | Dark system/status message |
| `.do-call`, `.do-missed` | Call record and missed-call emphasis |
| `.do-voice`, `.do-wave` | Voice-message style block |

### Documents, records, and institutional elements

| Class | Purpose |
|---|---|
| `.do-doc` | General formal document panel |
| `.do-doc-label` | Document type label |
| `.do-doc-title` | Document heading |
| `.do-lh` | Letterhead/institution heading |
| `.do-ref` | Reference number |
| `.do-docmeta` | Document metadata row |
| `.do-dossier` | Definition-list dossier details |
| `.do-photo` | Placeholder portrait/photo frame |
| `.do-sect` | Document section heading |
| `.do-status` | Status label |
| `.do-status-open` | Open status |
| `.do-status-hold` | On-hold status |
| `.do-status-closed` | Closed status |
| `.do-redact`, `.do-redact-name` | Inline redaction |
| `.do-redact-block` | Block redaction |
| `.do-missing` | Missing-record emphasis |
| `.do-sigline` | Signature line |
| `.do-dist` | Distribution notice |
| `.do-chainlist` | Numbered chain-of-custody list |
| `.do-news` | News/article document variant |
| `.do-dateline` | Publication dateline |
| `.do-transcript` | Transcript block |
| `.do-spk` | Transcript speaker label |
| `.do-receipt` | Narrow receipt layout |
| `.do-cert` | Certificate layout |
| `.do-stamp` | General document stamp |
| `.do-class` | Classification label |

### Banners, signatures, and banking

| Class | Purpose |
|---|---|
| `.do-banner` | Large organisation/editorial banner |
| `.do-banner-blue` | Blue-accent banner |
| `.do-banner-red` | Burgundy-accent banner |
| `.do-banner-black` | Near-black banner |
| `.do-banner-name`, `.do-banner-tag`, `.do-banner-est` | Banner text hierarchy |
| `.do-brand` | Compact letterhead/brand strip |
| `.do-brand-mark` | Initials or logo tile |
| `.do-brand-body` | Brand name and descriptor |
| `.do-brand-ref` | Right-side reference label |
| `.do-brand-blue`, `.do-brand-red` | Brand accent variants |
| `.do-signature` | Signature panel |
| `.do-sign`, `.do-sign-blue`, `.do-sign-red` | Signature-style name |
| `.do-signature-line` | Caption/role line |
| `.do-signature-blue`, `.do-signature-red` | Signature line accents |
| `.do-signature-sheet` | Formal multi-signatory sheet |
| `.do-signature-entry` | Individual signature entry |
| `.do-signature-name`, `.do-signature-caption` | Name and caption within a signature sheet |
| `.do-bank` | Banking/transaction notification |
| `.do-bank-alert` | Alert/declined-transaction variant |
| `.do-bank-dark` | Dark banking card |
| `.do-bank-app`, `.do-bank-icon`, `.do-bank-time` | Bank/app header details |
| `.do-bank-title`, `.do-bank-text`, `.do-bank-amt`, `.do-bank-bal` | Transaction content |
| `.do-bank-cr`, `.do-bank-dr` | Credit and debit amount accents |

### Radio and classification variants

- `.do-radio` formats radio/dispatch transcripts.
- `.do-ts` styles timestamps.
- `.do-cs` styles callsigns or speaker identifiers.
- `.do-class-ts`, `.do-class-s`, `.do-class-c`, `.do-class-rs`, `.do-class-dc`, `.do-class-fouo` provide Top Secret, Secret, Confidential, Restricted, Declassified, and For Official Use Only label variants.
- Matching stamp variants are available: `.do-stamp-ts`, `.do-stamp-s`, `.do-stamp-c`, `.do-stamp-rs`, `.do-stamp-dc`, and `.do-stamp-fouo`.
- `.do-stamp-y` and `.do-stamp-r` provide pending/gold and red stamp accents.

### Document type accents

Use these modifier classes alongside `.do-doc`:

- `.do-d-personnel`
- `.do-d-service`
- `.do-d-intel`
- `.do-d-brief`
- `.do-d-field`
- `.do-d-incident`
- `.do-d-medical`
- `.do-d-inv`
- `.do-d-interrog`
- `.do-d-casualty`
- `.do-d-chain`
- `.do-d-corr`

They change the document's top-border accent to help distinguish record types.

## Responsive behaviour

The stylesheet includes a breakpoint at `42em`. On narrower screens it:

- Reduces outer and reading-panel padding.
- Removes the outer frame's rounded corners.
- Reduces title and chapter-title sizes.
- Allows metadata labels and values to stack vertically.
- Expands chat bubbles to use more of the available width.
- Reduces padding in letters, documents, and certificates.
- Stacks email metadata fields.
- Adjusts brand reference labels to a new line.
- Makes signature entries full width.
- Allows long radio/transcript strings to wrap.

## Installation on AO3

1. Open **AO3 → Dashboard → Skins**.
2. Choose **Create Site Skin**.
3. Give the skin a name, such as `Noir Cinema`.
4. Paste the complete contents of `Theme Noir Cinema.css` into the CSS field.
5. Save the skin.
6. Open the saved skin and use **Use** to apply it.
7. To use the component classes in a work, enable the appropriate HTML formatting option in the work editor and add the class markup to the work text.

AO3 may restrict some HTML or CSS behaviour. If a component does not render as expected, test it in a draft work first.

## Basic usage examples

### Book-style paragraphs

```html
<div class="do-book">
  <p>The first paragraph begins here.</p>
  <p>The next paragraph receives the book-style first-line indent.</p>
</div>
```

### Chapter heading

```html
<div class="do-chapter">
  <span class="do-chapter-num">Chapter One</span>
  <span class="do-chapter-title">A Quiet Beginning</span>
  <span class="do-chapter-sub">in which something changes</span>
  <span class="do-chapter-orn">◆ ◆ ◆</span>
</div>
```

### Chat conversation

```html
<div class="do-chat">
  <div class="do-chat-head">Contact Name<small>online</small></div>
  <div class="do-chat-body">
    <div class="do-day">Today</div>
    <div class="do-msg">
      <span class="do-sender">Alex</span>
      Are you there?
      <span class="do-time">21:14</span>
    </div>
    <div class="do-msg do-out">
      I'm here.
      <span class="do-time">21:15</span>
    </div>
  </div>
</div>
```

### Classified-style document

```html
<div class="do-doc do-d-intel">
  <div class="do-lh">Department Name<small>Records Division</small></div>
  <div class="do-doc-label">Intelligence Report</div>
  <span class="do-ref">Ref: INT/024</span>
  <span class="do-doc-title">Subject Report</span>
  <span class="do-class do-class-c">Confidential</span>
  <p>Document text goes here.</p>
  <p>Source: <span class="do-redact">Redacted</span></p>
</div>
```

### Banking alert

```html
<div class="do-bank do-bank-alert">
  <p class="do-bank-app">Bank Name</p>
  <p class="do-bank-title">Payment declined</p>
  <p class="do-bank-text">Your payment could not be processed.</p>
</div>
```

## Preview

`Theme Noir Cinema.html` is a standalone demonstration page titled **The Salt Archive**. It showcases the work preface, chapter layout, literary text treatments, banners, signatures, chat variants, social posts, banking cards, emails, system alerts, radio transcripts, classification labels, dossiers, document subtypes, receipts, certificates, and footnotes.

Open the HTML file in a browser to inspect the components. Its sample story and fictional organisations are demonstration content, not required text for your own work.

## Customisation notes

- Change the palette by editing the colour values in the CSS. Keep text/background contrast strong.
- Use `.do-banner-blue`, `.do-banner-red`, or `.do-banner-black` to vary organisation banners.
- Combine `.do-doc` with one `.do-d-*` modifier to distinguish document types.
- Combine `.do-chat` with `.do-wa` or `.do-secure` for alternate messaging styles.
- Combine `.do-bank` with `.do-bank-alert` or `.do-bank-dark` for transaction variants.
- Keep the class names intact when reusing the supplied HTML examples. The CSS selectors depend on them.

## Compatibility notes

- The stylesheet is scoped to `#workskin` to reduce unintended effects on the surrounding AO3 interface.
- Font stacks include fallbacks. Cormorant Garamond and Libre Baskerville are used when available; otherwise the browser falls back to the listed serif fonts.
- The HTML preview duplicates the stylesheet inside its `<style>` element so it can be viewed independently.
- The supplied files were inspected for this README, but the skin has not been independently tested on a live AO3 account or across every browser/device combination.
