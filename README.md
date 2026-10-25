# caliptic-packages

Static distribution site for Caliptic Agro AI on-device model packages.

- `index.json` is the package catalog the iOS app reads.
- Every package ships a manifest, a detached Ed25519 manifest signature and the artifact.
  The app verifies both signatures against keys bundled in the app before installing;
  a file changed here without the release key is refused on the device.
- Nothing is uploaded from devices. This site only serves files; the app sends no
  user data, photos or farm records anywhere.

Current release key: `caliptic-release-2026-10-r2`.

## Packages

| Package | Version | Notes |
|---|---|---|
| agro.vision.disease | 0.1.0 | Pilot disease classifier (5 crops). |
| agro.knowledge | 0.1.0 | 19 disease articles. AI-written summaries of the listed university and FAO sources, checked twice against those sources but **not reviewed by an agricultural expert**. The app labels them as such. No pesticide names or doses. |
