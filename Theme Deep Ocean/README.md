# Deep Ocean — AO3 Work Skin

A literary, coastal-inspired AO3 Work Skin built around deep blue-green ink, muted sea-glass tones, warm paper, sand, and restrained terracotta accents. It combines a clean long-form reading layout with a large library of story inserts, messaging interfaces, phone screens, and archival or classified-document elements.

The supplied `Theme Deep Ocean.html` is a standalone browser preview. It contains the stylesheet inside its `<style>` element and demonstrates the components with sample story content.

## Design direction

Deep Ocean is designed to feel like an annotated novel, an archive, and a collection of found documents. The main reading surface is warm and quiet, while the inserts can resemble letters, records, phone interfaces, institutional paperwork, or digital communication.

The theme includes three page appearances:

- **Default / light:** warm ivory paper with deep ink text.
- **Dark:** deep blue-green page surfaces with pale text and muted sea-glass details.
- **Parchment:** sand-coloured paper with ivory panels and darker muted text for legibility.

The mode class belongs on the `.fic-page` element.

## Colour palette

| Colour | Hex | Use |
|---|---|---|
| Deep ink | `#26383A` | Main text and primary dark details |
| Deep blue-green | `#172B32` | Headings, dark panels, banners |
| Muted sea green | `#526D73` | Labels, rules, secondary text |
| Sea-glass mist | `#A7B3AF` | Soft accents and borders |
| Warm ivory | `#F7F5EF` | Main paper surface |
| Sand | `#EAE5D9` | Metadata, panels, message bubbles |
| Warm stone | `#C1B8A5` | Borders and separators |
| Terracotta | `#A47D68` | Warm accent, warning and diary details |
| Pale blue-green | `#DCE5E1` | Outgoing message bubbles |
| Dark-mode page | `#121F24` | Dark reading surface |
| Dark-mode raised panel | `#1D343C` | Dark-mode cards and inserts |
| Dark-mode accent | `#C49A83` | Warm accent in dark mode |

## Typography

The stylesheet uses serif typography for the main reading experience and sans-serif typography for labels and interface details.

- **Body text:** Source Serif 4, Source Serif Pro, Lora, Georgia, Times New Roman.
- **Titles and display headings:** Cormorant Garamond, Libre Baskerville, Georgia.
- **Interface labels and metadata:** Inter, Arial, Helvetica.
- **Monospaced details:** Courier New for timestamps, references, and technical readouts.

Fallback fonts are included, so the layout remains usable when a preferred font is unavailable.

## Main page layout

The core page structure uses these classes:

- `.fic-page` — main reading surface and mode container.
- `.fic-header` — work title and introductory material.
- `.fic-title` and `.fic-subtitle` — work title and subtitle.
- `.fic-kicker` — small uppercase introductory label.
- `.fic-metadata`, `.fic-section`, `.fic-label`, `.fic-tags`, `.fic-tag` — metadata and tag presentation.
- `.chapter-header`, `.chapter-number`, `.chapter-title`, `.chapter-subtitle` — chapter heading.
- `.chapter-content` — chapter text container.
- `.author-note`, `.note-label`, `.note-ending` — author notes.
- `.end-notes`, `.end-notes-label` — end notes.
- `.fic-divider`, `.scene-break`, `.scene-break-ocean`, `.scene-break-symbol`, `.scene-break-line` — scene separators.

The stylesheet also includes drop caps, quotation styling, internal-monologue treatments, and reusable insert framing.

## Reading and narrative components

| Component | Purpose |
|---|---|
| `.do-book` | Book-style paragraph treatment, including first-line indentation |
| `.do-justify` | Justifies paragraph text |
| `.do-title`, `.do-subtitle` | Additional display title and subtitle |
| `.do-epigraph` | Centred epigraph with optional citation |
| `.do-meta`, `.do-chip` | Compact metadata list and tag-like chips |
| `.do-chapter` | Decorative chapter heading |
| `.do-dialogue` | Dialogue paragraph helper |
| `.do-thought`, `.do-thought-bar`, `.do-th` | Internal thought variations |
| `.do-dropcap`, `.do-lead` | Drop cap and small-caps opening |
| `.do-pov`, `.do-tag` | Point-of-view and section labels |
| `.do-flashback`, `.do-memory`, `.do-dream` | Flashback, memory, and dream passages |
| `.do-pull` | Large pull quote |
| `.do-poem`, `.do-poem-title` | Poem layout |
| `.do-hl`, `.do-hl-sea` | Inline highlighting |
| `.do-fnref`, `.do-footnotes` | Footnote reference and footnote area |
| `.do-break` and variants | Decorative scene breaks |
| `.do-note`, `.do-endnotes`, `.do-warn`, `.do-disclaimer` | Notes, endnotes, warnings, and disclaimers |

