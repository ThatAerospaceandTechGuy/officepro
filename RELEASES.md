# Release policy

This repository publishes OfficePro binaries and their documentation. The
application source is maintained privately and is not part of a release.

## Channels

| Channel | Tag pattern | Example | Latest release? |
| --- | --- | --- | --- |
| OfficePro suite | `vMAJOR.MINOR.PATCH` | `v1.0.0` | Yes |
| Word Pro | `wordpro-vMAJOR.MINOR.PATCH` | `wordpro-v0.14.0` | No |
| Sheet Pro | `sheetpro-vMAJOR.MINOR.PATCH` | `sheetpro-v0.15.0` | No |
| Slides Pro | `slidespro-vMAJOR.MINOR.PATCH` | `slidespro-v0.14.1` | No |
| PDF Pro | `pdfpro-vMAJOR.MINOR.PATCH` | `pdfpro-v0.17.0` | No |

The suite release is always the repository's **latest** release. The product page
and portable launcher use `releases/latest/download/<asset>`, so an app release
must never become the latest release.

Pre-release builds use a suffixed tag such as `v1.1.0-rc.1`, are marked as
pre-releases on GitHub, and never become the latest release.

## Asset contract

The suite release contains:

| Asset | Purpose |
| --- | --- |
| `OfficePro-Setup.exe` | Complete suite installer |
| `OfficePro-Suite-Windows-x64.zip` | Portable suite archive |
| `OfficePro.exe` | Portable launcher |
| `WordPro-Setup.exe` | Word Pro standalone installer |
| `SheetPro-Setup.exe` | Sheet Pro standalone installer |
| `SlidesPro-Setup.exe` | Slides Pro standalone installer |
| `PDFPro-Setup.exe` | PDF Pro standalone installer |
| `WordPro-Windows-x64.zip` | Word Pro portable archive |
| `SheetPro-Windows-x64.zip` | Sheet Pro portable archive |
| `SlidesPro-Windows-x64.zip` | Slides Pro portable archive |
| `PDFPro-Windows-x64.zip` | PDF Pro portable archive |
| `SHA256SUMS.txt` | SHA-256 hashes for every suite asset |

Each standalone app release contains only that app's installer, portable ZIP and
`SHA256SUMS.txt`.

Asset names are part of the public interface. Do not rename an asset that the
product page, launcher or existing download links depend on.

## Checksums

- Every release must include `SHA256SUMS.txt`.
- The suite checksum file must cover every suite asset.
- An app checksum file must cover that app's installer and portable ZIP.
- Publish checksums in the same release as the binaries, never in a separate
  release.
- The download page should show the exact command used to verify a file:

  ```powershell
  Get-FileHash .\OfficePro-Setup.exe -Algorithm SHA256
  ```

## Publishing checklist

1. Build and package the four apps and the launcher.
2. Test the suite installer, each standalone installer and the portable archive.
3. Test the launcher's download, update and relaunch paths.
4. Generate `SHA256SUMS.txt` and verify every hash.
5. Create the suite release as the latest release.
6. Create app releases with `--latest=false`.
7. Confirm every `releases/latest/download/...` URL returns the expected asset.
8. Update `CHANGELOG.md`, the README versions and the release notes.
9. Recheck that `LICENSES.md` and the in-app licence files are present.

## Stability and support

- The current suite line is `1.0.x`; app releases use their own version lines.
- Windows 10 and Windows 11 on x64 are the supported platforms for these
  downloads.
- Builds are currently unsigned. Windows SmartScreen warnings are expected; use
  the checksum and the release page to confirm provenance.
- Published assets should be treated as immutable. If a build is defective,
  publish a new patch release rather than silently replacing a tagged asset. If a
  replacement is unavoidable, update `SHA256SUMS.txt` and say so in the release
  notes.
- Security reports follow [SECURITY.md](SECURITY.md); ordinary bugs follow
  [SUPPORT.md](SUPPORT.md).

## Scope

This repository contains public release documentation and binaries only. Build
scripts and application source are not published here.
