# Light Avelton

Light Avelton is part of the Avelton creative suite, based on the open-source [LightCraft](https://github.com/storytold/lightcraft) project.

- Browser: https://light.avelton.online
- Windows, macOS and Linux alpha downloads: https://github.com/avelton-ai/light-avelton/releases
- Support and bugs: https://github.com/avelton-ai/light-avelton/issues

The first Avelton releases are unsigned alpha builds. macOS packages use ad-hoc signatures and are not notarized. Projects stay on your device; the hosted browser app has no Avelton account or cloud project storage. Browser capabilities and file support depend on the upstream implementation.

## Build and verify

Install Rust (see `rust-version` in Cargo.toml), the wasm32-unknown-unknown target and the native platform dependencies described in the upstream development documentation. Run `cargo xtask ci` for the repository's checks. Desktop: `cargo run --release -p lightcraft`. CLI: `cargo run --release -p lightcraft-cli -- --help`. Release scripts are under `packaging/`; the Avelton release workflow builds browser and native packages together.

Rust crate names, command APIs and project file formats retain upstream identifiers for compatibility. Installed binary names are `light-avelton` and `light-avelton-cli`. Avelton uses a separate application identifier (`online.avelton.light`), installer identities and settings directory.

## Attribution and updates

Source: https://github.com/storytold/lightcraft, initial commit `543695129932c92338186911405ef26444c5a1c6`. Original copyright notices, contributors, third-party credits and MIT/Apache licences are preserved. Avelton branding is independent original artwork; bundled Inter lettering remains OFL-1.1. See NOTICE and the asset attribution files. The original ArtCraft brand artwork is excluded from this fork's distributions.

Upstream updates are reviewed and tested manually before an Avelton release. This fork is independently maintained and is not an official ArtCraft distribution.
