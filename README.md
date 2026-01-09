# QR Code Multi Generator

A simple single-file web app that generates multiple QR codes from a list of codes (one code per line). Paste up to 30 lines and click the button to render QR codes in a 3-column grid. Designed for fast generation and printing.

## Features

- Generate up to 30 QR codes at once.
- Grid layout (3 columns) optimized for A4 printing.
- Each QR shows its text label underneath.
- No build steps — single `index.html` file using a CDN for QRCode.js.

## Usage

1. Open the app in your browser:
   - Open [index.html](index.html)
2. Paste or type your codes into the textarea (one per line).
   - Input element: [`#inputCodes`](index.html)
3. See line count update in real time: [`#lineCount`](index.html)
4. Click "Tạo mã QR" to generate QR codes (function: [`generateQRs`](index.html))
5. The generated QR items appear in [`#qrcode-grid`](index.html). Print from the browser if needed.

## Notes

- The app uses QRCode.js from CDN: https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js
- Each QR is generated at 150×150 pixels with high error correction.
- Lines beyond 30 are ignored.

## Customization

- Edit layout, sizes, or colors directly in [index.html](index.html).
- To change QR size or error-correction, modify the options in [`generateQRs`](index.html).

## License

Use as you wish.
