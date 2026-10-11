<p align="center">
  <img src="https://github.com/aesir-oss/.github/raw/main/profile/assets/aesir-oss-ravens.jpg" width="280" alt="Huginn and Muninn, Odin's ravens of Thought and Memory, facing each other above Yggdrasil">
</p>

<h1 align="center">Aesir Open Source Solutions</h1>

<p align="center">
  <b>Know what you ship, enforce what you allow.</b><br>
  Open source tooling for software supply chain security: SBOMs, policy enforcement, auditing, and attestation.
</p>

---

### Thought and Memory

Every dawn, Odin sends his two ravens out across the nine worlds. **Huginn** is *Thought*, **Muninn** is *Memory*. By nightfall they return and tell him everything they have seen, and that is how the Allfather knows what happens in every corner of Yggdrasil.

Securing a software supply chain takes the same two things:

- **Memory**: a faithful record of what your software is made of, where each piece came from, and how it was built. SBOMs, provenance, attestations, and audit trails.
- **Thought**: reasoning over that record to decide what is allowed to grow on your tree. Policy, enforcement, and gates in CI.

Between them stands the world tree: your dependency graph, where everything you ship has its roots.

### Projects

| Project | Raven | What it does |
| --- | --- | --- |
| [pixi-sbom](https://github.com/aesir-oss/pixi-sbom) | Memory | Pixi extension that generates SBOMs from Pixi manifests and lock files |
| [pixi-sbom-pre-commit](https://github.com/aesir-oss/pixi-sbom-pre-commit) | Memory | pre-commit hooks for pixi-sbom |
| [pixi-ext-contrib](https://github.com/aesir-oss/pixi-ext-contrib) | Both | Community Pixi extensions for supply chain security: SBOMs, license and dependency policy, and more |
| pixi-policy *(in development)* | Thought | Policy engine for Pixi environments: decide which packages, licenses, and sources are allowed |

### Principles

- **Verifiable by default.** Every claim a tool makes should be checkable by someone else.
- **Built for the ecosystem.** Tools run where you already work: as Pixi extensions, pre-commit hooks, and CI steps.
- **Open standards.** We build on CycloneDX and SPDX for SBOMs, and on in-toto, SLSA, and Sigstore for provenance and signing.
- **Held to our own bar.** Every project is type-checked and tested, and we work toward shipping each release with its own SBOM and signed provenance.

### Get involved

Issues and pull requests are welcome on any project. Open an issue first for larger changes so we can agree on the approach.

To report a security vulnerability, please **do not** open a public issue. Use GitHub's private vulnerability reporting from the **Security** tab of the affected repository.

<p align="center"><sub>"Huginn and Muninn fly each day over the wide world." (Grímnismál, paraphrased)</sub></p>
