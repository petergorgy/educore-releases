# EduCore 1.1.0 — signed release

Packages are verified by EduCore before installation (Ed25519-signed manifest + SHA-256 per package). Do not edit files here by hand; any change breaks the signature and EduCore will refuse the package.

| Manifest | Use when the site runs | Contents |
|---|---|---|
| `manifest-step1.json` | EduCore Core 1.0.2 | 7 packages (updates Core, Notifications, theme) |
| `manifest-step2.json` | EduCore Core 1.1.0 | 8 packages (adds the Teaching & Tutoring Hub) |

Manifest URLs (paste into EduCore → Settings → Release channel):
- Step 1: https://raw.githubusercontent.com/petergorgy/educore-releases/releases/1.1.0/manifest-step1.json
- Step 2: https://raw.githubusercontent.com/petergorgy/educore-releases/releases/1.1.0/manifest-step2.json

`packages/SHA256SUMS.txt` lists the package checksums.
