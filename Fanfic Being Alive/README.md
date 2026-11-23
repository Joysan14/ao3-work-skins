# Fanfic Being Alive — AO3 Work Skin

A literary, coastal-inspired AO3 work skin designed for long-form fiction, internal monologue, and story inserts. The visual style combines deep ink and muted teal with warm paper tones and a restrained terracotta accent.

The accompanying HTML file is a standalone browser preview. Its sample story is titled **“The Tide Remembers”** and demonstrates the skin's components and three display modes.

## Files

- **`Fanfic Being Alive.css`** — the stylesheet to paste into an AO3 Site Skin.
- **`Fanfic Being Alive.html`** — a standalone preview page showing the stylesheet in use, including sample chapter content and interface elements.

Keep the CSS and HTML files together for your own reference. The HTML preview contains its own embedded copy of the styling, so it can be opened independently in a browser.

## Design direction

The skin uses a calm, literary editorial aesthetic: soft off-white paper, deep blue-green ink, misty teal details, and warm terracotta accents. Serif typography gives the story text a book-like feel, while small uppercase sans-serif labels distinguish metadata and interface elements.

### Colour palette

| Role | Colour | Hex |
|---|---|---|
| Main ink | Deep muted green-grey | `#26383A` |
| Deep ink | Dark blue-green | `#172B32` |
| Muted teal | Slate teal | `#526D73` |
| Mist | Pale grey-green | `#A7B3AF` |
| Paper | Warm off-white | `#F7F5EF` |
| Sand | Soft beige | `#EAE5D9` |
| Line | Warm grey-beige | `#C1B8A5` |
| Terracotta | Muted warm brown | `#A47D68` |
| Outer backdrop | Soft stone grey | `#ddd9cf` |

Dark mode introduces deeper blue-green surfaces and pale text. Parchment mode uses warmer paper surfaces and slightly darker muted text.

## Display modes

The stylesheet includes three modes:

1. **Light (default)** — warm off-white page, dark ink text, muted teal details, and sand-coloured panels.
2. **Dark** — deep blue-green page and panels, pale text, mist-coloured secondary labels, and a soft terracotta accent.
3. **Parchment** — a warmer sand-toned page with lighter paper panels and adjusted text contrast.

In the HTML preview, use the Light, Dark, and Parchment buttons at the top to switch modes. The preview's JavaScript only changes the mode class for demonstration; it is not required for AO3.

To use a mode in the markup, place the relevant class on the `.fic-page` element:

```html
<div class="fic-page">
  <!-- Light mode -->
</div>

<div class="fic-page mode-dark">
  <!-- Dark mode -->
</div>

<div class="fic-page mode-parchment">
  <!-- Parchment mode -->
</div>
```

## Main styling features

### Story layout and typography

- Centred work header with kicker, title, and subtitle.
- Chapter number, chapter title, and chapter subtitle.
- Comfortable reading column and generous paragraph spacing.
- Optional drop caps using `.dropcap`.
- Metadata and tag panels.
- Author notes and end notes.
- Decorative scene breaks in several styles.

### Narrative and text treatments

- `.thought` — inline internal thought, italicised in teal.
- `.thought-block` — longer private thoughts with a dotted vertical rule.
- `.thought-who` — optional small label identifying the speaker of a thought block.
- `.thought-stream` — centred, fragmented or intrusive thoughts.
- `.fic-quote` — quoted or remembered speech with a terracotta left border.

### Story inserts and in-world interfaces

The shared `.insert` styling supports a range of fictional artefacts and interface elements:

- `.do-chat` — compact text-message conversation.
- `.do-email` — email with sender, recipient, date, subject, signature, and attachment details.
- `.do-post` — social-media-style post.
- `.do-notify` — reminder or notification panel.
- `.do-system` — centred system message.
- `.do-letter` — letter layout.
- `.do-diary` — diary entry.
- `.do-doc` — document or form with labelled rows.
- `.do-call` — phone-call screen, including incoming-call and connected-call layouts.
- `.do-transcript` — recorded interview or dialogue transcript.

### Phone interface elements

The stylesheet also includes reusable phone UI details:

- `.do-status` — status bar with time, network, signal strength, and battery.
- `.batt` and `.batt-fill` — battery icon with level classes such as `.batt-100`, `.batt-50`, `.batt-20`, `.batt-10`, and `.batt-5`.
- `.batt-charge` — green charging indicator.
- `.do-lock` — lock screen with clock, date, and notifications.
- `.notif-list` and `.notif` — standalone notification cards.
- Notification icon variants for messages, email, banking, alerts, calls, and calendar items.
- `.do-alert` — system alert panel, such as a low-battery warning.

## Scene-break options

Use the following classes on an `<hr>` element:

```html
<hr class="fic-divider">
<hr class="scene-break">
<hr class="scene-break-ocean">
<hr class="scene-break-symbol">
<hr class="scene-break-line">
```

They provide different visual separators, including repeated wave-like marks, asterisks, an ocean-inspired mark, a diamond symbol, and a short horizontal rule.

## Installing the CSS on AO3

1. Open **AO3 → Dashboard → Skins**.
2. Select **My Site Skins**.
3. Choose **Create Site Skin**.
4. Give the skin a name, such as **Fanfic Being Alive**.
5. Paste the contents of `Fanfic Being Alive.css` into the CSS field.
6. Save the skin.
7. Select **Use** to apply it.

The stylesheet is scoped to `#workskin`, so its rules are intended to style work content rather than the wider AO3 interface.

## Using the HTML preview

Open `Fanfic Being Alive.html` in a modern web browser. It includes:

- A sample story page titled **“The Tide Remembers”**.
- Examples of the narrative treatments and insert components.
- Light, Dark, and Parchment preview controls.
- Responsive adjustments for narrower screens.

The HTML file is a demonstration and reference. For AO3, use the CSS in the Site Skin editor and add the relevant HTML structures to your work where AO3 permits them. The preview controls and their JavaScript are for local demonstration only.

## Responsive behaviour

The stylesheet includes a mobile breakpoint at `42em`. It reduces outer and page padding, adjusts title sizes, allows insert panels to fit the available width, and changes document label/value rows to stack vertically. Chat bubbles are also allowed more width on small screens.

## Notes

- The stylesheet uses font-family fallbacks. If a preferred font is unavailable on a reader's device, the browser will use the next listed fallback.
- The HTML preview embeds its own stylesheet. Editing the external CSS file will not automatically update the embedded CSS in the HTML file; keep the two copies in sync if you customise both.
- The preview's mode-switching buttons and script are not part of the AO3 Site Skin.
- The sample story and interface text are demonstration content. Replace them with your own material when adapting the components.

---
**Theme:** Fanfic Being Alive  
**Preview sample:** “The Tide Remembers”  
**Format:** AO3 Site Skin CSS + standalone HTML preview
