# sandupal.github.io: career profile

A four-page Jekyll site (about, publications, research, experience) in the style of the al-folio theme, built natively by GitHub Pages. All content lives in `_data/`; the pages and layout never need editing for routine updates.

## Add an update (three steps)

1. Open `_data/updates.yml` and copy an existing block:
   ```yaml
   - date: 2026-11-01
     text: Started a postdoctoral position at ...
     url: https://...          # or "" for no link
   ```
2. Commit the change (on github.com you can edit the file directly in the browser).
3. GitHub Pages rebuilds the site in about a minute. The page sorts updates newest first.

## Other edits

| What | File |
|---|---|
| Bio, roles, contact links, LinkedIn, CV link | `_data/profile.yml` |
| Papers (Abs and Bib buttons, journal badge, thumbnail, "selected" flag for the home page; keys listed at the top of the file) | `_data/publications.yml` |
| Talks and posters | `_data/talks.yml` |
| Key projects | `_data/projects.yml` |
| Navy career, honours, Navy photos and press links | `_data/navy.yml` |
| Education | `_data/education.yml` |
| Research page cards (optional `image` and `image_alt` per project) | `_data/projects.yml` |
| Top navigation | `_data/nav.yml` |
| Look and feel (light and dark palettes follow the reader's system setting) | `assets/css/style.css` |

Pages: `index.html` (about, news, selected publications), `publications.html`, `research.html`,
`experience.html` (Navy career, honours, education). Shared pieces are in `_includes/`.

Navy photos and press links stay hidden until `confirmed: true` is set on the entry.

## Preview locally

```bash
conda activate jekyll          # Ruby 3.3 + Jekyll 4 environment
jekyll serve                   # then open http://localhost:4000
```
