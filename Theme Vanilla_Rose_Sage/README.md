# Vanilla Rose & Sage — AO3 Work Skin

A reusable Archive of Our Own (AO3) Work Skin with literary layouts and in-story interface components. The supplied files retain the original **Vanilla Rose & Sage** filename and HTML title, but the later stylesheet overrides substantially change the visual treatment to a dark slate/charcoal background with rosewood accents and brushed-metal detailing.

> **Theme naming note:** The stylesheet contains a section explicitly titled “RED VELVET + BRUSHED METAL OVERRIDES”, while the HTML document title says “Vanilla Rose & Sage”. The final appearance is therefore darker and more dramatic than the original light vanilla-and-sage palette suggested by the filename. This README documents the final overrides as well as the reusable component system.

## Files

| File | Purpose |
|---|---|
| `Theme Vanilla_Rose_Sage.css` | Main stylesheet to paste into an AO3 Work Skin. |
| `Theme Vanilla_Rose_Sage.html` | Standalone browser preview. It contains an embedded copy of the CSS and sample story content. |

The HTML preview is for testing and viewing the design outside AO3. Do not paste the entire HTML document into the AO3 CSS editor.

## Design direction

The final override gives the work a dark, cinematic presentation: deep slate surfaces, warm ivory text, rosewood borders and accents, and fine metallic lines. The original component structure remains intact, so the same HTML classes can be reused.

### Core colours

| Colour | Hex | Role |
|---|---|---|
| Deep slate / charcoal | `#2D3A47` | Main page and dark component backgrounds |
| Warm ivory | `#FFF7E6` | Light panels and text on dark surfaces |
| Rosewood | `#B46A72` | Primary accent, borders, rules, links and labels |
| Muted rose | `#8C4D59` | Hover and focus accent |
| Brushed silver-blue | `#A9B7C6` | Outer border and cool metallic detail |
| Pale rose | `#F7C8D3` | Decorative highlights and SMS header |
| Dark rose-red | `#7D1830` | Subtle background glow |
| Warm bronze | `rgba(190,157,130,.55)` | Inset metallic frame detail |

Some components also use translucent warm overlays to create depth and a lightly textured finish.

## Typography

The stylesheet uses system font stacks rather than requiring external font downloads.

- **Georgia / Palatino:** title cards, chapter headings, literary headings and signatures.
- **Times New Roman:** story prose, letters, diary entries and selected quotations.
- **Arial / Helvetica:** labels, metadata, interface elements and compact headings.
- **Courier New:** timestamps, transcript details, references and archival-style metadata.

## Component guide

All component classes use the `hgm-` prefix and are scoped under `#workskin`.

### 1. Opening and chapter layouts

| Main class | Use |
|---|---|
| `.hgm-open` | Story opening or title card |
| `.hgm-open--minimal` | Minimal opening layout |
| `.hgm-open--cinematic` | Dark cinematic title card |
| `.hgm-chap` | Chapter heading block |
| `.hgm-chap--ornament` | Chapter heading with decorative ornament |
| `.hgm-chap--left` | Left-aligned chapter heading |
| `.hgm-chap--cinematic` | Dark chapter heading |
| `.hgm-sep` | Scene divider |
| `.hgm-sep--rule` | Simple horizontal rule |
| `.hgm-sep--ornament` | Decorative symbol divider |
| `.hgm-sep--dots` | Dotted divider |
| `.hgm-sep--cine` | Cinematic text divider |
| `.hgm-mark` | Flashback, memory, time, location, POV or interlude marker |

Opening and chapter blocks include child elements for titles, subtitles, epigraphs, dates, attribution and metadata. For example: `.hgm-open__title`, `.hgm-open__epigraph`, `.hgm-chap__num` and `.hgm-chap__title`.

### 2. Narrative and prose treatments

