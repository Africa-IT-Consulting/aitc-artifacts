# aitc-artifacts

Mirror of third-party runtime binaries that AITC servers install. Each release holds exactly one upstream build:

- the tag names the version and the sha256, e.g. `frankenphp-v1.13.3-sha256-d210c06b`;
- the assets are the upstream file, `SHA256SUMS`, the upstream release metadata and the attestation verification output;
- releases are immutable (repository setting), so a tag always serves the same bytes.

Do not upload anything by hand. Releases are published by the pin helper in the infrastructure repository after upstream attestation and checks. Consumers must verify the full sha256 from their own pin, never trust this repository alone.
