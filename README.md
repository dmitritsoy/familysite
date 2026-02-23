# Simple site (GitHub Pages)

Minimal Jekyll site, ready to deploy on GitHub Pages.

## Run locally

```bash
bundle install
bundle exec jekyll serve
```

Open [http://localhost:4000](http://localhost:4000).

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. In the repo: **Settings → Pages**.
3. Under **Build and deployment**, choose **GitHub Actions** (recommended) or **Deploy from a branch**.
   - **GitHub Actions**: add the Jekyll workflow (e.g. from the Actions tab, use “Jekyll” or the `pages` preset). Push to trigger a build.
   - **Branch**: set source to **main** (or your default branch), folder **/ (root)**. GitHub will build Jekyll automatically.

If the repo is `username.github.io`, the site will be at **https://username.github.io**.  
Otherwise it will be at **https://username.github.io/reponame** — in that case set `baseurl: "/reponame"` in `_config.yml`.

## Add content later

- Edit `_config.yml` for site title and options.
- Edit `index.html` or add new `.html`/`.md` pages with front matter `layout: default`.
- Use `_layouts/`, `_includes/`, and `_data/` like in [dmitritsoy.github.io](https://github.com/dmitritsoy/dmitritsoy.github.io) when you need more structure.
