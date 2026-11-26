# CRAVETCHI — website

This is a static GitHub Pages site. The homepage is the index of the four installments of Sidetracks. Installment I has its own permanent page at `/sidetracks/i/`.

## Publish Installment I

Put both complete versions of the installment in the existing directory:

```
sidetracks/i/
    index.html       (already prepared; leave unchanged)
    Cravetchi-Sidetracks-I.pdf   (add your finished PDF)
    manuscript.txt   (replace the empty file with your full text)
```

Use exactly these case-sensitive filenames. Save the text as UTF-8 plain text, with blank lines between paragraphs. In Word, use Save As > Plain Text (.txt), and select UTF-8 encoding if prompted. The web page preserves line breaks and paragraphs but does not reproduce Word typography, italics, footnote formatting or pagination; the PDF remains the formatted edition. Both files are detected independently. The PDF appears with open/download links and a desktop viewer; the text appears as selectable, searchable on-page prose with a direct download and a jump link. On phones the PDF uses direct links rather than an embedded viewer. The empty text file and missing PDF are intentionally not shown. No HTML editing is needed for publication.

Upload the whole extracted folder contents (not the ZIP itself) to the root of your GitHub Pages repository, preserving the paths. The direct addresses after publication are:

- https://mcravetchi.github.io/sidetracks/i/
- https://mcravetchi.github.io/sidetracks/i/Cravetchi-Sidetracks-I.pdf
- https://mcravetchi.github.io/sidetracks/i/manuscript.txt

For local testing, serve the repository root using `python -m http.server 8000` and visit `http://localhost:8000/sidetracks/i/`. Opening the HTML directly from disk may prevent file detection. No external scripts, build step or framework is used.

## Replace the existing website

Upload the contents of this ZIP to the root of the existing repository, replacing the matching files. **Explicitly delete** `essays/`, `pdfs/`, `sidetracks-1.html`, `sidetracks-2.html`, and any old segment PDFs in `sidetracks/i/` from the existing repository. Delete the prior `EDIT_NOTES.md` if present. Uploading replacement files alone does not delete old files on GitHub. Old essay and PDF URLs will intentionally stop working; previous commits may still contain them.

## Add future installments

Copy `sidetracks/i/index.html` into `sidetracks/ii/index.html` (then `iii`, `iv`). Adjust the title, description, canonical URL, installment numeral and current navigation cell. Use `Cravetchi-Sidetracks-II.pdf`, `Cravetchi-Sidetracks-III.pdf`, or `Cravetchi-Sidetracks-IV.pdf` for the respective PDF. In each copied HTML file, replace every occurrence of `Cravetchi-Sidetracks-I.pdf` with the corresponding filename. Keep the UTF-8 text file named `manuscript.txt`. On the homepage replace the corresponding `?` with `<a href="sidetracks/ii/" aria-label="Installment II">II</a>`. In each existing installment navigation, replace that placeholder with `<a href="../ii/">II</a>` (except on Installment II itself, where it is the current span). Add each new page URL to `sitemap.xml`.

The sitemap, author links and Google site verification remain intact. The old update describing three parts has been removed to avoid confusing it with the current four-installment structure.
