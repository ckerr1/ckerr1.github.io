# Conor Kerr — academic website

Website: https://ckerr1.github.io/

Repository: https://github.com/ckerr1/ckerr1.github.io

A small, responsive academic website for GitHub Pages. It works as plain HTML, with no installation, build step, external font service, or JavaScript dependency.

## Publish on GitHub Pages

1. Create a public repository called `YOUR_USERNAME.github.io`, replacing `YOUR_USERNAME` with your GitHub username. If you already have that repository, use its existing contents as the starting point instead of replacing it blindly.
2. Put `index.html`, `headshot.jpeg`, and `.nojekyll` at the root of the repository. Include this README if useful. Upload the extracted files, rather than the ZIP file itself.
3. Open **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, then **main** and **/(root)**. Save.
4. Your site will appear at `https://YOUR_USERNAME.github.io/`. GitHub notes that publication can take up to 10 minutes.

The relative image path also works if you decide to host this as a project site, such as `https://YOUR_USERNAME.github.io/academic-website/`.

## Update your bio

On GitHub, open `index.html`, choose the pencil icon, and find the `ABOUT` comment. Edit the two paragraphs and commit your changes. The site updates automatically when Pages publishes the commit.

Research interests live under the `RESEARCH` comment. Update both the paragraph and list when your interests change. The exact title is in the `<p class="appointment">` element. Contact details appear in both the profile and the Contact section.

If you change the name, title, or research emphasis, also update the `<title>`, description, and Open Graph text in the document's `<head>`.

## Add your CV

Upload a public version of your CV as `cv.pdf` in the repository root. Then replace the navigation comment about your CV with:

```html
<a href="cv.pdf">CV</a>
```

Only add the link after the PDF is uploaded. The site currently omits a CV link because a current CV has not been supplied.

## Add a paper

Upload the paper as `paper-short-name.pdf`. Add this structure at the end of the Research section, before its closing `</section>`, and replace every example field with real information:

```html
<article class="paper">
  <h3>Your actual paper title</h3>
  <p class="paper-meta">Actual coauthors, if any · Working paper · 2026</p>
  <p>A short, accurate summary of the question and contribution.</p>
  <div class="paper-links">
    <a href="paper-short-name.pdf">Paper</a>
    <!-- Add a code link only if a public repository exists. -->
  </div>
</article>
```

For several papers, change the section heading to `Research` and group articles under `Working papers`, `Publications`, or `Work in progress` only when those labels accurately describe the work. Do not list course assignments as publications.

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

Colors are set near the top of `index.html` in `:root`. The typography uses system fonts, so the site remains readable and does not need to contact a font provider.

## Review locally

Open `index.html` in your browser. All navigation, email links, and the photo work without running a server. The layout adapts to phones and includes keyboard focus styles, a skip link, reduced-motion support, and print styles.

## Content and design sources

The public profile, photo, email, undergraduate background, and office were checked against:

- [Conor Kerr's Emory Economics profile](https://economics.emory.edu/people/doctoral-students/kerr-conor.html)
- [Public Emory headshot](https://economics.emory.edu/images/headshot/student-graduate/kerr-conor.jpeg)

The site uses the title and econometrics/statistics emphasis you supplied. The Oxford wording says “studied” because the supplied dissertation establishes your program but not the date a degree was formally awarded. No private dissertation, course solutions, or unpublished manuscript is included.

Reference sites reviewed for structure:

- [Aikaterini-Christina Katsimpri](https://akatsim22.github.io/)
- [Juhee Kim](https://juheekim.org/)
- [Amy Lim](https://alim415.github.io/)
- [Pedro H. C. Sant'Anna](https://psantanna.com/)

Publishing instructions were checked against [GitHub's quickstart](https://docs.github.com/en/pages/quickstart) and [publishing-source documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).
