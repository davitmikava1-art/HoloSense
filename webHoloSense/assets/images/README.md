# Images Folder

This folder contains all images used in the HoloSense website.

The HTML uses fixed local filenames for all images.  
You can simply place files with the following names into this folder and they will be picked up by the site.

## Required Images (current setup)

### University Logo
- `ilia-state-university-logo.png` – Ilia State University logo (used in navigation, hero and footer)

### Hero Section
- `hero.jpg` – main hero image on the first screen

### Device / Diagram Images
- `device.png` – visualization of the HoloSense device / multi-slot design
- `how-it-works.png` – diagram showing how the system works

### Device Parts (cards in “მოწყობილობის ნაწილები”)
- `part-1.png` – ESP32 microcontroller
- `part-2.png` – perfume pump
- `part-3.png` – 38mm magnetic pump
- `part-4.png` – 12V 10A power supply
- `part-5.png` – step‑down converter 5A
- `part-6.png` – PTC ceramic heating plate 5V
- `part-7.png` – supporting electronics / cables

## Adding or duplicating parts

To add a new part to the Device Components section:

1. Add your image file as `part-X.png` (where X is the next free number) or any other name.
2. In `index.html`, find the **Device Components / Parts Section** (`id="device-parts"`).
3. Copy one of the part card blocks (between `<!-- Duplicate this block to add a new part -->` comments).
4. Update:
   - `src` path for the image
   - `alt` text (in Georgian)
   - `<h3>` title and `<p>` description
   - the `href` of the `part-link` button (there is a TODO comment for each link).

Example:
```html
<!-- Duplicate this block to add a new part -->
<div class="part-card">
    <div class="part-image-wrapper">
        <img src="assets/images/part-X.png" alt="ნაწილი X - Part Name" class="part-image">
    </div>
    <div class="part-content">
        <h3>Part Name</h3>
        <p>Description text here.</p>
    </div>
</div>
<!-- End of part block -->
```

## Image Guidelines

- Recommended format: PNG or JPG
- Recommended size: 
  - Hero image: 1200x800px
  - Device images: 800x600px
  - Part images: 600x400px
  - Logo: 200x80px (maintain aspect ratio)
- All images should be optimized for web use
- Use descriptive alt text in Georgian for accessibility

> Note: Product URLs in the parts grid are **not hardcoded** –  
> each button has `href="#"` plus a TODO comment where you can paste your own link.
