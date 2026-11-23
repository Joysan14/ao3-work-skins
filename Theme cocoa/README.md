# Midnight Cocoa — AO3 Work Skin

A dark, atmospheric Archive of Our Own (AO3) Work Skin with a deep blue-green reading surface, cool teal accents, pale document panels, and a restrained editorial style. The accompanying HTML file is a standalone browser preview of the skin and its sample components.

## Files

- `Theme cocoa.css` — stylesheet intended for AO3's Work Skin system.
- `Theme cocoa.html` — standalone HTML preview. It includes the skin styling and example content so the components can be inspected outside AO3.

## Design direction

Midnight Cocoa combines a midnight blue-green frame with cool, pale reading panels. The result is intended to feel atmospheric and cinematic without sacrificing legibility. Teal and blue accents distinguish interface elements, while the light inner panels keep long-form prose and fictional documents readable.

### Core colour palette

| Role | Colour | Hex |
|---|---|---|
| Main outer background | Deep midnight blue | `#0B2B3D` |
| Main text | Dark blue-grey | `#1E3440` |
| Primary teal | Deep teal | `#1F6A80` |
| Secondary teal | Ocean teal | `#4C9AAF` |
| Muted blue | Steel blue | `#3A6379` |
| Deep accent | Dark ocean blue | `#12445A` |
| Blue accent | Slate ocean | `#3F6F85` |
| Pale panel | Cool near-white | `#F6FAFB` |
| Panel border | Misty blue-grey | `#B7D0DA` |
| Soft pale blue | `#E4EEF2` |
| Soft teal | `#9FC3D1` |
| Pale mist | `#DCEBEF` |
| Light blue tint | `#CFE3EA` |
| Additional green accent | `#2A6F63` |

The stylesheet uses some translucent versions of these colours for shadows, borders, and layered backgrounds.

## Typography and reading layout

The skin uses a traditional serif reading style, with Georgia and Palatino-family fallbacks. Interface labels and metadata use smaller, more compact treatments to separate them from the main narrative.

The CSS styles AO3's work content areas, including the preface, chapter content, and afterword. It also provides paragraph spacing, indented book-style paragraphs, justified text helpers, link styling, and responsive sizing for embedded content.

## Component catalogue

The HTML preview demonstrates a broad set of reusable fictional inserts and narrative treatments. The main component families include:

### Story and narrative formatting

- Work title, subtitle, epigraph, and metadata blocks
- Chapter heading and chapter ornament
- Dialogue and internal thoughts
- Drop caps and lead paragraphs
- Point-of-view markers and scene tags
- Flashbacks, memories, dreams, and pull quotes
- Scene breaks and decorative separators
- Book-style and justified paragraph helpers

### Notes and reading aids

- Author notes and endnotes
- Footnote references and footnote sections
- Warning panels and warning titles
- Disclaimers
- Highlighted text and redacted passages

### Personal writing

- Letters and signatures
- Diary entries and date markers
- Poems and poem titles

### Digital communication

- Chat conversations, including incoming and outgoing messages
- WhatsApp-style and secure-chat variants
- Message timestamps, sender labels, day separators, read ticks, and typing indicators
- Social-media-style posts with avatar, display name, handle, and post statistics
- Email layouts with sender/recipient metadata, subject, and message body
- Calls, voice/audio elements, notifications, and system messages

### Documents and institutional interfaces

- Document headers, titles, labels, and metadata
- Reports, briefs, correspondence, incident records, intelligence and personnel files
- Medical, service, investigation, and transcript-style document variants
- Dossiers, chain-of-custody lists, receipts, and records
- Classification labels, stamps, status markers, and redaction blocks
- Organisation/brand marks, banners, certificates, and signatures
- Banking and transaction-style notifications, balances, and transaction amounts

These components are presentation styles. They do not create interactive applications or validate the information placed inside them.

## Using the skin on AO3

1. Open AO3 and go to **Dashboard → Skins**.
2. Choose **Create Site Skin**.
3. Give the skin a name, such as **Midnight Cocoa**.
4. Open `Theme cocoa.css` in a text editor.
5. Copy the complete CSS and paste it into the Site Skin CSS field.
6. Save the skin.
7. Select the saved skin as your active Site Skin.

AO3 may display some elements differently from the standalone preview because AO3 controls the surrounding page layout and sanitises or restricts certain CSS. The stylesheet is scoped to AO3's `#workskin` content area.

## Using the HTML preview

Open `Theme cocoa.html` in a modern browser. No build tools or local server are required for the basic preview.

The preview is a demonstration page, not an AO3 upload file. It contains sample story text and example component markup. Use the CSS file for the actual AO3 Work Skin.

## Reusing components in a work

The preview's HTML is the reference for the component structures and class names. When adding a component to an AO3 work:

1. Copy the relevant example element from the preview.
2. Replace its sample text with your own content.
3. Keep the class names and nested structure intact.
4. Paste the markup into an AO3 chapter or work field that accepts HTML.
5. Preview the work on AO3 and check both desktop and mobile layouts.

For example, changing or removing a class name may cause the corresponding styling to stop applying. Some components use modifier classes such as `do-wa`, `do-secure`, `do-brand-blue`, or document-type classes. Keep both the base class and modifier class where they appear in the example.

## Customisation

You can customise the theme by editing the colour values in `Theme cocoa.css`. For a consistent result:

- Change the outer background and its shadows together if you want to alter the overall atmosphere.
- Keep the reading panel light enough to maintain strong contrast with the dark text.
- Use the teal and blue accents consistently for links, labels, borders, and interface details.
- Check warning panels, muted metadata, and small timestamps separately. These elements can become difficult to read if their contrast is reduced.
- Test long messages, narrow screens, and large blocks of fictional documents after making layout changes.

AO3 supports a limited subset of CSS. Avoid relying on browser-only layout features if AO3 rejects them or renders them inconsistently. The standalone HTML preview may support CSS that AO3 does not.

## Accessibility and readability

- Preserve clear contrast between text and its background.
- Do not use colour alone to communicate warnings, status, or message direction.
- Keep meaningful text in the HTML rather than embedding it in images.
- Check the skin at mobile widths and browser zoom levels.
- Keep timestamps and metadata readable, especially inside chat and document components.

## Suggested project structure

```text
Midnight Cocoa/
├── README.md
├── Theme cocoa.css
└── Theme cocoa.html
```

## Credits and usage

This is a custom AO3 Work Skin and standalone preview. The sample names, messages, organisations, and document content are demonstration material. Replace them with content appropriate to your own work.

If you redistribute or adapt the files, keep the stylesheet and its matching HTML reference together and clearly identify any substantial modifications.