| Main class | Use |
|---|---|
| `.hgm-n-std` | Standard literary prose |
| `.hgm-n-std--dropcap` | Standard prose with a drop cap |
| `.hgm-n-std--lead` | Opening line in small capitals |
| `.hgm-n-mono` | Indented or reflective passage |
| `.hgm-n-stream` | Stream-of-consciousness passage |
| `.hgm-n-flash` | Flashback or memory panel |
| `.hgm-n-flash--memory` | Memory variation |
| `.hgm-n-dream` | Dream sequence |
| `.hgm-n-dream--left` | Left-aligned dream sequence |
| `.hgm-n-pov` | Point-of-view label and optional location |
| `.hgm-n-quote` | Featured quotation |
| `.hgm-n-quote--scripture` | Left-aligned scripture or formal quotation |
| `.hgm-n-em` | Small-cap emphasis |
| `.hgm-n-soft` | Soft or understated emphasis |
| `.hgm-n-loud` | Uppercase emphasis |
| `.hgm-n-strike` | Strikethrough text |
| `.hgm-sc` | Small-cap text helper |
| `.hgm-redact` | Redacted text effect |

### 3. Letters, diaries and email

| Main class | Use |
|---|---|
| `.hgm-letter` | Letter or formal correspondence |
| `.hgm-letter--formal` | Formal letter with letterhead |
| `.hgm-diary` | Diary or journal entry |
| `.hgm-diary--fragment` | Fragmented diary layout |
| `.hgm-diary--aged` | Aged-paper diary variation |
| `.hgm-diary--dark` | Dark diary variation |
| `.hgm-mail` | Email message |
| `.hgm-mail--urgent` | Urgent email variation |
| `.hgm-mail--chapter` | Chapter-themed email header |

These components include dedicated child classes for sender, recipient, date, subject, message body, forwarding details, signatures, postscript and metadata.

### 4. Messages and transcripts

| Main class | Use |
|---|---|
| `.hgm-sms` | SMS conversation |
| `.hgm-sms--dark` | Dark SMS variation |
| `.hgm-sms__row--in` | Incoming message |
| `.hgm-sms__row--out` | Outgoing message |
| `.hgm-sms__bubble` | Message bubble |
| `.hgm-tx` | Transcript or recorded exchange |
| `.hgm-tx--readable` | More readable transcript typography |
| `.hgm-tx--numbered` | Numbered transcript lines |
| `.hgm-tx--dark` | Dark transcript variation |

SMS components support a contact header, status, date, system messages, speaker names, message bubbles and timestamps. The later contrast-fix section gives incoming bubbles a pale silver-blue fill and outgoing bubbles a rosewood fill.

Transcript components support timestamps, speaker labels, pauses, notes, line numbers, breaks and cut-off markers.

### 5. Documents, news and records

| Main class | Use |
|---|---|
| `.hgm-doc` | Formal document or report |
| `.hgm-doc--fraternity` | Dark fraternity-style document |
| `.hgm-doc--file` | File or archival document |
| `.hgm-news` | Newspaper article |
| `.hgm-news--campus` | Campus newspaper variation |
| `.hgm-news--editorial` | Editorial variation |
| `.hgm-skel` | Structured dossier, case file or record |
| `.hgm-skel--dark` | Dark dossier variation |
| `.hgm-skel--archival` | Monospaced archival record |

Document layouts include stamps, organisation names, titles, reference numbers, metadata fields, section headings, tables, signature blocks and footers. Newspaper layouts include mastheads, datelines, headlines, bylines, lead paragraphs, image plates, captions, pull quotes and information boxes. Dossier layouts support timelines, profiles, case records, status labels, lists, annotations and inventory-style details.

### 6. Author notes and metadata helpers

| Main class | Use |
|---|---|
| `.hgm-an` | Author note or information panel |
| `.hgm-an--open` | Opening note |
| `.hgm-an--close` | Closing note |
| `.hgm-an--chapter` | Compact chapter note |
| `.hgm-an--content` | Content-related note |
| `.hgm-an--research` | Research note |
| `.hgm-an--thanks` | Thank-you note |
| `.hgm-field` | Metadata row |
| `.hgm-field__k` | Metadata label |
| `.hgm-field__v` | Metadata value |

