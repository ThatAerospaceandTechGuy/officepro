# OfficePro downloads

Native Windows apps for documents, spreadsheets, presentations and PDFs. Install the full suite, a single app, or use the portable launcher.

**[Download OfficePro](https://officepro.pages.dev)**

## Releases

| Release | Version | What it contains |
| --- | ---: | --- |
| [OfficePro full suite](https://github.com/ThatAerospaceandTechGuy/officepro/releases/tag/v1.0.0) | 1.0.0 | `OfficePro-Setup.exe`, `OfficePro-Suite-Windows-x64.zip`, `OfficePro.exe`, all standalone installers and app ZIPs |
| [Word Pro](https://github.com/ThatAerospaceandTechGuy/officepro/releases/tag/wordpro-v0.14.0) | 0.14.0 | `WordPro-Setup.exe` and `WordPro-Windows-x64.zip` |
| [Sheet Pro](https://github.com/ThatAerospaceandTechGuy/officepro/releases/tag/sheetpro-v0.15.0) | 0.15.0 | `SheetPro-Setup.exe` and `SheetPro-Windows-x64.zip` |
| [Slides Pro](https://github.com/ThatAerospaceandTechGuy/officepro/releases/tag/slidespro-v0.14.1) | 0.14.1 | `SlidesPro-Setup.exe` and `SlidesPro-Windows-x64.zip` |
| [PDF Pro](https://github.com/ThatAerospaceandTechGuy/officepro/releases/tag/pdfpro-v0.17.0) | 0.17.0 | `PDFPro-Setup.exe` and `PDFPro-Windows-x64.zip` |

Each app release includes its own `SHA256SUMS.txt`. The full-suite release is also the **latest** release, so existing `releases/latest/download/...` links and the portable launcher keep working.

## Install

1. Download `OfficePro-Setup.exe` from the full-suite release and run it for the complete suite. It installs to your user profile and creates a Start menu shortcut, optional desktop shortcut and uninstaller.
2. Or open an app release and download its `*-Setup.exe`: it installs only that app, with its own Start menu shortcut, optional desktop shortcut and uninstaller.
3. Or download `OfficePro.exe` and put it in a folder you control. Run it and press **Get** next to any app you want; the launcher downloads and unpacks that app beside itself.
4. A standalone installer can launch its app when setup finishes; the launcher shows **Open** for installed apps.

The suite archive is portable: extract it and run `OfficePro.exe`.

## Notes

- Windows 10 or Windows 11, 64-bit.
- The installers and launcher are unsigned, so Windows SmartScreen may ask you to confirm them.
- No account, telemetry, background service or runtime internet requirement. A connection is needed only when downloading an app.
- Cloud sync is optional and uses the OneDrive or Google Drive desktop client you already have. OfficePro does not create its own cloud folder.

## Licence

The four apps are licensed under the MIT License or the Apache License, Version 2.0, at your option. The launcher, installer wrappers and product site are all rights reserved. See [LICENSES.md](LICENSES.md) for the scope and where each app keeps its licence and third-party notices.

This repository hosts release downloads. The application source is not published here.
