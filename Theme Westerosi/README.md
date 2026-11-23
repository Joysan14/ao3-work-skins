# Westerosi — AO3 Work Skin

A dark, medieval-inspired AO3 Work Skin built around the atmosphere of *Westeros*: aged parchment, weathered stone, muted metal, deep wine-red accents, and formal book typography. The theme pairs a shadowed outer reading surface with dark charcoal story panels and restrained antique-gold detailing.

## Files

- `Theme Westerosi.css` — the stylesheet to install in your AO3 Work Skin.
- `Theme Westerosi.html` — a standalone browser preview and component sampler. It includes embedded CSS and example markup for the theme's visual elements.

## Visual direction

The design aims for an archival, courtly, and slightly weathered look rather than a bright fantasy aesthetic. Its main visual features include:

- A near-black outer background with subtle linear texture and a deep red glow.
- Charcoal reading panels with fine antique-gold inner borders.
- Warm parchment and aged-ivory text.
- Muted bronze, stone-grey, and wine-red accents.
- Serif typography for a literary, old-world reading experience, with sans-serif and monospaced text for labels, records, and interface-like inserts.

### Core colour palette

| Colour | Hex | Use |
|---|---|---|
| Near-black | `#191A1C` | Outer background and dark surfaces |
| Charcoal | `#222426` | Main panel and document surfaces |
| Dark slate | `#292B2D` | Secondary dark panels and headers |
| Warm parchment | `#E5DDCC` | Light paper surfaces and contrast text |
| Aged ivory | `#D8D0C1` | Main text, borders, and pale details |
| Stone grey | `#55504A` | Muted labels, outlines, and borders |
| Antique gold | `#B08A52` | Decorative borders and highlights |
| Muted bronze | `#A99C85` | Secondary accents and fine details |
| Wine red | `#783B3D` | Strong accent, warnings, and red banner variants |
| Deep red | `#8B3035` | Red signature ink |
| Blue-grey | `#43515A` | Blue signature and banner variant |
| Warm gold | `#C49B62` | Links and highlighted text |

## Typography

The theme uses a literary serif stack led by Libre Baskerville and Crimson Text, with Palatino and Georgia fallbacks. Cormorant Garamond and related serif fonts are used for display titles and decorative headings. Arial is used for compact labels and metadata, while Courier New is used for timestamps, system messages, and document-style details.

AO3 Work Skins cannot load external web fonts. Font appearance therefore depends on the fonts installed on the reader's device, and may vary between Windows, macOS, Android, and iOS.

## Included components

The stylesheet provides a broad set of reusable `do-` components for presenting both ordinary prose and in-world materials.

### Story and chapter presentation

- Work title, subtitle, epigraph, byline, and metadata treatments.
- Chapter number, title, subtitle, and ornamental divider.
- Point-of-view labels, dialogue spacing, thoughts, drop caps, small-caps lead-ins, and justified prose.
- Flashbacks, memories, dreams, pull quotes, and scene-break variations.
- Notes, endnotes, disclaimers, and warning panels.

### Letters and personal writing

- Letters with paper-like styling and signature placement.
- Diary entries with date labels.
- Poetry blocks and poem titles.
- Footnote references and footnote sections.

### Digital communication and interface inserts

- General chat and message bubbles.
- WhatsApp-style chat variant (`do-wa`).
- Secure or encrypted chat variant (`do-secure`).
- Social-media-style posts and profile details.
- Email layouts with sender/recipient/subject fields.
- Notifications, system alerts, calls, missed-call labels, voice-message panels, and radio/transmission logs.
- Banking notifications, including credit, debit, alert, and dark variants.

### Documents, records, and institutional materials

- Formal document panels, document headings, metadata, section labels, and signature lines.
- Personnel, service, intelligence, briefing, field, incident, medical, inventory, interrogation, casualty, chain-of-custody, and correspondence variants.
- Dossiers, distribution lists, status labels, classification banners, stamps, and redaction blocks.
- Newspaper-style layouts, transcripts, receipts, certificates, framed inserts, and highlighted text.

### Signatures and organisation branding

The add-on section includes handwritten-style signature treatments, formal signature blocks, initials, and organisation banners.

- Signature ink variants: black, blue, and red.
- Signature sizes and flat/initials variants.
- Light signatures for dark panels.
- Signature blocks with printed names and optional titles.
- Compact organisation banners with emblem, organisation name, tagline, and reference text.
- Wide title-card banners in black, blue, and red variants.

## Responsive behaviour

The stylesheet includes a narrow-screen layout adjustment at approximately `700px`. It reduces outer and panel padding, scales down large headings, allows signature lines to use the available width, and adapts document, chat, and other inserts to smaller screens. Tables and images are constrained to the available width, and long text is allowed to wrap.

## Installation on AO3

1. Open **AO3 → Dashboard → Skins**.
2. Choose **My Work Skins**, then select **Create Work Skin**.
3. Give the skin a name, such as `Westerosi`.
4. Open `Theme Westerosi.css` in a text editor.
5. Copy the complete CSS and paste it into the Work Skin CSS field.
6. Save the Work Skin.
7. Open a work, choose **Edit**, and select the new skin under **Work Skin**.

The CSS file is the file to install. Do not paste the HTML preview into the AO3 CSS editor.

## Previewing the theme

Open `Theme Westerosi.html` in a browser to view the standalone preview. The HTML file is intended as a visual reference and component sampler. It contains its own embedded styles and sample markup, so it can be viewed independently of AO3.

Use the preview to inspect the appearance of the components before adding their corresponding HTML snippets to a work.

## Using the components

The component styles are activated by their class names. Add the relevant class to the HTML element in your AO3 work, following the example markup in the preview. Keep the class names unchanged, including the `do-` prefix.

For example, the stylesheet documents patterns for:
- A signature: `do-sign` plus an ink colour class.
- A signature block: `do-signature` containing a signature and printed-name line.
- A compact brand banner: `do-brand` plus a colour variant.
- A wide organisation banner: `do-banner` plus a colour variant.

The exact structure and nesting matter. Refer to the HTML preview and the usage comments in the CSS when copying a component.

## Compatibility notes

- The stylesheet is scoped primarily under `#workskin` to style work content rather than the entire AO3 site.
- The HTML preview is a separate browser document, not an AO3 upload format.
- AO3 may restrict or handle some CSS properties differently from a regular browser. The AO3 stylesheet is the authoritative version for use on the site.
- Decorative cursive signatures use device-installed font fallbacks. Their appearance will not be identical on every device.
- The theme uses text and border contrast to distinguish light paper inserts from dark panels. Check any customised text or added HTML against both surfaces for readability.

## Suggested repository structure

```text
Westerosi/
├── README.md
├── Theme Westerosi.css
└── Theme Westerosi.html
```

## Credits and use

This is a custom AO3 Work Skin and preview package. The HTML file demonstrates the stylesheet's components; adapt the sample text, names, organisation marks, and in-world records to suit your own work.
