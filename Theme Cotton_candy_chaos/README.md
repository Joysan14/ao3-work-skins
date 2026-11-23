# Cotton Candy Riot
### AO3 Work Skin Documentation

**Cotton Candy Riot** is a responsive AO3 Work Skin built around a bright bubblegum-pink page, cotton-candy-white reading panels, near-black typography, and selective midnight-dark interface elements. Its visual direction is playful and pastel, with a sharper editorial and digital-interface edge.

The package includes a CSS stylesheet and a standalone HTML preview:

- `Theme Cotton_candy_chaos.css` — the stylesheet to install as an AO3 Work Skin.
- `Theme Cotton_candy_chaos.html` — a browser preview demonstrating the styling and reusable components.

## 1. Design direction

The final overrides intentionally simplify the earlier textured background. The page canvas is bubblegum pink, while the preface, chapter, and afterword use clean, near-white surfaces. Body copy is forced to a near-black colour for readability.

Dark panels remain available for secure messages, radio/system displays, notification interfaces, and organisation banners. This contrast keeps the pastel palette from making every interface look identical.

## 2. Colour palette

| Role | Colour | Hex |
|---|---|---|
| Main page background | Bubblegum pink | `#F28FB7` |
| Main reading surface | Cotton-candy white | `#FFF9FC` |
| Main text | Near-black | `#141116` |
| Soft pink border | Pale rose | `#E7A4C0` |
| Message bubble / pink accent | Warm bubblegum | `#E989B2` |
| Dark panel background | Ink black | `#17131A` |
| Deep navy | Midnight blue | `#07457D` |
| Blue accent | Strong blue | `#045BA3` |
| Dark rose | Berry pink | `#A84D70` |
| Light pink text on dark panels | Pale blush | `#F4B5D1` |
| Soft blue accent | Powder blue | `#ADD1E7` |
| Pale blue interface surface | Cool blue-white | `#EAF4F9` |
| Secondary muted text (legacy component styling) | Dusty mauve | `#604B5D` |

The final clean-background overrides take precedence over earlier colours where the same selectors are restyled. In particular, the main text colour is `#141116`, and the main reading surface is `#FFF9FC`.

## 3. Typography and reading layout

- **Narrative text:** Georgia with Palatino and other serif fallbacks.
- **Display headings:** Cormorant Garamond / Garamond fallback stacks.
- **Document and chapter headings:** Libre Baskerville / Baskerville fallback stacks.
- **Interface labels:** Arial or Helvetica.
- **Timestamps and system-style text:** Courier New or another monospace fallback.
- **Reading structure:** centred preface, chapter, and afterword surfaces with clear paragraph spacing and responsive padding.

AO3 Work Skins cannot reliably load external web fonts. Font stacks therefore use fonts available on the reader's device, and the exact appearance may vary between operating systems.

## 4. Component catalogue

The stylesheet provides reusable classes for narrative presentation and fictional in-world interfaces.

### Story and narrative formatting

| Component | Main class | Purpose |
|---|---|---|
| Story title / display heading | `.do-title` | Prominent title treatment |
| Subtitle | `.do-subtitle` | Secondary italic heading |
| Epigraph | `.do-epigraph` | Centred quotation and attribution |
| Chapter heading | `.do-chapter` | Chapter number, title, subtitle, ornament |
| Drop cap | `.do-dropcap` | Enlarged opening letter |
| Small-caps lead | `.do-lead` | Introductory emphasis |
| Point-of-view marker | `.do-pov` | Centred POV transition |
| Dialogue / thought | `.do-dialogue`, `.do-thought` | Narrative emphasis |
| Flashback / memory / dream | `.do-flashback`, `.do-memory`, `.do-dream` | Visually distinct narrative passages |
| Pull quote | `.do-pull` | Featured quotation |
| Scene break | `.do-break` | Decorative separators, including dots, tide, and line variants |
| Poem | `.do-poem` | Indented poetic text |
| Highlight | `.do-hl`, `.do-hl-sea` | Inline highlighted text |
| Footnotes | `.do-fnref`, `.do-footnotes` | Footnote markers and notes |

