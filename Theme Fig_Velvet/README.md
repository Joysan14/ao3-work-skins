# Fig & Velvet — AO3 Work Skin

A dark, literary AO3 Work Skin with a velvet-toned reading surface, warm parchment panels, muted metallic details, and a collection of in-story document components.

The accompanying `Theme Fig_Velvet.html` is a standalone preview and component sampler. It demonstrates the CSS and provides example HTML for the reusable elements.

## Design direction

**Fig & Velvet** combines a dark, atmospheric reading environment with warm archival paper. The main reading area uses near-black plum and deep velvet tones. Letters, reports, emails, transcripts, and other artefacts use parchment-like surfaces so that they read as objects within the story.

The visual language is suited to fiction involving family histories, secrets, archives, investigations, correspondence, testimony, and other document-led storytelling.

## Colour palette

| Colour | Hex | Use |
|---|---|---|
| Velvet black | `#160E1C` | Main reading background |
| Deep plum | `#2A1B35` | Inset panels and dark headers |
| Archive violet | `#492E65` | Secondary headings and labels |
| Fig plum | `#6E296C` | Accent panels and outgoing message bubbles |
| Muted red | `#A64B55` | Urgent labels, stamps, and emphasis |
| Burnished amber | `#D47C18` | Metallic accent and highlights |
| Champagne parchment | `#E8BF81` | Fine borders and warm highlights |
| Warm ivory | `#F4E9D8` | Text on dark surfaces and paper panels |
| Pale lavender-grey | `#C9BFD1` | Secondary metallic accent |
| Brushed silver-lilac | `#D6C5D1` | Borders and fine detailing |

## Typography

The stylesheet uses system font stacks rather than externally hosted fonts.

- **Georgia / Palatino:** title treatments, headings, and literary text.
- **Times New Roman:** body passages, letters, and diary entries.
- **Arial / Helvetica:** interface labels, metadata, and compact headings.
- **Courier New:** timestamps, transcript details, references, and archival identifiers.

## Components

All component classes use the `hgm-` prefix.

### Story structure and navigation

| Component | Purpose |
|---|---|
| `.hgm-open` | Opening title panel with kicker, title, subtitle, epigraph, dedication, and metadata |
| `.hgm-open--minimal` | Restrained title-panel variation |
| `.hgm-open--cinematic` | Darker, more dramatic opening variation |
| `.hgm-chap` | Chapter heading with number, title, subtitle, date, and epigraph |
| `.hgm-chap--ornament` | Chapter heading with decorative ornament |
| `.hgm-chap--left` | Left-aligned chapter heading |
| `.hgm-chap--cinematic` | Dark cinematic chapter heading |
| `.hgm-sep` | Scene or section divider |
| `.hgm-sep--rule` | Fine horizontal rule |
| `.hgm-sep--ornament` | Decorative glyph divider |
| `.hgm-sep--dots` | Dotted divider |
| `.hgm-sep--cine` | Cinematic text divider |
| `.hgm-mark` | Context marker for a change in scene or narrative frame |

Narrative marker variants include:

- `.hgm-mark--flashback`
- `.hgm-mark--memory`
- `.hgm-mark--timejump`
- `.hgm-mark--location`
- `.hgm-mark--pov`
- `.hgm-mark--interlude`

### Narrative text treatments

| Component | Purpose |
|---|---|
| `.hgm-n-std` | Standard prose block with paragraph indentation |
| `.hgm-n-std--dropcap` | Enlarged first letter |
| `.hgm-n-std--lead` | Small-cap opening line |
| `.hgm-n-mono` | Indented, italicised internal passage |
| `.hgm-n-stream` | Stream-of-consciousness passage |
| `.hgm-n-stream__drift` | Indented drifting line |
| `.hgm-n-stream__fade` | Faded line |
| `.hgm-n-flash` | Flashback or inset memory passage |
| `.hgm-n-flash--memory` | Memory-specific variation |
| `.hgm-n-dream` | Dream sequence |
| `.hgm-n-dream--left` | Left-aligned dream passage |
| `.hgm-n-pov` | Point-of-view label |
| `.hgm-n-quote` | Standalone literary quotation |
| `.hgm-n-quote--scripture` | Left-aligned quotation with verse marker |

