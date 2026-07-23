# My Site — Minimal Mistakes Starter

This is a starter Jekyll site using the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) theme,
set up to deploy straight to GitHub Pages via `remote_theme` (no need to fork the whole theme repo).

## 1. Create the GitHub repo

- Go to https://github.com/new
- **If you want it at `https://yourusername.github.io`**, name the repo exactly `yourusername.github.io`
  (replace `yourusername` with your actual GitHub username). GitHub Pages will serve it from the root domain automatically.
- **If you want it at a sub-path** (e.g. `https://yourusername.github.io/my-project`), name the repo anything you like,
  e.g. `my-project`, and add `baseurl: "/my-project"` to `_config.yml`.

## 2. Push this project

From this folder, run:

```bash
git init
git add .
git commit -m "Initial commit: Minimal Mistakes starter site"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

## 3. Enable GitHub Pages

- Go to your repo → **Settings** → **Pages**
- Under "Build and deployment", set **Source** to `Deploy from a branch`
- Set **Branch** to `main` (or `master`) and folder to `/ (root)`
- Save. Your site will be live in a minute or two at the URL shown.

## 4. Customize

Edit these files first:

- `_config.yml` — site title, description, your name, bio, social links, `url`, and `repository`
- `_pages/about.md` — your About page content
- `_data/navigation.yml` — top navigation menu links
- `_posts/` — add new posts here, named `YYYY-MM-DD-title.md`

## 5. Preview locally (optional, requires Ruby)

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000

## Notes

- Because this uses `remote_theme`, GitHub Pages fetches the Minimal Mistakes theme automatically at build time —
  you don't need to copy theme files into your repo.
- Full theme documentation and configuration options: https://mmistakes.github.io/minimal-mistakes/docs/configuration/
