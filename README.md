# Clear Cut Photo Editor

A free browser-based photo editor with AI background removal, colour adjustments, shadows, crop and batch export.

**[Click here to use the editor](https://lonesoulsurfer.github.io/clear-cut-photo-editor/)**

This photo editor was built to make batch changes on images simple and easy. Primarily — I made it so I could batch process images for Instructables builds. However, it's a great tool to use for individual images as well.

The 2 highlights in this editor are the background removal and adding shadows to images. Once the background has been removed, you can pick the colour you want or have it transparent.

There are multiple controls to help with adjusting the image so it looks just right. Again, these are simple to use and you can also add a preset to your favourite adjustments to use in other editing projects.

I've kept the tools to a minimum and have made a concerted effort not to include any controls that just waste space or are hardly ever used.

Below is a how to use the editor with images — enjoy and let me know if you find any bugs or if I am missing any controls you think essential.

---

## Getting Started

1. Click the link at the top of this page to open the editor, or open `index.html` directly in any modern browser (Chrome recommended for full File System Access support)
2. Drop images onto the left panel, or click the drop zone to browse
3. Edit and export — everything stays in your browser, nothing is uploaded

---

## Session

When you open the editor you'll be prompted to start a new session or resume a previous one.

![Session panel](session.png)

- **New session** — starts fresh with a clean workspace. Give it a name or leave the default (auto-named by date)
- **Resume** — picks up where you left off, including the folder you were working from
- Click **Choose Photos folder & start** to select your working folder and begin

Files are saved to `Photos / [session name] /` inside the folder you choose.

---

## Loading Images

Click or drag photos directly onto the drop zone in the preview area. Supports JPG, PNG, and WebP. You can load multiple images at once.

![Load images](load-images.png)

Once loaded, images appear in the **filmstrip** at the bottom of the preview. Click any thumbnail to switch to it. Hover a thumbnail to reveal the **✕** remove button.

> **Tip:** When you add new images, any slider adjustments you've already made are automatically inherited by the new images.

Here's an example of a finished edit — background removed, shadow added, and adjustments dialled in:

![Preview example with background removed and shadow](preview-example.png)

---

## Adjustment Controls

The right panel contains all tone and colour controls.

![Adjustment controls panel](adjustments-panel.png)

| Slider | What it does |
|---|---|
| **Brightness** | Overall exposure — push up to lift shadows, pull down to darken |
| **Contrast** | Separation between lights and darks |
| **Sharpness** | Edge crispness — useful for product shots |
| **Colour** | Saturation — pull left to desaturate, push right to boost |
| **Warmth** | Colour temperature — orange/warm vs blue/cool |
| **Highlights** | Recover blown highlights or push them brighter |
| **Shadows** | Lift or crush the shadow areas independently |

All sliders default to `0`. The value badge turns accent-coloured when a slider is active.

### Rotation & Straighten

Below the sliders, four buttons handle **90° rotation** (CCW, CW, 180°, reset to 0°). The **Straighten** slider fine-tunes tilt from −45° to +45°.

### Presets

Save your current slider state as a named preset so you can reuse it across projects.

1. Dial in the adjustments you want
2. Type a name in the preset field and click **+ Save current as preset**
3. Click any saved preset to instantly apply it to the current image
4. Click **×** on a preset to delete it

Presets are saved to your browser's local storage and persist between sessions.

### Apply to All & Reset

![Apply adjustments to all and Reset](apply-reset.png)

- **Apply adjustments to all** — copies the current image's slider settings across every image in the session
- **Reset** — zeros out all sliders and rotation for the current image

### Undo / Redo

Each image has its own undo/redo history. Use the **Undo** and **Redo** buttons above the drop zone.

---

## Background Colour

Choose what background to place behind a subject after background removal.

![Background colour swatches](background-colour.png)

Pick from the preset swatches (including transparent), or click the **+** tile to choose a custom colour. The label below the swatches shows your current selection.

---

## Shadow

After background removal, the Shadow panel lets you add a realistic drop shadow.

![Shadow panel](shadow.png)

- Drag the **angle dial** to set the light direction
- Click **Disabled** to toggle the shadow on or off
- Adjust the sliders to refine the look:

| Slider | What it does |
|---|---|
| **Strength** | Opacity of the shadow |
| **Softness** | How blurred/feathered the edges are |
| **Spread** | How far the shadow extends outward |
| **Width** | Horizontal scale of the shadow |
| **Distance** | How far the shadow is offset from the subject |

Click **Apply background & shadow to all** to push these settings across every image in the session.

---

## Export & Output

The left panel controls canvas size and export resolution.

![Export and output panel](export-output.png)

**Canvas** — choose the output aspect ratio:
- **Original** — keeps the image's native dimensions
- **Landscape 3:2 / Portrait 2:3 / Square 1:1** — crops to a standard ratio
- **Fit to canvas** — fits the image within the canvas without cropping
- **Freehand selection** — drag to define a custom crop region

**Export size** — set the output resolution at 100%, 75%, 50%, or 25% of the canvas size.

---

## Mouse Controls

Use your mouse to navigate and crop within the preview area.

![Crop and zoom](crop-zoom.png)

| Action | How |
|---|---|
| **Zoom in / out** | Scroll wheel over the preview |
| **Pan** | Right-click and drag |
| **Freehand crop selection** | Left-click and drag to draw a crop region |
| **Zoom to selection** | Left-drag then release — the canvas zooms to fit your selection |
| **Next / Prev image** | Hover the left or right edge of the preview for arrow navigation |

> **Tip:** When in freehand selection mode, the canvas ratio tooltip at the bottom shows the pixel dimensions of your selection as you drag. Release to confirm the crop.

---

## Saving

![Save buttons](save.png)

- **Save this photo + Remove BG** — exports the current image with all adjustments and background removal applied
- **Save all photos** — batch exports every image in the filmstrip; a progress bar tracks the queue

Exports are saved directly to your session folder. If background removal was applied, images export as PNG to preserve transparency (unless a solid background colour was chosen).

