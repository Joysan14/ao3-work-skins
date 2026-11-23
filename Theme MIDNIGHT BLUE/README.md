# Midnight Blue — AO3 Work Skin

A refined, literary AO3 Work Skin built around deep midnight navy, cool silver-blue accents, and warm ivory reading surfaces. The design pairs an atmospheric dark outer frame with pale, paper-like story panels, then uses restrained blue-grey details for chapter headings, metadata, messages, and document interfaces.

## Included files

| File | Purpose |
|---|---|
| `Theme MIDNIGHT BLUE.css` | Stylesheet to install as an AO3 Work Skin |
| `Theme MIDNIGHT BLUE.html` | Standalone browser preview and component sampler |

The HTML file is a visual preview. It contains its own embedded stylesheet and sample markup. For AO3, install the CSS file in the Work Skin editor. Copy the relevant HTML snippets into a work's chapter or notes only when you want to use those components.

## Design direction

- **Atmospheric outer frame:** deep navy background with layered inset shadows.
- **Reading surface:** warm ivory panels with a fine silver-blue border and subtle inset framing.
- **Editorial typography:** Georgia/Palatino body text, with Cormorant Garamond and Libre Baskerville-style headings where available.
- **Interface contrast:** compact sans-serif labels and monospaced system/document panels.
- **Accent treatment:** muted blue and steel tones rather than bright or saturated colour.

## Colour palette

The following values are taken from the supplied stylesheet.

| Colour | Hex | Use |
|---|---|---|
| Midnight navy | `#09182B` | Outer background, dark chat headers, system panels |
| Deep blue-black | `#12243A` | Titles, dark accents, stamps and outgoing message bubbles |
| Slate blue | `#203149` | Main text on light panels |
| Muted steel blue | `#344A63` | Secondary text, borders and document details |
| Dusty blue | `#52769B` | Links, emphasis, warning accents and selected variants |
| Blue-grey | `#52677F` | Alternate message-sender colour |
| Silver blue | `#8295AB` | Fine rules, muted labels and decorative details |
| Pale silver | `#AAB9CA` | Borders, message timestamps and light accents |
| Warm ivory | `#F3F1EC` | Main reading panels and light text |
| Soft ivory | `#FAF9F6` | Cards, letters and light message bubbles |
| Pale grey | `#E7E6E2` | Secondary panels, chat backgrounds and notes |
| Pale blue | `#DCE6F0` | Highlighted text and selected document variation |
| Cool grey | `#D9D9D6` | Secondary highlight and photo placeholder |
| Muted green | `#526B62` | Credit/status accent in bank and status examples |
| Signature blue | `#496A8A` | Handwritten-style signature accents |

> Note: The stylesheet's section comment mentions muted burgundy accents, but the actual component rules use muted blue/steel accents. This README documents the colour values and styling rules present in the CSS.

## Installation on AO3

1. Open **Dashboard → Skins → My Work Skins**.
2. Choose **Create Work Skin**.
3. Give the skin a name, such as **Midnight Blue**.
4. Open `Theme MIDNIGHT BLUE.css` in a text editor.
5. Copy the complete CSS into the AO3 Work Skin CSS field.
6. Save the skin.
7. Open the work you want to style, choose **Edit**, and select the new Work Skin under the work's **Customize** options.
8. Save and preview the work.

The standalone HTML preview is not the stylesheet to paste into AO3. It is provided to demonstrate the styling and component markup.

## Layout and typography

### Work layout

- The outer `#workskin` area uses a midnight navy background, layered inset shadows, and generous desktop padding.
- The preface, chapters, and afterword are styled as centred reading panels with a maximum width of approximately 760px.
- Reading panels use warm ivory backgrounds, slate text, a silver-blue border, and a subtle double inset frame.
- The main reading font is Georgia with Palatino-style fallbacks.
- Body copy uses a spacious line height and avoids first-line indentation by default.
- `.do-book` enables traditional book-style paragraph indentation.
- `.do-justify` justifies paragraphs.
- Links use dusty blue with an underline and a visible keyboard-focus outline.

### Display typography

- Main work titles use a Cormorant Garamond-style serif stack.
- Chapter titles use a Libre Baskerville-style serif stack.
- Subtitles, epigraphs, and literary inserts use italic serif styling.
- Metadata, labels, timestamps, and interface text use Arial/Helvetica.
- System and dossier/document panels use Courier New or another monospace fallback.

Font families such as Cormorant Garamond and Libre Baskerville are listed as preferred stacks. The stylesheet does not import or bundle those fonts, so the browser uses them only if they are available locally and otherwise falls back to the listed alternatives.

## Component guide

The CSS includes a broad set of optional classes for formatting story text, fictional interfaces, and in-world documents. Add the matching class to HTML in your AO3 work to use a component.

### 1. Story and literary formatting

