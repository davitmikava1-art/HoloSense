# Images Folder

This folder contains all images used in the HoloSense website.

## Required Images

Place the following images in this folder:

### University Logo
- `ilia-state-university-logo.png` - Ilia State University logo (used in header and footer)

### Hero Section
- `hero.jpg` - Main hero image for the landing section

### Device Images
- `device.png` - Device visualization for multi-slot design section
- `how-it-works.png` - Diagram showing how the device works

### Device Parts
- `part-1.png` - PTC Heating Pads
- `part-2.png` - Raspberry Pi 4
- `part-3.png` - Scent Capsules
- `part-4.png` - 30mm Fans
- `part-5.png` - Acrylic Panels
- `part-6.png` - Wiring and Connectors

## Adding New Parts

To add a new part to the Device Components section:

1. Add your image file as `part-X.png` (where X is the next number)
2. In `index.html`, find the Device Components section
3. Copy one of the part card blocks (marked with comments)
4. Update the image path, alt text, title, and description

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
