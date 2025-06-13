[![Deploy Astro site to Pages](https://github.com/pnposch/blog/actions/workflows/astro.yml/badge.svg)](https://github.com/pnposch/blog/actions/workflows/astro.yml)

# My Blog Repo
Simply my blog where i keep stuff, actually this is part 1 of the repo, the actual stuff is linked via the github action.

If you plan to use this for your own setup, ensure appropriate changes to the workflow.

# GitHub Pages Deployment
1. Set `site` and `base` in astro.config.mjs
2. Create repository `<username>.github.io`
3. Push code to main branch
4. Enable GitHub Pages in repo settings

Either use src/content locally or link as I did


# Local Deployment
## Start the Development Server

```sh
npm i -g pnpm
```
All commands are run from the root of the project, from a terminal:

| Command                    | Action                                           |
| :------------------------- | :----------------------------------------------- |
| `pnpm install`             | Installs dependencies                            |
| `pnpm run dev`             | Starts local dev server at `localhost:4321`      |
| `pnpm run build`           | Build your production site to `./dist/`          |
| `pnpm run preview`         | Preview your build locally, before deploying     |
| `pnpm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `pnpm run astro -- --help` | Get help using the Astro CLI                     |
| `pnpm run upgrade`         | Upgrade dependencies interactively               |
| `pnpm run format`          | Formats codebase using Prettier                  |
| `pnpm run commit`          | Commits changes to version control               |

## Production Build & Run

```sh
sudo docker build . --build-arg SITE_URL=https://example.com --build-arg DIRECTUS_URL=https://example.directus.com -t astro-deploy
docker run -d -p 1234:80 astro-deploy
```

## License
[based on dante-astro-theme](https://github.com/JustGoodUI/dante-astro-theme)
Licensed under the [GPL-3.0](https://github.com/JustGoodUI/dante-astro-theme/blob/main/LICENSE) license.
