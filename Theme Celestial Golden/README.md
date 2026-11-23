# Theme Celestial Golden

An AO3 Work Skin with a light sky-blue atmosphere, warm golden accents, and soft parchment reading panels.

## 1. Overview

**Theme name:** Celestial Golden  
**Preview title:** Celestial Reverie — Sky Blue & Gold  
**Files:**
- `Theme Celestial Golden.css` — the AO3 Work Skin stylesheet
- `Theme Celestial Golden.html` — a standalone browser preview and component sampler

Celestial Golden pairs an airy, luminous blue backdrop with understated gold detailing and warm ivory document surfaces. The result is intended to feel calm, elegant, literary, and slightly celestial without sacrificing the readability of long-form fiction.

The HTML preview demonstrates the visual system through a fictional sample titled **“The House Beneath the Ashes.”** Its chapter sample, **“Chapter One: The Quiet Hour,”** includes narrative passages and a range of in-story interface elements.

## 2. Colour palette

The stylesheet uses a coordinated palette of sky blue, slate blue, warm gold, parchment, and dark brown.

| Role | Colour | Hex |
|---|---|---|
| Work-skin background | Pale blue | `#CFE5F3` |
| Preview canvas | Light sky blue | `#C7E0F0` |
| Background highlight | Cloud white | `#FFFFFF` |
| Background gradient | Very pale blue | `#EAF6FC` |
| Background gradient | Soft blue | `#C9E1F0` |
| Background gradient | Pale golden cream | `#F2E4C2` |
| Main reading surface | Warm ivory | `#F4F1EA` |
| Secondary paper surface | Warm parchment | `#EEE3D6` |
| Light insert surface | Near-white blue | `#F5FBFB` |
| Main text | Deep warm brown | `#453A2F` |
| Muted blue accent | Slate blue | `#798EA8` |
| Blue border | Mist blue | `#D3DEE8` |
| Blue structural accent | Muted sky blue | `#92ACC3` |
| Pale blue accent | Powder blue | `#A8CCE1` |
| Gold accent | Champagne gold | `#CBAB78` |
| Warm brown accent | Taupe | `#675B4D` |
| Highlight | Soft yellow | `#FCF5AD` |
| Highlight | Light blue | `#BBE5F9` |

The page background combines radial highlights and a diagonal gradient to create the impression of open sky and warm late-afternoon light. Gold is used for borders, separators, and small ornamental details rather than large blocks of text.

## 3. Typography

The stylesheet uses a mix of serif and sans-serif typefaces to distinguish literary content from interface elements.

- **Cormorant Garamond** — prominent titles, subtitles, epigraphs, letters, diary entries, and decorative literary text.
- **Libre Baskerville** — chapter headings and selected document titles.
- **Georgia / Palatino** — primary story text and longer reading passages.
- **Arial / Helvetica** — labels, metadata, interface headers, and compact notices.
- **Courier New** — timestamps, dates, technical records, and document-style metadata.

The HTML preview loads Cormorant Garamond and Libre Baskerville from Google Fonts. The CSS includes fallback font stacks, so the layout can still render if those external fonts are unavailable.

## 4. Layout and reading experience

The stylesheet styles AO3's `#workskin` area with a pale-blue background, layered gradients, a fine gold border, and subtle inset highlights.

The work's preface, chapter content, and afterword are presented on centered warm-ivory panels. These panels use a maximum width of approximately **760px**, generous padding, and a serif reading font with a relaxed line height.

Additional reading styles include:
- Paragraph spacing without default first-line indentation.
- Optional book-style paragraph indentation through `.do-book`.
- Optional justified text through `.do-justify`.
- Responsive images and tables constrained to the available content width.
- Link styling in muted blue with gold underline accents.
- Visible keyboard-focus outlines for links.

## 5. Component catalogue

The stylesheet provides reusable classes for narrative formatting, chapter presentation, correspondence, social media, records, and other fictional inserts. All selectors are scoped under `#workskin`.

### Titles and chapter presentation

| Class | Purpose |
|---|---|
| `.do-title` | Main title treatment |
| `.do-subtitle` | Italic subtitle |
| `.do-epigraph` | Centered quotation with citation |
| `.do-meta` | Work or scene metadata panel |
| `.do-chip` | Small inline metadata label |
| `.do-chapter` | Chapter heading container |
| `.do-chapter-num` | Chapter number or label |
| `.do-chapter-title` | Chapter title |
| `.do-chapter-sub` | Chapter subtitle |
| `.do-chapter-orn` | Decorative chapter ornament |

The AO3 preface title and chapter title also receive dedicated styling through selectors targeting `.preface .title` and `#chapters .preface .title`.

### Narrative and scene formatting

