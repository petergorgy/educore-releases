# EduCore signed release channel

Release artifacts live on the **`releases` branch** (this `main` branch only holds this file), one folder per version:

| Version | Manifest (set in EduCore → Settings → Release channel) | Package(s) |
|---|---|---|
| 1.3.0 | `https://raw.githubusercontent.com/petergorgy/educore-releases/releases/1.3.0/manifest.json` | educore-assessments 1.3.0 |
| 1.2.0 | `https://raw.githubusercontent.com/petergorgy/educore-releases/releases/1.2.0/manifest.json` | educore-recovery 1.2.0 |
| 1.1.0 | `https://raw.githubusercontent.com/petergorgy/educore-releases/releases/1.1.0/manifest-step2.json` | core, notifications, teaching hub, theme 1.1.0 |

Each folder contains `manifest.json` (Ed25519-signed), `packages/*.zip`, `packages/SHA256SUMS.txt` and `SOURCE.txt` (source commit).
Git tags `v1.2.0` and `v1.3.0` point at the `releases` commit that contains them. (GitHub "Releases" entries are not used; the raw branch URLs above are the distribution channel.)

EduCore installs a package only if the manifest signature verifies against the public key built into EduCore Core
(`wnG3eFq9qP96czwqUJ5/qtUDzA1ZPync7tR9wQnh+So=`) **and** the package SHA-256 matches the manifest. The private key is never stored here.
