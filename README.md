# launcher-storybook

Published Storybook for the supercloud frontend:
<https://supergate-hub.github.io/launcher-storybook/>

This repository only hosts the built site. It contains no Storybook source.

## How the site is updated

Stories, MDX pages, and Storybook configuration live in `apps/frontend` of
[`supergate-hub/launcher-dev`](https://github.com/supergate-hub/launcher-dev),
which is a private repository. Its `Deploy Storybook` workflow builds the static
site on pushes to `main` and publishes the result to the `gh-pages` branch here.

## Contributing

- Do not commit to `gh-pages`. Every deploy replaces the branch contents with a
  fresh build, so manual changes are lost on the next run.
- Change a story or a component in `launcher-dev`; the site follows after the
  merge.
- `main` holds this README and the license only.
