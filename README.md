# Jie Liu — Academic Homepage

Personal academic website for Jie Liu, Postdoctoral Associate in Mathematics at New York University Abu Dhabi.
Built with Jekyll and the gem-based al-folio v1 runtime.

## Pages and content

| Content                         | Source                                                                 |
| ------------------------------- | ---------------------------------------------------------------------- |
| About and contact details       | `_pages/about.md`                                                      |
| Research interests              | `_pages/research.md`                                                   |
| AI4Math project and demo        | `_pages/ai-research-workflow.md`, `assets/demos/ai4math-workflow.html` |
| Math Paper Editor and demo      | `_pages/math-paper-editor.md`, `assets/demos/math-paper-editor.html`   |
| Publications page               | `_pages/publications.md`                                               |
| Publication records             | `_bibliography/papers.bib`                                             |
| Talks                           | `_pages/talks.md`                                                      |
| Teaching                        | `_pages/teaching.md`                                                   |
| Site metadata and feature flags | `_config.yml`                                                          |

The website contains published articles and public preprints. The source CV and work in progress are not website assets.
Do not add the CV PDF to this repository or link to it from public pages. CV filenames are ignored by Git and excluded from the Jekyll build.

## Add a profile photo

The homepage displays `assets/img/jie-liu.jpg` on the right. The supplied original photo is preserved without cropping or retouching.
To replace the photo:

1. Copy your original JPG or PNG into `assets/img/`, for example `assets/img/jie-liu.jpg`.
   Use a filename without spaces. A portrait at least 800 pixels wide is sufficient; keep the original elsewhere as a backup.
   Export HEIC photos to JPG or PNG first.
2. In `_pages/about.md`, keep the following profile settings, updating `image` if the filename changes:

   ```yaml
   profile:
     align: right
     image: jie-liu.jpg
     image_circular: false
   ```

3. Preview the homepage and check the crop on desktop and mobile before committing.

You can also add the image through GitHub: open `assets/img/` in this repository, choose **Add file → Upload files**,
select the photo, and commit. Then update the homepage's `profile` setting as above.
Do not put the CV PDF in the image folder.

Responsive image conversion is disabled so a plain photo works without ImageMagick.
Enable `imagemagick.enabled` only when ImageMagick is available in the build environment.

## Update publications

Add records to `_bibliography/papers.bib`; the Publications page renders them automatically.
Use `@article` for published papers and `@unpublished` for public preprints. Keep stable, unique citation keys.
The page renders these two types separately and groups each by year in descending order.

Useful fields include `doi`, `arxiv`, `pdf`, `abstract`, and `bibtex_show = {true}`.
Use public URLs for PDFs. The theme displays journal volume, issue, and page information through `additional_info`,
so keep that field in sync with the standard `volume`, `number`, and `pages` fields.
Do not add unpublished work in progress or private submission information.

## Mathematics

MathJax is enabled site-wide through `al_math` and `enable_math: true`.
Use `$...$` for inline mathematics and `$$...$$` on separate lines for display equations.
The `align` and `equation` environments, labels, and `\eqref` are supported.
If a BibTeX title contains mathematics, check its rendered appearance because the Scholar `latex` filter also processes titles.

## Local preview and checks

Use Ruby 3.3 or later with the Bundler version recorded in `Gemfile.lock`, and Node.js 20 or later.

```bash
bundle install
npm ci
npm run lint:prettier
npm run lint:style-contract
bundle exec jekyll build
bundle exec jekyll serve
```

Open `http://localhost:4000/`. This repository is a GitHub Pages user site:
`url` is `https://jieliu-maths.github.io`, and `baseurl` must remain empty.
Do not pass the upstream demo's `--baseurl /al-folio` when building this site.

The Deploy site workflow builds pushes to `main` or `master` and publishes to the `gh-pages` branch.
In GitHub **Settings → Pages**, select **Deploy from a branch**, then **gh-pages / (root)**.
Local edits alone do not publish the website.

## Framework maintenance

Dependency pins are intentionally retained. Feature activation and dependency changes must keep `Gemfile`
and `_config.yml` aligned. See [AGENTS.md](AGENTS.md) and [the architecture guide](docs/ARCHITECTURE.md)
for the al-folio runtime boundaries. No local theme overrides or CSS build pipeline are used.
