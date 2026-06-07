# Hangyu Guo's Personal Homepage

Personal academic homepage built on the [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io) Jekyll theme (same template as [JoeYing1019.github.io](https://joeying1019.github.io)).

## Structure

- `_config.yml` — site / author config (name, email, github, scholar, …)
- `_pages/about.md` — entry; includes the section files below
- `_pages/includes/intro.md` — Bio
- `_pages/includes/news.md` — News timeline
- `_pages/includes/pub.md` — Selected publications
- `_pages/includes/honers.md` — Honors / awards (currently empty)
- `_pages/includes/others.md` — Experience, Education, Academic Service
- `images/` — favicons + avatar (drop your photo at `images/avatar.jpg`)

## Deploy to GitHub Pages

1. Create a new repo named `pyogher.github.io` (replace `pyogher` with your GitHub username).
2. From this `homepage/` directory:
   ```bash
   git init
   git add .
   git commit -m "init homepage"
   git branch -M main
   git remote add origin git@github.com:pyogher/pyogher.github.io.git
   git push -u origin main
   ```
3. Enable GitHub Pages in the repo settings (Source: `main` branch, root). The site goes live at `https://pyogher.github.io`.

## Local preview

```bash
gem install bundler jekyll
bundle install
bundle exec jekyll serve   # or: ./run_server.sh
# open http://localhost:4000
```

## TODO

- Drop your avatar at `images/avatar.jpg` (square, ≥512×512 recommended).
- Optionally enable the Google Scholar citation badge crawler (`google_scholar_crawler/` — see original template README).
- Replace favicons in `images/` if you want personal ones.
