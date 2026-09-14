# HEIC/JPG/PNG Image Processor

A client-side web application for converting, resizing, and compressing HEIC/HEIF, JPG, and PNG images directly in the browser. 
The application uses `libheif-js` compiled to WebAssembly to decode high-efficiency HEIC files, while standard image formats are processed using native browser Canvas APIs and `createImageBitmap`.

Users can select multiple images, preview them in an interactive thumbnail grid, choose their preferred scaling ratio  and output format (JPG or Original), and process files locally without uploading data to any external server.

### How It Works

* **Client-Side Privacy:** Performs all image processing entirely on the client side, keeping original files strictly on the user's device with zero server interaction.
* **HEIC/HEIF Decoding:** Full support for HEIC/HEIF photos, decoding images using `libheif-js` via WebAssembly.
* **Batch & Parallel Processing:** Converts and scales multiple images concurrently with real-time processing progress indicators.
* **Flexible Scale Options**
* **Format Conversion:** Converts processed images to standard JPG format or preserves original format types.
* **Automatic EXIF Removal:** Automatically strips EXIF metadata (GPS location, camera settings, timestamp) during canvas re-rendering to protect user privacy.
* **Live Thumbnail Previews:** 
* **Flexible Export Options:** Export the processed batch as a `.zip` archive (using JSZip) or share directly through native mobile share sheets.

### Tech Stack

* **Core:** Pure HTML5, CSS3, Vanilla JavaScript (ES6+) — zero build setup required.
* **HEIC Decoder:** `libheif-js` (WebAssembly)
* **ZIP Generation:** `JSZip`
* **Image Engine:** HTML5 Canvas API & `createImageBitmap` for hardware-accelerated scaling and EXIF stripping.

### Getting Started

1. Download or clone this repository.
2. Open `index.html` directly in any modern web browser (Chrome, Safari, Firefox, Edge).
3. Select your images and process them.

The application is designed to provide a simple, privacy-friendly way to convert and resize images directly in the browser, with particular support for HEIC photographs commonly produced by modern smartphones.