| Class | Purpose |
|---|---|
| `.do-book` | Book-style paragraph indentation |
| `.do-justify` | Justified text |
| `.do-dialogue` | Dialogue spacing |
| `.do-thought` | Italicized internal thought |
| `.do-dropcap` | Large decorative opening letter |
| `.do-lead` | Small-caps lead-in |
| `.do-pov` | Point-of-view marker |
| `.do-tag` | Small uppercase scene or section label |
| `.do-flashback` | Flashback passage |
| `.do-memory` | Memory passage |
| `.do-dream` | Dream passage |
| `.do-pull` | Centered pull quote with optional citation |
| `.do-narrative` | Indented narrative emphasis |
| `.do-cycle` | Seasonal or cycle marker |
| `.do-cycle-label` | Main cycle label |
| `.do-cycle-note` | Secondary cycle note |
| `.do-break` | Decorative scene separator |
| `.do-break-dots` | Dotted scene separator |
| `.do-break-tide` | Double-line scene separator |
| `.do-break-line` | Plain centered rule |

### Notes, warnings, and reading aids

| Class | Purpose |
|---|---|
| `.do-note` | Note panel |
| `.do-note-title` | Note heading |
| `.do-endnotes` | Endnote panel |
| `.do-warn` | Content warning or notice panel |
| `.do-warn-title` | Warning heading |
| `.do-disclaimer` | Compact disclaimer |
| `.do-label` | Small label |
| `.do-hl` | Yellow text highlight |
| `.do-hl-sea` | Blue text highlight |
| `.do-fnref` | Superscript footnote reference |
| `.do-footnotes` | Footnote section |
| `.do-frame` | Framed content |
| `.do-center` | Center-aligned content |

### Letters, diaries, and poetry

| Class | Purpose |
|---|---|
| `.do-letter` | Letter-style insert |
| `.do-sig` | Right-aligned letter signature |
| `.do-diary` | Diary entry |
| `.do-date` | Diary date or timestamp |
| `.do-poem` | Poetry block |
| `.do-poem-title` | Poem title |

### Chats and social media

| Class | Purpose |
|---|---|
| `.do-chat` | Message conversation container |
| `.do-chat-head` | Conversation header |
| `.do-chat-body` | Conversation body |
| `.do-day` | Date separator |
| `.do-msg` | Incoming message |
| `.do-out` | Outgoing message |
| `.do-sender` | Message sender label |
| `.do-s2`, `.do-s3` | Alternate sender colours |
| `.do-time` | Message timestamp |
| `.do-tick` | Read/delivery marks |
| `.do-wa` | WhatsApp-style chat variant |
| `.do-secure` | Dark secure-message variant |
| `.do-typing` | Typing indicator |
| `.do-post` | Social-media post |
| `.do-avatar` | Circular avatar placeholder |
| `.do-name` | Display name |
| `.do-handle` | Account handle |
| `.do-post-body` | Post text |
| `.do-post-stats` | Engagement or post statistics |

### Email, calls, notifications, and audio

| Class | Purpose |
|---|---|
| `.do-email` | Email container |
| `.do-email-head` | Email header |
| `.do-k` | Email field label |
| `.do-v` | Email field value |
| `.do-email-subject` | Email subject |
| `.do-email-body` | Email message body |
| `.do-notify` | Notification panel |
| `.do-system` | System or device notice |
| `.do-call` | Call record |
| `.do-missed` | Missed-call status |
| `.do-voice` | Voice-message panel |
| `.do-wave` | Decorative audio waveform |
| `.do-radio` | Radio or dispatch transcript |
| `.do-ts` | Timestamp |
| `.do-cs` | Dispatch or channel speaker label |

### Documents, reports, and records

| Class | Purpose |
|---|---|
| `.do-doc` | General document panel |
| `.do-doc-label` | Document classification or label |
| `.do-doc-title` | Document title |
| `.do-docmeta` | Document metadata |
| `.do-ref` | Reference label |
| `.do-sect` | Document section heading |
| `.do-sigline` | Signature line |
| `.do-lh` | Formal document letterhead |
| `.do-photo` | Photo placeholder or caption area |
| `.do-dossier` | Definition-list dossier |
| `.do-status` | Status label |
| `.do-status-open` | Active/open status |
| `.do-status-closed` | Closed status |
| `.do-status-hold` | On-hold status |
| `.do-chainlist` | Chain-of-custody list |
| `.do-dist` | Distribution information |
| `.do-class` | Full-width classification bar |
| `.do-stamp` | Classification or record stamp |
| `.do-redact` | Inline redaction |
| `.do-redact-name` | Redacted name |
| `.do-redact-block` | Block redaction |
| `.do-missing` | Missing-information marker |
| `.do-news` | News-style document |
| `.do-dateline` | News dateline |
| `.do-transcript` | Transcript formatting |
| `.do-spk` | Transcript speaker label |
| `.do-receipt` | Receipt-style insert |
| `.do-cert` | Certificate-style insert |
| `.do-card` | Structured information card |
| `.do-card-head` | Card heading |
| `.do-card-title` | Card title |
| `.do-regno` | Record or registration number |
| `.do-mono` | Monospaced text |
| `.do-fiction` | Fictional-record disclaimer |
| `.do-bio-note` | Biographical note |