There are also utility classes for centring, labels, muted text, and text alignment.

## Communication and digital inserts

The insert library supports fictional documents and in-story digital communication.

| Component | Purpose |
|---|---|
| `.insert`, `.insert-head`, `.insert-body` | Shared insert frame and its header/body |
| `.do-chat` | Compact chat conversation |
| `.do-chat.do-wa` | WhatsApp-inspired conversation variation |
| `.do-chat.do-secure` | Dark, monospaced secure-message variation |
| `.do-msg`, `.do-out`, `.do-sender`, `.do-time`, `.do-day` | Message bubbles, sender, timestamp, and date divider |
| `.do-typing`, `.do-tick` | Typing indicator and message ticks |
| `.do-post` | Social-media post |
| `.do-avatar`, `.do-name`, `.do-handle`, `.do-post-body`, `.do-post-stats` | Social post details |
| `.do-email` | Email layout, including nested replies |
| `.do-email-head`, `.do-email-body`, `.do-k`, `.do-v` | Email header fields and body |
| `.do-notify`, `.do-system` | Notification and system-message panels |
| `.do-call` | Compact phone-call screen |
| `.do-voice`, `.do-wave` | Voice-message style insert |
| `.do-radio` | Radio or dispatch transcript |
| `.do-transcript`, `.do-spk` | Interview or recorded transcript |
| `.do-bank` | Banking notification card |
| `.do-alert` | System alert dialog |
| `.do-lock` | Phone lock screen with notification cards |
| `.notif-list`, `.notif` | Standalone notification list and individual cards |
| `.do-status`, `.batt`, `.sig` | Phone status bar, battery, and signal indicators |

### Banking card variants

The banking component includes these combinations:

- `.do-bank` — standard light card.
- `.do-bank-alert` — alert treatment with a terracotta rule.
- `.do-bank-dark` — dark card.
- `.do-bank-alert.do-bank-dark` — dark alert card.

Use `.do-bank-cr` for incoming/credit amounts and `.do-bank-dr` for outgoing/debit amounts.

### Phone status and battery variants

The battery component uses level classes such as `.batt-100`, `.batt-90`, `.batt-80`, `.batt-70`, `.batt-60`, `.batt-50`, `.batt-40`, `.batt-30`, `.batt-20`, `.batt-10`, and `.batt-5`. Add `.batt-charge` for the charging state. Low battery levels use a red fill.

Notification icon variants include `.notif-icon-msg`, `.notif-icon-mail`, `.notif-icon-bank`, `.notif-icon-alert`, `.notif-icon-call`, and `.notif-icon-cal`.

## Documents, records, and institutional design

The extended component library includes a substantial archive and classified-document system.

| Component | Purpose |
|---|---|
| `.do-doc` | General document or form |
| `.do-doc-label`, `.do-doc-title`, `.do-ref` | Document label, title, and reference number |
| `.do-docmeta`, `.do-sect` | Document metadata and section heading |
| `.do-dossier` | Label-and-value dossier details |
| `.do-photo` | Photo placeholder |
| `.do-lh` | Institutional letterhead |
| `.do-sigline` | Signature line |
| `.do-chainlist` | Chain-of-custody or event sequence |
| `.do-dist` | Distribution list |
| `.do-class` | Full-width classification banner |
| `.do-stamp` | Inline status or classification stamp |
| `.do-redact`, `.do-redact-name`, `.do-redact-block` | Inline, name, and block redactions |
| `.do-missing` | Missing-record marker |
| `.do-news`, `.do-dateline` | Newspaper-style insert |
| `.do-receipt` | Receipt with tabular line items |
| `.do-cert` | Certificate |
| `.do-frame` | Framed passage |
| `.do-sign`, `.do-signature` | Handwritten-style signature and signature block |
| `.do-brand`, `.do-banner` | Organisation identity card and full-width organisation banner |

### Document style variants

The `.do-doc` family includes optional accent classes:

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

These alter border placement, thickness, or accent treatment to help distinguish document types.

### Classification banners and stamps

Classification styles include:

- `.do-class-ts` / `.do-stamp-ts` — Top Secret
- `.do-class-s` / `.do-stamp-s` — Secret
- `.do-class-c` / `.do-stamp-c` — Confidential
- `.do-class-rs` / `.do-stamp-rs` — Restricted
- `.do-class-dc` / `.do-stamp-dc` — Declassified
- `.do-class-fouo` / `.do-stamp-fouo` — For Official Use Only

The base `.do-class` and `.do-stamp` styles can also be used for labels such as Received, Pending, or Denied. The sample HTML demonstrates the available variants.

