# HEIC/Other formats Image Converter/Resizer

A client-side web application for converting and resizing HEIC/HEIF images directly in the browser. The application uses `libheif-js` and WebAssembly to decode HEIC files, while standard image formats are handled using native browser APIs.

Users can select multiple images, preview them as thumbnails, choose the desired output format and scale, and process the images without uploading them to a server.

### How It Works

* Detects HEIC/HEIF files and decodes them using `libheif-js`.
* Generates thumbnails for selected images.
* Resizes images.
* Converts processed images to the selected output format.
* Supports batch processing of multiple images.
* Performs image processing entirely on the client side, keeping the original files on the user's device.

The application is designed to provide a simple, privacy-friendly way to convert and resize images directly in the browser, with particular support for HEIC photographs commonly produced by modern smartphones.
