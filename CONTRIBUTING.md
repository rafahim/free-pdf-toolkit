# Contributing

## Principles

Keep the toolkit browser-only. Do not add upload endpoints, analytics that transmit document data, or server-side PDF processing.

Keep the runtime dependency-light. Prefer native browser APIs, pdf-lib, PDF.js, and Web Workers.

Keep files understandable. Avoid adding comments unless a single short comment is essential.

## Local workflow

1. Open the project with a local static server.
2. Test with Chromium-based and Firefox browsers.
3. Test light mode, dark mode, English, and Bengali.
4. Test small PDFs and large multi-page PDFs.
5. Verify downloaded output opens in common PDF viewers.

## Pull requests

Describe the user-facing behavior that changed. Mention browser compatibility risks. Include manual test steps. Do not include private PDF files in commits.

## Privacy

Do not introduce code that sends PDF bytes, rendered pages, filenames, metadata, or image data to external services.
