# sandupal.github.io: career profile

A one-page Jekyll site that GitHub Pages builds automatically. All content lives in `_data/`; the page layout never needs editing for routine updates.

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
| Papers | `_data/publications.yml` |
| Talks and posters | `_data/talks.yml` |
| Key projects | `_data/projects.yml` |
| Navy career, honours, Navy photos and press links | `_data/navy.yml` |
| Education | `_data/education.yml` |

Navy photos and press links stay hidden until `confirmed: true` is set on the entry.

## Preview locally

```bash
conda activate jekyll          # Ruby 3.3 + Jekyll 4 environment
jekyll serve                   # then open http://localhost:4000
```
