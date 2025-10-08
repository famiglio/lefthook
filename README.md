# @famiglio/lefthook

> Famiglio's remote Lefthook configs.

## Configs

- [lint-commit-msg](./configs/lint-commit-msg.yml): `commit-msg` hook to lint commit messages with `commitlint`. `commitlint.config.mjs` is required. See [Commitlint](https://commitlint.js.org/).
- [lint-fmt-staged](./configs/lint-fmt-staged.yml): `pre-commit` hook top lint and format files with `ESLint` and `Prettier`. `eslint.config.mjs`, `.prettierrc.mjs`, and `.prettierignore` are required. See [ESLint](https://eslint.org/), [Prettier](https://prettier.io/).

## Usage:

```yaml
# Root lefthook.yml config file

remotes:
  - git_url: git@github.com:famiglio/lefthook
    refetch: true
    refetch_frequency: "24h"
    configs:
      - config/lint-commit-msg.yml
      - config/lint-fmt-staged.yml
```

## License

[MIT License](./LICENSE)