The document system includes modifier classes for different record types, such as `.do-d-personnel`, `.do-d-service`, `.do-d-intel`, `.do-d-brief`, `.do-d-field`, `.do-d-incident`, `.do-d-medical`, `.do-d-inv`, `.do-d-interrog`, `.do-d-casualty`, `.do-d-chain`, and `.do-d-corr`.

Additional card accents include `.do-acc-burgundy`, `.do-acc-forest`, `.do-acc-taupe`, `.do-acc-slate`, and `.do-acc-rose`.

### Omegaverse and relationship-record components

The stylesheet also includes components for fictional pack, bond, and status records:

| Class | Purpose |
|---|---|
| `.do-pack-members` | Pack-member list |
| `.do-bond-consensual` | Consensual bond styling |
| `.do-bond-unconfirmed` | Unconfirmed bond styling |
| `.do-bond-disputed` | Disputed bond styling |
| `.do-bond-recognized` | Recognized bond styling |
| `.do-status-consent` | Consent-related status |
| `.do-status-unconf` | Unconfirmed status |
| `.do-status-disp` | Disputed status |
| `.do-status-legal` | Legal/official status |
| `.do-seal` | Circular seal or insignia |

The class names are visual formatting hooks. Their use does not establish or determine the meaning of a story's fictional events.

## 6. HTML preview contents

`Theme Celestial Golden.html` is a standalone preview page. It includes embedded styling so it can be opened directly in a browser without first installing the AO3 stylesheet.

The sample demonstrates:
- AO3-style work preface, summary, and author's notes.
- Chapter heading and narrative text.
- Point-of-view, thought, epigraph, and pull-quote treatments.
- Flashback, memory, dream, and seasonal markers.
- Standard and WhatsApp-style chat conversations.
- Social-media post and email layouts.
- Notifications, system notices, calls, voice messages, and radio dispatch.
- A confidential incident report, receipt, personnel card, letter, diary entry, and poem.
- A content notice and disclaimer.

The sample story and its names, records, and correspondence are placeholder fiction used to demonstrate the components.

## 7. Installation on Archive of Our Own

1. Open **AO3 → Dashboard → Skins**.
2. Select **Create Site Skin**.
3. Give the skin a name, such as **Theme Celestial Golden**.
4. Open `Theme Celestial Golden.css` in a text editor.
5. Copy the stylesheet into the Site Skin CSS field.
6. Save the skin.
7. Open the saved skin and select **Use**.

The CSS is scoped to `#workskin`, so its principal formatting is intended for the work content area rather than the entire AO3 website.

### Using the HTML components in a work

The HTML file is a browser preview, not a stylesheet installation file. To use a component in an AO3 work:

1. Install and activate the CSS Site Skin.
2. Open the work or chapter editor.
3. Switch the work text editor to **HTML** mode.
4. Copy only the relevant component markup from the preview or your own saved snippets.
5. Replace the sample text with your story content.
6. Preview the work before publishing.

Do not paste the entire standalone HTML document into an AO3 chapter. It contains document-level elements such as `<!doctype html>`, `<html>`, `<head>`, `<style>`, and `<body>`, which belong in a browser preview rather than the work editor.

## 8. Preview and compatibility notes

- Open `Theme Celestial Golden.html` in a modern browser to inspect the complete component sampler.
- The preview includes Google Fonts. If those fonts do not load, the declared fallback fonts will be used.
- The stylesheet uses AO3's `#workskin` scope and ordinary class-based markup.
- Check long messages, tables, and document inserts on a narrow screen before publishing.
- The preview demonstrates the CSS components; it does not automatically add those components to a work. The corresponding HTML markup must be inserted where needed.
- Some visual details may vary depending on AO3's page layout, the user's browser, and available fonts.

## 9. Suggested folder structure

Keep the stylesheet, preview, and README together:

```text
Theme Celestial Golden/
├── README_Theme_Celestial_Golden.md
├── Theme Celestial Golden.css
└── Theme Celestial Golden.html
```

## 10. Credits and customisation

This theme is a custom AO3 Work Skin. You can adapt the colour values, typography, and component markup to suit an individual work, while keeping the CSS class names consistent between the stylesheet and the HTML you use.

If you modify a class name in the CSS, update the corresponding HTML markup as well. Otherwise, the component will no longer receive its intended styling.
