# homebrew-spookiui

Homebrew tap for [SpookiUI](https://github.com/mattj85/SpookiUI) — a live
configurator TUI for the [Ghostty](https://ghostty.org) terminal.

## Install

```bash
brew install mattj85/spookiui/spookiui
```

Or tap first, then install:

```bash
brew tap mattj85/spookiui
brew install spookiui
```

Works on macOS and Linux. SpookiUI needs the `ghostty` binary at runtime
(`brew install --cask ghostty` on macOS, or https://ghostty.org/docs/install).

## Updating

```bash
brew upgrade spookiui
```

SpookiUI's in-app updater detects a Homebrew install and defers to `brew upgrade`.

## Maintaining this tap

The canonical formula lives in the main repo at
[`homebrew/spookiui.rb`](https://github.com/mattj85/SpookiUI/blob/main/homebrew/spookiui.rb).
On each SpookiUI release, update `Formula/spookiui.rb` here: bump `url` to the
new tag and refresh `sha256` with `curl -sL <tarball> | shasum -a 256`.
