# laser-ready
A simple, lightning-fast utility for converting PDFs from Onshape so they are ready to laser cut using a ULS laser engraver.

To use the utility, just upload a PDF that contains line art. The utility will select all lines in the PDF, change them to the correct RBG color value of 255,0,0, then change the line width to 0.001 inches. A new PDF, named `LaserReady_<original name>.pdf` by default, will then be downloaded, which can be opened in Adobe Acrobat and sent to a ULS laser engraver for cutting.

This was built using Claude. Please don't use this tool if you have qualms about using code created with AI tools.

## Privacy

All processing happens in your browser. No file is ever uploaded to a server.

## Credits & support

- Designed by **Bill Van Loo**
- Found a bug or want a feature? Email `billvanloo.tech+feedback@gmail.com` (the subject line is pre-filled from the in-app links).
- If this tool saved you time, you can [support the work on Ko-fi](https://ko-fi.com/billvanloo).

## License

[MIT](LICENSE) © 2026 Bill Van Loo

