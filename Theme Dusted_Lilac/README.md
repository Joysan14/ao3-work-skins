# Gemini Dusted Lilac — AO3 Work Skin

A decorative Archive of Our Own (AO3) Work Skin with a dark indigo outer frame, pale lilac reading panels, muted plum accents, and a library of reusable story-formatting components.

The accompanying HTML file is a standalone browser preview. It demonstrates the skin using sample story content, fictional documents, messages, notifications, and other inserts.

## Design direction

**Gemini Dusted Lilac** combines a dark, atmospheric indigo background with soft lilac paper-like panels. The overall effect is editorial and archival, with serif typography for prose and clean sans-serif or monospaced typography for interface elements.

### Colour palette

| Colour | Hex | Use |
|---|---|---|
| Deep indigo | `#25264D` | Main Work Skin background and dark headers |
| Midnight indigo | `#1B1B38` | Deep accents, stamps, redactions |
| Plum ink | `#34263B` | Main text on light surfaces |
| Muted plum | `#754A68` | Links, emphasis, borders and labels |
| Dusty lilac | `#9B7897` | Secondary accents and headings |
| Mauve | `#B18A9F` | Borders and decorative details |
| Pale mauve | `#C2A0C0` | Dividers and message details |
| Lavender grey | `#D8C9D9` | Secondary panel backgrounds |
| Soft lilac paper | `#E7DDE8` | Main reading panels |
| Pale lavender | `#F3EDF2` | Cards, email and document surfaces |
| Slate lavender | `#8790C2` | Status and classification accents |

The stylesheet uses dark plum text on pale surfaces and pale text on dark indigo surfaces to improve readability.

## Typography

The stylesheet uses system font stacks so it does not depend on externally hosted fonts.

- **Story prose:** Georgia, Palatino and similar serif fonts.
- **Display titles:** Cormorant Garamond and Georgia fallbacks.
- **Document and chapter headings:** Libre Baskerville and related serif fallbacks.
- **Interface labels:** Arial and Helvetica.
- **System messages and records:** Courier New and other monospace fonts.
- **Signature effects:** Available script fonts with cursive fallbacks.

If a preferred font is not installed on the reader's device, the browser uses the next available fallback.

## What is included

### 1. Work layout and story typography

- Styled AO3 work preface, chapter area and afterword.
- Main title, subtitle, epigraph and metadata panel.
- Chapter title card with number, title, subtitle and ornament.
- Book-style paragraph indentation and justified prose.
- Drop caps, small-cap lead-ins, dialogue and point-of-view labels.
- Italic thoughts and thought panels.
- Flashbacks, memories and dream passages.
- Pull quotes and decorative scene breaks.
- Author notes, warnings, disclaimers, endnotes and footnotes.
- Letters, diary entries and poems.

Useful classes include `.do-title`, `.do-subtitle`, `.do-epigraph`, `.do-meta`, `.do-chapter`, `.do-book`, `.do-justify`, `.do-dropcap`, `.do-lead`, `.do-dialogue`, `.do-thought`, `.do-th`, `.do-thought-bar`, `.do-pov`, `.do-flashback`, `.do-memory`, `.do-dream`, `.do-pull`, `.do-break`, `.do-note`, `.do-warn`, `.do-disclaimer`, `.do-letter`, `.do-diary` and `.do-poem`.

### 2. Organisation and brand elements

- Full-width organisation banners.
- Compact brand strips with initials, organisation name and reference.
- Decorative signatures and signature panels.

Classes include `.do-banner`, `.do-banner-blue`, `.do-banner-red`, `.do-banner-black`, `.do-brand`, `.do-brand-blue`, `.do-brand-red`, `.do-signature`, `.do-signature-blue`, `.do-signature-red` and `.do-signature-sheet`.

### 3. Messages and digital interfaces

- General group chat.
- WhatsApp-style chat using `.do-chat.do-wa`.
- Secure or encrypted chat using `.do-chat.do-secure`.
- Social media posts with avatar, display name, handle and engagement figures.
- Bank transaction cards and security alerts, including light and dark variants.
- Email messages, including a nested reply.
- Notifications, system messages, missed calls and voice-message displays.
- Radio or dispatch transcripts with timestamps and speaker labels.

Related classes include `.do-chat`, `.do-chat-head`, `.do-chat-body`, `.do-day`, `.do-msg`, `.do-out`, `.do-sender`, `.do-time`, `.do-typing`, `.do-post`, `.do-bank`, `.do-bank-alert`, `.do-bank-dark`, `.do-email`, `.do-notify`, `.do-system`, `.do-call`, `.do-voice` and `.do-radio`.

### 4. Fictional documents and records

- Monospaced document panels with labels, titles, references and metadata.
- Personnel and dossier records.
- Document tables, signatures and distribution details.
- Classification banners and stamps.
- Inline and block redactions.
- Status labels for open, on-hold and closed records.
- News articles, datelines and interview transcripts.
- Receipts, certificates and framed passages.
- Endnote and footnote sections.

