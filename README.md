# Shahyad Khamnei — website redesign

A small, responsive academic website in ivory and burgundy. No installation, build process, JavaScript, or external fonts required.

## Preview

Extract this ZIP, then open index.html in your browser. Keep the css, images, and files folders alongside it.

## Replace your GitHub Pages site

1. Keep a backup of your existing repository (GitHub's Code > Download ZIP).
2. Copy the contents of this folder into the ROOT of your website repository, replacing matching files. Upload the extracted contents, not the ZIP itself or a containing folder.
3. Commit and push, or use GitHub's Add file > Upload files and commit the upload.
4. After GitHub Pages finishes deploying, reload your site. A hard refresh may be needed for cached styles.

Leave other existing files in place. This package replaces index.html, research.html, notes.html, cv.html, and css/styles.css. research.html redirects to the homepage's research section; old Notes and CV URLs remain usable. Notes is intentionally omitted from the new main navigation.

## Content to review

- The portrait is your existing images/profile.jpg.
- The CV is the actual PDF from the original repository, named CV_05_01_2026 (3).pdf, copied to files/Shahyad_Khamnei_CV.pdf. It is not newly updated. Replace that PDF with your latest CV using the same filename.
- Your previous CV page linked to missing files; the new link uses the included PDF.
- No publication citations appeared on the previous research page. No publications have been invented. Replace the short empty-state line when you supply real citations.
- The introductory MPIPKS affiliation and research interests follow the information you provided. Edit index.html to refine the wording.
- Existing public email and academic GitHub links were retained.

## Adding publications

In index.html, replace the paragraph with class="empty-state" with a list like this, substituting real citation details and URLs:

```html
<ol class="publication-list">
  <li>
    <h3><a href="YOUR_PAPER_URL">Exact paper title</a></h3>
    <p>Author names, including Shahyad Khamnei.</p>
    <p>Journal or preprint status · Year</p>
    <div class="publication-links">
      <a href="YOUR_PAPER_URL">Paper ↗</a>
      <a href="YOUR_CODE_URL">Code ↗</a>
    </div>
  </li>
</ol>
```

Omit a Code link if no public code exists. Add more li entries as needed.

## Styling

Colors are defined at the top of css/styles.css. The portrait crop is controlled by .portrait. The website adapts to narrow screens and includes keyboard focus states, reduced-motion support, and print styles.

No live site was changed while preparing this package.