| Class | Purpose |
|---|---|
| `.do-title` | Large centred story or section title |
| `.do-subtitle` | Italic subtitle beneath a title |
| `.do-epigraph` | Centred quotation with optional citation |
| `.do-meta` | Definition-list metadata panel |
| `.do-chip` | Small inline metadata label |
| `.do-chapter` | Centred chapter heading group |
| `.do-chapter-num` | Chapter number or label |
| `.do-chapter-title` | Chapter title |
| `.do-chapter-sub` | Optional chapter subtitle |
| `.do-chapter-orn` | Decorative chapter marker |
| `.do-dialogue` | Adds spacing beneath a dialogue paragraph |
| `.do-thought` | Indented italic internal thought |
| `.do-th`, `.thought`, `.thought-plain` | Short or paragraph-style thought helpers |
| `.do-thought-bar` | Internal thought set apart by a left rule |
| `.do-dropcap` | Large initial letter |
| `.do-lead` | Small-caps opening phrase |
| `.do-pov` | Centred point-of-view label |
| `.do-tag` | Small uppercase contextual label |
| `.do-flashback` | Flashback block with a left border |
| `.do-memory` | Shaded memory passage |
| `.do-dream` | Dashed-border dream passage |
| `.do-pull` | Large centred pull quote |
| `.do-break` | Decorative scene break |
| `.do-break-dots`, `.do-break-tide`, `.do-break-line` | Alternative scene-break styles |
| `.do-note`, `.do-note-title` | Author's note or explanatory panel |
| `.do-endnotes` | Numbered endnotes panel |
| `.do-warn`, `.do-warn-title` | Content warning panel |
| `.do-disclaimer` | Smaller disclaimer paragraph |
| `.do-letter`, `.do-sig` | Letter and right-aligned sign-off |
| `.do-diary`, `.do-date` | Diary entry with date label |
| `.do-poem`, `.do-poem-title` | Poem block and title |
| `.do-footnotes`, `.do-fnref` | Footnote text and superscript reference |
| `.do-hl`, `.do-hl-sea` | Inline text highlights |
| `.do-frame` | Framed passage or quotation |
| `.do-center` | Centres an element or paragraph |
| `.do-lh` | Labelled local heading with optional small subtitle |

### 2. Chats and digital communication

| Class | Purpose |
|---|---|
| `.do-chat` | General chat conversation panel |
| `.do-chat-head` | Chat contact or group header |
| `.do-chat-body` | Chat message area |
| `.do-day` | Date divider |
| `.do-msg` | Incoming message bubble |
| `.do-out` | Outgoing message bubble |
| `.do-sender` | Sender label |
| `.do-s2`, `.do-s3` | Alternate sender colours |
| `.do-time` | Message timestamp |
| `.do-tick` | Read/delivery indicators |
| `.do-wa` | WhatsApp-style colour variant |
| `.do-secure` | Secure/encrypted chat variant |
| `.do-typing` | Typing indicator |
| `.do-post` | Social-media post card |
| `.do-avatar` | Circular initials/avatar marker |
| `.do-name`, `.do-handle` | Account name and handle |
| `.do-post-body`, `.do-post-stats` | Post content and engagement line |
| `.do-email` | Email panel, including nested replies |
| `.do-email-head`, `.do-email-body` | Email header and body |
| `.do-k`, `.do-v`, `.do-email-subject` | Email metadata labels and values |
| `.do-notify` | Notification card |
| `.do-system` | Dark system/status message |
| `.do-call`, `.do-missed` | Call log and missed-call label |
| `.do-voice`, `.do-wave` | Voice-message style panel and waveform text |
| `.do-radio`, `.do-ts`, `.do-cs` | Radio/transmission log with timestamps and call signs |

### 3. Organisations and brand panels

| Class | Purpose |
|---|---|
| `.do-banner` | Large organisation or institutional banner |
| `.do-banner-blue`, `.do-banner-red`, `.do-banner-black` | Banner colour variations |
| `.do-banner-name` | Organisation name |
| `.do-banner-tag` | Motto or descriptor |
| `.do-banner-est` | Establishment date or footer line |
| `.do-brand` | Compact brand identity card |
| `.do-brand-mark` | Initials or logo-style mark |
| `.do-brand-body` | Brand text container |
| `.do-brand-name` | Brand or organisation name |
| `.do-brand-tag` | Short descriptor |
| `.do-brand-ref` | Reference code or establishment detail |
| `.do-brand-blue`, `.do-brand-red` | Compact brand variations |

### 4. Bank notifications

| Class | Purpose |
|---|---|
| `.do-bank` | Bank transaction notification |
| `.do-bank-app` | App/bank name row |
| `.do-bank-icon` | Small circular icon |
| `.do-bank-time` | Notification time |
| `.do-bank-title` | Transaction or alert heading |
| `.do-bank-text` | Main notification text |
| `.do-bank-amt` | Transaction amount |
| `.do-bank-cr` | Credit amount styling |
| `.do-bank-dr` | Debit amount styling |
| `.do-bank-bal` | Balance or supporting detail |
| `.do-bank-alert` | Alert-style top border |
| `.do-bank-dark` | Dark notification variation |

### 5. Documents, records and dossiers

