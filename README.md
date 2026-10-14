# Joel Lo — personal website

Hugo source for [joelloliangze.com](https://joelloliangze.com/).
Generated files are published to the `gh-pages` branch of this repository.

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

Pull requests run the Hugo build. Only a push to `main` publishes `public/` to the `gh-pages` branch using `GITHUB_TOKEN`. The workflow preserves the custom domain `joelloliangze.com`; `baseURL` must match it.

## Profile content

Career dates and education were checked against Joel’s LinkedIn profile export supplied on 14 October 2026. The current JPMorgan Credit Middle Office role began in October 2026, following an Asia Rates traineeship from March to September 2026. WorldQuant ended in March 2024. The public contact email matches the profile. The archived résumé remains unlinked; the profile export itself is not published.

Built with [Hugo Profile](https://github.com/gurusabarish/hugo-profile/).
