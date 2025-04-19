# my blog

### Start the Development Server

```sh
npm i -g pnpm
pnpm install
pnpm dev
```

### Production Build & Run

```sh
sudo docker build . --build-arg SITE_URL=https://example.com --build-arg DIRECTUS_URL=https://example.directus.com -t astro-deploy
docker run -d -p 1234:80 astro-deploy
```

## 🧞 Commands

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

## License
[based on](https://app.netlify.com/start/deploy?repository=https://github.com/JustGoodUI/dante-astro-theme)
Licensed under the [GPL-3.0](https://github.com/JustGoodUI/dante-astro-theme/blob/main/LICENSE) license.
