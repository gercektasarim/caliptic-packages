# caliptic-packages

Static distribution site for Caliptic Agro AI on-device model packages.

- `index.json` is the package catalog the iOS app reads.
- Every package ships a manifest, a detached Ed25519 manifest signature and the artifact.
  The app verifies both signatures against keys bundled in the app before installing;
  a file changed here without the release key is refused on the device.
- Nothing is uploaded from devices. This site only serves files; the app sends no
  user data, photos or farm records anywhere.

Current release key: `caliptic-release-2026-10-r2`.
