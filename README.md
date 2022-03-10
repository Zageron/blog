# Game Dev Blog

[![discord](https://img.shields.io/discord/921110926751584346?label=discord&color=7289DA&logo=discord&logoColor=white&style=flat-square)](https://discord.gg/Je3yyqnSDN)

<!-- omit in toc -->
## Table of Contents

- [Game Dev Blog](#game-dev-blog)
  - [Authoring a new Article](#authoring-a-new-article)
    - [Pre-publish steps](#pre-publish-steps)
  - [Building and Deploying](#building-and-deploying)
  - [License](#license)

---

## Authoring a new Article

```pwsh
hugo new posts/name-of-article/index.en.md
```

### Pre-publish steps

1. Modify the publish date to the current time.
2. Append the timestamp, including the hour.
    - Ex. `posts/2022-01-01T00-name-of-article/index.en.md`

## Building and Deploying

From an elevated powershell run:

```pwsh
choco install hugo-extended -confirm
```

VSC should take care of everything after that.

See `.vscode/tasks.json` for details.

---

## License

Copyright © 2022 Zageron ([@zageron](https://twitter.com/zageron))
