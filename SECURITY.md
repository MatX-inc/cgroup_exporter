# Security

This repository is MatX's fork of
[plazonic/cgroup_exporter](https://github.com/plazonic/cgroup_exporter). The
`matx` branch carries a few patches on top of upstream, and MatX publishes its
own release binaries from it.

## Reporting a vulnerability

- In the exporter's code as it exists upstream: please report it to the
  upstream project, which owns that code.
- In our patches, our release binaries, or the workflows that build them: use
  [private vulnerability reporting](https://github.com/MatX-inc/cgroup_exporter/security/advisories/new)
  on this repository. Please do not open a public pull request or discussion.

## Supported versions

Only the latest `v*-matx*` release receives fixes.

## Verifying a release

Each release attaches `SHA256SUMS` and a build provenance attestation:

    gh attestation verify cgroup_exporter-<tag>-linux-amd64 --repo MatX-inc/cgroup_exporter
