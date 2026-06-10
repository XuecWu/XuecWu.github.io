# Xuecheng Wu's Personal Homepage

This repository hosts the source code for [Xuecheng Wu's personal academic homepage](https://XuecWu.github.io/).

Xuecheng Wu is a first-year member of [MM Lab](https://mmlab.ie.cuhk.edu.hk/) at [The Chinese University of Hong Kong](https://www.cuhk.edu.hk/), working on multimodal learning, computer vision, generative AI, and world modeling.

## Website Structure

The homepage is built with Jekyll and adapted from the AcadHomepage template.

Main files and directories:

- `_config.yml` — site metadata, author profile, links, and sidebar information.
- `_pages/about.md` — main homepage content, including biography, news, education, internships, publications, awards, honors, academic services, and mentorship.
- `_data/navigation.yml` — top navigation menu.
- `_includes/` — layout snippets such as masthead, author profile, and custom head content.
- `images/` — profile photo, favicon, organization logos, and publication figures.
- `assets/` and `_sass/` — stylesheets and theme assets.

## Local Preview

This site uses Ruby/Jekyll. In this local workspace, dependencies are installed under `vendor/bundle`.

```bash
BUNDLE_PATH="vendor/bundle" bundle exec jekyll serve --host 127.0.0.1 --port 4000 --no-watch
```

Then open:

```text
http://127.0.0.1:4000/
```

If using the current local workspace where Bundler 2.2.19 is installed under the user gem path:

```bash
BUNDLE_PATH="$PWD/vendor/bundle" PATH="$HOME/.gem/ruby/2.6.0/bin:$PATH" bundle _2.2.19_ exec jekyll serve --host 127.0.0.1 --port 4000 --no-watch
```

## Deployment

For GitHub Pages, push the repository content to the `XuecWu.github.io` repository. GitHub Pages will build the Jekyll site automatically.

Before pushing, do not include local build/dependency outputs:

- `_site/`
- `vendor/bundle/`
- `.bundle/`
- `.sass-cache/`
- `.jekyll-cache/`
- `.jekyll-metadata`

These are already listed in `.gitignore`.

## Acknowledgements

This homepage is adapted from [AcadHomepage](https://github.com/RayeRen/acad-homepage.github.io), which is influenced by [minimal-mistakes](https://github.com/mmistakes/minimal-mistakes) and [academicpages](https://github.com/academicpages/academicpages.github.io).

Thanks to the open-source community for the original templates and assets.