### Notes and reader information

| Component | Main class | Purpose |
|---|---|---|
| Metadata panel | `.do-meta` | Structured work or story information |
| Author's note | `.do-note` | Note panel with heading |
| Endnotes | `.do-endnotes` | Numbered notes |
| Warning | `.do-warn` | Content warning or disclaimer panel |
| Disclaimer | `.do-disclaimer` | Compact fictional-work notice |
| Label | `.do-label` | Small component identifier |

### Personal writing and correspondence

| Component | Main class | Purpose |
|---|---|---|
| Letter | `.do-letter` | Styled letter or handwritten correspondence |
| Signature | `.do-sig` | Signature line or sign-off |
| Diary entry | `.do-diary` | Journal-style passage |
| Date label | `.do-date` | Date or timestamp label |
| Email | `.do-email` | Email header and message body |
| Email fields | `.do-k`, `.do-v` | Sender, recipient, subject and related fields |

### Digital communication and interface cards

| Component | Main class | Purpose |
|---|---|---|
| Chat conversation | `.do-chat` | General messaging interface |
| WhatsApp-style variant | `.do-chat.do-wa` | Alternate chat palette |
| Secure chat | `.do-secure` | Dark, classified or encrypted conversation |
| Message bubble | `.do-msg`, `.do-out` | Incoming and outgoing messages |
| Sender / timestamp | `.do-sender`, `.do-time` | Message metadata |
| Social post | `.do-post` | Social-media-style post |
| Notification | `.do-notify` | App or device notification |
| System message | `.do-system` | Technical/system alert |
| Call interface | `.do-call` | Call log or call notification |
| Voice message | `.do-voice` | Voice-message panel |
| Radio transcript | `.do-radio` | Radio or dispatch communication |
| Bank notification | `.do-bank` | Transaction alert |
| Bank alert / dark variant | `.do-bank-alert`, `.do-bank-dark` | Alert and dark bank notification styles |
| Receipt | `.do-receipt` | Receipt or transaction record |

### Documents and institutional material

| Component | Main class | Purpose |
|---|---|---|
| Document panel | `.do-doc` | General in-world document |
| Document title / label | `.do-doc-title`, `.do-doc-label` | Document hierarchy |
| Document metadata | `.do-docmeta` | Reference, date, author or status details |
| Section heading | `.do-sect` | Internal document section |
| Document variants | `.do-d-personnel`, `.do-d-service`, `.do-d-intel`, `.do-d-brief`, `.do-d-field`, `.do-d-incident`, `.do-d-medical`, `.do-d-inv`, `.do-d-interrog`, `.do-d-casualty`, `.do-d-chain`, `.do-d-corr` | Different institutional document types |
| Dossier | `.do-dossier` | Structured profile or case information |
| Status label | `.do-status` | Open, closed or on-hold status |
| Distribution list | `.do-dist`, `.do-chainlist` | Distribution and chain-of-custody details |
| Classification banner | `.do-class` | Document classification |
| Stamp | `.do-stamp` | Status or handling stamp |
| Redaction | `.do-redact` | Redacted text |
| Missing information | `.do-missing` | Missing or unavailable record |
| News article | `.do-news` | Newspaper or news-page treatment |
| Transcript | `.do-transcript`, `.do-spk` | Transcript and speaker labels |
| Certificate | `.do-cert` | Formal certificate |
| Framed panel | `.do-frame` | Featured or inset content |

### Signatures and organisation branding

The stylesheet includes an add-on for handwritten-style signatures and organisation identity elements.

