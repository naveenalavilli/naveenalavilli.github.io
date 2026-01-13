# Architecture Notes (Jekyll + Minima)

This repo hosts a Jekyll site using the Minima theme, intended for GitHub Pages.

## Local dev

```bash
bundle install
bundle exec jekyll serve
```

## GitHub Pages setup

For a user/organization site (`<username>.github.io`), you can deploy directly from the `main` branch with no GitHub Actions required.

1. In GitHub, go to **Settings → Pages**.
2. Set **Source** to **Deploy from a branch**.
3. Select `main` and `/ (root)`.

If you prefer a GitHub Actions workflow later (for custom build steps), you can switch to **GitHub Actions** in that same settings page.
