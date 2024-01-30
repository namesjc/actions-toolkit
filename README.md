# Actions-Toolkit

> Reusable Actions and Workflows for personal projects.

All actions and reusable workflows are designed with transparency and security in mind and can be combined as needed. There are actions for different software ecosystems and languages.

## Versioning

The same immutable git-tag is used for all actions and workflows when they are released. There are no floating-tags for this repository available. The versions are semver based. Third-party actions used internally are referenced with git-sha to prevent unexpected updates and ensure the build-system is reproducible.

## Workflows

| Name                                                                     | Description |
| ------------------------------------------------------------------------ | ----------- |
| [Build and test](.github/workflows/toolkit-build-test.yml)   | Builds and tests a project with different technologies and tools. |
| [Lint](.github/workflows/toolkit-lint.yml)   | Lints and checks a project with different technologies and tools. |
| [Release OCI](.github/workflows/toolkit-release-oci.yml)                 | Releases a OCI-Image project with optional Signing (Cosign), SBOM, SLSA provenance generation, Changelog and a GitHub release. |
| [Release GoReleaser](.github/workflows/toolkit-release-goreleaser.yml)   | Releases a GoReleaser project with a OCI-Image, optional signing (Cosign), SBOM, SLSA provenance generation, Changelog and a GitHub release. |

## Actions

| Name                                   | Description                                                                            |
| -------------------------------------- | -------------------------------------------------------------------------------------- |
| [Docker](docker/README.md)             | Creates a OCI-Image with multi-arch support. It can be signed with Cosign optionally.  |
| [Grype](grype/README.md)               | Scans a target for vulnerabilities with grype.                                         |
| [Push-Release](push-release/README.md) | Commits and pushes possible changes and creates a GitHub-Release.                      |
| [SBOM](sbom/README.md)                 | Creates SBOMs from OCI-Images. They can be optionally signed and attested with Cosign. |
| [Setup-Syft](setup-syft/README.md)     | Installs the syft binary.                                                              |
