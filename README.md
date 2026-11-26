# CRAVETCHI — website

Static GitHub Pages website. Installment I is published at `/sidetracks/i/`.

## Installment I

```
sidetracks/i/
    index.html                 Publication page and PDF viewer
    Cravetchi-Sidetracks-I.pdf   Original PDF (unchanged)
    manuscript.html            Complete HTML reading edition
```

The READ TEXT link opens the HTML edition. It uses native HTML headings, paragraphs, block quotations, linked contents, footnotes and ordinary CSS. It requires no JavaScript, frameworks or build step. The PDF is the authoritative formatted edition; the HTML edition reflows on smaller screens. Footnotes are grouped at the end and have return links. Reference 78 occurs in the PDF, but its note text is absent from the supplied PDF; this is explicitly marked in the HTML. The introductory paragraph from the PDF is included before Motivation.

## Updating the manuscript

Replace the PDF with a new PDF of the same name. Edit `manuscript.html` directly: use `<p>` for paragraphs, `<h2>` for headings, `<blockquote>` for quotations, `<em>` for italics and `<strong>` for bold. Preserve heading IDs and footnote anchors when editing. The PDF and HTML are separate editions; changing one does not automatically update the other. There is no `manuscript.txt` dependency.

Upload the extracted contents (not the ZIP) to the root of the GitHub repository. Delete the old `sidetracks/i/manuscript.txt` from GitHub; uploading replacement files does not delete it. No other legacy essay or PDF files are needed.

## Future installments

Copy the installment directory structure for `ii`, `iii`, or `iv`, update the numeral, titles, metadata, canonical links, PDF filename and navigation. Replace the manuscript HTML content. On the homepage and other installment pages, replace the corresponding question mark with a link to the new installment. Add both the installment page and its HTML reading edition to `sitemap.xml`.

To test locally, open the website files in a browser or serve the repository root with `python -m http.server 8000`.
