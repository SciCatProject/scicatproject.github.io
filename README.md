# SciCat Project website

This repository contains all the files that are needed to generate the SciCat homepage.
It is that is hosted using github pages at https://scicatproject.github.io/. Source
code can be cloned from [github](https://github.com/SciCatProject/scicatproject.github.io).

In addition to the homepage, the technical documentation served under `/documentation`
and hosted in the [SciCatProject/documentation](https://github.com/SciCatProject/documentation)
repository.

# Building

The site is generated using [jekyll](https://jekyllrb.com/). It is typically built by
github directly, but can also be run locally for testing.

## Running locally with ruby

If you have ruby installed you can run jekyll locally:

```bash
gem install bundler jekyll
 bundle exec jekyll serve
```

## Running with docker

You may prefer to build using a docker container to avoid installing all the dependencies.
This can be done by simply running the following from the projlect directory:

```bash
docker-compose up
```

This will serve the site at http://localhost:4000. Most changes live-update, with the
exception of changes to `_config.yml`.


# Resources
- https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll
- https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll
- https://medium.com/codex/how-to-add-bootstrap-5-to-jekyll-in-two-easy-ways-4d9dd3c8c895
- https://github.com/jekyll/jekyll/issues/8523
- https://github.com/actions/jekyll-build-pages
