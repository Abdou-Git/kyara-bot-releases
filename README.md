# Kyara Bot for Windows

Download the [latest Windows installer](https://github.com/Abdou-Git/kyara-bot-releases/releases/latest).

The installer includes Node.js, Chromium and Kyara Companion. Windows 10/11 x64 is required. No manual Node.js, npm, Git, Python or browser installation is required. Install for your Windows user, launch Kyara Bot, add an account and sign in normally.

Each managed account has an independent browser profile. Initial authentication and mandatory interactive verifications remain manual. Existing account settings, histories and profiles are kept outside application files in `%LOCALAPPDATA%\KyaraBot`.

This repository contains distribution information and release artifacts. The development repository remains private. Application JavaScript included in the installer is compiled and minified; distribution is not a claim of source confidentiality or obfuscation security.

Updates authenticate an Ed25519-signed `latest.json` manifest and verify the installer's SHA-256 before execution. The public verification key is included here. The executables do not currently have an Authenticode signing certificate; Windows SmartScreen may show a warning. They are not guaranteed to install without warnings.

The release notes distinguish verified installation tests from remaining clean-Windows validation. Browser profiles and user data are retained by uninstalling; account automation is stopped through the application's normal shutdown.
