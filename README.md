# Foundry Pre-Commit Hook

Runs [Foundry](https://github.com/foundry-rs/foundry) `forge fmt` and/or `forge snahshot` before
commit.

## Usage

1. Install [Foundry](https://book.getfoundry.sh/getting-started/installation).
2. Install [`pre-commit`](https://pre-commit.com/#install).
3. Add the following to `.pre-commit-config.yaml` in your repo.

```
repos:
-   repo: https://github.com/0xYYY/foundry-pre-commit
    hooks:
    -   id: format
    -   id: snapshot
```

4. Run `pre-commit install` to setup the hooks.
5. 🎉 From now on, before each commit, `forge fmt` and `forge snapshot` will be ran automatically.

## License

Dual licensed under either [MIT License](./LICENSE-MIT) or [Apache License, Version 2.0](./LICENSE-APACHE).
