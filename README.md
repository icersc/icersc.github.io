# ICER Steering Committee website

Jekyll site using the [Just the Docs](https://just-the-docs.github.io/just-the-docs/) theme, deployed to GitHub Pages.

## Test locally

Requires Ruby 3.1+ and Bundler.

```sh
bundle install
bundle exec jekyll serve --livereload
```

Open http://localhost:4000.

## Deploy

1. Create the GitHub organization `icersc` (owned by the committee, with at least two owners).
2. Create a public repository named `icersc.github.io` and push this directory to `main`.
3. In the repository, go to Settings → Pages → Build and deployment and set Source to **GitHub Actions**.
4. The workflow in `.github/workflows/pages.yml` publishes the site to https://icersc.github.io/.
5. Protect `main`: Settings → Branches → require one pull request approval.

## Custom domain (later)

1. Add a file named `CNAME` containing `icer.acm.org`.
2. Ask ACM to point `icer.acm.org` to `icersc.github.io` with a CNAME record.
3. In Settings → Pages, enter the domain and enable **Enforce HTTPS**.
4. Update `url` in `_config.yml`.

## Annual handover

- Update `current_conference` in `_config.yml`. This drives the header banner and the homepage callout.
- Add the finished conference to the top of `_data/conferences.yml`.
- Update `_data/committee.yml`.
