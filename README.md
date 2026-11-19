# AOM (Application for Office Management) - Public Release & Update Channel

Official public distribution and cryptographically verified auto-update repository for **AOM (Application for Office Management)** desktop applications.

## Latest Version
- **Version:** `v1.4.2` (Build 80)
- **Release Date:** November 20, 2026
- **Architecture:** Electron Multi-Platform Desktop (Windows / macOS)
- **Security:** Ed25519 Asymmetric Digital Signature Verification + SHA-256 Checksum
- **Status:** Public In-App Auto-Update Channel (Active & Branch-Protected)

## Cryptographic Update Verification
AOM Desktop clients automatically check `version.json` in this repository upon launch. When a newer version is released, clients download the update package and enforce dual-layer cryptographic validation:
1. **SHA-256 Checksum Verification:** Ensures file integrity during transmission.
2. **Ed25519 Asymmetric Digital Signature Verification:** Verifies that the package was signed by the developer's trusted private key using the client's embedded public key. Unsigned, intercepted, or tampered packages are strictly rejected before being applied.
