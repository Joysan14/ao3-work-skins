# Theme: ABOverse

**ABOverse** is a literary-style AO3 Work Skin built around the atmosphere of an old archive: oxblood framing, pale parchment reading surfaces, charcoal details, muted slate, and antique-gold accents. Its typography and decorative details aim to make long-form fiction feel like a carefully kept book or a collection of private records.

## Preview

Open **`Theme ABOverse.html`** in a web browser. The preview uses the stylesheet in this folder directly, so keep the HTML and CSS together. It includes sample work metadata, chapter text, and examples of the theme's custom story elements.

The preview is a local demonstration, not an AO3 page. Google Fonts are requested by the preview for the display typography; if you are offline, the browser will use the fallback fonts.

## Files

| File | Purpose |
|---|---|
| `Theme ABOverse.css` | The AO3 Work Skin stylesheet to paste into AO3. |
| `Theme ABOverse.html` | A standalone browser preview of the theme and its custom formatting elements. |

## Visual direction

| Colour | Hex | Role |
|---|---|---|
| Oxblood | `#4A171F` | Main outer reading-area background |
| Muted wine | `#843D48` | Borders and selected accents |
| Parchment | `#F3F1EC` | Main text panels |
| Charcoal | `#242124` | Dark text and interface-style panels |
| Antique gold | `#B39A70` | Fine rules, highlights, and decorative accents |
| Soft slate | `#B8BBC0` | Secondary borders and muted details |

## Install on Archive of Our Own

1. Open **AO3 → My Dashboard → Skins**.
2. Choose **Create Site Skin**.
3. Give the skin a name, such as **ABOverse**.
4. Paste the full contents of `Theme ABOverse.css` into the CSS field.
5. Save the skin.
6. If you want to use it as your default reading appearance, select **Use** on the saved skin. You can also select it from the Skins page when needed.

AO3's skin editor is the source of truth for compatibility. The standalone preview can demonstrate the CSS in a regular browser, but AO3 may render some interface elements differently.

## Custom formatting classes

The stylesheet includes optional classes for formatting content inside a work. Add the relevant class to an HTML element in your work, using AO3's supported HTML editor. Examples below show the class names and intended use; the complete styling is defined in the CSS.

| Class | Intended use |
|---|---|
| `do-book` | Book-like paragraph treatment, including first-line paragraph indents |
| `do-title`, `do-subtitle` | A custom title and subtitle within the work |
| `do-epigraph` | A centered quotation with an optional citation |
| `do-dropcap` | A decorative first letter |
| `do-pov` | A point-of-view marker |
| `do-thought`, `do-dialogue` | Distinguish internal thoughts and dialogue styling |
| `do-flashback`, `do-memory`, `do-dream` | Visually distinguish shifts in time or recollection |
| `do-break` | Decorative scene break |
| `do-note`, `do-warn`, `do-disclaimer` | Notes, content notices, and disclaimers |
| `do-chat`, `do-chat do-wa` | In-story chat and WhatsApp-style message layouts |
| `do-post`, `do-email` | Social post and email mockups |
| `do-letter`, `do-diary`, `do-poem` | Letter, diary-entry, and poem treatments |
| `do-doc`, `do-card`, `do-receipt` | In-story records, profile cards, and receipts |

Use only the elements you need. The classes are optional; ordinary paragraphs and standard AO3 work metadata remain styled without them.

## Notes and limitations

- Keep the CSS and HTML preview files in the same folder so the preview can find its stylesheet.
- The HTML preview contains fictional sample copy to demonstrate the layout. Replace it with your own test text if you want to check a particular work.
- The stylesheet is intended for AO3 Work Skin use. It is not a general-purpose website theme.
- If you modify the CSS, test it on AO3 at both desktop and mobile widths. Browser previews cannot perfectly reproduce AO3's own page structure or every skin interaction.
- The supplied stylesheet is kept as the theme source. The HTML file is a separate preview document and does not need to be pasted into AO3.

---

**Theme name:** Theme ABOverse  
**Included files:** CSS stylesheet and standalone HTML preview
