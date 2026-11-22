# Proto plugin for Cilium CLI

Install [Cilium CLI](https://github.com/cilium/cilium-cli) with [Proto](https://moonrepo.dev/proto).

## Install

```sh
proto plugin add cilium https://github.com/BarretoTech/proto-cilium-plugin/releases/download/v0.1.0/plugin.toml
proto install cilium 0.20.2
proto run cilium 0.20.2 -- version --client
```

Add the locator and tool version to `.prototools` to pin them for a project.

```toml
cilium = "0.20.2"

[plugins.tools]
cilium = "https://github.com/BarretoTech/proto-cilium-plugin/releases/download/v0.1.0/plugin.toml"
```

Install tests cover Linux x64 and ARM64, macOS Intel and Apple Silicon, and Windows x64 with Proto 0.63.2.

The plugin configuration is available under the [MIT License](LICENSE).
