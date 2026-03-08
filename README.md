# diogobaerlocher.github.io

Personal academic website built with Jekyll and hosted on GitHub Pages. Forked from [academicpages](https://github.com/academicpages/academicpages.github.io), which is based on [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/).

## Run locally

```bash
bundle install
bundle exec jekyll serve
```

Site will be available at `localhost:4000`. Jekyll will watch for changes and rebuild automatically.

## Key files

| File | Purpose |
|---|---|
| `_config.yml` | Site-wide settings (name, bio, author info, collections) |
| `_pages/about.md` | Main (and only) page |
| `_data/navigation.yml` | Top navigation bar links |
| `assets/css/main.scss` | Custom CSS (accordion, spacing, etc.) |
| `_sass/_variables.scss` | Colors and fonts |
| `_includes/archive-single.html` | Renders each publication/project entry |

## Collections

| Folder | Appears as |
|---|---|
| `_publications/` | Peer-Reviewed Publications |
| `_projects/` | Working Papers |
| `_portuguese/` | Peer-Reviewed Publications (Portuguese) |

## Add a publication or working paper

Create a `.md` file in `_publications/` or `_projects/` with the following front matter:

```yaml
---
title        : "Paper Title"
collection   : publications        # or: projects, portuguese
permalink    : /publications/slug
doilink      : "https://doi.org/..."
journal      : "Journal Name"
year         : "2024"
coauthors    : {"Co-author Name" : "https://their-website.com"}
buttons      :
    wppdf    : "/files/paper.pdf"  # local PDF
    wplink   : "https://..."       # external WP link
    srrn     : "https://ssrn..."
    repec    : "https://ideas..."
    repfiles : "https://..."       # replication files
    bibtex   : "/files/bibtex/cite.txt"
    scholar  : "https://scholar..."
abstract     : "Abstract text here."
presentations:
  - "Conference 1, Year"
  - "Conference 2, Year"
---
```

`coauthors` is a dictionary where the key is the name and the value is their website URL (leave blank if no website). All `buttons` fields are optional.
