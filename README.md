# Crop & WebP Tool ✂️

A lightweight, browser-based tool for cropping multiple images to a **16:9 aspect ratio** and exporting them as WebP files inside a named folder.

## ✨ Features

- **16:9 Aspect Ratio:** Crop images in widescreen format.
- **Batch Image Selection:** Upload multiple images at once.
- **Sequential Cropping:** Move through images using Previous and Next.
- **Automatic Center Crop:** Images without a manual crop selection are center-cropped to 16:9.
- **WebP Conversion:** Convert images into WebP format.
- **Adjustable Quality:** Set WebP quality from 10% to 100%.
- **Multiple Resolutions:** Export at the crop's natural resolution, 1920 × 1080, 1280 × 720, or 960 × 540.
- **Custom Folder Name:** Choose the output folder name before exporting.
- **Duplicate First Image:** Save the first cropped image as both `banner.webp` and `01.webp`.
- **ZIP Export:** Download all processed images in one ZIP archive.
- **Privacy-Friendly:** Images are processed locally in your browser.

## 📂 Output Structure

For example, if you enter `wedding-gallery` as the folder name:

```text
wedding-gallery/
├── banner.webp
├── 01.webp
├── 02.webp
├── 03.webp
├── 04.webp
└── ...
```

### File Naming Rules

| File | Description |
|---|---|
| `banner.webp` | Duplicate of the first cropped image |
| `01.webp` | First cropped image |
| `02.webp` | Second cropped image |
| `03.webp` | Third cropped image |
| `04.webp` | Fourth cropped image |
| `...` | Remaining images in selection order |

The first cropped image is intentionally saved twice: once as `banner.webp` and again as `01.webp`.

## 🚀 Getting Started

### Requirements

- A modern web browser such as Google Chrome, Safari, Firefox, or Microsoft Edge.
- An internet connection to load the JSZip library used for ZIP exports.

### Installation

1. Download `crop_webp_tool.html`.
2. Save it anywhere on your computer.
3. Open the file in your web browser.
4. Select the images you want to process.

No Node.js installation or development server is required.

## 🖼️ How to Use

1. Open the tool in your browser.
2. Click **Select images** and choose multiple images.
3. Enter your preferred output folder name, such as `wedding-gallery`.
4. Select the first image and draw a 16:9 crop.
5. Use **Next** to move through the remaining images and adjust their crops.
6. Choose your preferred WebP quality.
7. Select an output resolution.
8. Click **Export all as ZIP**.
9. Extract the downloaded ZIP to access your images.

## ⚙️ Export Settings

### Aspect Ratio

All crops use a fixed **16:9** aspect ratio.

### WebP Quality

The quality slider ranges from 10% to 100%. Higher quality generally produces larger files.

### Output Resolution

- **Original crop resolution:** Retains the crop's natural dimensions.
- **1920 × 1080:** Full HD.
- **1280 × 720:** HD.
- **960 × 540:** Smaller widescreen images.

Selecting a fixed output resolution resizes the crop to the selected dimensions.

## 🔒 Privacy

Images are loaded and processed in the browser. They are not uploaded to an image-processing server.

The JSZip library is loaded from a CDN, so an internet connection is required for ZIP export.

## 🛠️ Technology

- HTML5
- CSS3
- JavaScript
- Canvas API
- JSZip
- WebP image encoding

## 📌 Notes

- Images are processed in the order they are selected.
- The first cropped image is duplicated as `banner.webp` and `01.webp`.
- Images are exported into a ZIP archive containing the named folder.
- If no crop is manually selected, the tool uses an automatic center crop.
- The original image files are not modified.

---

**Crop & WebP Tool**  
Simple image cropping. Consistent aspect ratios. Lightweight WebP exports.
