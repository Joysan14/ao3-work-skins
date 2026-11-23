# Theme Blood Skin
## Red Velvet & Brushed Metal — AO3 Work Skin

**Theme:** Blood Skin  
**Visual direction:** Dark red velvet, antique parchment, champagne gold, and brushed silver  
**Preview title:** Blood Skin — Red Velvet & Metallic Preview  
**CSS namespace:** `.hgm-`  
**Primary wrapper:** `#workskin`

---

## 1. Design concept

Blood Skin is a dramatic, literary AO3 Work Skin built around a dark red velvet reading surface and metallic detailing. Its visual language combines the atmosphere of an old archive, a private family chronicle, and a cinematic dossier.

The main reading area uses a deep burgundy-black background with subtle layered gradients and fine texture. Warm ivory text provides contrast. Champagne, muted rose, and silver-blue accents distinguish headings, dividers, labels, document markings, and interface details.

The theme is especially suited to stories that use:
- Letters, diaries, emails, and private messages.
- Historical records, reports, case files, and institutional documents.
- Flashbacks, memories, dreams, and shifting points of view.
- Newspaper clippings, transcripts, and other inserted media.

## 2. Colour palette

The CSS contains a base archival palette and later Red Velvet overrides. The following colours describe the final visual direction.

| Colour | Hex | Use |
|---|---|---|
| Velvet black | `#16090D` | Outer page background |
| Deep burgundy | `#241016` | Main reading surface |
| Wine red | `#3A101D` | Opening panels and title treatments |
| Crimson accent | `#A52D49` | Borders, emphasis, chapter accents |
| Dark rose | `#8F2944` | Labels and secondary red accents |
| Warm ivory | `#F0E5DC` | Main reading text |
| Soft cream | `#F5EAE1` | Bright title and heading text |
| Parchment | `#EFE4D5` | Document and message panels |
| Light parchment | `#F2E9DD` | Letters and lighter paper surfaces |
| Champagne gold | `#B99A72` | Fine borders, rules, and metallic details |
| Antique bronze | `#A98475` | Muted metallic borders |
| Copper | `#C28D69` | Warm decorative accents |
| Brushed silver | `#AEB7C2` | Flashback and research accents |
| Slate blue | `#39495A` | Cool secondary accent |
| Dusty mauve | `#80666A` | Outer frame and subdued borders |

**Colour behaviour:** The main story field is dark, while document-like inserts deliberately switch to pale parchment with dark ink. This creates the impression of physical records placed on a velvet-covered archive table and keeps long inserted text readable.

## 3. Typography and layout

- **Literary headings:** Georgia and compatible serif fallbacks.
- **Narrative and document text:** Times New Roman and serif fallbacks.
- **Interface labels and metadata:** Arial and sans-serif fallbacks.
- **Archival metadata and timestamps:** Courier New and monospace fallbacks.
- **Reading column:** Centred, with a maximum width of approximately 900px in the preview styling.
- **Text handling:** Components use box sizing and word wrapping to prevent long content from overflowing.
- **Responsive layout:** A mobile breakpoint at 700px reduces outer padding, title sizes, and document spacing.

The design uses borders, inset highlights, subtle gradients, and restrained shadows to suggest velvet, paper, and metal without relying on images.

## 4. Main component catalogue

All components use the `.hgm-` class prefix. Keep the class names and nested structure when reusing the HTML examples.

### Opening and chapter elements

| Component | Purpose |
|---|---|
| `.hgm-open` | Story opening or title page |
| `.hgm-open--minimal` | Minimal opening treatment |
| `.hgm-open--cinematic` | Dark cinematic title panel |
| `.hgm-chap` | Chapter heading |
| `.hgm-chap--ornament` | Chapter heading with decorative ornament |
| `.hgm-chap--left` | Left-aligned chapter heading |
| `.hgm-chap--cinematic` | Dark, dramatic chapter heading |

