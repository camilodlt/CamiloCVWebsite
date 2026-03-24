# Personal Academic Website

This repository contains a HugoBlox Academic CV site prepared for a simple research-oriented personal website with three public sections:

- Home
- Publications
- Contact

## Current setup

The starter has already been trimmed to:

- a homepage with bio, research summary, selected publications, and contact section
- a `Publications` page
- a `Contact` page in the navigation
- GitHub Pages deployment through GitHub Actions

## Files you will edit next

- `data/authors/me.yaml`: your name, affiliation, links, bio, and interests
- `content/_index.md`: homepage text and section wording
- `content/publications/`: your papers
- `config/_default/hugo.yaml`: final production URL

## How to add publications

For each paper, create a new folder inside `content/publications/`, copy the structure from `content/publications/conference-paper/`, and replace the placeholder values.

Minimum useful fields in `index.md`:

- `title`
- `authors`
- `date`
- `publication_types`
- `publication`
- `abstract`
- `summary`

Optional extras:

- `cite.bib` for citation export
- a PDF file
- `featured.jpg` if you want a thumbnail image
- `links` for code, arXiv, or project pages

The existing `content/publications/conference-paper/` entry is kept as a hidden template with `draft: true`, so it will not appear on the live site.

## Local development

You do not currently have `hugo` installed on this machine. To run the site locally later, install:

- Hugo extended
- Node.js
- pnpm

Then run:

```bash
pnpm install
hugo server --disableFastRender
```

## GitHub Pages deployment

The repository already includes `.github/workflows/build.yml` and `.github/workflows/deploy.yml`.

To publish:

1. Push this repository to GitHub.
2. In GitHub, open `Settings` -> `Pages`.
3. Set `Source` to `GitHub Actions`.
4. Update `baseURL` in `config/_default/hugo.yaml` to:

```yaml
baseURL: 'https://YOUR_GITHUB_USERNAME.github.io/'
```

If you publish from a project repository instead of a user site, use:

```yaml
baseURL: 'https://YOUR_GITHUB_USERNAME.github.io/REPOSITORY_NAME/'
```

5. Push to `main`.

GitHub Actions will build the Hugo site and deploy it automatically.

## Notes

- The template still contains some extra example content folders from HugoBlox. They are not linked in the main navigation.
- We can now replace the placeholders with your actual bio, publications, and contact details.
