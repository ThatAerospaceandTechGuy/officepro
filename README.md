<p align="center">
  <strong>OfficePro</strong><br>
  Native Windows apps for documents, spreadsheets, presentations and PDFs.
</p>

<p align="center">
  <a href="https://github.com/ThatAerospaceandTechGuy/officepro/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/ThatAerospaceandTechGuy/officepro?style=flat-square&amp;label=latest"></a>
  <a href="https://github.com/ThatAerospaceandTechGuy/officepro/releases"><img alt="Total downloads" src="https://img.shields.io/github/downloads/ThatAerospaceandTechGuy/officepro/total?style=flat-square&amp;label=downloads"></a>
  <img alt="Windows 10 and 11, 64-bit" src="https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-0078D4?style=flat-square">
  <a href="LICENSES.md"><img alt="Applications are MIT OR Apache-2.0" src="https://img.shields.io/badge/license-MIT%20OR%20Apache--2.0-2ea44f?style=flat-square"></a>
</p>

<p align="center">
  <a href="https://github.com/ThatAerospaceandTechGuy/officepro/releases/latest/download/OfficePro-Setup.exe"><img alt="Download OfficePro for Windows" src="https://img.shields.io/badge/Download-OfficePro%20for%20Windows-2ea44f?style=for-the-badge"></a>
</p>

<p align="center">
  Windows 10/11 &middot; 64-bit &middot; no account required
</p>

OfficePro is a lightweight, native office suite built around four focused apps:
**Word Pro**, **Sheet Pro**, **Slides Pro** and **PDF Pro**. Install the complete
suite, install a single app, or take the portable launcher and fetch only the apps
you need.

## Downloads