The document variants include:

| Class | Intended use |
|---|---|
| `.do-d-personnel` | Personnel file |
| `.do-d-service` | Service record |
| `.do-d-intel` | Intelligence report |
| `.do-d-brief` | Briefing document |
| `.do-d-field` | Field report |
| `.do-d-incident` | Incident report |
| `.do-d-medical` | Medical record |
| `.do-d-inv` | Investigation file |
| `.do-d-interrog` | Interrogation record |
| `.do-d-casualty` | Casualty report |
| `.do-d-chain` | Chain-of-custody record |
| `.do-d-corr` | Correspondence record |

Other document helpers include `.do-doc`, `.do-doc-label`, `.do-doc-title`, `.do-docmeta`, `.do-dossier`, `.do-class`, `.do-stamp`, `.do-redact`, `.do-redact-name`, `.do-redact-block`, `.do-status`, `.do-news`, `.do-transcript`, `.do-receipt`, `.do-cert`, `.do-frame`, `.do-sigline` and `.do-dist`.

## Responsive behaviour

The stylesheet contains narrow-screen adjustments at approximately **620px** and additional compact layout rules.

On smaller screens, it:
- Reduces outer and panel padding.
- Allows chat bubbles to use more of the available width.
- Makes document, email and chat panels fit the reading column.
- Stacks dossier labels and values vertically.
- Adjusts photo placeholders and signature entries.
- Keeps bank cards and social posts aligned within the available width.

The HTML preview includes sample content for checking the appearance of these components in a browser. Actual AO3 rendering can differ because AO3 applies its own page structure and stylesheet rules.

## Installation on AO3

1. Open **AO3 → Dashboard → Skins**.
2. Choose **Create Site Skin**.
3. Give the skin a name, such as **Gemini Dusted Lilac**.
4. Copy the CSS from the HTML preview's `<style>` section into the Site Skin CSS editor. Do not paste the HTML document itself.
5. Save the Site Skin.
6. Open the Site Skin and choose **Use**.
7. If you want to use it only on a particular work, create or edit a Work Skin and select it for that work, subject to AO3's available skin settings.

**Important:** The HTML preview contains both the Work Skin CSS and sample HTML. AO3 needs the CSS only. The preview's sample markup is there to demonstrate the class names and component structures.

## Using the components in a work

AO3 work content can use HTML supported by the Archive. To use a component, place the appropriate class on an element in the work's HTML.

For example, a simple scene label:

```html
<p class="do-pov">Austin</p>
```

A chapter title card:

```html
<div class="do-chapter">
  <span class="do-chapter-num">Chapter One</span>
  <span class="do-chapter-title">The Things We Run From</span>
  <span class="do-chapter-sub">A chapter subtitle</span>
  <span class="do-chapter-orn">■■■</span>
</div>
```

A WhatsApp-style chat:

```html
<div class="do-chat do-wa">
  <div class="do-chat-head">
    Mum
    <small>online</small>
  </div>
  <div class="do-chat-body">
    <div class="do-day">Today</div>
    <div class="do-msg">
      Are you eating properly?
      <span class="do-time">18:01</span>
    </div>
    <div class="do-msg do-out">
      Yes. Soup.
      <span class="do-time">18:03</span>
    </div>
  </div>
</div>
```

A document panel:

```html
<div class="do-doc do-d-personnel">
  <div class="do-doc-label">Personnel File</div>
  <span class="do-ref">Ref: PF/0147</span>
  <span class="do-doc-title">Personnel Record</span>
  <p>Document text goes here.</p>
</div>
```

Use the sample HTML in the preview as the reference for the full component structure. Keep the class names unchanged unless you also update the CSS.

## Files

- **`Theme Dusted_Lilac.html`** — standalone browser preview containing the embedded stylesheet and component sampler.
- **AO3 Site Skin CSS** — the CSS portion of the HTML file, copied into AO3's Site Skin editor.

## Notes and compatibility

- The preview is a visual reference, not a guarantee of identical rendering on AO3.
- AO3 sanitises work HTML and restricts which CSS properties and selectors can be used in Site Skins. If a component looks different on AO3, test the relevant CSS there and simplify unsupported rules.
- The stylesheet is built from several successive styling and contrast patches. Later rules override earlier rules when selectors have equal or greater specificity. When editing colours or spacing, check the final rules near the end of the stylesheet as well as the original component definitions.
- One intermediate CSS section contains a legacy comment referring to “Industrial Grunge”; the actual preview title and palette are **Gemini Dusted Lilac**.
- The stylesheet includes a `display: grid` declaration in an email-header rule. If AO3 does not render that layout as expected, replace it with a block/float-based arrangement.
- No JavaScript is required for the visual components. They are static HTML and CSS decorations.

## Credits and use

This is a custom fanfiction formatting and presentation skin. Replace the sample story, organisation names, messages and records with your own content. The preview's fictional names and interface text are examples only.
