# Shipwright — Releases

Signed, notarized macOS builds of **Shipwright**, a vertical project inbox for local coding agents (Claude Code, Codex, and other agent CLIs).

> This repository hosts **release binaries and notes only** — it does not contain source code.

## Download

Grab the latest `.dmg` from the [**Releases**](https://github.com/RRCummins/shipwright/releases/latest) page.

## Install

1. Download `Shipwright-<version>.dmg`.
2. Open the DMG and drag **Shipwright.app** into your **Applications** folder.
3. Launch it from Applications.

The build is signed with an Apple **Developer ID** and **notarized by Apple**, so it launches without Gatekeeper warnings — no need to right-click → Open or clear quarantine.

## Requirements

- macOS on Apple Silicon or Intel
- No additional runtime dependencies

## Verifying the signature (optional)

```sh
spctl --assess --type execute --verbose=2 /Applications/Shipwright.app
# => accepted / source=Notarized Developer ID
```

## Release notes

See [`CHANGELOG.md`](CHANGELOG.md) for per-version notes.
