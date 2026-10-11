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

### The Norns at the Well

At the roots of Yggdrasil, the world tree, lies the Well of Urd. Three Norns live there. Each day they draw water from the well to keep the tree from rotting, and they carve into its trunk the fates of everything that lives beneath its branches.

- **Urd** is *what has been*.
- **Verdandi** is *what is becoming*.
- **Skuld** is *what shall be*.

Below them, the serpent Nidhogg gnaws at the roots.

Your dependency graph is that tree. Everything you ship grows from roots you did not plant yourself, and something is always gnawing at them. Keeping it healthy takes the same three kinds of work:

- **Urd: the record.** A faithful account of what your software is made of, where each piece came from, and how it was built. SBOMs, provenance, and audit trails.
- **Verdandi: the moment of change.** Checks that run as a change happens, at commit time and in CI, so the record is written while the work is fresh rather than reconstructed later.
- **Skuld: the rule.** Policy that decides what is allowed to grow on your tree: which packages, licenses, and sources may enter, and what gets turned away at the gate.

### Projects

| Project | Norn | What it does |
| --- | --- | --- |
| [pixi-ext-contrib](https://github.com/aesir-oss/pixi-ext-contrib) | All three | Community Pixi extensions for supply chain security. Home of `pixi sbom` (stable) and `pixi policy` (planned). |
| [pixi-sbom-action](https://github.com/aesir-oss/pixi-sbom-action) | Urd | GitHub Action that generates CycloneDX or SPDX SBOMs from `pixi.lock` and other lockfiles |
| [pixi-sbom-pre-commit](https://github.com/aesir-oss/pixi-sbom-pre-commit) | Verdandi | pre-commit hooks that keep SBOMs current as you commit |
| [pixi-policy-pre-commit](https://github.com/aesir-oss/pixi-policy-pre-commit) | Verdandi | pre-commit hooks that check dependency policy before a change lands |
| [pixi-policy-action](https://github.com/aesir-oss/pixi-policy-action) | Skuld | GitHub Action that enforces dependency policy for Pixi environments in CI |

### Principles

- **Verifiable by default.** Every claim a tool makes should be checkable by someone else.
- **Built for the ecosystem.** Tools run where you already work: as Pixi extensions, pre-commit hooks, and CI steps.
- **Open standards.** We build on CycloneDX and SPDX for SBOMs, and on in-toto, SLSA, and Sigstore for provenance and signing.
- **Held to our own bar.** Every project is type-checked and tested, and we work toward shipping each release with its own SBOM and signed provenance.

### Get involved

Issues and pull requests are welcome on any project. Open an issue first for larger changes so we can agree on the approach.

To report a security vulnerability, please **do not** open a public issue. Use GitHub's private vulnerability reporting from the **Security** tab of the affected repository.

<p align="center"><sub>"The Norns draw water from the well each day and pour it over the ash, so that its limbs neither wither nor rot." (Gylfaginning, paraphrased)</sub></p>
