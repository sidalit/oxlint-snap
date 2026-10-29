<div align="center">

<img src="snap/gui/oxlint.png" alt="Oxlint logo" width="128" />

# Oxlint

**A fast JavaScript and TypeScript linter**

[![oxlint](https://snapcraft.io/oxlint/badge.svg)](https://snapcraft.io/oxlint)
[![Base: core26](https://img.shields.io/badge/Base-core26-2C8C3C?logo=canonical&logoColor=white)](https://snapcraft.io/core26)
![Confinement: strict](https://img.shields.io/badge/Confinement-strict-2C8C3C)
[![Maintainer: sidaliteir](https://img.shields.io/badge/Maintainer-sidaliteir-2C8C3C?logo=snapcraft&logoColor=white)](https://snapcraft.io/publisher/sidaliteir)
![Architectures: amd64 and arm64](https://img.shields.io/badge/Architectures-amd64%20%7C%20arm64-2C8C3C?logo=linux&logoColor=white)

[Getting Started](#getting-started) · [Configure](#configure) · [Limitations](#limitations) · [Build](#build) · [Support](#support) · [License](#license)

Unofficial snap packaging for [Oxlint](https://github.com/oxc-project/oxc), a JavaScript and TypeScript linter with automatic fixes.

</div>

---

## Getting Started

<a href="https://snapcraft.io/oxlint"><img alt="Get it from the Snap Store" src="https://snapcraft.io/en/dark/install.svg" width="180"></a>

```bash
sudo snap install oxlint
cd ~/project/my-project
oxlint .
```

## Configure

Use your project's `.oxlintrc.json`. See the [upstream documentation](https://oxc.rs/docs/guide/usage/linter.html) for settings and editor integration.

```bash
sudo snap connect oxlint:removable-media   # optional: /media, /mnt
```

## Limitations

- Projects must be in non-hidden home folders or connected removable storage.
- Standalone release: no JavaScript plugins or JS/TS configuration. The optional type-aware helper is not included.

## Build

```bash
git clone https://github.com/sidalit/oxlint-snap.git
cd oxlint-snap
sudo snap install snapcraft --classic
snapcraft pack
```

## Support

- **Installation or snap issues:** [open a packaging issue](https://github.com/sidalit/oxlint-snap/issues).
- **Application bugs:** [report them upstream](https://github.com/oxc-project/oxc/issues).

## License

Snap packaging: [MIT](https://github.com/sidalit/oxlint-snap/blob/main/LICENSE).