Status and warning helpers include `.hgm-status`, `.hgm-alert` and `.hgm-warning`.

## Responsive behaviour

The stylesheet includes mobile adjustments at **700px and below**. These reduce outer margins and padding, scale down large title and newspaper headings, stack document signature blocks, and adapt metadata labels and values to narrow screens. SMS bubbles are allowed more width on smaller displays.

The layout also applies `box-sizing: border-box`, `max-width: 100%` and word wrapping to help prevent long text and component content from overflowing.

## Installation on AO3

1. Open **AO3 → My Dashboard → Skins**.
2. Select **Create Site Skin**.
3. Give the skin a name, such as *Vanilla Rose & Sage* or *Red Velvet & Brushed Metal*.
4. Paste the contents of `Theme Vanilla_Rose_Sage.css` into the CSS field.
5. Save the skin.
6. Open the skin's page and select **Use**.
7. Add the matching HTML component structures to your work wherever you want the layouts to appear.

AO3 Work Skins style the HTML you place in a work. The CSS alone does not create title cards, letters, messages or dossiers; those elements must be added using the matching classes.

## Basic usage examples

### Story opening

```html
<div class="hgm-open">
  <p class="hgm-open__kicker">A story of power and belonging</p>
  <h1 class="hgm-open__title">A House of Good Men</h1>
  <p class="hgm-open__subtitle">An original work</p>
  <hr class="hgm-open__rule">
  <p class="hgm-open__epigraph">Some places belonged to everyone. Others only pretended to.</p>
</div>
```

### Chapter heading

```html
<div class="hgm-chap">
  <p class="hgm-chap__num">Chapter One</p>
  <h2 class="hgm-chap__title">The Presidency</h2>
</div>
```

### Scene divider

```html
<div class="hgm-sep hgm-sep--ornament">❦</div>
```

### SMS conversation

```html
<div class="hgm-sms">
  <div class="hgm-sms__bar">
    <span class="hgm-sms__contact">Alex</span>
    <span class="hgm-sms__status">online</span>
  </div>
  <div class="hgm-sms__date">Tuesday · 9:12 PM</div>
  <div class="hgm-sms__row hgm-sms__row--in">
    <span class="hgm-sms__bubble">Are you still there?</span>
    <span class="hgm-sms__time">9:12</span>
  </div>
  <div class="hgm-sms__row hgm-sms__row--out">
    <span class="hgm-sms__bubble">I'm here.</span>
    <span class="hgm-sms__time">9:13</span>
  </div>
</div>
```

### Diary entry

```html
<div class="hgm-diary">
  <div class="hgm-diary__head">
    <span class="hgm-diary__no">Entry 04</span>
    <span class="hgm-diary__date">14 October</span>
  </div>
  <div class="hgm-diary__body">
    <p>I heard the gate again. Three knocks, then silence.</p>
  </div>
</div>
```

## Preview

Open `Theme Vanilla_Rose_Sage.html` in a browser to inspect the standalone sample. The preview includes the embedded stylesheet and demonstrates the story opening, chapter layout, prose treatments and supporting in-story components using sample fiction content.

## Customisation notes

- To keep the final dark look, retain the **Red Velvet + Brushed Metal** override section near the end of the stylesheet.
- To return to the earlier light vanilla-paper appearance, review or remove the later colour overrides carefully. Removing them may also remove the final contrast corrections.
- Keep the `hgm-` class names unchanged when editing the HTML unless you also update the corresponding CSS selectors.
- Change the sample text in the HTML preview to test your own story content.
- The stylesheet uses system font stacks, so the appearance may vary slightly across operating systems and browsers.

## Compatibility note

The CSS is scoped primarily to `#workskin` so that its component styles are less likely to affect unrelated page elements. The file includes AO3 layout and mobile compatibility adjustments, but rendering can still vary with AO3's own markup, browser behaviour and future site changes. Check the skin on both desktop and mobile after installation.
