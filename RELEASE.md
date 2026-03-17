# Release / Build Notes (Internal)

This repo is **not open source**. Release artifacts are distributed via SnippetSupply.

## Artifact formats

We currently ship:
- AppImage (amd64)
- Debian package (.deb, amd64)
- Tarball (x86_64)

Optional manifests/specs may exist for:
- Snap (snapcraft.yaml)
- RPM spec (.spec)
- Nix flake (flake.nix)
- AUR PKGBUILD variants

## Release outputs

A typical release output folder contains:

- `release_out/appimage/*.AppImage`
- `release_out/deb/*.deb`
- `release_out/tarball/*.tar.gz`
- `release_out/SHA256SUMS.txt`

## Versioning

- App version: `MAJOR.MINOR.PATCH` (example: `1.0.0`)
- Keep the version consistent across all packaging outputs.

## Basic release checklist

1. Update version in the app metadata (Tauri config, package names, etc.).
2. Build artifacts.
3. Generate checksums.
4. Smoke test:
   - Launch + sign in
   - Start a chat
   - Verify long-chat virtualization behavior
   - Confirm CPU/RAM usage is reasonable
5. Upload artifacts to SnippetSupply product listing.
6. Tag the release in git.

## Notes

- Do **not** commit OpenAI session cookies or user tokens.
- Keep any internal secrets out of the repo.
