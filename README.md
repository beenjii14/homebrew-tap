# beenjii14/tap

Homebrew tap for [Benjamin Cruz](https://github.com/beenjii14)'s tools.

## Formulae

| Formula | Description |
| --- | --- |
| [`sprout`](https://github.com/beenjii14/sprout) | Create cleanly named Git branches straight from Jira tickets |

## Install

```sh
brew tap beenjii14/tap
brew trust beenjii14/tap      # Homebrew 7+ asks you to trust third-party taps
brew install sprout
sprout-setup
```

Or in one go: `brew install beenjii14/tap/sprout`.

## Update and remove

```sh
brew upgrade sprout
sprout-uninstall && brew uninstall sprout
```

## Maintainers

Formulae live in [`Formula/`](Formula). To release a new version of a tool, update `url` and `sha256`, then run:

```sh
brew style beenjii14/tap/<formula>
brew audit --strict --new --online beenjii14/tap/<formula>
brew test beenjii14/tap/<formula>
```
