# Conor Kerr — academic website

Website: https://ckerr1.github.io/

Repository: https://github.com/ckerr1/ckerr1.github.io

A small, responsive academic website for GitHub Pages. It works as plain HTML, with no installation, build step, external font service, or JavaScript dependency.

## Publish on GitHub Pages

1. Create a public repository called `YOUR_USERNAME.github.io`, replacing `YOUR_USERNAME` with your GitHub username. If you already have that repository, use its existing contents as the starting point instead of replacing it blindly.
2. Put the site files at the root of the repository, preserving the `assets/` and `papers/` folders. Include `index.html`, `research.html`, `headshot.jpeg`, `cv.pdf`, and `.nojekyll`. Upload the extracted files, rather than the ZIP file itself.
3. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/(root)**. Save.
4. Your site will appear at `https://YOUR_USERNAME.github.io/`. GitHub notes that publication can take up to 10 minutes.

The relative document and stylesheet paths also work if you decide to host this as a project site, such as `https://YOUR_USERNAME.github.io/academic-website/`.

## Update your bio

On GitHub, open `index.html`, choose the pencil icon, and find the `ABOUT` comment. Edit the two paragraphs and commit your changes. The site updates automatically when Pages publishes the commit.

Research interests are a plain paragraph under the `RESEARCH INTERESTS` comment on the home page. Papers and posters live on the separate `research.html` page, reached from the Research navigation tab. The exact three-line title is in the `<p class="appointment">` element on both pages. Contact details appear in both the profile and the Contact section.

If you change the name, title, or research emphasis, also update the `<title>`, description, and Open Graph text in the document's `<head>`.

## Update your CV and research PDFs

The site includes three documents:

- `cv.pdf`: your October 2026 CV, linked in the navigation and profile.
- `papers/learning-optimal-commodity-taxation.pdf`: your September 2026 MSc dissertation.
- `papers/consumer-demand-incarcerated-communications.pdf`: your April 2025 senior honors thesis.

To update a document, upload its replacement using the same path and filename. GitHub Pages publishes the replacement automatically. Research titles, dates, descriptions, and links are in `research.html`. The source PDFs are included without altering their contents.

The Posters section lists the three entries from your CV. All three entries link to official Celebration of Undergraduate Research materials. The 2024 insulin entry links to its abstract page. The 2023 training-load and 2022 body-composition entries link directly to the poster and abstract PDFs in their respective archives. The 2023 archive uses filenames ending in `2025.pdf`; preserve those URLs as published by UNC.

## Add a paper

Upload the paper as `papers/paper-short-name.pdf`. Add this structure at the end of the Papers section of `research.html`, before its closing `</section>`, and replace every example field with real information:

```html
<article class="paper">
  <h4>Your actual paper title</h4>
  <p class="paper-meta">Actual coauthors, if any · Working paper · 2026</p>
  <p>A short, accurate summary of the question and contribution.</p>
  <div class="paper-links">
    <a href="papers/paper-short-name.pdf">Paper (PDF)</a>
    <!-- Add a code link only if a public repository exists. -->
  </div>
</article>
```

If your list grows, group articles under `Working papers`, `Publications`, or `Work in progress` only when those labels accurately describe the work. The current entries are labeled as an MSc dissertation and a senior honors thesis.

## Add teaching

Add a navigation link `<a href="#teaching">Teaching</a>`. Insert this section before Contact, replacing the example with a real appointment:

```html
<section id="teaching" aria-labelledby="teaching-heading">
  <h2 id="teaching-heading">Teaching</h2>
  <ul class="teaching-list">
    <li>Actual course name — actual role, university, semester.</li>
  </ul>
</section>
```

## Change your photo or colors

Replace `headshot.jpeg` with a new photo using the same filename. The original image is the publicly posted headshot from your Emory Economics profile.

Colors are set near the top of `assets/styles.css` in `:root`. Both pages use this shared stylesheet. The typography uses system fonts, so the site remains readable and does not need to contact a font provider.

## Review locally

Open `index.html` in your browser. All navigation, email links, and the photo work without running a server. The layout adapts to phones and includes keyboard focus styles, a skip link, reduced-motion support, and print styles.

## Content and design sources

The public profile, photo, email, undergraduate background, and office were checked against:

- [Conor Kerr's Emory Economics profile](https://economics.emory.edu/people/doctoral-students/kerr-conor.html)
- [Public Emory headshot](https://economics.emory.edu/images/headshot/student-graduate/kerr-conor.jpeg)

The site uses the title and econometrics/statistics emphasis you supplied. The CV and research entries use the documents you provided for inclusion on the website. The biography uses your wording “read for an M.Sc.” and includes rowing, coxing for Emory Crew, and watching the Tar Heels.

Reference sites reviewed for structure:

- [Aikaterini-Christina Katsimpri](https://akatsim22.github.io/)
- [Juhee Kim](https://juheekim.org/)
- [Amy Lim](https://alim415.github.io/)
- [Pedro H. C. Sant'Anna](https://psantanna.com/)

Publishing instructions were checked against [GitHub's quickstart](https://docs.github.com/en/pages/quickstart) and [publishing-source documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Poster archive sources

- [2024 Celebration](https://our.unc.edu/share/celebration/spring-2024/)
- [2023 Celebration presenters](https://our.unc.edu/celebration-presenters/)
- [2022 Celebration](https://our.unc.edu/share/celebration/2022-celebration-of-undergraduate-research/)

Both pages explicitly use the transparent `assets/blank-favicon.svg` as their browser-tab icon. The profile photo remains on the pages themselves. Navigation contains About, Research, and CV.