| Package | Version | What you get | Download |
| --- | ---: | --- | --- |
| **Complete suite** (recommended) | 1.0.0 | All four apps and the launcher, with Start menu entries and an uninstaller | [Installer](https://github.com/ThatAerospaceandTechGuy/officepro/releases/latest/download/OfficePro-Setup.exe) &middot; [Portable ZIP](https://github.com/ThatAerospaceandTechGuy/officepro/releases/latest/download/OfficePro-Suite-Windows-x64.zip) |
| **Portable launcher** | 1.0.0.0 | The 0.6 MB launcher; download apps on demand | [OfficePro.exe](https://github.com/ThatAerospaceandTechGuy/officepro/releases/latest/download/OfficePro.exe) |
| **Word Pro** | 0.14.0 | Word processor for `.docx` documents | [Installer](https://github.com/ThatAerospaceandTechGuy/officepro/releases/download/wordpro-v0.14.0/WordPro-Setup.exe) &middot; [Portable ZIP](https://github.com/ThatAerospaceandTechGuy/officepro/releases/download/wordpro-v0.14.0/WordPro-Windows-x64.zip) |
| **Sheet Pro** | 0.15.0 | Spreadsheet editor for `.xlsx` workbooks | [Installer](https://github.com/ThatAerospaceandTechGuy/officepro/releases/download/sheetpro-v0.15.0/SheetPro-Setup.exe) &middot; [Portable ZIP](https://github.com/ThatAerospaceandTechGuy/officepro/releases/download/sheetpro-v0.15.0/SheetPro-Windows-x64.zip) |
| **Slides Pro** | 0.14.1 | Presentation editor for `.pptx` decks | [Installer](https://github.com/ThatAerospaceandTechGuy/officepro/releases/download/slidespro-v0.14.1/SlidesPro-Setup.exe) &middot; [Portable ZIP](https://github.com/ThatAerospaceandTechGuy/officepro/releases/download/slidespro-v0.14.1/SlidesPro-Windows-x64.zip) |
| **PDF Pro** | 0.17.0 | PDF reader and editor for `.pdf` files | [Installer](https://github.com/ThatAerospaceandTechGuy/officepro/releases/download/pdfpro-v0.17.0/PDFPro-Setup.exe) &middot; [Portable ZIP](https://github.com/ThatAerospaceandTechGuy/officepro/releases/download/pdfpro-v0.17.0/PDFPro-Windows-x64.zip) |

Every release includes `SHA256SUMS.txt`. Browse [all releases](https://github.com/ThatAerospaceandTechGuy/officepro/releases)
for release notes, checksums and direct asset links.

## Install

### Complete suite

1. Download `OfficePro-Setup.exe` from the latest release.
2. Run it and follow the setup wizard. It installs per user, creates Start menu
   entries, offers an optional desktop shortcut and adds an uninstaller.
3. Launch OfficePro from the Start menu.

The suite archive is portable: extract `OfficePro-Suite-Windows-x64.zip` and run
`OfficePro.exe`. Nothing is written to the registry or installed system-wide.

### One app only

Download a `*-Setup.exe` from its app release. It installs only that app, with its
own Start menu entry and uninstaller, and does not install the launcher or the
other apps.

### Portable launcher

Put `OfficePro.exe` in a folder you control and run it. Press **Get** next to any
app you want; the launcher downloads the app archive and unpacks it beside itself.
The button then changes to **Open**. The launcher checks GitHub for newer suite
releases and can update in place, keeping installed apps, settings, shortcuts and
the uninstaller.

## Verify your download

The builds are currently unsigned, so Windows SmartScreen may ask you to confirm
them. Before running an installer, compare its SHA-256 hash with the matching
entry in `SHA256SUMS.txt` from the same release:

```powershell
Get-FileHash .\OfficePro-Setup.exe -Algorithm SHA256
```

The hashes must match exactly. Every app release also has its own
`SHA256SUMS.txt` containing the hashes for that app's installer and archive.

## What is included

| App | Purpose | Native format |
| --- | --- | --- |
| **Word Pro** | Documents, styles, tables and page layout | `.docx` |
| **Sheet Pro** | Workbooks, formulas, charts and formatting | `.xlsx` |
| **Slides Pro** | Presentations, layouts, shapes and speaker notes | `.pptx` |
| **PDF Pro** | Reading, editing, annotating and exporting PDFs | `.pdf` |

Each app is a self-contained native build. The suite is four app folders plus the
launcher, not one process or a shared runtime. The four apps use a common
OfficePro Soft interface: neutral surfaces, rounded controls and one accent colour
per app.

## Release channels

| Channel | Tag pattern | Latest release? | Contents |
| --- | --- | --- | --- |
| **OfficePro suite** | `vX.Y.Z` | Yes | Suite installer, suite archive, launcher, all app installers and ZIPs, checksums |
| **Standalone apps** | `wordpro-vX.Y.Z`, `sheetpro-vX.Y.Z`, `slidespro-vX.Y.Z`, `pdfpro-vX.Y.Z` | No | That app's installer, portable archive and checksums |

The latest release always points to the OfficePro suite. This keeps
`releases/latest/download/<asset>` links and the portable launcher stable. App
releases are tagged separately and never take over `latest`.

See [RELEASES.md](RELEASES.md) for the asset contract, checksum rules, release
checklist and stability policy.

## Requirements and privacy

- **Windows 10 or Windows 11, 64-bit.** The Linux port is in development and is
  not part of these Windows downloads.
- **No account, telemetry, background service or bundled runtime.**
- **Network access is optional** and used only for downloads, update checks and
  fetching apps from the launcher. There is no analytics or usage reporting.
- **Cloud sync is optional.** OfficePro uses the OneDrive or Google Drive desktop
  client you already have and never creates its own cloud folder.

## Licensing

OfficePro is a mixed distribution:

| Material | Terms |
| --- | --- |
| Word Pro, Sheet Pro, Slides Pro and PDF Pro | MIT License **or** Apache License 2.0, at your option |
| Portable launcher, installers and product site | Copyright &copy; 2026 ThatAerospaceandTechGuy. All rights reserved |
| OfficePro and app names, icons and the OfficePro Soft interface | Copyright &copy; 2026 ThatAerospaceandTechGuy. All rights reserved |
| Third-party fonts, icons, libraries and data | Their own licences; see each app's `NOTICE` and `ATTRIBUTION.md` |
| Documentation in this repository | Copyright &copy; 2026 ThatAerospaceandTechGuy. All rights reserved |

Every app ships with `LICENSE-MIT`, `LICENSE-APACHE`, `NOTICE`,
`ATTRIBUTION.md` and `README.txt`; those in-app notices are authoritative. Read
[LICENSES.md](LICENSES.md) for the full scope and [licenses/](licenses/) for
reference copies of the MIT and Apache-2.0 texts.

The application source is not published in this repository and is not licensed
for redistribution. Microsoft fonts, templates and proprietary artwork are never
bundled.

## Support and security

- **Installation and app help:** [open an issue](https://github.com/ThatAerospaceandTechGuy/officepro/issues)
  after reading [SUPPORT.md](SUPPORT.md).
- **Security reports:** follow [SECURITY.md](SECURITY.md). Please do not post
  exploit details, secrets or malicious files in a public issue.
- **Release changes:** see [CHANGELOG.md](CHANGELOG.md).

## Repository scope

This repository hosts public release downloads and their documentation. It does
not contain the OfficePro application source.
