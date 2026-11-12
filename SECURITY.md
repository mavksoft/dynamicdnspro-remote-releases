# Security Policy — DDNSPro Remote

DDNSPro Remote is distributed through this repository as signed binary releases.

## Verifying a download

- macOS builds are Developer-ID signed and notarized by Apple.
- Every release ships `.sha256` checksums — verify before running.
- Auto-updates are fetched over verified TLS and signature-checked
  against an Ed25519 release key, with automatic rollback on failure.
- Installs before 1.1.0 update through a legacy Sparkle EdDSA appcast.

## Session security

- Remote sessions run over WebRTC (DTLS-SRTP); signaling uses
  authenticated TLS channels.
- Host-side consent and per-machine access policies are enforced
  before any session opens — failed authorization fails closed.
- Report any session-security concern with maximum priority.

## Reporting a vulnerability

Please report security issues privately to
**support@it-systems.es** — do not open a public issue for
vulnerabilities. We aim to acknowledge reports within 48 hours.

## Privacy

See https://dynamicdnspro.com for the product privacy policy. These applications are
designed to run locally; where the product uses an account or cloud
service, only the data required for the feature is transmitted.
