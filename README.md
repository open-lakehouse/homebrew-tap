# open-lakehouse/homebrew-tap

Homebrew tap for [open-lakehouse](https://github.com/open-lakehouse) tools.

```bash
brew install open-lakehouse/tap/trestle
```

(the first `install` from this tap auto-runs `brew tap open-lakehouse/tap`; you
can also tap explicitly with `brew tap open-lakehouse/tap`.)

## Formulae

| Formula | Description | Source |
|---------|-------------|--------|
| `trestle` | Unified CLI for proto-driven code generation and full-project scaffolding | [open-lakehouse/trestle](https://github.com/open-lakehouse/trestle) |

Each formula installs a prebuilt binary from the corresponding project's GitHub
Releases. Supported platforms: macOS (Apple Silicon + Intel) and Linux
(x86_64 + arm64, glibc).

## How this tap stays up to date

The formulae here are **generated, not hand-edited**. Each source repository's
release pipeline regenerates its formula and pushes it here on every release
(for `trestle`, the `bump-homebrew` job in
[`release-plz.yml`](https://github.com/open-lakehouse/trestle/blob/main/.github/workflows/release-plz.yml)).
Do not edit `Formula/*.rb` by hand — changes will be overwritten on the next
release. To change a formula, change the generator in its source repo
(`scripts/gen-homebrew-formula.sh`).
