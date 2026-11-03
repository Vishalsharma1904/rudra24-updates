# Rudra24 AI updates

Public Windows installers and cryptographically signed update files for Rudra24 AI.

## Download

[Download Rudra24 AI 1.0.12 for Windows x64](https://github.com/Vishalsharma1904/rudra24-updates/releases/download/v1.0.12/Rudra24-AI-Setup-1.0.12.exe)

[Latest installer release](https://github.com/Vishalsharma1904/rudra24-updates/releases/latest)

The published installer is version **1.0.12**, as embedded in the binary. It includes its Python engine.

## Integrity

The installer release includes `SHA256SUMS.txt`, a detached Ed25519 installer signature (`.exe.sig`), and `update-public-key.pem`. The public key matches the update trust pinned inside the installer.

Installer SHA-256:

```text
3afd17532698e58d5bace7dc08cce85f19b14e081c41d03ff3b26d85829e9ff5
```

Windows Authenticode publisher signing is not present. Windows installation and live login/provider acceptance remain to be tested.

## Signed update feed

- [feed.json](https://github.com/Vishalsharma1904/rudra24-updates/releases/download/feed/feed.json)
- [feed.json.sig](https://github.com/Vishalsharma1904/rudra24-updates/releases/download/feed/feed.json.sig)

The app verifies the feed with its pinned Ed25519 public key and checks the installer's SHA-512 before offering installation. The `feed` release is separate from the latest installer release.

This repository contains release artifacts and documentation. Application source repositories, private signing keys, credentials, and customer databases are not published here. GitHub's automatically generated source archives contain this repository's documentation only.
