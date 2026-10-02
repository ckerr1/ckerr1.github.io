# Conor Kerr — academic website

Website: https://ckerr1.github.io/

Repository: https://github.com/ckerr1/ckerr1.github.io

A static website for GitHub Pages. There is no build step or JavaScript dependency.

## Edit the site

- `index.html` contains the biography, plain-text research interests, and contact details.
- `research.html` contains the papers and posters reached from the Research navigation tab.
- `assets/styles.css` controls the shared layout, typography, and colors.
- `headshot.jpeg` is the profile photo.

The title appears on three lines on both pages: Doctoral Student, Economics, Emory University. Update the `<p class="appointment">` element in both pages to change it. Navigation uses ordinary page links, with the current page marked for accessibility.

Edit files on GitHub using the pencil icon, then commit. GitHub Pages publishes the changes automatically from `main`, at the repository root. Preserve `.nojekyll`.

## Add or replace PDFs

For a CV, upload `cv.pdf` at the repository root and add `<a href="cv.pdf">CV</a>` to the navigation on both pages. Upload research PDFs under `papers/` and link them from the relevant article in `research.html`. Keep filenames the same when replacing documents.

Each paper or poster uses an `<article class="paper">` with a title, bibliographic details, and available links. Use accurate labels such as Paper (PDF), Poster (PDF), Abstract, or Project page. Add document links after the corresponding file is available.

## Current research links

The senior thesis links to the Carolina Digital Repository record identified in the CV. The 2024 insulin poster links to its UNC abstract page; the 2023 training-load poster links to its SAIL project page. The 2022 body-composition entry currently has no verified document link.

## Sources

Biographical information and the headshot come from the [Emory profile](https://economics.emory.edu/people/doctoral-students/kerr-conor.html), the supplied CV, and the supplied research documents.

Poster records: [UNC insulin abstract](https://our.unc.edu/abstract/kerr-impact-of-copay-coupons-on-diabetes-patients-access-to-insulin/) and [SAIL projects](https://supermariogiacomazzo.github.io/sports-analytics-intelligence-laboratory/projects.html).

Design references included the academic sites of [Aikaterini-Christina Katsimpri](https://akatsim22.github.io/), [Juhee Kim](https://juheekim.org/), [Amy Lim](https://alim415.github.io/), and [Pedro H. C. Sant’Anna](https://psantanna.com/).
