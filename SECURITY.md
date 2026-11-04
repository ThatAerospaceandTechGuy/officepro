# Security policy

## Supported versions

| Product | Supported |
| --- | --- |
| OfficePro suite 1.0.x | Yes |
| Word Pro 0.14.x | Current release |
| Sheet Pro 0.15.x | Current release |
| Slides Pro 0.14.x | Current release |
| PDF Pro 0.17.x | Current release |
| Older releases | No |

Security fixes are published in a new release. There are no long-term support
branches for older builds.

## Reporting a vulnerability

Please use GitHub's private vulnerability reporting from the repository's
[Security tab](https://github.com/ThatAerospaceandTechGuy/officepro/security).
If private reporting is unavailable, open a minimal public issue asking the
maintainer for a private channel; do not include exploit details.

Do not open a public issue containing a working exploit, secret, credential,
sensitive crash dump or malicious file. Give the maintainers a reasonable
opportunity to investigate and coordinate a fix before publishing details.

A useful report includes:

- the affected app, version and release asset name;
- the Windows version and architecture;
- the affected component or file path;
- the security impact and required attacker access;
- exact reproduction steps;
- expected and actual behaviour;
- relevant logs with personal paths and document contents removed;
- whether the problem reproduces from a clean download.

## Scope

Reports are welcome for:

- the portable launcher and its in-place update path;
- the suite and standalone installers;
- the released app binaries;
- release integrity, asset naming and checksum handling;
- download or update behaviour that could execute unintended code.

Expected SmartScreen warnings for the current unsigned builds are not
vulnerabilities. A report that the warning can be bypassed without any other
security impact is also out of scope.

The application source is not published in this repository. Source-level reports
should still describe the released build and the observable impact.

## Response

This is a small, independent project. Reports are handled on a best-effort basis;
there is no guaranteed response time, bounty or disclosure deadline. The
maintainer will confirm the report, assess the impact and coordinate a fix and
disclosure when appropriate.

## Safe testing

Test only against your own installation and data. Do not target other users, the
GitHub infrastructure, the product site or third-party services. Do not attach
potentially harmful or non-redistributable files to a public issue.
