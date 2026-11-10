# MESH AI — Releases

Public distribution channel for official MESH AI Android packages.

The application source code remains in the private repository:
https://github.com/MarcosMesh/TECHNIKER-MESH-ASSISTANT

## Release contract

Each published version will provide:

- `latest.json`: machine-readable metadata for the latest stable release.
- A versioned APK asset, for example `mesh-ai-0.1.1.apk`.
- SHA-256 checksum for integrity verification.
- Release notes and minimum supported app version when applicable.

The Android app must verify the metadata and APK checksum before handing the package to the Android package installer.

## Security requirements

- Never publish signing private keys, API tokens, or other secrets here.
- All installable APKs must be signed with the same protected Android signing key.
- The updater must not bypass Android's package installer or user confirmation.
- Do not publish CI debug APKs as production updates.
- Only publish an APK after a successful build and release validation.

## Current status

Repository initialized for the update channel. No installable release has been published yet.