Opening panels can include a kicker, title, subtitle, decorative rule, epigraph, attribution, dedication, and edition metadata. Chapter panels support chapter number, title, subtitle, date, and epigraph.

### Scene and narrative elements

| Component | Purpose |
|---|---|
| `.hgm-sep--rule` | Simple horizontal scene divider |
| `.hgm-sep--ornament` | Decorative symbol divider |
| `.hgm-sep--dots` | Dotted divider |
| `.hgm-sep--cine` | Cinematic text divider |
| `.hgm-mark` | Context marker for a narrative transition |
| `.hgm-n-std` | Standard prose block |
| `.hgm-n-std--dropcap` | Prose with an opening drop cap |
| `.hgm-n-std--lead` | Prose with small-cap opening line |
| `.hgm-n-mono` | Indented, italic monologue or internal thought |
| `.hgm-n-stream` | Stream-of-consciousness passage |
| `.hgm-n-flash` | Flashback passage |
| `.hgm-n-flash--memory` | Memory-styled passage |
| `.hgm-n-dream` | Dream sequence |
| `.hgm-n-pov` | Point-of-view label |
| `.hgm-n-quote` | Standalone quotation |
| `.hgm-n-quote--scripture` | Left-aligned scripture or formal quotation |

Context markers include variants for flashbacks, memories, time jumps, locations, points of view, and interludes. Inline text helpers include small caps, softened emphasis, uppercase emphasis, and strikethrough.

### Letters and personal records

| Component | Purpose |
|---|---|
| `.hgm-letter` | Personal or formal letter |
| `.hgm-letter--formal` | Formal letter with letterhead treatment |
| `.hgm-diary` | Diary entry |
| `.hgm-diary--fragment` | Fragmented diary entry |
| `.hgm-diary--aged` | Aged-paper diary variation |
| `.hgm-diary--dark` | Dark diary variation |

Letter elements support sender, place, date, recipient, salutation, body, closing, signature, postscript, letterhead, and reference number. Diary elements support entry number, date, metadata, marginal notes, indented passages, crossed-out text, and signatures.

### Digital messages and communication

| Component | Purpose |
|---|---|
| `.hgm-mail` | Email message |
| `.hgm-mail--urgent` | Urgent email variation |
| `.hgm-mail--chapter` | Chapter or plot-specific email variation |
| `.hgm-sms` | SMS or phone-message conversation |
| `.hgm-sms--dark` | Dark message interface |

Email layouts include sender/recipient fields, subject, flags, message body, quoted text, forwarded content, signatures, and legal footers. SMS layouts support contact details, status, date, system notices, incoming and outgoing bubbles, names, and timestamps.

### Documents, news, and transcripts

| Component | Purpose |
|---|---|
| `.hgm-doc` | Formal document or report |
| `.hgm-doc--fraternity` | Dark institutional document |
| `.hgm-doc--file` | File or archival document |
| `.hgm-news` | Newspaper or news article |
| `.hgm-news--campus` | Campus-news layout |
| `.hgm-news--editorial` | Editorial layout |
| `.hgm-tx` | Transcript or recorded exchange |
| `.hgm-tx--readable` | More literary, readable transcript |
| `.hgm-tx--numbered` | Numbered transcript lines |
| `.hgm-tx--dark` | Dark transcript variation |

Document layouts support stamps such as confidential, restricted, draft, and archived; organisational headings; reference numbers; metadata; tables; signatures; and footers.

News layouts support mastheads, datelines, headlines, subtitles, bylines, lead paragraphs, image plates, captions, pull quotes, and information boxes.

Transcript layouts support timestamps, speaker labels, pauses, editorial notes, line numbers, and cut markers.

### Structured records and author notes

| Component | Purpose |
|---|---|
| `.hgm-skel` | Structured record, dossier, or case file |
| `.hgm-skel--dark` | Dark record variation |
| `.hgm-skel--archival` | Monospaced archival variation |
| `.hgm-an` | Author note panel |
| `.hgm-an--open` | Opening author note |
| `.hgm-an--close` | Closing author note |
| `.hgm-an--chapter` | Chapter-specific note |
| `.hgm-an--content` | Content note |
| `.hgm-an--research` | Research note |
| `.hgm-an--thanks` | Acknowledgements |