| Class | Purpose |
|---|---|
| `.do-doc` | General in-world document panel |
| `.do-doc-label` | Document type label |
| `.do-doc-title` | Document heading |
| `.do-docmeta` | Compact document metadata row |
| `.do-ref` | Reference or file number |
| `.do-sect` | Document section heading |
| `.do-dossier` | Definition-list dossier |
| `.do-photo` | Photo placeholder block |
| `.do-status` | Status label |
| `.do-status-open`, `.do-status-hold`, `.do-status-closed` | Status variations |
| `.do-redact`, `.do-redact-name`, `.do-redact-block` | Inline, name, and block redactions |
| `.do-missing` | Missing-record indicator |
| `.do-chainlist` | Chain-of-custody or event list |
| `.do-dist` | Distribution line |
| `.do-stamp` | General document stamp |
| `.do-class` | Full-width classification strip |
| `.do-class-ts`, `.do-class-s`, `.do-class-c`, `.do-class-rs`, `.do-class-dc`, `.do-class-fouo` | Classification variations |
| `.do-stamp-ts`, `.do-stamp-s`, `.do-stamp-c`, `.do-stamp-r`, `.do-stamp-rs`, `.do-stamp-dc`, `.do-stamp-fouo`, `.do-stamp-y` | Stamp variations |
| `.do-d-brief`, `.do-d-casualty`, `.do-d-chain`, `.do-d-corr`, `.do-d-field`, `.do-d-incident`, `.do-d-intel`, `.do-d-interrog`, `.do-d-inv`, `.do-d-medical`, `.do-d-personnel`, `.do-d-service` | Document border/style variants |

### 6. News, transcripts and formal records

| Class | Purpose |
|---|---|
| `.do-news` | Newspaper-style document variation |
| `.do-dateline` | Publication/date line |
| `.do-transcript` | Interview or recorded transcript |
| `.do-spk` | Speaker label |
| `.do-receipt` | Receipt-style panel |
| `.do-cert` | Certificate-style panel |
| `.do-sign` | Handwritten-style signature text |
| `.do-sign-blue`, `.do-sign-red` | Signature colour variations |
| `.do-signature` | Signature container |
| `.do-signature-blue`, `.do-signature-red` | Signature container variations |
| `.do-signature-line` | Signature line with optional caption |
| `.do-signature-entry` | Signature entry in a sheet |
| `.do-signature-name` | Name above signature caption |
| `.do-signature-caption` | Small uppercase caption |
| `.do-signature-sheet` | Multi-signature acknowledgement sheet |
| `.do-sigline` | Inline signature line |

## Responsive behaviour

The stylesheet includes a media query for screens up to 600px wide. On narrow screens it:

- Reduces the outer work padding and reading-panel padding.
- Reduces title and chapter-title sizes.
- Removes floated labels in metadata and email headers so labels stack vertically.
- Allows chat bubbles to use more of the available width.
- Reduces padding in letters, documents, and certificates.
- Narrows thought padding and drop-cap sizing.
- Stacks dossier labels and values.
- Makes signature entries full-width.
- Removes the float from compact brand reference text.

The HTML preview uses a viewport meta tag and is intended to be opened in a browser for visual inspection.

## Using the components in a work

1. Install and select the Work Skin.
2. Open the HTML preview to identify the component you want.
3. Copy only the relevant component markup from the preview.
4. Paste it into the work's chapter or notes using AO3's HTML editor.
5. Replace the sample wording, names, dates, amounts, and labels with your own content.
6. Preview the work on desktop and mobile.

Use the class names exactly as written. For example, `.do-chat.do-wa` combines the general chat structure with the WhatsApp-style variation, while `.do-doc.do-d-personnel` combines the document base with a personnel-file treatment.

## Compatibility notes

- The stylesheet scopes its styling under `#workskin` to keep the rules focused on the work content.
- It uses conventional block, inline-block, float, and table-based layout techniques.
- It does not use CSS Grid or the `gap` property.
- It does not rely on JavaScript or external font imports.
- Some effects depend on browser font availability and AO3's handling of user-supplied HTML/CSS. Check the published work preview after installation.
- The CSS includes responsive adjustments at `max-width: 600px`.

## Customisation

To adapt the theme while keeping its visual identity:

- Change the navy background (`#09182B`) for a different outer atmosphere.
- Adjust the ivory panel colours (`#F3F1EC`, `#FAF9F6`) to make the reading surface warmer or cooler.
- Use the steel-blue values (`#8295AB`, `#AAB9CA`) for borders and subtle details.
- Keep body text dark on light panels for readability.
- When changing a palette colour, search for its hex value throughout the stylesheet so related components remain consistent.

## Preview contents

The supplied HTML preview is titled **“Midnight Navy — Updated Work Skin Preview”** and uses a sample work called **The Salt Archive**. It demonstrates the stylesheet's literary, messaging, organisation, banking, signature, and document components in one page.

The preview's sample story and interface text are demonstration content. Replace it with your own material when using the snippets in a work.

---

*Documentation based on the supplied `Theme MIDNIGHT BLUE.css` and `Theme MIDNIGHT BLUE.html` files. It describes the included styles and preview examples; it does not claim independent live testing on AO3.*