Inline helpers:

- `.hgm-n-em` — small capitals
- `.hgm-n-soft` — softer italic emphasis
- `.hgm-n-loud` — uppercase emphasis
- `.hgm-n-strike` — struck-through text
- `.hgm-redact` — redacted text
- `.hgm-sc` — small-cap text

### Letters, diaries, and correspondence

| Component | Purpose |
|---|---|
| `.hgm-letter` | Formal or personal letter |
| `.hgm-letter--formal` | Formal letter variation with letterhead |
| `.hgm-diary` | Journal or diary entry |
| `.hgm-diary--fragment` | Fragmented diary treatment |
| `.hgm-diary--aged` | Aged-paper variation |
| `.hgm-diary--dark` | Dark diary variation |
| `.hgm-mail` | Email panel |
| `.hgm-mail--urgent` | Urgent email variation |
| `.hgm-mail--chapter` | Chapter-specific email variation |
| `.hgm-sms` | Text-message conversation |
| `.hgm-sms--dark` | Dark message interface |

The correspondence components include dedicated sub-elements for sender, recipient, date, salutation, body, signature, postscript, email fields, subject, forwarded messages, quoted replies, message bubbles, timestamps, and status labels.

### Records, reports, and media

| Component | Purpose |
|---|---|
| `.hgm-doc` | Formal document or report |
| `.hgm-doc--fraternity` | Dark institutional document |
| `.hgm-doc--file` | File or archival document variation |
| `.hgm-news` | Newspaper or news article |
| `.hgm-news--campus` | Campus-news layout |
| `.hgm-news--editorial` | Editorial layout |
| `.hgm-tx` | Interview or audio transcript |
| `.hgm-tx--readable` | More literary transcript text |
| `.hgm-tx--numbered` | Transcript with line numbering |
| `.hgm-tx--dark` | Dark transcript panel |
| `.hgm-skel` | Case file, evidence record, or investigation summary |
| `.hgm-skel--dark` | Dark case-file variation |
| `.hgm-skel--archival` | Monospaced archival variation |

Document sub-elements support stamps, organisation names, reference numbers, metadata, section headings, tables, signature lines, and footers. News sub-elements support mastheads, headlines, datelines, bylines, image placeholders, captions, pull quotes, and related-record boxes. Transcript sub-elements support speakers, timestamps, pauses, recording notes, and section breaks. Case-file sub-elements support profiles, timelines, evidence lists, status labels, annotations, and record labels.

### Author notes

`.hgm-an` provides a styled author-note panel.

Available variants:

- `.hgm-an--open`
- `.hgm-an--close`
- `.hgm-an--chapter`
- `.hgm-an--content`
- `.hgm-an--research`
- `.hgm-an--thanks`

Sub-elements include `.hgm-an__label`, `.hgm-an__title`, `.hgm-an__body`, `.hgm-an__list`, `.hgm-an__refs`, and `.hgm-an__sign`.

## Basic HTML examples

### Opening title panel

```html
<div class="hgm-open">
  <p class="hgm-open__kicker">A story in documents and memory</p>
  <h1 class="hgm-open__title">Fig &amp; Velvet</h1>
  <p class="hgm-open__subtitle">A story title or subtitle</p>
  <hr class="hgm-open__rule"/>
  <blockquote class="hgm-open__epigraph">
    “The past is never finished with the living.”
    <span class="hgm-open__attrib">An old family saying</span>
  </blockquote>
  <p class="hgm-open__meta">Archive edition · No. 07</p>
</div>
```

### Chapter heading

