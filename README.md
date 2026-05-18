# synchestra-io/homebrew-tap

Homebrew tap for Synchestra-io CLIs.

## Install a CLI

```bash
brew install synchestra-io/tap/<formula>
```

| Formula | Description | Repository |
|---|---|---|
| [`specscore`](Formula/specscore.rb) | Lint, validate, and navigate Markdown specifications. | [synchestra-io/specscore-cli](https://github.com/synchestra-io/specscore-cli) |
| _(more coming)_ | | |

## Maintenance

Formulae in this tap are managed automatically by [GoReleaser](https://goreleaser.com/customization/homebrew/). Each CLI's `.goreleaser.yml` contains a `brews:` block that writes its formula here on every release. **Do not hand-edit `Formula/*.rb` — changes will be overwritten on the next release.**

To bootstrap a new CLI into this tap, add a `brews:` block to the CLI's GoReleaser config pointing at `synchestra-io/homebrew-tap` with `branch: main`. See [`synchestra-io/specscore-cli/.goreleaser.yml`](https://github.com/synchestra-io/specscore-cli/blob/main/.goreleaser.yml) for the canonical example.

## License

Apache-2.0 — see [LICENSE](LICENSE). Individual formula installers point at their upstream CLI repository; each CLI carries its own license.
