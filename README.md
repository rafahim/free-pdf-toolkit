# Free PDF Toolkit

Free PDF tools that run entirely in the browser. Files stay on the device and are processed locally with JavaScript, PDF.js, pdf-lib, and Web Workers.

## Features

Merge PDFs with drag reorder.

Split by ranges, every N pages, or specific pages.

Compress PDFs by rendering pages at a smaller scale and JPEG quality, then rebuilding the PDF.

Rotate pages by 90, 180, or 270 degrees.

Delete and reorder pages visually.

Extract embedded raster images when exposed by PDF.js, with a page-render fallback for pages without directly accessible image objects.

Convert PDF pages to JPG or PNG.

Convert JPG and PNG images to a PDF.

Add page numbers.

Add text or image watermarks.

Edit common PDF metadata fields.

Live preview with PDF.js.

Batch queue with progress and downloadable results.

Dark mode and English/Bengali UI.

Web Workers for merge and raster compression assembly.

## Privacy notice

No application server is used. PDF bytes are read from local File objects, transformed in the browser, and saved back to the device using Blob URLs. The toolkit does not upload PDF content.

PDF.js and pdf-lib are loaded from public CDNs, so the browser requests those library assets from their respective CDN hosts. Your PDF bytes are not sent to those hosts by the application logic.

## Password support

The selected stack does not provide PDF writer encryption in pdf-lib. Password protection therefore cannot safely be advertised as true PDF encryption in this build. Password removal can be attempted by opening a password-protected PDF in PDF.js and rebuilding pages into a new unencrypted PDF, which can flatten interactive and vector features.

## GitHub Pages deployment

1. Create a repository and upload the project files.
2. Keep the `workers` folder and `.well-known` folder in the repository root.
3. Commit and push the files.
4. In GitHub, open Settings, Pages, and choose GitHub Actions or the branch-based static deployment flow.
5. Publish the repository as a static site.
6. Open the published `/pdf-toolkit/` path.
7. Update the canonical URLs in `index.html`, `robots.txt`, `sitemap.xml`, and `manifest.json` if your deployment URL differs.

## Author

RA Fahim

Web Developer & Creator

Full-stack

1 year

Dhaka, Bangladesh

https://rafahim.com

https://github.com/rafahim

mailto:dev@rafahim.com

https://twitter.com/rafahimn

https://linkedin.com/in/rafahimn

## SEO checklist

Title matches the requested canonical page title.

Meta description and keyword metadata are present.

Canonical URL is set.

Open Graph and Twitter Card metadata are set.

JSON-LD contains WebApplication, Person, and BreadcrumbList entities.

robots.txt and sitemap.xml are included.

The author identity and canonical site are linked from structured data.

Favicon and Open Graph artwork are included locally.

## Browser notes

Modern Chromium, Firefox, and Safari versions are recommended.

Large PDFs may require substantial client RAM because pages may be rasterized during compression and conversion.

Image-based compression trades searchable/selectable PDF text for smaller, predictable output.
