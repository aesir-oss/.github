<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/aesir-oss/.github/raw/main/profile/assets/readme_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/aesir-oss/.github/raw/main/profile/assets/readme_light.svg">
    <img alt="Aesir Open Source Solutions, @aesir-oss" src="https://github.com/aesir-oss/.github/raw/main/profile/assets/readme_light.png" width="100%">
  </picture>
</p>

<p align="center">
  <b>Know what you ship, enforce what you allow.</b><br>
  Open source tooling for software supply chain security: SBOMs, policy enforcement, auditing, and attestation.
</p>

---

> *Before you walk through a doorway, look around you carefully. You never know where an enemy may be sitting in the hall.*
> <br>— Hávamál, stanza 1

### Who we are

Aesir Open Source Solutions builds open source tools that help teams understand and control what goes into their software. We started in the [Pixi](https://pixi.sh) and conda ecosystem, where environments pull in packages from many channels and languages at once, and where supply chain tooling has lagged behind.

### Why we exist

Most of the code you ship was written by someone else. Every dependency is a doorway into your project, and most teams cannot say with confidence what came through, where it came from, or whether it should have been let in at all.

We build tools that answer those questions:

- **What is in this environment?** Accurate SBOMs generated straight from your lock files, so you have a record of every package, version, source, and license.
- **Is it allowed?** Policy checks for channels, packages, and licenses that run before a change lands, not after it ships.
- **Can someone else verify it?** Output in open standards that auditors, customers, and other tools can check independently.

### Projects

| Project | What it does |
| --- | --- |
| [pixi-ext-contrib](https://github.com/aesir-oss/pixi-ext-contrib) | Community Pixi extensions for supply chain security. Home of `pixi sbom` (stable) and `pixi policy` (planned). |
| [pixi-sbom-action](https://github.com/aesir-oss/pixi-sbom-action) | GitHub Action that generates CycloneDX or SPDX SBOMs from `pixi.lock` and other lockfiles |
| [pixi-sbom-pre-commit](https://github.com/aesir-oss/pixi-sbom-pre-commit) | pre-commit hooks that keep SBOMs current as you commit |
| [pixi-policy-action](https://github.com/aesir-oss/pixi-policy-action) | GitHub Action that enforces dependency policy for Pixi environments in CI |
| [pixi-policy-pre-commit](https://github.com/aesir-oss/pixi-policy-pre-commit) | pre-commit hooks that check dependency policy before a change lands |

### Principles

- **Verifiable by default.** Every claim a tool makes should be checkable by someone else.
- **Built for the ecosystem.** Tools run where you already work: as Pixi extensions, pre-commit hooks, and CI steps.
- **Open standards.** We build on CycloneDX and SPDX for SBOMs, and on in-toto, SLSA, and Sigstore for provenance and signing.
- **Held to our own bar.** Every project is type-checked and tested, and we work toward shipping each release with its own SBOM and signed provenance.

### Get involved

Issues and pull requests are welcome on any project. Open an issue first for larger changes so we can agree on the approach.

To report a security vulnerability, please **do not** open a public issue. Use GitHub's private vulnerability reporting from the **Security** tab of the affected repository.

<p align="center"><sub>"No better burden can you carry on the road than good sense." (Hávamál, stanza 10)</sub></p>
