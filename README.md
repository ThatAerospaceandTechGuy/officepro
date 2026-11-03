# OfficePro downloads

Native Windows apps for documents, spreadsheets, presentations and PDFs. Install the full suite, a single app, or use the portable launcher.

**[Download OfficePro](https://officepro.pages.dev)**

## Releases

Every build is published on the [latest release](https://github.com/ThatAerospaceandTechGuy/officepro/releases/latest):

| Asset | What it is |
| --- | --- |
| `OfficePro-Setup.exe` | Windows installer for the full suite; creates shortcuts and an uninstaller. |
| `OfficePro.exe` | The portable launcher. Download this if you want to add apps individually. |
| `WordPro-Setup.exe` | Standalone Word Pro installer; installs only Word Pro. |
| `SheetPro-Setup.exe` | Standalone Sheet Pro installer; installs only Sheet Pro. |
| `SlidesPro-Setup.exe` | Standalone Slides Pro installer; installs only Slides Pro. |
| `PDFPro-Setup.exe` | Standalone PDF Pro installer; installs only PDF Pro. |
| `OfficePro-Suite-Windows-x64.zip` | Launcher and all four apps in one archive |
| `SHA256SUMS.txt` | SHA-256 checksums for the downloads |

The portable launcher still uses the individual app ZIP archives, which remain available on the release page for that purpose.

## Install

1. Download `OfficePro-Setup.exe` and run it for the complete suite. It installs to your user profile and creates a Start menu shortcut, optional desktop shortcut and uninstaller.
2. Or choose one standalone app installer: it adds only that app, with its own Start menu shortcut, optional desktop shortcut and uninstaller.
3. Or download `OfficePro.exe` and put it in a folder you control. Run it and press **Get** next to any app you want; the launcher downloads and unpacks that app beside itself.
4. A standalone installer can launch its app when setup finishes; the launcher shows **Open** for installed apps.

The suite archive is portable: extract it and run `OfficePro.exe`.

## Notes

- Windows 10 or Windows 11, 64-bit.
- The installers and launcher are unsigned, so Windows SmartScreen may ask you to confirm them.
- No account, telemetry, background service or runtime internet requirement. A connection is needed only when downloading an app.
- Cloud sync is optional and uses the OneDrive or Google Drive desktop client you already have. OfficePro does not create its own cloud folder.
- Licences, third-party notices and attribution files are included in every app folder.

This repository hosts release downloads. The application source is not published here.