```html
<div class="hgm-chap">
  <p class="hgm-chap__num">Chapter One</p>
  <h2 class="hgm-chap__title">The House at the Waterline</h2>
  <p class="hgm-chap__subtitle">Where the record begins</p>
  <p class="hgm-chap__date">The seventh day of the frost moon</p>
</div>
```

### Text-message exchange

```html
<div class="hgm-sms">
  <div class="hgm-sms__bar">
    <span class="hgm-sms__contact">Elias</span>
    <span class="hgm-sms__status">online</span>
  </div>
  <p class="hgm-sms__date">Today · 21:04</p>
  <div class="hgm-sms__row hgm-sms__row--in">
    <span class="hgm-sms__name">Elias</span>
    <span class="hgm-sms__bubble">Are you at the house?</span>
    <span class="hgm-sms__time">21:04</span>
  </div>
  <div class="hgm-sms__row hgm-sms__row--out">
    <span class="hgm-sms__name">You</span>
    <span class="hgm-sms__bubble">I just arrived.</span>
    <span class="hgm-sms__time">21:05</span>
  </div>
</div>
```

### Case file

```html
<div class="hgm-skel">
  <p class="hgm-skel__kicker">Case file · Greyhaven</p>
  <h3 class="hgm-skel__title">The North Residence</h3>
  <p class="hgm-skel__sub">Investigation summary</p>
  <div class="hgm-skel__head">
    <span class="hgm-skel__label">Case status</span>
    <span class="hgm-skel__status hgm-skel__status--open">Open</span>
  </div>
  <div class="hgm-skel__profile">
    <p class="hgm-skel__name">Maren Voss</p>
    <p class="hgm-skel__role">Primary witness</p>
  </div>
</div>
```

## Installation on Archive of Our Own

1. Open **AO3 → My Dashboard → Skins**.
2. Choose **Create Site Skin**.
3. Give the skin a name, such as `Fig & Velvet`.
4. Copy the CSS from the HTML file's `<style>` sections into the Site Skin CSS editor. Do not copy the HTML document structure.
5. Save the skin.
6. Open the work, choose **的Work Skin** in the work's settings, and select the new skin. The exact label may vary slightly in AO3's interface.
7. Add the relevant component HTML to the work text using AO3's HTML editor.

**Important:** The standalone HTML preview includes example markup and embedded CSS. AO3 needs the CSS in the Site Skin and only the component markup in the work. Do not paste the full HTML document into the work.

## Responsive behaviour

The stylesheet includes a mobile breakpoint at `700px`. At narrower widths it:

- Reduces the outer reading-surface width and padding.
- Reduces title and newspaper masthead sizing.
- Changes document signature columns to a single column.
- Reduces padding on letters, diaries, emails, documents, news panels, transcripts, and case files.
- Allows long content to wrap within component boundaries.

The layout also uses `box-sizing`, `max-width`, and word-wrapping rules to reduce horizontal overflow.

## AO3 compatibility notes

- The components are built with ordinary HTML elements and CSS class selectors.
- The stylesheet uses system font stacks; it does not require external font loading or JavaScript.
- The preview contains decorative gradients, shadows, and other visual treatments. AO3 may render some details differently depending on its CSS sanitisation and the reader's site settings.
- The HTML file contains several successive theme and contrast override sections. CSS rules appearing later in the file take precedence when selectors have equal specificity. Keep the final overrides when extracting the complete stylesheet.
- The stylesheet includes preview-oriented `body` styling. AO3 Site Skins generally apply to AO3's own page structure, so the standalone page background may not transfer exactly.
- Test the skin on desktop and mobile after installation. Check especially long emails, transcript lines, tables, stamps, and nested document content.

This README describes the supplied HTML and its visible CSS structure. It does not claim that the skin has been independently tested on AO3.

## File guide

- `Theme Fig_Velvet.html` — standalone preview, embedded stylesheet, and example markup.
- `README_Fig_and_Velvet.md` — component guide, palette reference, installation instructions, and compatibility notes.
