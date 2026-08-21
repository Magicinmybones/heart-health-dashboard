# Asset Guide

## 1. Reference Summary

The reference is a desktop hero/dashboard concept for a cardiology care experience. It places a large stylized anatomical heart over a dark, dreamlike forest and frames the remaining content with translucent blue-violet glass panels.

The client-marked reference explicitly crosses out three elements. Do not implement or source assets for:

- the top-left Recovery widget
- the top-right Scheduled Visits widget, including the doctor portrait
- the bottom meditation/music player, including its cover artwork

## 2. Available Assets

### enchanted-forest.webp

Path: `assets/backgrounds/enchanted-forest.webp`

Purpose: Full-page enchanted forest background with the same navy, cyan, violet, moss, tropical foliage, mist, and soft-focus direction as the reference.

Where it appears: Behind the complete hero/dashboard composition.

Transparency: No.

Recommended usage: Use as a full-bleed background with `background-size: cover` and centered positioning. A dark navy overlay and subtle blue/violet radial glows may be added in CSS to match the final viewport. The exposed perimeter includes pixels preserved directly from the supplied reference; place the main interface in the same general footprint so reconstructed center areas remain beneath the interface.

### anatomical-heart.png

Path: `assets/illustrations/anatomical-heart.png`

Purpose: Main sculptural heart with the reference's broad shape, cyan-blue body, magenta split lighting, pale lobes, and dark branching vessels.

Where it appears: Centered prominently over the main glass dashboard panel.

Transparency: Yes, true alpha transparency.

Recommended usage: Use directly as a responsive image with `object-fit: contain`. Do not recreate it with CSS or replace it with a generic medical heart render. Layer CSS glows behind it rather than baking glow into the image.

## 3. Elements Claude Should Recreate

The following are intentionally not image assets and should be recreated with HTML, CSS, and simple SVG where appropriate:

- main translucent dashboard panel and its rounded corners
- headline and supporting copy
- left informational card, pills, and button
- simple SpO2 line chart, label, guide line, and heart marker
- pink-to-violet valve alert card
- shadows, borders, backdrop blur, bloom, and radial glows
- spacing, typography, and responsive layout

The circular visual in the left informational card may reuse a cropped instance of `anatomical-heart.png`; no separate bitmap is needed.

## 4. Explicit Client Exclusions

Do not create or display the crossed elements from the annotated reference:

- Recovery indicator card
- Scheduled Visits card/carousel and doctor photo
- meditation/music player and cover thumbnail

These exclusions override the uncrossed original screenshot.
