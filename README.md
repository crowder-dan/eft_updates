# Elite Field Tech — Updates

Release channel for the **Elite Field Tech Desktop Beta**, the Windows workspace for field service technicians. Part of Elite Suite.

This repository holds **installers and update files only**. The application source code lives in a separate private repository.

## What's here

Each beta version is published as a GitHub **Release** containing:

| File | Purpose |
| --- | --- |
| `Elite-Field-Tech-Desktop-Setup-<version>-x64.exe` | Windows installer |
| `Elite-Field-Tech-Desktop-Setup-<version>-x64.exe.blockmap` | Lets updates download only what changed |
| `latest.yml` | Version information the app reads to detect updates |

Release notes for each version describe what changed and what still needs testing.

## Status

- **Beta.** For approved pilot laptops only (Dell Pro Rugged 14, Lenovo E16; Windows x64).
- **Automatic updates are being added.** Until a release says otherwise, installed copies do not update themselves; install the newer version over the existing one.
- **Unsigned.** Windows may show an "unknown publisher" warning. Follow company IT policy.

## Installing or updating manually

1. Open the latest entry under **Releases**.
2. Download `Elite-Field-Tech-Desktop-Setup-<version>-x64.exe`.
3. Run it under your normal Windows login. No uninstall is needed first.

Technician data in `%APPDATA%\EliteFieldTechDesktopBeta` is kept across installs and updates. Installed diagnostic programs are not affected.

## How automatic updates will work

Once enabled, the app checks this repository's latest release at startup, downloads a newer version in the background, and asks the technician to restart when convenient. It will not restart on its own during a job.

## Rules for this repository

- Publish only installers, blockmaps, `latest.yml`, and release notes.
- Never upload source code, credentials, configuration files, customer records, or technician workspace exports.
- Version numbers must increase with every release (for example `0.4.0-beta.2`, then `0.4.0-beta.3`), or installed copies will not detect the update.
- Releases are published only at Elite Suite owner's direction.

## Feedback

Report problems to your Field Services manager. Include the app version, laptop, what you expected, what happened, and steps to reproduce. Do not include passwords, sign-in codes, or customer information in screenshots.

---

Third-party diagnostic software, trademarks, and service access remain subject to their owners' terms. No license is granted to redistribute this software outside its intended audience.
