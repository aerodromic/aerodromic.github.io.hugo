# Joel Lo — personal website

Hugo source for [joelloliangze.com](https://joelloliangze.com/).
Generated files are published to [`aerodromic/aerodromic.github.io`](https://github.com/aerodromic/aerodromic.github.io).

## Local preview

Use Hugo **0.110.0 extended**, matching the deployment workflow.

```sh
git submodule update --init --recursive
hugo server --disableFastRender
```

Open the localhost URL printed by Hugo. Build the production site with `hugo --minify`.

## Editing

- `config.yaml`: biography, experience, education, selected projects, links and colours.
- `content/blog/`: blog posts; `content/gallery.md`: photo gallery.
- `static/css/refresh.css`: portfolio styling overrides.
- `layouts/`: local template overrides for the Hugo Profile theme.
- `static/`: images and downloadable files.

The homepage links to selected projects instead of the archived 2024 résumé. Add a current PDF and update `params.hero.button` if a résumé download is wanted again.

## Publishing

Pull requests run the Hugo build. Only a push to `main` publishes `public/` to the serving repository using the existing deploy key. The workflow preserves the custom domain `joelloliangze.com`; `baseURL` must match it.

## Content review

The refresh includes the confirmed current role: Analyst in Private Banking Credit Operations at JPMorgan. The date is shown as “Current” until the start month and year are confirmed. Confirm WorldQuant status and the preferred public contact email; the existing NUS address is retained. No new résumé is supplied.

Built with [Hugo Profile](https://github.com/gurusabarish/hugo-profile/).