### Signature and identity variations

Signature styling supports colour and size modifiers such as `.do-sign-blue`, `.do-sign-red`, `.do-sign-black`, `.do-sign-light`, `.do-sign-sm`, `.do-sign-lg`, `.do-initials`, and `.do-sign-flat`. Signature blocks can be aligned with `.do-signature-right` or `.do-signature-center`.

Organisation cards and banners also have blue, red, and black variants, including `.do-brand-blue`, `.do-brand-red`, `.do-brand-black`, `.do-banner-blue`, `.do-banner-red`, and `.do-banner-black`.

## Appearance modes

The mode class is added to the main `.fic-page` element.

```html
<div class="fic-page">
  <!-- Default light appearance -->
</div>

<div class="fic-page mode-dark">
  <!-- Dark appearance -->
</div>

<div class="fic-page mode-parchment">
  <!-- Parchment appearance -->
</div>
```

The dark mode changes the reading surface, headings, labels, inserts, messages, document panels, phone interfaces, and notification colours. Lock-screen notification cards intentionally remain light so they continue to read as phone notifications.

Parchment mode uses a sand-coloured page with ivory panels. Its muted text is darkened compared with the default mode to preserve contrast.

## AO3 installation

1. Open **AO3 → My Dashboard → Skins**.
2. Choose **Create Site Skin**.
3. Give the skin a name, such as `Deep Ocean`.
4. Copy the CSS from the `<style> ... </style>` section of the supplied HTML preview into the Site Skin CSS field.
5. Save the skin.
6. Open the saved skin and choose **Use**.

The HTML preview itself is not uploaded as the AO3 Site Skin. AO3 needs the CSS.

### Important: scope and mode placement

The stylesheet is scoped to `#workskin`, so it is intended for use as a Work Skin. The `.mode-dark` or `.mode-parchment` class must be placed on `.fic-page` in the work HTML. For example:

```html
<div class="fic-page mode-dark">
  <!-- Your work content -->
</div>
```

If you are using the classes in an AO3 work, make sure the relevant wrapper and component markup are included in the work's HTML. The preview file is a reference for the expected structure.

## Using the HTML preview

Open `Theme Deep Ocean.html` in a modern web browser to view the sample layout and component gallery. The file is self-contained and includes its CSS internally.

The preview demonstrates:

- Work and chapter headings.
- Light, dark, and parchment appearance rules in the stylesheet.
- Narrative formatting and scene breaks.
- Letters, diaries, poems, and quotations.
- Chat, WhatsApp-style, secure chat, social posts, email, bank cards, and phone UI.
- Radio and interview transcripts.
- Classified banners, stamps, dossiers, redactions, receipts, certificates, signatures, and organisation branding.

The preview is a visual reference. It does not automatically install the skin on AO3 or switch the AO3 page mode.

## Responsive behaviour

The stylesheet includes a mobile breakpoint at `42em` (approximately 672px, depending on browser font sizing).

At smaller widths it:

- Reduces outer and page padding.
- Scales down work and chapter titles.
- Allows inserts to fit the available width.
- Expands message bubbles slightly while retaining their alignment.
- Changes document label/value rows to a vertical layout.
- Reduces padding on letters and diary inserts.
- Reflows signature, photo, and dossier elements for narrow screens.
- Centres insert components within the chapter content.

The CSS uses a single-column, float-based approach for many document fields rather than relying on a complex grid layout.

## Customisation

You can customise the skin while retaining its structure:

- Change the palette by editing the colour values in the stylesheet.
- Adjust the reading width through `.fic-page` and the outer `#workskin` wrapper.
- Change the serif and sans-serif font stacks in the base page and component rules.
- Add a mode class to `.fic-page` to use the dark or parchment palette.
- Combine modifier classes to create variations, such as `.do-chat do-wa`, `.do-bank do-bank-dark`, or `.do-doc do-d-medical`.
- Keep the `#workskin` prefix on selectors so the styling remains scoped to the work area.

When editing for AO3, prefer conservative CSS and test the result in both desktop and mobile layouts. Font availability can vary by device, so retain sensible fallback fonts.

## Files

- **`Theme Deep Ocean.html`** — standalone browser preview containing the embedded CSS and example markup.
- **AO3 Site Skin CSS** — use the stylesheet content from the HTML file's `<style>` block when creating the AO3 Work Skin.

## Notes and limitations

- The sample story text and fictional institutions in the HTML are demonstration content. Replace them with your own material.
- Some font names are fallbacks rather than guaranteed installed fonts.
- The preview demonstrates the component structure, but actual AO3 rendering can differ from a local browser preview.
- The theme styles presentation only. It does not create interactive phone behaviour, working notifications, or functional document controls.