Structured records can display profiles, timelines, case status, inventories, annotations, labels, and record excerpts. Author notes use a pale panel with dark text for readability against the dark story background.

### Redaction

`.hgm-redact` provides a redaction-style text treatment. It can be used for censored names, classified information, or deliberately obscured details. The CSS includes adjustments for dark document variations.

## 5. Preview contents

The supplied HTML file is a visual component sampler rather than a complete story. It demonstrates the theme with sample text and examples of the available structures, including:
- Main and alternate story-opening panels.
- Chapter heading and narrative formatting.
- Scene separators and context markers.
- Monologue, stream-of-consciousness, flashback, dream, and quotation blocks.
- Letters and diary entries.
- Email and SMS conversations.
- Formal documents, news layouts, and transcripts.
- Structured records and author-note panels.

The sample opening identifies the theme as **Blood Skin** and uses the subtitle **A formatting and component sampler**. The sample narrative is titled **The House at the Waterline**.

## 6. Installation on Archive of Our Own

1. Open **AO3 → My Dashboard → Skins**.
2. Choose **Create Site Skin**.
3. Give the skin a name, such as **Blood Skin**.
4. Open the supplied `Theme Blood Skin.css` file in a text editor.
5. Copy the CSS contents into the AO3 CSS editor.
6. Save the skin.
7. Select **Use** to apply it to your account.
8. Open a work that uses the matching `.hgm-` HTML classes to check the result.

The standalone HTML preview is for browser testing. AO3 work content should contain the component HTML, while the CSS belongs in the Site Skin editor.

## 7. Using the HTML components in a work

- Copy the relevant component structure from the preview HTML.
- Paste it into the work or chapter HTML editor where appropriate.
- Replace the sample text with your own content.
- Preserve the class names exactly. The CSS depends on those names.
- Keep the component's child elements in their intended hierarchy.
- Use the matching modifier class only when you want that variation.

For example, the base opening panel uses `.hgm-open`; the cinematic variation adds `.hgm-open--cinematic`. A standard diary uses `.hgm-diary`; the dark variation adds `.hgm-diary--dark`.

Do not paste the full standalone HTML document, including its `head`, `style`, or `body` elements, into an AO3 work. Use the CSS in the Site Skin and only the relevant component markup in the work.

## 8. Mobile and readability notes

The stylesheet includes responsive adjustments for screens up to 700px wide. These reduce padding, scale down large headings, stack document signature areas, and adapt metadata fields for narrow screens.

Parchment-based artefacts use dark text on pale backgrounds. The author-note panel also has its own dark-text treatment, so it remains readable against the velvet reading surface. Long words and content are allowed to wrap, and tables and images are constrained to the available width.

The HTML preview can be checked at desktop and mobile widths using the browser's responsive design tools.

## 9. Files

The theme package should keep the original filenames:

```text
Theme Blood Skin/
├── README_Theme_Blood_Skin.md
├── Theme Blood Skin.css
└── Theme Blood Skin.html
```

- `Theme Blood Skin.css` — AO3 Site Skin stylesheet.
- `Theme Blood Skin.html` — standalone browser preview and component sampler.
- `README_Theme_Blood_Skin.md` — theme documentation and installation guide.

## 10. Notes

- This is a CSS-and-HTML formatting theme. It does not require external fonts, scripts, or image assets for its core appearance.
- The HTML preview may include browser-only presentation code. AO3 uses the CSS and the component markup, not the standalone preview page as a whole.
- AO3 may handle some HTML and CSS differently from a local browser. Always test the saved Site Skin on an actual AO3 work.
- The theme is designed around its `.hgm-` class system. Avoid renaming classes unless you also update every corresponding CSS selector.
