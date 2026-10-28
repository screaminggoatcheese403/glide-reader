GLIDE READER — PERSONAL SPEED READER (v1.1, EPUB import update)

WHAT CHANGED
- EPUB import works with the built-in JSZip library, even offline.
- Better parsing of EPUB2 / EPUB3 manifests and reading spine order.
- Better chapter text extraction, Unicode paths, and error messages.
- File chooser is more reliable on iPhone Safari.

TO OPEN AN EPUB ON AN IPHONE
1. Save a regular, DRM-free .epub ebook into the iPhone Files app (On My iPhone or iCloud Drive).
2. Open Glide Reader's hosted HTTPS website in Safari. iOS Files HTML preview is not a complete browser; an extracted HTML file may not work properly in Quick Look.
3. Tap 'Choose file' under 'Import PDF, EPUB, TXT, MD or HTML'.
4. Choose Browse > Downloads or the folder containing your .epub.
5. Wait for 'Imported ... successfully', then tap Play.
An Apple Books library entry itself is not a file you can select from the picker. DRM-protected books are not supported.

TRY ON A MAC
Double-click index.html in Safari or Chrome. This updated index.html has a built-in EPUB reader and requires no internet for EPUB (PDFs still require internet).

USE AS AN IPHONE HOME-SCREEN APP
This is a web app (HTML/PWA), not a native IPA. Host all files on HTTPS, e.g. via GitHub Pages:
1. Make a new GitHub repository and upload all files from this folder to the repository root.
2. In Settings > Pages, choose Deploy from a branch > main > /(root).
3. Open the published HTTPS URL in iPhone Safari.
4. Use Share > Add to Home Screen.
If replacing a previous version, update all files and reload twice to allow an existing service worker to update.

PRIVACY AND LIMITATIONS
Book text is parsed locally in your browser. Files are not uploaded to a server by Glide Reader. Saved library texts live in browser storage and can be lost if Safari site data is cleared. No cloud backup or synchronization.
EPUB is best effort. DRM-protected, image-only, corrupted, and unusually formatted EPUB files may not import. PDFs with unusual layouts or image-only pages may not import (no OCR). PDF.js is still loaded from an online CDN.
Browser speech support varies, particularly iOS Safari.

DEPENDENCIES
JSZip 3.10.1 bundled within index.html (MIT/GPLv3). PDF.js 3.11.174 loaded from cdnjs (Apache 2.0).
