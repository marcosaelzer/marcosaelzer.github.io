# Marco Sälzer's website

Source for [marcosaelzer.github.io](https://marcosaelzer.github.io), built with Jekyll and the AcademicPages / Minimal Mistakes theme.

## Content map

| Content | Location |
| --- | --- |
| Biography, research, award, and news | `_pages/about.md` |
| Publication list, grouped by year | `_pages/publications.md` |
| Individual publication records | `_publications/*.md` |
| Sidebar, profile links, and build settings | `_config.yml` |
| Main navigation | `_data/navigation.yml` |
| Profile photo | `images/profile.png` |
| Publication links and display | `_includes/publication-links.html`, `_includes/archive-single.html`, `_layouts/single.html` |

The unused template CV, blog posts, talks, teaching, portfolio, and example pages remain in the repository but are excluded from the published site in `_config.yml`. Add real content before enabling them.

## Local preview

Install Ruby, Bundler, a compiler, and the Ruby development headers required by native gems, then run:

```sh
bundle install
bundle exec jekyll serve --config _config.yml,_config.dev.yml
```

Open <http://localhost:4000>. On systems with versioned Ruby commands, use `bundle3.2` in place of `bundle` if appropriate.

The current lockfile uses an older Jekyll/Liquid stack. On Ruby 3.2 it encounters an `undefined method tainted?` error in Liquid; updating the dependencies for that runtime remains a separate maintenance task.

To check a production build:

```sh
bundle exec jekyll build --safe
```

The output goes to `_site/`, which is ignored by Git. Keep `Gemfile.lock` under version control; dependency upgrades should be reviewed separately from content edits.

## Updating publications

Add a Markdown file to `_publications/` with `title`, `collection: publications`, a unique `permalink`, `authors`, `publication_kind` (`conference`, `journal`, or `preprint`), `date`, `venue`, `paperurl`, and a short `excerpt`. Use `arxivurl` for an optional open-access version. Write a short summary below the front matter.

Use the final publisher title and author order, and link an earlier preprint from the same record instead of listing it twice. Dates control sorting; the publication list displays the year. Keep slugs free of spaces, `#`, and other reserved URL characters.

## October 2026 content review

The review added seven publication records, linked the dissertation and GI award, and corrected publication metadata and links. Google Scholar blocked automated access, so publication details were checked against DBLP, official proceedings, journal metadata, and arXiv.

- [DBLP bibliography](https://dblp.org/pid/275/3108)
- [Google Scholar, newest first](https://scholar.google.com/citations?user=bxhpseQAAAAJ&sortby=pubdate)
- [GI award announcement](https://gi.de/meldung/gesellschaft-fuer-informatik-zeichnet-dr-marco-saelzer-mit-dissertationspreis-aus)

The site still presents a selected bibliography. Older workshop papers and some journal extensions are not listed separately.

Next improvements: add a real CV and a preferred contact link; provide slides and code alongside selected papers; review mobile navigation accessibility and favicon assets; add an automated build and internal-link check.

## Theme credits

Based on [AcademicPages](https://github.com/academicpages/academicpages.github.io), originally adapted by Stuart Geiger from Michael Rose's [Minimal Mistakes](https://github.com/mmistakes/minimal-mistakes). See `LICENSE`.