- `.do-sign` — cursive-style signature.
- `.do-sign-blue`, `.do-sign-red`, `.do-sign-black`, `.do-sign-light` — ink colour variants.
- `.do-sign-sm`, `.do-sign-lg`, `.do-initials`, `.do-sign-flat` — size and shape options.
- `.do-signature` — signature block with printed name and optional role.
- `.do-signature-right`, `.do-signature-center` — alignment options.
- `.do-brand` — compact organisation banner with emblem, name, tagline, and reference.
- `.do-brand-blue`, `.do-brand-red`, `.do-brand-black` — brand colour variants.
- `.do-banner` — wide title-card banner.
- `.do-banner-blue`, `.do-banner-red`, `.do-banner-black` — banner colour variants.

The cursive signature appearance depends on fonts installed on the reader's device.

## 5. Installing the Work Skin on AO3

1. Open **AO3 → Dashboard → Skins**.
2. Choose **Create Work Skin**.
3. Give the skin a name, such as **Cotton Candy Riot**.
4. Open `Theme Cotton_candy_chaos.css` in a text editor.
5. Copy the complete CSS and paste it into the Work Skin CSS field.
6. Save the skin.
7. Open the Work Skin page and select **Use**.
8. Apply the skin to a work through the work's **Associations** or **Work Skin** setting, depending on the posting/editing screen.

Use the CSS file for AO3. The HTML file is a standalone preview and is not uploaded as the Work Skin.

## 6. Viewing the HTML preview

Open `Theme Cotton_candy_chaos.html` in a modern browser. The page includes its own preview shell and embeds the Work Skin CSS, so it can be viewed locally without a server.

The preview demonstrates the appearance of the reading area and a selection of reusable narrative, correspondence, messaging, and document components. The preview shell is for browser presentation only; it is not part of the CSS that should be pasted into AO3.

## 7. Reusing components in a work

To use a component, add the corresponding HTML structure to the work's HTML editor and apply the class names documented in the stylesheet. Keep the outer component classes and nested class names intact because the CSS selectors depend on them.

For example, a basic scene separator can be inserted as:

```html
<hr class="do-break do-break-dots">
```

A POV marker can be inserted as:

```html
<div class="do-pov">Maren</div>
```

A basic warning panel can be inserted as:

```html
<div class="do-warn">
  <span class="do-warn-title">Content Warning</span>
  Drowning (non-graphic), implied family loss.
</div>
```

For more complex components such as chats, emails, documents, and organisation banners, use the full example structures in the HTML preview as the reference. Replace only the sample text and labels unless you are intentionally changing the component.

## 8. Responsive behaviour

The stylesheet includes smaller-screen adjustments. These reduce outer padding, adjust panel spacing and heading sizes, and allow structured fields to stack vertically. Chat bubbles expand to use more of the available width, while document and correspondence panels use narrower internal padding.

The HTML preview also has a separate mobile-friendly outer shell. AO3's own page layout may differ from the local preview, so check the installed skin on both desktop and mobile.

## 9. Customisation notes

- Change the final `CLEAN BACKGROUND OVERRIDES` section to adjust the main page, reading surfaces, and body text.
- Keep body text dark against the near-white panels. Avoid using pale pink for long paragraphs.
- Retain the dark component overrides when using secure chats, radio/system panels, and dark bank notifications.
- If changing message colours, check both incoming and outgoing text, including sender names and timestamps.
- Preserve the `#workskin` selector so styles remain scoped to the work content.
- Make changes in a copy of the CSS first so the original theme remains available.

## 10. Compatibility and accessibility

The stylesheet is designed for AO3's Work Skin environment and includes responsive rules, but AO3 may handle some browser CSS differently from a standalone preview. The HTML preview is a visual reference, not a guarantee that every browser will render every detail identically on AO3.

For readability:

- Keep paragraph text high-contrast.
- Do not rely on colour alone to communicate warnings, status, or classification.
- Use descriptive labels for document status and content warnings.
- Check long names, URLs, and table content on narrow screens.
- Review the final work on desktop and mobile after applying the skin.

---

**Theme:** Cotton Candy Riot  
**Format:** AO3 Work Skin (CSS) + standalone HTML preview  
**Visual identity:** Bubblegum pink, cotton-candy white, near-black text, and midnight interface accents.
